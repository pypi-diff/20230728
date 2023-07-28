# Comparing `tmp/agora_config-1.1.32-py2.py3-none-any.whl.zip` & `tmp/agora_config-1.1.33-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -3,13 +3,13 @@
 -rw-r--r--  2.0 fat     5994 b- defN 23-Jun-30 14:21 agora_config/agora_config.py
 -rw-r--r--  2.0 fat      540 b- defN 23-May-12 13:38 agora_config/command_line_provider.py
 -rw-r--r--  2.0 fat     2283 b- defN 23-May-12 13:38 agora_config/dict_of_dict.py
 -rw-r--r--  2.0 fat      410 b- defN 23-May-12 13:38 agora_config/environment_variable_provider.py
 -rw-r--r--  2.0 fat     3164 b- defN 23-May-12 13:38 agora_config/file_key_provider.py
 -rw-r--r--  2.0 fat     1974 b- defN 23-May-18 11:05 agora_config/file_provider.py
 -rw-r--r--  2.0 fat      550 b- defN 23-May-12 13:38 agora_config/last_value_callbacks.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 12:37 agora_config/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.32.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.32.dist-info/WHEEL
--rw-r--r--  2.0 fat     1847 b- defN 16-Jan-01 00:00 agora_config-1.1.32.dist-info/METADATA
--rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.32.dist-info/RECORD
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 13:00 agora_config/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_config-1.1.33.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_config-1.1.33.dist-info/WHEEL
+-rw-r--r--  2.0 fat     1847 b- defN 16-Jan-01 00:00 agora_config-1.1.33.dist-info/METADATA
+-rw-r--r--  2.0 fat     1107 b- defN 16-Jan-01 00:00 agora_config-1.1.33.dist-info/RECORD
 13 files, 18232 bytes uncompressed, 6139 bytes compressed:  66.3%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: agora_config/last_value_callbacks.py
 Comment: 
 
 Filename: agora_config/version.py
 Comment: 
 
-Filename: agora_config-1.1.32.dist-info/LICENSE
+Filename: agora_config-1.1.33.dist-info/LICENSE
 Comment: 
 
-Filename: agora_config-1.1.32.dist-info/WHEEL
+Filename: agora_config-1.1.33.dist-info/WHEEL
 Comment: 
 
-Filename: agora_config-1.1.32.dist-info/METADATA
+Filename: agora_config-1.1.33.dist-info/METADATA
 Comment: 
 
-Filename: agora_config-1.1.32.dist-info/RECORD
+Filename: agora_config-1.1.33.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_config/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.32'
+__version__ = '1.1.33'
```

## Comparing `agora_config-1.1.32.dist-info/METADATA` & `agora_config-1.1.33.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: agora_config
-Version: 1.1.32
+Version: 1.1.33
 Summary: Configuration libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.32
+Requires-Dist: agora_logging == 1.1.33
 Project-URL: Home, https://agoraiot.github.io
 
 # agora_config
 
 This package is the Configuration library for the Agora Edge Apps SDK (Python) developed by SLB.
 
 Use this SDK to construct an edge application, and then containerize it for the running on the edge with AgoraIoT.  Documentation on using the entire SDK can be found at: [AgoraIoT SDK Documentation](https://slb-edge.github.io).
```

