# Comparing `tmp/PyTubeThumbs-0.0.23-py3-none-any.whl.zip` & `tmp/pytubethumbs-0.0.33-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 3577 bytes, number of entries: 7
+Zip file size: 3741 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       41 b- defN 23-Jul-28 14:35 pytubethumbs/__init__.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-28 14:42 pytubethumbs/main.py
 -rw-rw-rw-  2.0 fat     1883 b- defN 23-Jul-28 14:25 pytubethumbs/src.py
--rw-rw-rw-  2.0 fat     1106 b- defN 23-Jul-28 14:46 PyTubeThumbs-0.0.23.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1688 b- defN 23-Jul-28 14:46 PyTubeThumbs-0.0.23.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-28 14:46 PyTubeThumbs-0.0.23.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-28 14:46 PyTubeThumbs-0.0.23.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      571 b- defN 23-Jul-28 14:46 PyTubeThumbs-0.0.23.dist-info/RECORD
-7 files, 5394 bytes uncompressed, 2559 bytes compressed:  52.6%
+-rw-rw-rw-  2.0 fat     1106 b- defN 23-Jul-28 14:55 pytubethumbs-0.0.33.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1772 b- defN 23-Jul-28 14:55 pytubethumbs-0.0.33.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-28 14:55 pytubethumbs-0.0.33.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       13 b- defN 23-Jul-28 14:55 pytubethumbs-0.0.33.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      645 b- defN 23-Jul-28 14:55 pytubethumbs-0.0.33.dist-info/RECORD
+8 files, 5552 bytes uncompressed, 2607 bytes compressed:  53.0%
```

## zipnote {}

```diff
@@ -1,22 +1,25 @@
 Filename: pytubethumbs/__init__.py
 Comment: 
 
+Filename: pytubethumbs/main.py
+Comment: 
+
 Filename: pytubethumbs/src.py
 Comment: 
 
-Filename: PyTubeThumbs-0.0.23.dist-info/LICENSE
+Filename: pytubethumbs-0.0.33.dist-info/LICENSE
 Comment: 
 
-Filename: PyTubeThumbs-0.0.23.dist-info/METADATA
+Filename: pytubethumbs-0.0.33.dist-info/METADATA
 Comment: 
 
-Filename: PyTubeThumbs-0.0.23.dist-info/WHEEL
+Filename: pytubethumbs-0.0.33.dist-info/WHEEL
 Comment: 
 
-Filename: PyTubeThumbs-0.0.23.dist-info/top_level.txt
+Filename: pytubethumbs-0.0.33.dist-info/top_level.txt
 Comment: 
 
-Filename: PyTubeThumbs-0.0.23.dist-info/RECORD
+Filename: pytubethumbs-0.0.33.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `PyTubeThumbs-0.0.23.dist-info/LICENSE` & `pytubethumbs-0.0.33.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PyTubeThumbs-0.0.23.dist-info/METADATA` & `pytubethumbs-0.0.33.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: PyTubeThumbs
-Version: 0.0.23
+Name: pytubethumbs
+Version: 0.0.33
 Summary: It is a library that helps you create thumbnails for your YouTube channel
 Author: Free Python Code (Amr Elgarhy)
 Author-email: <amr.ee@yahoo.com>
 Keywords: python,thumbnails,images,youtube
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -32,15 +32,21 @@
 
 Create thumbnail
 
 
 
 ```python
 
-generator = PyTubeThumbs(title = 'How to make ChatBot in python', out_path='G:/')
+
+
+import pytubethumbs
+
+
+
+generator = pytubethumbs.PyTubeThumbs(title = 'How to make ChatBot in python', out_path='G:/')
 
 generator.add_text(
 
             pos=(80, 50),
 
             text = generator.title, 
 
@@ -68,15 +74,19 @@
 
 
 
 ```python
 
 
 
-generator = PyTubeThumbs(title = 'How to make ChatBot in python', out_path='G:/')
+import pytubethumbs
+
+
+
+generator = pytubethumbs.PyTubeThumbs(title = 'How to make ChatBot in python', out_path='G:/')
 
 generator.template_text_2imgs(generator.title, 'fonts/Cairo-Black.ttf', 'python.png', 'robot.png')
 
 
 
 generator.save_thumb()
```

## Comparing `PyTubeThumbs-0.0.23.dist-info/RECORD` & `pytubethumbs-0.0.33.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
 pytubethumbs/__init__.py,sha256=OSvhd5nn65Z2m-3qYLAp1v9DEma1BUkXuKM62qEK4ts,41
+pytubethumbs/main.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytubethumbs/src.py,sha256=gH5XoR0IpZNaUgeBBGT1w3U9Im06iF12AMH0i95OT_g,1883
-PyTubeThumbs-0.0.23.dist-info/LICENSE,sha256=2TCDdhu3FQ5QrVuG7Dyko34U0hQkcafC7yKeWtKsxu4,1106
-PyTubeThumbs-0.0.23.dist-info/METADATA,sha256=b7czCmCwcXXEuix0NYjS1dxapEr3tzdPg5jg_F1a1vo,1688
-PyTubeThumbs-0.0.23.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-PyTubeThumbs-0.0.23.dist-info/top_level.txt,sha256=PCN5B9z3ZoDj48p2VeaWGpKRQdCeoj7yzoDJigcDFmo,13
-PyTubeThumbs-0.0.23.dist-info/RECORD,,
+pytubethumbs-0.0.33.dist-info/LICENSE,sha256=2TCDdhu3FQ5QrVuG7Dyko34U0hQkcafC7yKeWtKsxu4,1106
+pytubethumbs-0.0.33.dist-info/METADATA,sha256=gyni-bUExHh06hVymariaqhb02XgFdvsZIZkZR2OGVY,1772
+pytubethumbs-0.0.33.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pytubethumbs-0.0.33.dist-info/top_level.txt,sha256=PCN5B9z3ZoDj48p2VeaWGpKRQdCeoj7yzoDJigcDFmo,13
+pytubethumbs-0.0.33.dist-info/RECORD,,
```

