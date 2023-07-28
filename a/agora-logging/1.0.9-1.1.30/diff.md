# Comparing `tmp/agora_logging-1.0.9-py2.py3-none-any.whl.zip` & `tmp/agora_logging-1.1.30-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 6488 bytes, number of entries: 12
--rw-r--r--  2.0 fat       67 b- defN 23-Feb-13 16:55 agora_logging/__init__.py
--rw-r--r--  2.0 fat     5933 b- defN 23-Jan-31 08:54 agora_logging/agora_logger.py
--rw-r--r--  2.0 fat     1618 b- defN 23-Feb-07 13:03 agora_logging/colored_text.py
--rw-r--r--  2.0 fat      993 b- defN 22-Dec-07 13:53 agora_logging/log_level.py
--rw-r--r--  2.0 fat       24 b- defN 23-Mar-16 20:19 agora_logging/version.py
--rw-r--r--  2.0 fat        0 b- defN 23-Jan-23 15:58 agora_logging/handlers/__init__.py
--rw-r--r--  2.0 fat     2824 b- defN 23-Feb-07 12:33 agora_logging/handlers/base_handler.py
--rw-r--r--  2.0 fat      895 b- defN 23-Jan-25 14:34 agora_logging/handlers/stream_handler.py
--rw-r--r--  2.0 fat      139 b- defN 23-Mar-07 09:10 agora_logging-1.0.9.dist-info/LICENSE
-?rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_logging-1.0.9.dist-info/WHEEL
-?rw-r--r--  2.0 fat      718 b- defN 16-Jan-01 00:00 agora_logging-1.0.9.dist-info/METADATA
-?rw-r--r--  2.0 fat     1008 b- defN 16-Jan-01 00:00 agora_logging-1.0.9.dist-info/RECORD
-12 files, 14318 bytes uncompressed, 4772 bytes compressed:  66.7%
+Zip file size: 6608 bytes, number of entries: 12
+-rw-r--r--  2.0 fat       67 b- defN 23-May-29 15:17 agora_logging/__init__.py
+-rw-r--r--  2.0 fat     6090 b- defN 23-May-12 13:38 agora_logging/agora_logger.py
+-rw-r--r--  2.0 fat     1612 b- defN 23-May-12 13:38 agora_logging/colored_text.py
+-rw-r--r--  2.0 fat      956 b- defN 23-May-12 13:38 agora_logging/log_level.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 11:19 agora_logging/version.py
+-rw-r--r--  2.0 fat        0 b- defN 23-May-12 13:38 agora_logging/handlers/__init__.py
+-rw-r--r--  2.0 fat     2824 b- defN 23-May-12 13:38 agora_logging/handlers/base_handler.py
+-rw-r--r--  2.0 fat      895 b- defN 23-May-12 13:38 agora_logging/handlers/stream_handler.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_logging-1.1.30.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_logging-1.1.30.dist-info/WHEEL
+-rw-r--r--  2.0 fat      898 b- defN 16-Jan-01 00:00 agora_logging-1.1.30.dist-info/METADATA
+-rw-r--r--  2.0 fat     1012 b- defN 16-Jan-01 00:00 agora_logging-1.1.30.dist-info/RECORD
+12 files, 14612 bytes uncompressed, 4884 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: agora_logging/handlers/base_handler.py
 Comment: 
 
 Filename: agora_logging/handlers/stream_handler.py
 Comment: 
 
-Filename: agora_logging-1.0.9.dist-info/LICENSE
+Filename: agora_logging-1.1.30.dist-info/LICENSE
 Comment: 
 
-Filename: agora_logging-1.0.9.dist-info/WHEEL
+Filename: agora_logging-1.1.30.dist-info/WHEEL
 Comment: 
 
-Filename: agora_logging-1.0.9.dist-info/METADATA
+Filename: agora_logging-1.1.30.dist-info/METADATA
 Comment: 
 
