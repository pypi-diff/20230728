# Comparing `tmp/drf-extra-fields-3.5.0.tar.gz` & `tmp/drf-extra-fields-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf-extra-fields-3.5.0.tar", last modified: Thu May 25 10:44:00 2023, max compression
+gzip compressed data, was "drf-extra-fields-3.6.1.tar", last modified: Fri Jul 28 20:23:04 2023, max compression
```

## Comparing `drf-extra-fields-3.5.0.tar` & `drf-extra-fields-3.6.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/
--rw-r--r--   0 furkan    (1000) furkan    (1000)    11324 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/LICENSE
--rw-r--r--   0 furkan    (1000) furkan    (1000)       59 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/MANIFEST.in
--rw-r--r--   0 furkan    (1000) furkan    (1000)    14197 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/PKG-INFO
--rw-r--r--   0 furkan    (1000) furkan    (1000)    13184 2023-05-25 10:42:58.000000 drf-extra-fields-3.5.0/README.md
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/drf_extra_fields/
--rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/__init__.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)      115 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/compat.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)    10848 2023-05-24 10:36:09.000000 drf-extra-fields-3.5.0/drf_extra_fields/fields.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     2131 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/geo_fields.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     3814 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/relations.py
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/drf_extra_fields/runtests/
--rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/runtests/__init__.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     4308 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/drf_extra_fields/runtests/settings.py
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/
--rw-r--r--   0 furkan    (1000) furkan    (1000)    14197 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/PKG-INFO
--rw-r--r--   0 furkan    (1000) furkan    (1000)      550 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/SOURCES.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)        1 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/dependency_links.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)       89 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/requires.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)       17 2023-05-25 10:44:00.000000 drf-extra-fields-3.5.0/drf_extra_fields.egg-info/top_level.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)       61 2023-05-23 10:44:44.000000 drf-extra-fields-3.5.0/requirements.txt
--rw-r--r--   0 furkan    (1000) furkan    (1000)       38 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/setup.cfg
--rw-r--r--   0 furkan    (1000) furkan    (1000)     1714 2023-05-25 10:42:58.000000 drf-extra-fields-3.5.0/setup.py
-drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-05-25 10:44:00.072485 drf-extra-fields-3.5.0/tests/
--rw-r--r--   0 furkan    (1000) furkan    (1000)    33952 2023-05-23 10:44:44.000000 drf-extra-fields-3.5.0/tests/test_fields.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     2241 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/tests/test_model_serializer.py
--rw-r--r--   0 furkan    (1000) furkan    (1000)     5169 2023-05-22 10:26:49.000000 drf-extra-fields-3.5.0/tests/test_relations.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.114493 drf-extra-fields-3.6.1/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    11324 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/LICENSE
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       59 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/MANIFEST.in
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    14342 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/PKG-INFO
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    13329 2023-07-28 20:13:39.000000 drf-extra-fields-3.6.1/README.md
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/drf_extra_fields/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/__init__.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)      115 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/compat.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    10838 2023-07-27 11:55:22.000000 drf-extra-fields-3.6.1/drf_extra_fields/fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     2131 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/geo_fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     3814 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/relations.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/drf_extra_fields/runtests/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        0 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/runtests/__init__.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     4308 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/drf_extra_fields/runtests/settings.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    14342 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/PKG-INFO
+-rw-r--r--   0 furkan    (1000) furkan    (1000)      550 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/SOURCES.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)        1 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/dependency_links.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       89 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/requires.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       17 2023-07-28 20:23:04.000000 drf-extra-fields-3.6.1/drf_extra_fields.egg-info/top_level.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       61 2023-05-23 10:44:44.000000 drf-extra-fields-3.6.1/requirements.txt
+-rw-r--r--   0 furkan    (1000) furkan    (1000)       38 2023-07-28 20:23:04.114493 drf-extra-fields-3.6.1/setup.cfg
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     1714 2023-07-28 20:22:48.000000 drf-extra-fields-3.6.1/setup.py
+drwxr-xr-x   0 furkan    (1000) furkan    (1000)        0 2023-07-28 20:23:04.111160 drf-extra-fields-3.6.1/tests/
+-rw-r--r--   0 furkan    (1000) furkan    (1000)    34084 2023-07-27 11:55:22.000000 drf-extra-fields-3.6.1/tests/test_fields.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     2241 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/tests/test_model_serializer.py
+-rw-r--r--   0 furkan    (1000) furkan    (1000)     5169 2023-05-22 10:26:49.000000 drf-extra-fields-3.6.1/tests/test_relations.py
```

### Comparing `drf-extra-fields-3.5.0/LICENSE` & `drf-extra-fields-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.5.0/PKG-INFO` & `drf-extra-fields-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-extra-fields
-Version: 3.5.0
+Version: 3.6.1
 Summary: Additional fields for Django Rest Framework.
 Home-page: https://github.com/Hipo/drf-extra-fields
 Author: hipo
 Author-email: pypi@hipolabs.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -33,14 +33,16 @@
 [![Build Status](https://github.com/Hipo/drf-extra-fields/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/Hipo/drf-extra-fields/actions)
 [![codecov](https://codecov.io/gh/Hipo/drf-extra-fields/branch/master/graph/badge.svg)](https://codecov.io/gh/Hipo/drf-extra-fields)
 [![PyPI Version](https://img.shields.io/pypi/v/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 [![Python Versions](https://img.shields.io/pypi/pyversions/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 
 Latest Changes
 ==============
+- **v3.6.0**
+  - File objects without an actual file-system path can now be used in `Base64ImageField`, `Base64FileField` and `HybridImageField`
 - **v3.5.0**
   - Development environment fixes & improvements.
   - Since `Python 3.6` support is ended, the codebase is refactored/modernized for `Python 3.7`.
   - `WebP` is added to default `ALLOWED_TYPES` of the `Base64ImageField`.
   - Deprecated `imghdr` library is replaced with `filetype`.
   - Unintended `Pillow` dependency is removed.
 - **v3.4.0**
```

### Comparing `drf-extra-fields-3.5.0/README.md` & `drf-extra-fields-3.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 [![Build Status](https://github.com/Hipo/drf-extra-fields/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/Hipo/drf-extra-fields/actions)
 [![codecov](https://codecov.io/gh/Hipo/drf-extra-fields/branch/master/graph/badge.svg)](https://codecov.io/gh/Hipo/drf-extra-fields)
 [![PyPI Version](https://img.shields.io/pypi/v/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 [![Python Versions](https://img.shields.io/pypi/pyversions/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 
 Latest Changes
 ==============
+- **v3.6.0**
+  - File objects without an actual file-system path can now be used in `Base64ImageField`, `Base64FileField` and `HybridImageField`
 - **v3.5.0**
   - Development environment fixes & improvements.
   - Since `Python 3.6` support is ended, the codebase is refactored/modernized for `Python 3.7`.
   - `WebP` is added to default `ALLOWED_TYPES` of the `Base64ImageField`.
   - Deprecated `imghdr` library is replaced with `filetype`.
   - Unintended `Pillow` dependency is removed.
 - **v3.4.0**
```

### Comparing `drf-extra-fields-3.5.0/drf_extra_fields/fields.py` & `drf-extra-fields-3.6.1/drf_extra_fields/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             # raised on `open`. When representing as base64, simply return an
             # empty base64 str rather than let the exception propagate unhandled
             # up into serializers.
             if not file:
                 return ""
 
             try:
-                with open(file.path, "rb") as f:
+                with file.open() as f:
                     return base64.b64encode(f.read()).decode()
             except Exception:
                 raise OSError("Error encoding file")
         else:
             return super().to_representation(file)
```

### Comparing `drf-extra-fields-3.5.0/drf_extra_fields/geo_fields.py` & `drf-extra-fields-3.6.1/drf_extra_fields/geo_fields.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.5.0/drf_extra_fields/relations.py` & `drf-extra-fields-3.6.1/drf_extra_fields/relations.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.5.0/drf_extra_fields/runtests/settings.py` & `drf-extra-fields-3.6.1/drf_extra_fields/runtests/settings.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.5.0/drf_extra_fields.egg-info/PKG-INFO` & `drf-extra-fields-3.6.1/drf_extra_fields.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-extra-fields
-Version: 3.5.0
+Version: 3.6.1
 Summary: Additional fields for Django Rest Framework.
 Home-page: https://github.com/Hipo/drf-extra-fields
 Author: hipo
 Author-email: pypi@hipolabs.com
 License: Apache-2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -33,14 +33,16 @@
 [![Build Status](https://github.com/Hipo/drf-extra-fields/actions/workflows/tests.yml/badge.svg?branch=master)](https://github.com/Hipo/drf-extra-fields/actions)
 [![codecov](https://codecov.io/gh/Hipo/drf-extra-fields/branch/master/graph/badge.svg)](https://codecov.io/gh/Hipo/drf-extra-fields)
 [![PyPI Version](https://img.shields.io/pypi/v/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 [![Python Versions](https://img.shields.io/pypi/pyversions/drf-extra-fields.svg)](https://pypi.org/project/drf-extra-fields)
 
 Latest Changes
 ==============
+- **v3.6.0**
+  - File objects without an actual file-system path can now be used in `Base64ImageField`, `Base64FileField` and `HybridImageField`
 - **v3.5.0**
   - Development environment fixes & improvements.
   - Since `Python 3.6` support is ended, the codebase is refactored/modernized for `Python 3.7`.
   - `WebP` is added to default `ALLOWED_TYPES` of the `Base64ImageField`.
   - Deprecated `imghdr` library is replaced with `filetype`.
   - Unintended `Pillow` dependency is removed.
 - **v3.4.0**
```

### Comparing `drf-extra-fields-3.5.0/drf_extra_fields.egg-info/SOURCES.txt` & `drf-extra-fields-3.6.1/drf_extra_fields.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.5.0/setup.py` & `drf-extra-fields-3.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     requirements = requirements_txt.read().strip().splitlines()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='drf-extra-fields',
-    version='3.5.0',
+    version='3.6.1',
     packages=['drf_extra_fields',
               'drf_extra_fields.runtests'],
     include_package_data=True,
     extras_require={
         "Base64ImageField": ["Pillow >= 6.2.1"],
     },
     license='Apache-2.0',
```

### Comparing `drf-extra-fields-3.5.0/tests/test_fields.py` & `drf-extra-fields-3.6.1/tests/test_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,23 +40,29 @@
 
 
 class DownloadableBase64Image:
     class ImageFieldFile:
         def __init__(self, path):
             self.path = path
 
+        def open(self):
+            return open(self.path, "rb")
+
     def __init__(self, image_path):
         self.image = self.ImageFieldFile(path=image_path)
 
 
 class DownloadableBase64File:
     class FieldFile:
         def __init__(self, path):
             self.path = path
 
+        def open(self):
+            return open(self.path, "rb")
+
     def __init__(self, file_path):
         self.file = self.FieldFile(path=file_path)
 
 
 class UploadedBase64ImageSerializer(serializers.Serializer):
     file = Base64ImageField(required=False)
     created = serializers.DateTimeField()
```

### Comparing `drf-extra-fields-3.5.0/tests/test_model_serializer.py` & `drf-extra-fields-3.6.1/tests/test_model_serializer.py`

 * *Files identical despite different names*

### Comparing `drf-extra-fields-3.5.0/tests/test_relations.py` & `drf-extra-fields-3.6.1/tests/test_relations.py`

 * *Files identical despite different names*

