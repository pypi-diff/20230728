# Comparing `tmp/agora_logging-1.1.35-py2.py3-none-any.whl.zip` & `tmp/agora_logging-1.1.36-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
 Zip file size: 6609 bytes, number of entries: 12
 -rw-r--r--  2.0 fat       67 b- defN 23-May-29 15:17 agora_logging/__init__.py
 -rw-r--r--  2.0 fat     6090 b- defN 23-May-12 13:38 agora_logging/agora_logger.py
 -rw-r--r--  2.0 fat     1612 b- defN 23-May-12 13:38 agora_logging/colored_text.py
 -rw-r--r--  2.0 fat      956 b- defN 23-May-12 13:38 agora_logging/log_level.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 16:38 agora_logging/version.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 19:32 agora_logging/version.py
 -rw-r--r--  2.0 fat        0 b- defN 23-May-12 13:38 agora_logging/handlers/__init__.py
 -rw-r--r--  2.0 fat     2824 b- defN 23-May-12 13:38 agora_logging/handlers/base_handler.py
 -rw-r--r--  2.0 fat      895 b- defN 23-May-12 13:38 agora_logging/handlers/stream_handler.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_logging-1.1.35.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_logging-1.1.35.dist-info/WHEEL
--rw-r--r--  2.0 fat      898 b- defN 16-Jan-01 00:00 agora_logging-1.1.35.dist-info/METADATA
--rw-r--r--  2.0 fat     1012 b- defN 16-Jan-01 00:00 agora_logging-1.1.35.dist-info/RECORD
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_logging-1.1.36.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_logging-1.1.36.dist-info/WHEEL
+-rw-r--r--  2.0 fat      898 b- defN 16-Jan-01 00:00 agora_logging-1.1.36.dist-info/METADATA
+-rw-r--r--  2.0 fat     1012 b- defN 16-Jan-01 00:00 agora_logging-1.1.36.dist-info/RECORD
 12 files, 14612 bytes uncompressed, 4885 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: agora_logging/handlers/base_handler.py
 Comment: 
 
 Filename: agora_logging/handlers/stream_handler.py
 Comment: 
 
-Filename: agora_logging-1.1.35.dist-info/LICENSE
+Filename: agora_logging-1.1.36.dist-info/LICENSE
 Comment: 
 
-Filename: agora_logging-1.1.35.dist-info/WHEEL
+Filename: agora_logging-1.1.36.dist-info/WHEEL
 Comment: 
 
-Filename: agora_logging-1.1.35.dist-info/METADATA
+Filename: agora_logging-1.1.36.dist-info/METADATA
 Comment: 
 
-Filename: agora_logging-1.1.35.dist-info/RECORD
+Filename: agora_logging-1.1.36.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_logging/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.35'
+__version__ = '1.1.36'
```

## Comparing `agora_logging-1.1.35.dist-info/METADATA` & `agora_logging-1.1.36.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agora_logging
-Version: 1.1.35
+Version: 1.1.36
 Summary: Logging libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://agoraiot.github.io
```