-Filename: agora_logging-1.0.9.dist-info/RECORD
+Filename: agora_logging-1.1.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_logging/agora_logger.py

```diff
@@ -1,35 +1,38 @@
 import sys
 from functools import wraps
 from inspect import currentframe, getframeinfo
 
 from .handlers.stream_handler import StreamHandler
 from .log_level import LogLevel
 
+
 def log_message(log_function):
     """
     Decorator that wraps context of the file and cast the message to str
     """
     @wraps(log_function)
-    def wrapper(self,message):
-        log_function(self,str(message))
+    def wrapper(self, message):
+        log_function(self, str(message))
     return wrapper
 
+
 class AgoraLogger():
     """
     Logger class 
 
     Returns:
         logger object: Singleton logger object
     """
-    loggers=[]
-    def __init__(self,level=None):
-        self.name="root"
+    loggers = []
+
+    def __init__(self, level=None):
+        self.name = "root"
         self.level = LogLevel.INFO if level is None else level
-        self.handler=StreamHandler(self.level)
+        self.handler = StreamHandler(self.level)
 
     def __str__(self):
         return f'''AgoraLogger<{self.name}>'''
 
     @classmethod
     def get_logger(cls):
         """
@@ -41,141 +44,146 @@
     def add_logger(cls):
         """
         Adds a new logger if it does not exist
 
         Returns:
             singleton logger
         """
-        if len(cls.loggers)>=1:
+        if len(cls.loggers) >= 1:
             return cls.loggers[0]
-        new_logger=AgoraLogger()
+        new_logger = AgoraLogger()
         cls.loggers.append(new_logger)
         return new_logger
 
-    def set_level(self,level):
+    def set_level(self, level):
         """
         Set the LogLevel of the logger
 
         Args:
             level (str|instance of loglevel): sets the LogLevel
         """
         if level == "":
             return
-        if isinstance(level,str):
-            level=LogLevel.from_string(level)
+        if isinstance(level, str):
+            level = LogLevel.from_string(level)
         if level is None:
-            self.write(LogLevel.ERROR,"Invalid value for verbosity")
+            self.write(LogLevel.ERROR, "Invalid value for verbosity")
         else:
-            self.level=level
-            self.handler.level=level
-
+            self.level = level
+            self.handler.level = level
 
-    def write_log(self,frame_info,log,level):
-        stream=sys.stdout
-        self.handler.write(stream,frame_info,log,level)
+    def write_log(self, frame_info, log, level):
+        self.handler.write(sys.stdout, frame_info, log, level)
 
-    def write_exception_log(self,exception_message):
-        stream=sys.stdout
-        self.handler.write_to_stream(exception_message,stream)
-
-    def write(self,level,message):
-        if not isinstance(level,LogLevel):
-            self.write(LogLevel.ERROR,f'''Expected an instance of Verbosity, received {type(level)}''')
+    def write_exception_log(self, exception_message):
+        self.handler.write_to_stream(exception_message, sys.stdout)
+        sys.stdout.flush()
+
+    def write(self, level, message):
+        if not isinstance(level, LogLevel):
+            self.write(
+                LogLevel.ERROR, f'''Expected an instance of Verbosity, received {type(level)}''')
             return 0
-        message=str(message)
+        message = str(message)
         frameinfo = getframeinfo(currentframe().f_back)
-        self.write_log(frameinfo,message,level)
+        self.write_log(frameinfo, message, level)
 
-    def exception(self,exception,message,level=LogLevel.WARN):
-        if not isinstance(level,LogLevel):
-            self.write(LogLevel.ERROR,f'''Expected an instance of Verbosity, received {type(level)}''')
+    def exception(self, ex, message, level=LogLevel.WARN):
+        if not isinstance(level, LogLevel):
+            self.write(
+                LogLevel.ERROR, f'''Expected an instance of LogLevel, received {type(level)}''')
             return 0
-        if not isinstance(exception,Exception):
-            self.write(LogLevel.ERROR,f'''Expected an instance of Exception, received {type(exception)}''')
+        if not isinstance(ex, Exception):
+            self.write(
+                LogLevel.ERROR, f'''Expected an instance of Exception, received {type(ex)}''')
             return 0
-        message=str(message)
+        message = str(message)
         frameinfo = getframeinfo(currentframe().f_back)
-        self.write_log(frameinfo,message,level)
-        self.write_exception_log(str(exception)+"\n")
+        self.write_log(frameinfo, message, level)
+        self.write_exception_log(str(ex)+"\n")
 
-    def write_unhandled_exception(self,exception,message,frameinfo):
-        if not isinstance(exception,Exception):
-            if isinstance(exception,KeyboardInterrupt):
-                self.write(LogLevel.INFO, '''Received keyboard interrupt . Exiting..''')
+    def write_unhandled_exception(self, ex, message, frameinfo):
+        if not isinstance(ex, Exception):
+            if isinstance(ex, KeyboardInterrupt):
+                self.write(LogLevel.INFO,
+                           '''Received keyboard interrupt . Exiting..''')
                 return 0
-            self.write(LogLevel.ERROR,f'''Expected an instance of Exception, received {type(exception)}''')
+            self.write(
+                LogLevel.ERROR, f'''Expected an instance of Exception, received {type(ex)}''')
             return 0
-        if not isinstance(message,str):
-            self.write(LogLevel.ERROR,f'''Expected an instance of String, received {type(message)}''')
+        if not isinstance(message, str):
+            self.write(
+                LogLevel.ERROR, f'''Expected an instance of String, received {type(message)}''')
             return 0
-        self.write_log(frameinfo,message,LogLevel.WARN)
-        self.write_exception_log(str(exception)+"\n")
+        self.write_log(frameinfo, message, LogLevel.WARN)
+        if self.level != LogLevel.OFF:
+            self.write_exception_log(str(ex)+"\n")
 
     @log_message
-    def heading(self,message):
+    def heading(self, message):
         """Writes a heading message to the log
 
         Args:
             message (str): the message"""
-        message=str(message)
+        message = str(message)
         frameinfo = getframeinfo(currentframe().f_back)
-        self.handler.heading(frameinfo,message)
-    
+        self.handler.heading(frameinfo, message)
+
     @log_message
-    def trace(self,message):
+    def trace(self, message):
         """Writes a trace (LogLevel.TRACE) message to the log
 
         Args:
             message (str): the message"""
         frameinfo = getframeinfo(currentframe().f_back.f_back)
-        self.write_log(frameinfo,message,LogLevel.TRACE)
-    
+        self.write_log(frameinfo, message, LogLevel.TRACE)
+
     @log_message
-    def debug(self,message):
+    def debug(self, message):
         """Writes a debug (LogLevel.DEBUG) message to the log
 
         Args:
             message (str): the message"""
         frameinfo = getframeinfo(currentframe().f_back.f_back)
-        self.write_log(frameinfo,message,LogLevel.DEBUG)
+        self.write_log(frameinfo, message, LogLevel.DEBUG)
 
     @log_message
-    def error(self,message):
+    def error(self, message):
         """Writes an error (LogLevel.ERROR) message to the log
 
         Args:
             message (str): the message"""
         frameinfo = getframeinfo(currentframe().f_back.f_back)
-        self.write_log(frameinfo,message,LogLevel.ERROR)
+        self.write_log(frameinfo, message, LogLevel.ERROR)
 
     @log_message
-    def warn(self,message):
+    def warn(self, message):
         """Writes a warning (LogLevel.WARN) message to the log
 
         Args:
             message (str): the message"""
         frameinfo = getframeinfo(currentframe().f_back.f_back)
-        self.write_log(frameinfo,message,LogLevel.WARN)
+        self.write_log(frameinfo, message, LogLevel.WARN)
 
     @log_message
-    def info(self,message):
+    def info(self, message):
         """Writes a informational (LogLevel.INFO) message to the log
 
         Args:
             message (str): the message"""
         frameinfo = getframeinfo(currentframe().f_back.f_back)
-        self.write_log(frameinfo,message,LogLevel.INFO)
+        self.write_log(frameinfo, message, LogLevel.INFO)
 
     @log_message
-    def fatal(self,message):
+    def fatal(self, message):
         """Writes a fatal (LogLevel.FATAL) message to the log
 
         Args:
             message (str): the message"""
         frameinfo = getframeinfo(currentframe().f_back.f_back)
-        self.write_log(frameinfo,message,LogLevel.FATAL)
+        self.write_log(frameinfo, message, LogLevel.FATAL)
 
 
 logger = AgoraLogger.get_logger()
 log_verbosity = LogLevel.INFO
 if log_verbosity is not None:
-    logger.set_level(log_verbosity)  
+    logger.set_level(log_verbosity)
```

