# Comparing `tmp/agoraiot-1.1.31-py2.py3-none-any.whl.zip` & `tmp/agoraiot-1.1.32-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2044 bytes, number of entries: 6
--rw-r--r--  2.0 fat      329 b- defN 23-Jul-20 18:48 agoraiot/__init__.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 12:13 agoraiot/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agoraiot-1.1.31.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agoraiot-1.1.31.dist-info/WHEEL
--rw-r--r--  2.0 fat      974 b- defN 16-Jan-01 00:00 agoraiot-1.1.31.dist-info/METADATA
--rw-r--r--  2.0 fat      450 b- defN 16-Jan-01 00:00 agoraiot-1.1.31.dist-info/RECORD
-6 files, 2011 bytes uncompressed, 1228 bytes compressed:  38.9%
+Zip file size: 2052 bytes, number of entries: 6
+-rw-r--r--  2.0 fat      346 b- defN 23-Jul-28 12:34 agoraiot/__init__.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 12:37 agoraiot/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agoraiot-1.1.32.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agoraiot-1.1.32.dist-info/WHEEL
+-rw-r--r--  2.0 fat      974 b- defN 16-Jan-01 00:00 agoraiot-1.1.32.dist-info/METADATA
+-rw-r--r--  2.0 fat      450 b- defN 16-Jan-01 00:00 agoraiot-1.1.32.dist-info/RECORD
+6 files, 2028 bytes uncompressed, 1236 bytes compressed:  39.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: agoraiot/__init__.py
 Comment: 
 
 Filename: agoraiot/version.py
 Comment: 
 
-Filename: agoraiot-1.1.31.dist-info/LICENSE
+Filename: agoraiot-1.1.32.dist-info/LICENSE
 Comment: 
 
-Filename: agoraiot-1.1.31.dist-info/WHEEL
+Filename: agoraiot-1.1.32.dist-info/WHEEL
 Comment: 
 
-Filename: agoraiot-1.1.31.dist-info/METADATA
+Filename: agoraiot-1.1.32.dist-info/METADATA
 Comment: 
 
-Filename: agoraiot-1.1.31.dist-info/RECORD
+Filename: agoraiot-1.1.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agoraiot/__init__.py

```diff
@@ -1,6 +1,5 @@
 from agora_busclient import IoDataReportMsg, IoPoint, RequestMsg, \
-      bus_client, IoPoint, IoDeviceData, IoTagDataDict, MessageHeader, EventMsg
+      bus_client, IoPoint, IoDeviceData, IoTagDataDict, MessageHeader, EventMsg, MediaData, WorkFlow
 from agora_utils import AgoraTimeStamp, UTCDateTime
 from agora_config import config, DictOfDict, config_overrides, config_defaults
-from agora_logging import logger, LogLevel
-
+from agora_logging import logger, LogLevel
```

## agoraiot/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.31'
+__version__ = '1.1.32'
```

## Comparing `agoraiot-1.1.31.dist-info/METADATA` & `agoraiot-1.1.32.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: agoraiot
-Version: 1.1.31
+Version: 1.1.32
 Summary: AgoraIoT Python Libraries
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.31
-Requires-Dist: agora_busclient == 1.1.31
-Requires-Dist: agora_config == 1.1.31
-Requires-Dist: agora_redis_client == 1.1.31
-Requires-Dist: agora_utils == 1.1.31
+Requires-Dist: agora_logging == 1.1.32
+Requires-Dist: agora_busclient == 1.1.32
+Requires-Dist: agora_config == 1.1.32
+Requires-Dist: agora_redis_client == 1.1.32
+Requires-Dist: agora_utils == 1.1.32
 Project-URL: Documentation, https://agoraiot.github.io
 Project-URL: Home, https://www.agoraiot.com
 
 # agoraiot
 
 This primary package for the entire Agora Edge Apps SDK (Python) developed by SLB.
```

