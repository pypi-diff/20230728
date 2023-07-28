# Comparing `tmp/agora_utils-1.1.32-py2.py3-none-any.whl.zip` & `tmp/agora_utils-1.1.33-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2561 bytes, number of entries: 8
+Zip file size: 2562 bytes, number of entries: 8
 -rw-r--r--  2.0 fat       75 b- defN 23-May-12 13:38 agora_utils/__init__.py
 -rw-r--r--  2.0 fat       23 b- defN 23-May-12 13:38 agora_utils/_version.py
 -rw-r--r--  2.0 fat      521 b- defN 23-Jul-27 17:24 agora_utils/agora_time.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 12:37 agora_utils/version.py
--rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_utils-1.1.32.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_utils-1.1.32.dist-info/WHEEL
--rw-r--r--  2.0 fat      880 b- defN 16-Jan-01 00:00 agora_utils-1.1.32.dist-info/METADATA
--rw-r--r--  2.0 fat      626 b- defN 16-Jan-01 00:00 agora_utils-1.1.32.dist-info/RECORD
-8 files, 2383 bytes uncompressed, 1461 bytes compressed:  38.7%
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 13:00 agora_utils/version.py
+-rw-r--r--  2.0 fat      134 b- defN 23-Jun-14 11:28 agora_utils-1.1.33.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_utils-1.1.33.dist-info/WHEEL
+-rw-r--r--  2.0 fat      880 b- defN 16-Jan-01 00:00 agora_utils-1.1.33.dist-info/METADATA
+-rw-r--r--  2.0 fat      626 b- defN 16-Jan-01 00:00 agora_utils-1.1.33.dist-info/RECORD
+8 files, 2383 bytes uncompressed, 1462 bytes compressed:  38.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: agora_utils/agora_time.py
 Comment: 
 
 Filename: agora_utils/version.py
 Comment: 
 
-Filename: agora_utils-1.1.32.dist-info/LICENSE
+Filename: agora_utils-1.1.33.dist-info/LICENSE
 Comment: 
 
-Filename: agora_utils-1.1.32.dist-info/WHEEL
+Filename: agora_utils-1.1.33.dist-info/WHEEL
 Comment: 
 
-Filename: agora_utils-1.1.32.dist-info/METADATA
+Filename: agora_utils-1.1.33.dist-info/METADATA
 Comment: 
 
-Filename: agora_utils-1.1.32.dist-info/RECORD
+Filename: agora_utils-1.1.33.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_utils/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.32'
+__version__ = '1.1.33'
```

## Comparing `agora_utils-1.1.32.dist-info/METADATA` & `agora_utils-1.1.33.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agora_utils
-Version: 1.1.32
+Version: 1.1.33
 Summary: Utilities libraries for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Project-URL: Home, https://agoraiot.github.io
```

## Comparing `agora_utils-1.1.32.dist-info/RECORD` & `agora_utils-1.1.33.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 agora_utils/__init__.py,sha256=bMi6zdciwSmg3ZDZCOfzQCUHMYaxcHk1GvAL_i2zh0s,75
 agora_utils/_version.py,sha256=kwEyWwKLIIqYSnkf5eXgPtRgw9Bz51riSupwtvDpJMA,23
 agora_utils/agora_time.py,sha256=3vMrPf5MGRQdXqqXxLEwcAv-jH1jcctgeEU-Nbo0d4Q,521
-agora_utils/version.py,sha256=g0EmYAMzvboJ32TdMNLZcoLdC3TIhGHXLgf4Ivquuds,25
-agora_utils-1.1.32.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
-agora_utils-1.1.32.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_utils-1.1.32.dist-info/METADATA,sha256=vHPfX9FUq8yS-YpAtijHTD8Qi_2FqHwLJCyIWfW4zsU,880
-agora_utils-1.1.32.dist-info/RECORD,,
+agora_utils/version.py,sha256=EScuLwcq-3hy2HikwoaxRp9r-IW-958r6RvFXuDxof4,25
+agora_utils-1.1.33.dist-info/LICENSE,sha256=R-TdODMyhPUhIFgVHS3Y973VNriIq35ZLKQ6iTN2ySo,134
+agora_utils-1.1.33.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_utils-1.1.33.dist-info/METADATA,sha256=YVK8LPNht578wtaNXorinuEa_ht6Uih3SyhadjdnKWc,880
+agora_utils-1.1.33.dist-info/RECORD,,
```

