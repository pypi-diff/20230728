# Comparing `tmp/tootstagram-0.0.6.tar.gz` & `tmp/tootstagram-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tootstagram-0.0.6.tar", last modified: Fri May 12 06:58:44 2023, max compression
+gzip compressed data, was "tootstagram-0.0.7.tar", last modified: Fri Jul 28 13:06:59 2023, max compression
```

## Comparing `tootstagram-0.0.6.tar` & `tootstagram-0.0.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-05-12 06:58:44.441347 tootstagram-0.0.6/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)    21387 2023-04-26 13:26:59.000000 tootstagram-0.0.6/LICENSE.md
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2154 2023-05-12 06:58:44.441347 tootstagram-0.0.6/PKG-INFO
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1583 2023-05-04 11:20:14.000000 tootstagram-0.0.6/README.md
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      710 2023-05-12 06:57:52.000000 tootstagram-0.0.6/pyproject.toml
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       38 2023-05-12 06:58:44.441347 tootstagram-0.0.6/setup.cfg
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-05-12 06:58:44.437347 tootstagram-0.0.6/tootstagram/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      243 2023-04-27 06:40:20.000000 tootstagram-0.0.6/tootstagram/__init__.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     1297 2023-05-01 06:26:22.000000 tootstagram-0.0.6/tootstagram/database.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2620 2023-05-12 06:56:53.000000 tootstagram-0.0.6/tootstagram/instagram.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2078 2023-05-01 06:26:22.000000 tootstagram-0.0.6/tootstagram/main.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2219 2023-04-27 11:25:42.000000 tootstagram-0.0.6/tootstagram/mastodon.py
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      459 2023-04-27 06:40:20.000000 tootstagram-0.0.6/tootstagram/utils.py
-drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-05-12 06:58:44.441347 tootstagram-0.0.6/tootstagram.egg-info/
--rw-rw-r--   0 gmc       (1000) gmc       (1000)     2154 2023-05-12 06:58:44.000000 tootstagram-0.0.6/tootstagram.egg-info/PKG-INFO
--rw-rw-r--   0 gmc       (1000) gmc       (1000)      385 2023-05-12 06:58:44.000000 tootstagram-0.0.6/tootstagram.egg-info/SOURCES.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)        1 2023-05-12 06:58:44.000000 tootstagram-0.0.6/tootstagram.egg-info/dependency_links.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       54 2023-05-12 06:58:44.000000 tootstagram-0.0.6/tootstagram.egg-info/entry_points.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       48 2023-05-12 06:58:44.000000 tootstagram-0.0.6/tootstagram.egg-info/requires.txt
--rw-rw-r--   0 gmc       (1000) gmc       (1000)       12 2023-05-12 06:58:44.000000 tootstagram-0.0.6/tootstagram.egg-info/top_level.txt
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-07-28 13:06:59.506335 tootstagram-0.0.7/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)    21387 2023-04-26 13:26:59.000000 tootstagram-0.0.7/LICENSE.md
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2154 2023-07-28 13:06:59.502335 tootstagram-0.0.7/PKG-INFO
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     1583 2023-05-04 11:20:14.000000 tootstagram-0.0.7/README.md
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      696 2023-07-28 13:06:42.000000 tootstagram-0.0.7/pyproject.toml
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       38 2023-07-28 13:06:59.506335 tootstagram-0.0.7/setup.cfg
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-07-28 13:06:59.494335 tootstagram-0.0.7/tootstagram/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      243 2023-04-27 06:40:20.000000 tootstagram-0.0.7/tootstagram/__init__.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     1297 2023-05-01 06:26:22.000000 tootstagram-0.0.7/tootstagram/database.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     3226 2023-07-28 13:03:39.000000 tootstagram-0.0.7/tootstagram/instagram.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2078 2023-05-01 06:26:22.000000 tootstagram-0.0.7/tootstagram/main.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2219 2023-04-27 11:25:42.000000 tootstagram-0.0.7/tootstagram/mastodon.py
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      459 2023-04-27 06:40:20.000000 tootstagram-0.0.7/tootstagram/utils.py
+drwxrwxr-x   0 gmc       (1000) gmc       (1000)        0 2023-07-28 13:06:59.502335 tootstagram-0.0.7/tootstagram.egg-info/
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)     2154 2023-07-28 13:06:59.000000 tootstagram-0.0.7/tootstagram.egg-info/PKG-INFO
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)      385 2023-07-28 13:06:59.000000 tootstagram-0.0.7/tootstagram.egg-info/SOURCES.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)        1 2023-07-28 13:06:59.000000 tootstagram-0.0.7/tootstagram.egg-info/dependency_links.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       54 2023-07-28 13:06:59.000000 tootstagram-0.0.7/tootstagram.egg-info/entry_points.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       41 2023-07-28 13:06:59.000000 tootstagram-0.0.7/tootstagram.egg-info/requires.txt
+-rw-rw-r--   0 gmc       (1000) gmc       (1000)       12 2023-07-28 13:06:59.000000 tootstagram-0.0.7/tootstagram.egg-info/top_level.txt
```

### Comparing `tootstagram-0.0.6/LICENSE.md` & `tootstagram-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.6/PKG-INFO` & `tootstagram-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tootstagram
-Version: 0.0.6
+Version: 0.0.7
 Summary: Duplicate posted images from Mastodon to Instagram
 Author-email: Koen Martens <kmartens@sonologic.se>
 Project-URL: Homepage, https://cvs.sonologic.net/gmc/nlgenerator
 Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/nlgenerator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tootstagram-0.0.6/README.md` & `tootstagram-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.6/pyproject.toml` & `tootstagram-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tootstagram"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
     { name="Koen Martens", email="kmartens@sonologic.se" },
 ]
 description = "Duplicate posted images from Mastodon to Instagram"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -14,15 +14,14 @@
     "Environment :: Console",
 ]
 dependencies = [
     "instagrapi",
     "Pillow>=8.1.1",
     "toml",
     "feedparser",
-    "Pillow",
 ]
 
 [project.scripts]
 tootstagram = "tootstagram.main:main"
 
 [project.urls]
 "Homepage" = "https://cvs.sonologic.net/gmc/nlgenerator"
