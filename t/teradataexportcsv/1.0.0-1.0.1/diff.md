# Comparing `tmp/teradataexportcsv-1.0.0-py3-none-any.whl.zip` & `tmp/teradataexportcsv-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 9071 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat      347 b- defN 23-Jul-28 17:56 teradataexportcsv/__init__.py
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-28 16:37 teradataexportcsv/vernumber.py
--rw-rw-rw-  2.0 fat    13919 b- defN 23-Jul-27 21:50 teradataexportcsv-1.0.0.data/data/teradataexportcsv/LICENSE
--rw-rw-rw-  2.0 fat     1191 b- defN 23-Jul-28 16:34 teradataexportcsv-1.0.0.data/data/teradataexportcsv/README.md
--rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-28 17:57 teradataexportcsv-1.0.0.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat       97 b- defN 23-Jul-28 17:57 teradataexportcsv-1.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     2265 b- defN 23-Jul-28 17:57 teradataexportcsv-1.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      751 b- defN 23-Jul-28 17:57 teradataexportcsv-1.0.0.dist-info/RECORD
-8 files, 18680 bytes uncompressed, 7747 bytes compressed:  58.5%
+Zip file size: 9066 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat      347 b- defN 23-Jul-28 21:04 teradataexportcsv/__init__.py
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-28 21:05 teradataexportcsv/vernumber.py
+-rw-rw-rw-  2.0 fat    13919 b- defN 23-Jul-28 21:04 teradataexportcsv-1.0.1.data/data/teradataexportcsv/LICENSE
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-Jul-28 21:04 teradataexportcsv-1.0.1.data/data/teradataexportcsv/README.md
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Jul-28 21:07 teradataexportcsv-1.0.1.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat       97 b- defN 23-Jul-28 21:07 teradataexportcsv-1.0.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     2265 b- defN 23-Jul-28 21:07 teradataexportcsv-1.0.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      751 b- defN 23-Jul-28 21:07 teradataexportcsv-1.0.1.dist-info/RECORD
+8 files, 18680 bytes uncompressed, 7742 bytes compressed:  58.6%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: teradataexportcsv/__init__.py
 Comment: 
 
 Filename: teradataexportcsv/vernumber.py
 Comment: 
 
-Filename: teradataexportcsv-1.0.0.data/data/teradataexportcsv/LICENSE
+Filename: teradataexportcsv-1.0.1.data/data/teradataexportcsv/LICENSE
 Comment: 
 
-Filename: teradataexportcsv-1.0.0.data/data/teradataexportcsv/README.md
+Filename: teradataexportcsv-1.0.1.data/data/teradataexportcsv/README.md
 Comment: 
 
-Filename: teradataexportcsv-1.0.0.dist-info/top_level.txt
+Filename: teradataexportcsv-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: teradataexportcsv-1.0.0.dist-info/WHEEL
+Filename: teradataexportcsv-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: teradataexportcsv-1.0.0.dist-info/METADATA
+Filename: teradataexportcsv-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: teradataexportcsv-1.0.0.dist-info/RECORD
+Filename: teradataexportcsv-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## teradataexportcsv/vernumber.py

```diff
@@ -1,3 +1,3 @@
 # Copyright 2023 by Teradata Corporation. All rights reserved.
 
-sVersionNumber = "1.0.0"
+sVersionNumber = "1.0.1"
```

## Comparing `teradataexportcsv-1.0.0.data/data/teradataexportcsv/LICENSE` & `teradataexportcsv-1.0.1.data/data/teradataexportcsv/LICENSE`

 * *Files identical despite different names*

## Comparing `teradataexportcsv-1.0.0.data/data/teradataexportcsv/README.md` & `teradataexportcsv-1.0.1.data/data/teradataexportcsv/README.md`

 * *Files identical despite different names*

## Comparing `teradataexportcsv-1.0.0.dist-info/METADATA` & `teradataexportcsv-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: teradataexportcsv
-Version: 1.0.0
+Version: 1.0.1
 Summary: teradataexportcsv package
 Home-page: http://www.teradata.com/
 Author: Teradata Corporation
 Author-email: teradatasql@teradata.com
 License: Teradata License Agreement
 Keywords: Teradata
 Platform: Windows
```

## Comparing `teradataexportcsv-1.0.0.dist-info/RECORD` & `teradataexportcsv-1.0.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 teradataexportcsv/__init__.py,sha256=puB6OCMyB7Dr9-HbRPka5MlrdrRCwx9HheooCn8mjOU,347
-teradataexportcsv/vernumber.py,sha256=qiYopaJlGj63gPqCRhWQmuf_5yGNyqIr482f22vGCoA,92
-teradataexportcsv-1.0.0.data/data/teradataexportcsv/LICENSE,sha256=OqE6M55_w5jILYnMnRJP2nlY-0iEIipHksvbbEyfjlo,13919
-teradataexportcsv-1.0.0.data/data/teradataexportcsv/README.md,sha256=nfDODZlxJFL6DvFZvlv0cbXAr4Wsz-LbwT087YUDjus,1191
-teradataexportcsv-1.0.0.dist-info/METADATA,sha256=0THfw1964RzAIOfVdR6SPfP0TWNdGmBplH8zHSczO-s,2265
-teradataexportcsv-1.0.0.dist-info/RECORD,,
-teradataexportcsv-1.0.0.dist-info/WHEEL,sha256=cScVKDQXc_cp1jHmxFDq9fIOIg17a2BsmfS6J39H6Eo,97
-teradataexportcsv-1.0.0.dist-info/top_level.txt,sha256=yrpNr0DDRO6Fx5aFxdVCLWycQzuVbuMK_F9bXm697GI,18
+teradataexportcsv/vernumber.py,sha256=aoWr2DKDI6_4EXKJKa3sO8MFfiA6HukImgZUrc0iPaQ,92
+teradataexportcsv-1.0.1.data/data/teradataexportcsv/LICENSE,sha256=OqE6M55_w5jILYnMnRJP2nlY-0iEIipHksvbbEyfjlo,13919
+teradataexportcsv-1.0.1.data/data/teradataexportcsv/README.md,sha256=nfDODZlxJFL6DvFZvlv0cbXAr4Wsz-LbwT087YUDjus,1191
+teradataexportcsv-1.0.1.dist-info/METADATA,sha256=cqON6eBJyKAJGiwH79HPIUrmGU3DB0KNhhUgTw2O7AY,2265
+teradataexportcsv-1.0.1.dist-info/RECORD,,
+teradataexportcsv-1.0.1.dist-info/WHEEL,sha256=cScVKDQXc_cp1jHmxFDq9fIOIg17a2BsmfS6J39H6Eo,97
+teradataexportcsv-1.0.1.dist-info/top_level.txt,sha256=yrpNr0DDRO6Fx5aFxdVCLWycQzuVbuMK_F9bXm697GI,18
```