## agora_logging/colored_text.py

```diff
@@ -8,58 +8,59 @@
 #  integer      (Style Enum)
 #  ;            Separator
 #  3 + integer  integer = Foreground Color (Color Enum)
 #  ;            Separator
 #  4 + integer  integer = Background Color (Color Enum)
 #  m            Stopper
 
+
 class Style(Enum):
     Normal = 0
     Bold = 1
     Light = 2
     Italicized = 3
     Underlined = 4
     Blink = 5
 
+
 class Color(Enum):
     Black = 0
     Red = 1
     Green = 2
     Yellow = 3
     Blue = 4
     Purple = 5
     Cyan = 6
     White = 7
     Default = 9
 
+
 class ColoredText:
     '''
     Color value for logging
     '''
     @staticmethod
     def gray(msg):
         return ColoredText.message(msg, Style.Bold, Color.Black)
-    
+
     @staticmethod
     def green(msg):
         return ColoredText.message(msg, Style.Bold, Color.Green)
 
     @staticmethod
     def dark_red(msg):
         return ColoredText.message(msg, Style.Bold, Color.White, Color.Red)
 
     @staticmethod
     def yellow(msg):
         return ColoredText.message(msg, Style.Normal, Color.Black, Color.Yellow)
-    
+
     @staticmethod
     def red(msg):
         return ColoredText.message(msg, Style.Normal, Color.Black, Color.Red)
 
     @staticmethod
     def message(message: str, style: Style, fg_color: Color, bg_color: Color = Color.Default):
         style_str = str(style.value)
         fg_color_str = ';3' + str(fg_color.value)
         bg_color_str = ';4' + str(bg_color.value)
         return '\x1b[' + style_str + fg_color_str + bg_color_str + 'm' + message.strip() + '\x1b[0m\n'
-
-
```

