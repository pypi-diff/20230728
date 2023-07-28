# Comparing `tmp/logPPP-1.1.1.tar.gz` & `tmp/logPPP-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logPPP-1.1.1.tar", last modified: Thu Jul 27 03:52:02 2023, max compression
+gzip compressed data, was "logPPP-1.1.2.tar", last modified: Fri Jul 28 10:02:57 2023, max compression
```

## Comparing `logPPP-1.1.1.tar` & `logPPP-1.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 03:52:02.791176 logPPP-1.1.1/
--rw-rw-rw-   0        0        0      126 2023-07-27 03:52:02.791176 logPPP-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-07-26 13:51:56.000000 logPPP-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-27 03:52:02.791176 logPPP-1.1.1/logPPP.egg-info/
--rw-rw-rw-   0        0        0      126 2023-07-27 03:52:02.000000 logPPP-1.1.1/logPPP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-07-27 03:52:02.000000 logPPP-1.1.1/logPPP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 03:52:02.000000 logPPP-1.1.1/logPPP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 03:52:02.000000 logPPP-1.1.1/logPPP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-27 03:52:02.791176 logPPP-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      379 2023-07-26 10:16:17.000000 logPPP-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 03:52:02.791176 logPPP-1.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-27 03:52:02.791176 logPPP-1.1.1/src/logPPP/
--rw-rw-rw-   0        0        0      116 2023-07-26 10:16:17.000000 logPPP-1.1.1/src/logPPP/_ConsoleColors.py
--rw-rw-rw-   0        0        0     1914 2023-07-27 03:46:44.000000 logPPP-1.1.1/src/logPPP/__init__.py
--rw-rw-rw-   0        0        0      453 2023-07-26 10:16:17.000000 logPPP-1.1.1/src/logPPP/_util.py
--rw-rw-rw-   0        0        0      373 2023-07-26 10:16:17.000000 logPPP-1.1.1/src/logPPP/logPPPLevel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:57.521660 logPPP-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-28 10:02:57.521660 logPPP-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-07-28 10:02:46.000000 logPPP-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:57.521660 logPPP-1.1.2/logPPP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3185 2023-07-28 10:02:57.000000 logPPP-1.1.2/logPPP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-28 10:02:57.000000 logPPP-1.1.2/logPPP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:02:57.000000 logPPP-1.1.2/logPPP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 10:02:57.000000 logPPP-1.1.2/logPPP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 10:02:57.521660 logPPP-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-28 10:02:46.000000 logPPP-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:57.521660 logPPP-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:02:57.521660 logPPP-1.1.2/src/logPPP/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 10:02:46.000000 logPPP-1.1.2/src/logPPP/__ConsoleColors__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-07-28 10:02:46.000000 logPPP-1.1.2/src/logPPP/__Level__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-07-28 10:02:46.000000 logPPP-1.1.2/src/logPPP/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-28 10:02:46.000000 logPPP-1.1.2/src/logPPP/__util__.py
```

### Comparing `logPPP-1.1.1/src/logPPP/__init__.py` & `logPPP-1.1.2/src/logPPP/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import datetime
-
-from ._ConsoleColors import ConsoleColors
-from ._util import *
-from .logPPPLevel import logPPPLevel
-
-__all__ = ['__version__', 'IS_COLOR', 'LEVEL', 'logPPPLevel', 'info', 'warning', 'error', 'debug', 'critical']
-__version__ = '1.1.1'
-
-# 是否开启颜色
-IS_COLOR = True
-# 等级
-LEVEL = logPPPLevel.INFO
-
-
-# 日志输出
-def _base(*args, sep=' ', end='\n', file=None, _level=logPPPLevel.INFO, color=ConsoleColors.RESET, is_color=True):
-    args = sep.join(map(str, args))
-    timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-    args = "{:<20} {:<8} {}  {}".format(timestamp, get_caller_file_basename_path(), _level.get('name'), args)
-    if is_color is None and IS_COLOR or is_color is True:
-        args = f"{color}{args}{ConsoleColors.RESET}"
-    if _level['level'] >= LEVEL['level']:
-        print(args, sep=sep, end=end, file=file)
-
-
-# info等级
-def info(*args, sep=' ', end='\n', file=None, is_color=None):
-    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.INFO, color=ConsoleColors.RESET, is_color=is_color)
-
-
-# warning等级
-def warning(*args, sep=' ', end='\n', file=None, is_color=None):
-    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.WARNING, color=ConsoleColors.YELLOW, is_color=is_color)
-
-
-# error等级
-def error(*args, sep=' ', end='\n', file=None, is_color=None):
-    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.ERROR, color=ConsoleColors.RED, is_color=is_color)
-
-
-# debug等级
-def debug(*args, sep=' ', end='\n', file=None, is_color=None):
-    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.DEBUG, color=ConsoleColors.RED, is_color=is_color)
-
-
-# critical等级
-def critical(*args, sep=' ', end='\n', file=None, is_color=None):
-    _base(*args, sep=sep, end=end, file=file, _level=logPPPLevel.CRITICAL, color=ConsoleColors.RED, is_color=is_color)
+import datetime
+
+from .__ConsoleColors__ import ConsoleColors
+from .__Level__ import Level
+from .__util__ import *
+
+__all__ = ['__version__', 'IS_COLOR', 'LEVEL', 'Level', 'info', 'warning', 'error', 'debug', 'critical']
+__version__ = '1.1.2'
+
+# 是否开启颜色
+IS_COLOR = True
+# 等级
+LEVEL = Level.INFO
+
+
+# 日志输出
+def _base(*args, sep=' ', end='\n', file=None, _level=Level.INFO, color=ConsoleColors.RESET, is_color=True):
+    args = sep.join(map(str, args))
+    timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    args = "{:<20} {:<8} {}  {}".format(timestamp, get_caller_file_basename_path(), _level.get('name'), args)
+    if is_color is None and IS_COLOR or is_color is True:
+        args = f"{color}{args}{ConsoleColors.RESET}"
+    if _level['level'] >= LEVEL['level']:
+        print(args, sep=sep, end=end, file=file)
+
+
+# info等级
+def info(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=Level.INFO, color=ConsoleColors.GREEN, is_color=is_color)
+
+
+# warning等级
+def warning(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=Level.WARNING, color=ConsoleColors.YELLOW, is_color=is_color)
+
+
+# error等级
+def error(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=Level.ERROR, color=ConsoleColors.RED, is_color=is_color)
+
+
+# debug等级
+def debug(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=Level.DEBUG, color=ConsoleColors.RED, is_color=is_color)
+
+
+# critical等级
+def critical(*args, sep=' ', end='\n', file=None, is_color=None):
+    _base(*args, sep=sep, end=end, file=file, _level=Level.CRITICAL, color=ConsoleColors.RED, is_color=is_color)
```

