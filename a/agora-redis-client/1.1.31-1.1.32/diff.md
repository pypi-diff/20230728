# Comparing `tmp/agora_redis_client-1.1.31-py2.py3-none-any.whl.zip` & `tmp/agora_redis_client-1.1.32-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2643 bytes, number of entries: 7
+Zip file size: 2644 bytes, number of entries: 7
 -rw-r--r--  2.0 fat       31 b- defN 23-Jun-14 11:28 agora_redis_client/__init__.py
 -rw-r--r--  2.0 fat     1325 b- defN 23-Jun-14 11:28 agora_redis_client/redis_client.py
--rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 12:13 agora_redis_client/version.py
--rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.1.31.dist-info/LICENSE
--rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.31.dist-info/WHEEL
--rw-r--r--  2.0 fat      824 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.31.dist-info/METADATA
--rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.31.dist-info/RECORD
-7 files, 3035 bytes uncompressed, 1563 bytes compressed:  48.5%
+-rw-r--r--  2.0 fat       25 b- defN 23-Jul-28 12:37 agora_redis_client/version.py
+-rw-r--r--  2.0 fat      131 b- defN 23-Jun-14 11:28 agora_redis_client-1.1.32.dist-info/LICENSE
+-rw-r--r--  2.0 fat       99 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.32.dist-info/WHEEL
+-rw-r--r--  2.0 fat      824 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.32.dist-info/METADATA
+-rw-r--r--  2.0 fat      600 b- defN 16-Jan-01 00:00 agora_redis_client-1.1.32.dist-info/RECORD
+7 files, 3035 bytes uncompressed, 1564 bytes compressed:  48.5%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: agora_redis_client/redis_client.py
 Comment: 
 
 Filename: agora_redis_client/version.py
 Comment: 
 
-Filename: agora_redis_client-1.1.31.dist-info/LICENSE
+Filename: agora_redis_client-1.1.32.dist-info/LICENSE
 Comment: 
 
-Filename: agora_redis_client-1.1.31.dist-info/WHEEL
+Filename: agora_redis_client-1.1.32.dist-info/WHEEL
 Comment: 
 
-Filename: agora_redis_client-1.1.31.dist-info/METADATA
+Filename: agora_redis_client-1.1.32.dist-info/METADATA
 Comment: 
 
-Filename: agora_redis_client-1.1.31.dist-info/RECORD
+Filename: agora_redis_client-1.1.32.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## agora_redis_client/version.py

```diff
@@ -1 +1 @@
-__version__ = '1.1.31'
+__version__ = '1.1.32'
```

## Comparing `agora_redis_client-1.1.31.dist-info/METADATA` & `agora_redis_client-1.1.32.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: agora_redis_client
-Version: 1.1.31
+Version: 1.1.32
 Summary: Redis Client for the Agora Edge Apps SDK 2.0 (Python)
 Author-email: AgoraIoT <agoraiot@slb.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Dist: agora_logging == 1.1.31
-Requires-Dist: agora_config == 1.1.31
+Requires-Dist: agora_logging == 1.1.32
+Requires-Dist: agora_config == 1.1.32
 Requires-Dist: redis
 Project-URL: Home, https://slb-edge.github.io
 
 
 # agora_redisclient
 
 This package is the Redis Client for the Agora Edge Apps SDK (Python) developed by SLB.
```

## Comparing `agora_redis_client-1.1.31.dist-info/RECORD` & `agora_redis_client-1.1.32.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 agora_redis_client/__init__.py,sha256=nIxsBty2jHDz3mqsvyOPRhUZoo6FtNNvfkNph7C4F4U,31
 agora_redis_client/redis_client.py,sha256=HYHn-q2svKm8mcFKb7dShYi92myrX8Gz9hpus3nDIDY,1325
-agora_redis_client/version.py,sha256=m6Gwb-2J7qH0YItWdRx6poaAJYM2sVamUx_y8wEEcbI,25
-agora_redis_client-1.1.31.dist-info/LICENSE,sha256=2RSWN0z_ADMOpyELJ0aJpy2UKIuZOOdYq0PpxyllwlA,131
-agora_redis_client-1.1.31.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
-agora_redis_client-1.1.31.dist-info/METADATA,sha256=jWnDqm3Vrx8XooWC213BsfZbTNU6LulIXpt4ruCnmSw,824
-agora_redis_client-1.1.31.dist-info/RECORD,,
+agora_redis_client/version.py,sha256=g0EmYAMzvboJ32TdMNLZcoLdC3TIhGHXLgf4Ivquuds,25
+agora_redis_client-1.1.32.dist-info/LICENSE,sha256=2RSWN0z_ADMOpyELJ0aJpy2UKIuZOOdYq0PpxyllwlA,131
+agora_redis_client-1.1.32.dist-info/WHEEL,sha256=Sgu64hAMa6g5FdzHxXv9Xdse9yxpGGMeagVtPMWpJQY,99
+agora_redis_client-1.1.32.dist-info/METADATA,sha256=HVtJ98MdNNFPKxo91Z4ESPpqeJq3rSJ_HoiDzAMjifA,824
+agora_redis_client-1.1.32.dist-info/RECORD,,
```

