# Comparing `tmp/agoraiot-1.0.9-py2.py3-none-any.whl.zip` & `tmp/agoraiot-1.1.30-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 1970 bytes, number of entries: 6
--rw-r--r--  2.0 fat      304 b- defN 23-Feb-13 17:21 agoraiot/__init__.py
--rw-r--r--  2.0 fat       24 b- defN 23-Mar-16 20:19 agoraiot/version.py
--rw-r--r--  2.0 fat      139 b- defN 23-Mar-07 09:10 agoraiot-1.0.9.dist-info/LICENSE
-?rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agoraiot-1.0.9.dist-info/WHEEL
-?rw-r--r--  2.0 fat      835 b- defN 16-Jan-01 00:00 agoraiot-1.0.9.dist-info/METADATA
-?rw-r--r--  2.0 fat      446 b- defN 16-Jan-01 00:00 agoraiot-1.0.9.dist-info/RECORD
-6 files, 1847 bytes uncompressed, 1162 bytes compressed:  37.1%
+Zip file size: 2042 bytes, number of entries: 6
+-rw-r--r--  2.0 fat      329 b- defN 23-Jul-20 18:48 agoraiot/__init__.py
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 11:19 agoraiot/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agoraiot-1.1.30.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agoraiot-1.1.30.dist-info/WHEEL
+-rw-r--r--  2.0 fat      974 b- defN 16-Jan-01 00:00 agoraiot-1.1.30.dist-info/METADATA
+-rw-r--r--  2.0 fat      450 b- defN 16-Jan-01 00:00 agoraiot-1.1.30.dist-info/RECORD
+6 files, 2011 bytes uncompressed, 1226 bytes compressed:  39.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: agoraiot/__init__.py
 Comment: 
 
 Filename: agoraiot/version.py
 Comment: 
 
-Filename: agoraiot-1.0.9.dist-info/LICENSE
+Filename: agoraiot-1.1.30.dist-info/LICENSE
 Comment: 
 
-Filename: agoraiot-1.0.9.dist-info/WHEEL
+Filename: agoraiot-1.1.30.dist-info/WHEEL
 Comment: 
 
-Filename: agoraiot-1.0.9.dist-info/METADATA
+Filename: agoraiot-1.1.30.dist-info/METADATA
 Comment: 
 
-Filename: agoraiot-1.0.9.dist-info/RECORD
+Filename: agoraiot-1.1.30.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agoraiot/__init__.py

```diff
@@ -1,6 +1,6 @@
 from agora_busclient import IoDataReportMsg, IoPoint, RequestMsg, \
-      bus_client, IoPoint, IoDeviceData, IoTagDataDict
+      bus_client, IoPoint, IoDeviceData, IoTagDataDict, MessageHeader, EventMsg
 from agora_utils import AgoraTimeStamp, UTCDateTime
 from agora_config import config, DictOfDict, config_overrides, config_defaults
 from agora_logging import logger, LogLevel
```

## agoraiot/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.0.9'
+__version__ = '1.1.30'
```

## Comparing `agoraiot-1.0.9.dist-info/METADATA` & `agoraiot-1.1.30.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 Metadata-Version: 2.1
 Name: agoraiot
-Version: 1.0.9
+Version: 1.1.30
 Summary: AgoraIoT Python Libraries
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging
-Requires-Dist: agora_busclient
-Requires-Dist: agora_config
-Requires-Dist: agora_utils
+Requires-Dist: agora_logging == 1.1.30
+Requires-Dist: agora_busclient == 1.1.30
+Requires-Dist: agora_config == 1.1.30
+Requires-Dist: agora_redis_client == 1.1.30
+Requires-Dist: agora_utils == 1.1.30
 Project-URL: Documentation, https://agoraiot.github.io
 Project-URL: Home, https://www.agoraiot.com
 
-
 # agoraiot
 
 This primary package for the entire Agora Edge Apps SDK (Python) developed by SLB.
 
-Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](http://agoraiot.github.io).
+Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
 
 ## Release Notes
 
+### v1.0.18
+
+- Make versions of all modules the same
+
 ### v1.0.7 - Beta
 
 - Initial test release.
```

