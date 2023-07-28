# Comparing `tmp/yk_utils-1.3.4.tar.gz` & `tmp/yk_utils-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/yk-utils-python/yk-utils-python/dist/.tmp-6m1fqdqq/yk_utils-1.3.4.tar", last modified: Thu Apr 20 17:06:43 2023, max compression
+gzip compressed data, was "/home/runner/work/yk-utils-python/yk-utils-python/dist/.tmp-k4r1n9nz/yk_utils-1.3.5.tar", last modified: Fri Jul 28 13:35:15 2023, max compression
```

## Comparing `yk_utils-1.3.4.tar` & `yk_utils-1.3.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-20 17:06:31.000000 yk_utils-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 17:06:43.000000 yk_utils-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-20 17:06:31.000000 yk_utils-1.3.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 17:06:43.000000 yk_utils-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-04-20 17:06:31.000000 yk_utils-1.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/apis/api_result.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/apis/base_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/apis/face_authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/apis/http_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/apis/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/apis/yoonik_api_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils/files/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/files/file_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils/images/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/images/image_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/images/image_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/models/base_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/models/deserialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/models/error.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/models/str_base_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils/objects/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/objects/object_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils/web/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/web/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-20 17:06:31.000000 yk_utils-1.3.4/yk_utils/web/url_operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 17:06:43.000000 yk_utils-1.3.4/yk_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-07-28 13:35:03.000000 yk_utils-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-28 13:35:15.000000 yk_utils-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-28 13:35:03.000000 yk_utils-1.3.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:35:15.000000 yk_utils-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-28 13:35:03.000000 yk_utils-1.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/apis/api_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/apis/base_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/apis/face_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/apis/http_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/apis/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/apis/yoonik_api_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils/files/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/files/file_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/images/image_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/images/image_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/models/base_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/models/deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/models/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/models/str_base_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/objects/object_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils/web/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/web/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-28 13:35:03.000000 yk_utils-1.3.5/yk_utils/web/url_operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-28 13:35:15.000000 yk_utils-1.3.5/yk_utils.egg-info/top_level.txt
```

### Comparing `yk_utils-1.3.4/LICENSE` & `yk_utils-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/PKG-INFO` & `yk_utils-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yk_utils
-Version: 1.3.4
+Version: 1.3.5
 Summary: Youverse utils package for python.
 Home-page: https://github.com/dev-yoonik/yk-utils-python
 Author: Youverse
 Author-email: tech@youverse.id
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yk_utils-1.3.4/README.md` & `yk_utils-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/setup.py` & `yk_utils-1.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yk_utils",
-    version="1.3.4",
+    version="1.3.5",
     description="Youverse utils package for python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Youverse",
     author_email="tech@youverse.id",
     url="https://github.com/dev-yoonik/yk-utils-python",
     license='MIT',
```

### Comparing `yk_utils-1.3.4/yk_utils/apis/base_url.py` & `yk_utils-1.3.5/yk_utils/apis/base_url.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/apis/face_authentication.py` & `yk_utils-1.3.5/yk_utils/apis/face_authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,17 +40,21 @@
                 message = inner_html.text if inner_html.p is None else inner_html.p.text
 
         if "face_not_found" in message:
             message = "Could not find a face in the image."
         elif "multiple_faces" in message:
             message = "The image has more than one person."
         elif "brightness_failed" in message:
-            message = "Please avoid glare or extreme light conditions."
+            message = "Avoid glare or extreme light conditions."
         elif "light_uniformity_failed" in message:
-            message = "Please avoid having parts of your face shadowed."
+            message = "Avoid having parts of your face shadowed."
+        elif "face_too_far" in message:
+            message = "Move a little closer to the camera."
+        elif "face_too_close" in message:
+            message = "Move a little further from the camera."
         elif "quality_failed" in message:
             message = "The provided image does not have enough quality."
         elif "mobile_app_no_response" in message:
             message = "Could not receive result from mobile app."
         elif extra_response_codes:
             for code in extra_response_codes:
                 if code in message:
```

### Comparing `yk_utils-1.3.4/yk_utils/apis/http_requests.py` & `yk_utils-1.3.5/yk_utils/apis/http_requests.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/apis/yoonik_api_exception.py` & `yk_utils-1.3.5/yk_utils/apis/yoonik_api_exception.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/files/file_operations.py` & `yk_utils-1.3.5/yk_utils/files/file_operations.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/images/image_parser.py` & `yk_utils-1.3.5/yk_utils/images/image_parser.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/models/base_enum.py` & `yk_utils-1.3.5/yk_utils/models/base_enum.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/models/base_model.py` & `yk_utils-1.3.5/yk_utils/models/base_model.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/models/deserialization.py` & `yk_utils-1.3.5/yk_utils/models/deserialization.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/models/error.py` & `yk_utils-1.3.5/yk_utils/models/error.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils/web/url_operations.py` & `yk_utils-1.3.5/yk_utils/web/url_operations.py`

 * *Files identical despite different names*

### Comparing `yk_utils-1.3.4/yk_utils.egg-info/PKG-INFO` & `yk_utils-1.3.5/yk_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yk-utils
-Version: 1.3.4
+Version: 1.3.5
 Summary: Youverse utils package for python.
 Home-page: https://github.com/dev-yoonik/yk-utils-python
 Author: Youverse
 Author-email: tech@youverse.id
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `yk_utils-1.3.4/yk_utils.egg-info/SOURCES.txt` & `yk_utils-1.3.5/yk_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

