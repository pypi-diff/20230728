# Comparing `tmp/minlog-0.3.1.tar.gz` & `tmp/minlog-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minlog-0.3.1.tar", max compression
+gzip compressed data, was "minlog-0.4.0.tar", max compression
```

## Comparing `minlog-0.3.1.tar` & `minlog-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       26 2023-06-07 18:56:59.420529 minlog-0.3.1/README.md
--rw-r--r--   0        0        0     4947 2023-07-27 06:10:47.792342 minlog-0.3.1/minlog/__init__.py
--rw-r--r--   0        0        0      523 2023-07-27 05:52:40.500198 minlog-0.3.1/minlog/_test.py
--rw-r--r--   0        0        0      297 2023-07-27 06:11:00.115657 minlog-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 minlog-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2023-06-07 18:56:59.420529 minlog-0.4.0/README.md
+-rw-r--r--   0        0        0     5808 2023-07-28 02:24:13.998579 minlog-0.4.0/minlog/__init__.py
+-rw-r--r--   0        0        0      917 2023-07-28 02:24:03.648586 minlog-0.4.0/minlog/_test.py
+-rw-r--r--   0        0        0      297 2023-07-28 02:24:27.301903 minlog-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 minlog-0.4.0/PKG-INFO
```

### Comparing `minlog-0.3.1/minlog/__init__.py` & `minlog-0.4.0/minlog/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,18 +27,21 @@
     WARN = 2
     INFO = 3
     TRACE = 4
     DEBUG = 5
 
 
 class Logger(object):
-    def __init__(self, verbosity: Verbosity = Verbosity.INFO):
+    def __init__(self, verbosity: Verbosity = Verbosity.INFO, log_source: str = None):
         # maximum verbosity of messages to print
         self.verbosity = verbosity
 
+        # log source tag
+        self.log_source = log_source
+
         # default to rich
         self.backend = Backend.RICH
         # but if compiled, default to colorama
         if IS_COMPILED:
             self.backend = Backend.COLORAMA
 
         if self.backend == Backend.RICH:
@@ -46,53 +49,55 @@
 
             self.rich_console = Console()
 
         elif self.backend == Backend.COLORAMA:
             # initialize colorama
             colorama.init()
 
-    def short_verbosity(self, message_verbosity: Verbosity):
-        if message_verbosity == Verbosity.DEBUG:
-            return "dbg"
-        elif message_verbosity == Verbosity.TRACE:
-            return "trc"
-        elif message_verbosity == Verbosity.INFO:
-            return "inf"
-        elif message_verbosity == Verbosity.WARN:
-            return "wrn"
-        elif message_verbosity == Verbosity.ERROR:
-            return "err"
-        elif message_verbosity == Verbosity.CRITICAL:
-            return "crt"
+    def logger_for(self, log_source: str):
+        # create a clone of this logger, but with a different log source
+        return Logger(self.verbosity, log_source=log_source)
 
     def log(self, message: str, message_verbosity: Verbosity):
         # if the message verbosity is within the configured maximum verbosity
         if message_verbosity.value > self.verbosity.value:
             return
 
         # then print the message
-        meta_str = f"{self.short_verbosity(message_verbosity)}"
+        meta_str = f"[{self.short_verbosity(message_verbosity)}]"
         message_str = message
+        source_str = ""
+        if self.log_source is not None:
+            source_str = f"[{self.log_source}]"
 
         if self.backend == Backend.RICH:
             # mprint(message)
-            meta_style_rich = self.get_style_rich(message_verbosity)
-            self.rich_console.print(f"\[{meta_str}]", style=meta_style_rich, end="")
+            meta_str_escaped = meta_str.replace("[", "\[")
             message_str_escaped = message_str.replace("[", "\[")
+            source_str_escaped = source_str.replace("[", "\[")
+
+            meta_style_rich = self.get_style_rich(message_verbosity)
+            self.rich_console.print(meta_str_escaped, style=meta_style_rich, end="")
+            self.rich_console.print(" ", end="")
+            self.rich_console.print(
+                f"{source_str_escaped}", style="bright_black", end=""
+            )
             self.rich_console.print(f" {message_str_escaped}")
         elif self.backend == Backend.COLORAMA:
             meta_bg = Back.BLACK
             meta_fg = self.get_fg_color_colorama(message_verbosity)
+            source_fg = Fore.LIGHTBLACK_EX
             message_bg = Back.RESET
             message_fg = Fore.RESET
 
-            meta_frm = f"{meta_bg}{meta_fg}[{meta_str}]{Style.RESET_ALL}"
+            meta_frm = f"{meta_bg}{meta_fg}{meta_str}{Style.RESET_ALL}"
+            source_frm = f"{source_fg}{source_str}{Style.RESET_ALL}"
             message_frm = f"{message_bg}{message_fg}{message_str}{Style.RESET_ALL}"
 
-            print(f"{meta_frm} {message_frm}")
+            print(f"{meta_frm} {source_frm} {message_frm}")
 
     def debug(self, message: str):
         self.log(message, Verbosity.DEBUG)
 
     def trace(self, message: str):
         self.log(message, Verbosity.TRACE)
 
@@ -123,14 +128,31 @@
 
     def be_quiet(self):
         self.verbosity = Verbosity.ERROR
 
     def be_verbose(self):
         self.verbosity = Verbosity.TRACE
 
+    def be_debug(self):
+        self.verbosity = Verbosity.DEBUG
+
+    def short_verbosity(self, message_verbosity: Verbosity):
+        if message_verbosity == Verbosity.DEBUG:
+            return "dbg"
+        elif message_verbosity == Verbosity.TRACE:
+            return "trc"
+        elif message_verbosity == Verbosity.INFO:
+            return "inf"
+        elif message_verbosity == Verbosity.WARN:
+            return "wrn"
+        elif message_verbosity == Verbosity.ERROR:
+            return "err"
+        elif message_verbosity == Verbosity.CRITICAL:
+            return "crt"
+
     def get_fg_color_colorama(self, message_verbosity: Verbosity):
         if message_verbosity == Verbosity.DEBUG:
             return Fore.LIGHTBLACK_EX
         elif message_verbosity == Verbosity.TRACE:
             return Fore.LIGHTBLACK_EX
         elif message_verbosity == Verbosity.INFO:
             return Fore.GREEN
```

