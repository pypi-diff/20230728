# Comparing `tmp/importTime-1.0.0-py2.py3-none-any.whl.zip` & `tmp/importTime-1.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6327 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 23:21 importTime/__init__.py
--rw-r--r--  2.0 unx     1445 b- defN 23-Jul-27 23:21 importTime/importTime.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-27 23:21 importTime-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      848 b- defN 23-Jul-27 23:21 importTime-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Jul-27 23:21 importTime-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-27 23:21 importTime-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      563 b- defN 23-Jul-27 23:21 importTime-1.0.0.dist-info/RECORD
-7 files, 14334 bytes uncompressed, 5325 bytes compressed:  62.9%
+Zip file size: 6340 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-27 23:28 importTime/__init__.py
+-rw-r--r--  2.0 unx     1445 b- defN 23-Jul-27 23:28 importTime/importTime.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      866 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      563 b- defN 23-Jul-27 23:28 importTime-1.0.1.dist-info/RECORD
+7 files, 14352 bytes uncompressed, 5338 bytes compressed:  62.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: importTime/__init__.py
 Comment: 
 
 Filename: importTime/importTime.py
 Comment: 
 
-Filename: importTime-1.0.0.dist-info/LICENSE.txt
+Filename: importTime-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: importTime-1.0.0.dist-info/METADATA
+Filename: importTime-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: importTime-1.0.0.dist-info/WHEEL
+Filename: importTime-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: importTime-1.0.0.dist-info/top_level.txt
+Filename: importTime-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: importTime-1.0.0.dist-info/RECORD
+Filename: importTime-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `importTime-1.0.0.dist-info/LICENSE.txt` & `importTime-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `importTime-1.0.0.dist-info/METADATA` & `importTime-1.0.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: importTime
-Version: 1.0.0
+Version: 1.0.1
 Summary: Debug import time or use this inside of a profiler.
-Home-page: https://VLTMedia.com
+Home-page: https://github.com/vltmedia/importTime
 Author: Justin Jaro
 Author-email: info@VLTMedia.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

## Comparing `importTime-1.0.0.dist-info/RECORD` & `importTime-1.0.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 importTime/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 importTime/importTime.py,sha256=qOChsvs7lVIRBwAkzInMJme5CFV4g0wnXokLK31TPEw,1445
-importTime-1.0.0.dist-info/LICENSE.txt,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-importTime-1.0.0.dist-info/METADATA,sha256=9xakhmyfnyOVNYJnH-3fynshSsQ2ZakEAmtEV6Ekd6w,848
-importTime-1.0.0.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
-importTime-1.0.0.dist-info/top_level.txt,sha256=JH9k6SWVkd-fOX-HVOobga6KlggF4tyK-jb9ceOpe1M,11
-importTime-1.0.0.dist-info/RECORD,,
+importTime-1.0.1.dist-info/LICENSE.txt,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+importTime-1.0.1.dist-info/METADATA,sha256=AQaymZ_6vBxX393Qpz2zdOFJfoUpUogn1NQn3Q8POro,866
+importTime-1.0.1.dist-info/WHEEL,sha256=k3vXr0c0OitO0k9eCWBlI2yTYnpb_n_I2SGzrrfY7HY,110
+importTime-1.0.1.dist-info/top_level.txt,sha256=JH9k6SWVkd-fOX-HVOobga6KlggF4tyK-jb9ceOpe1M,11
+importTime-1.0.1.dist-info/RECORD,,
```