```

### Comparing `tootstagram-0.0.6/tootstagram/database.py` & `tootstagram-0.0.7/tootstagram/database.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.6/tootstagram/instagram.py` & `tootstagram-0.0.7/tootstagram/instagram.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 
 Licensed under a hippocratic license. License terms can be found in
 LICENSE.md or online:
 
 https://firstdonoharm.dev/version/3/0/bds-cl-eco-extr-ffd-media-my-soc-sv-tal-xuar.md
 
 """
+import math
 import os
 from tempfile import TemporaryDirectory
 
 import instagrapi
-from PIL import Image
+from PIL import Image, ImageOps
 from instagrapi.exceptions import LoginRequired
 
 from tootstagram.utils import download_file
 
 
 class InstagramClient:
     def __init__(self, username: str, password: str, session_file_path: str) -> None:
@@ -61,13 +62,24 @@
             download_file(image_url, image_path)
             image = Image.open(image_path)
             if image.format != 'JPEG':
                 image_path = f"{image_path}.jpg"
                 if image.mode != 'RGB':
                     image = image.convert('RGB')
                 image.save(image_path)
+            width = image.size[0]
+            height = image.size[1]
+            aspect = width / height
+            if aspect > 1.91:  # too broad, put bars above and below
+                new_height = int(math.ceil(width/1.91))
+                image = ImageOps.pad(image, (width, new_height), color=(255, 255, 255))
+                image.save(image_path)
+            elif aspect < 0.8:  # too narrow
+                new_width = int(math.ceil(height*0.8))
+                image = ImageOps.pad(image, (new_width, height), color=(255, 255, 255))
+                image.save(image_path)
             self._client.photo_upload(
                 image_path,
                 description,
                 extra_data=extra_data
             )
```

### Comparing `tootstagram-0.0.6/tootstagram/main.py` & `tootstagram-0.0.7/tootstagram/main.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.6/tootstagram/mastodon.py` & `tootstagram-0.0.7/tootstagram/mastodon.py`

 * *Files identical despite different names*

### Comparing `tootstagram-0.0.6/tootstagram.egg-info/PKG-INFO` & `tootstagram-0.0.7/tootstagram.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tootstagram
-Version: 0.0.6
+Version: 0.0.7
 Summary: Duplicate posted images from Mastodon to Instagram
 Author-email: Koen Martens <kmartens@sonologic.se>
 Project-URL: Homepage, https://cvs.sonologic.net/gmc/nlgenerator
 Project-URL: Bug Tracker, https://cvs.sonologic.net/gmc/nlgenerator/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 3 - Alpha
```