## agora_logging/log_level.py

```diff
@@ -1,31 +1,25 @@
-'''
-Enum for verbosity
-'''
-
 import enum
 
 
 class LogLevel(enum.IntEnum):
     '''
     verbosity
     '''
-    TRACE = 0, # Trace level - used for the finest level of debugging 
-    DEBUG = 1, # Debug level - used for debugging - specifically log values that should not go to Release     
-    INFO = 2,  # Info level - general logging information - filename, line number,  and method are not included 
-    WARN = 3,  # Warning level - indicates something is not happening as expected 
-    ERROR = 4, # Error level - indicates an error occurred, but not fatally 
-    FATAL = 5, # Fatal level - generally used just before the application gives up
+    TRACE = 0,  # Trace level - used for the finest level of debugging
+    DEBUG = 1,  # Debug level - used for debugging - specifically log values that should not go to Release
+    INFO = 2,  # Info level - general logging information - filename, line number,  and method are not included
+    WARN = 3,  # Warning level - indicates something is not happening as expected
+    ERROR = 4,  # Error level - indicates an error occurred, but not fatally
+    FATAL = 5,  # Fatal level - generally used just before the application gives up
     OFF = 6    # Off Level - no logging will be produced at this level
 
     @classmethod
-    def from_string(cls,level):
+    def from_string(cls, level):
         '''
         convert text to enum value
         '''
-        level=level.upper()
+        level = level.upper()
         if level in cls._member_names_:
             return LogLevel[level]
         else:
             return None
-
-
```

## agora_logging/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.9'
+__version__ = '1.1.30'
```

## Comparing `agora_logging-1.0.9.dist-info/METADATA` & `agora_logging-1.1.30.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 Metadata-Version: 2.1
 Name: agora_logging
-Version: 1.0.9
+Version: 1.1.30
 Summary: Logging libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://agoraiot.github.io
 
 
 # agora_logging
 
 This package is the Logging library for the Agora Edge Apps SDK (Python) developed by SLB.
 
-Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](http://agoraiot.github.io).
+Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.0.20
+
+- Fix message about Verbosity instead of LogLevel
+- Force flush of sys.stdout when writing exception logs
+
+### v1.0.18
+
+- Make versions of all modules all the same
+
 ### v1.0.7 - Beta
 
 - Initial test release.
```

## Comparing `agora_logging-1.0.9.dist-info/RECORD` & `agora_logging-1.1.30.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 agora_logging/__init__.py,sha256=PPi6BVmhWVjdeOMQYg-FEj51McSHrNif9p05X9otteo,67
-agora_logging/agora_logger.py,sha256=lpTlV7nZia8G_0jU4xGkJ6pA1cdrd6ve1K_jcNAaV0o,5933
-agora_logging/colored_text.py,sha256=b2sPEecFHco5Nye5EmqUK3sOJqVUBtwPADf9-rlZQD8,1618
-agora_logging/log_level.py,sha256=sNp1II2mLhfRoWyVOrXGbraoJJujY245xLzAgtRRImY,993
-agora_logging/version.py,sha256=-nHdmfbrEEZoCUg1nFNZBjmdzMhPwWALABnXcptli_o,24
+agora_logging/agora_logger.py,sha256=crxU0isyWJOn5qfRqNkEs4KGLOQnns9oy99Uvm4Fywc,6090
+agora_logging/colored_text.py,sha256=EpksqRhjUz1clYH4YZWqnYUAvbSaETtJya6PxFZAat0,1612
+agora_logging/log_level.py,sha256=eDrfcKgYdHQrF1q34-McZnEhuhW2T2u1HyMpwRTbiWQ,956
+agora_logging/version.py,sha256=kY1O3TourfpBaahGTuaQtrU_kHRo-l8s0QqCEsehNGc,25
 agora_logging/handlers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 agora_logging/handlers/base_handler.py,sha256=rEfP6S3PZL8TsYX1qISy5kCYHQpS3Le9toV2itWQqzc,2824
 agora_logging/handlers/stream_handler.py,sha256=jX4zNGMHlHgSiXuq8-1MZ_Nx2-2q6xp_vtO23OPrELE,895
-agora_logging-1.0.9.dist-info/LICENSE,sha256=0FV-B2w7SRxv5WB_RriZppfctNE6t4pLFm_BUw2Ajcw,139
-agora_logging-1.0.9.dist-info/WHEEL,sha256=kdeDBNPvBI0w3meLKPoGgAnEr54n1jzrZWUoaLmGzVY,99
-agora_logging-1.0.9.dist-info/METADATA,sha256=YbviV0LLcTU1aFGVolNGRv4A6LRmcDQNEwQZmrPKSaI,718
-agora_logging-1.0.9.dist-info/RECORD,,
+agora_logging-1.1.30.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_logging-1.1.30.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_logging-1.1.30.dist-info/METADATA,sha256=R2IwZdV-07Lum9eqAsH9kYE2n6hl_DEzidbcrghwXFw,898
+agora_logging-1.1.30.dist-info/RECORD,,
```

