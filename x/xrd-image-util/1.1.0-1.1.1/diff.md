# Comparing `tmp/xrd-image-util-1.1.0.tar.gz` & `tmp/xrd-image-util-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrd-image-util-1.1.0.tar", last modified: Wed Jun  7 16:17:54 2023, max compression
+gzip compressed data, was "xrd-image-util-1.1.1.tar", last modified: Fri Jul 28 17:04:13 2023, max compression
```

## Comparing `xrd-image-util-1.1.0.tar` & `xrd-image-util-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/tests/test_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/xrd_image_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 16:17:54.000000 xrd-image-util-1.1.0/xrd_image_util.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 16:17:54.536685 xrd-image-util-1.1.0/xrdimageutil/
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/xrdimageutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19687 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/xrdimageutil/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-07 16:17:44.000000 xrd-image-util-1.1.0/xrdimageutil/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:04:13.209388 xrd-image-util-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-28 17:04:01.000000 xrd-image-util-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-28 17:04:13.209388 xrd-image-util-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-28 17:04:01.000000 xrd-image-util-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-28 17:04:02.000000 xrd-image-util-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-28 17:04:02.000000 xrd-image-util-1.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:04:13.209388 xrd-image-util-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:04:13.209388 xrd-image-util-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-28 17:04:02.000000 xrd-image-util-1.1.1/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 17:04:02.000000 xrd-image-util-1.1.1/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:04:13.209388 xrd-image-util-1.1.1/xrd_image_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-28 17:04:13.000000 xrd-image-util-1.1.1/xrd_image_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-28 17:04:13.000000 xrd-image-util-1.1.1/xrd_image_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:04:13.000000 xrd-image-util-1.1.1/xrd_image_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 17:04:13.000000 xrd-image-util-1.1.1/xrd_image_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 17:04:13.000000 xrd-image-util-1.1.1/xrd_image_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:04:13.209388 xrd-image-util-1.1.1/xrdimageutil/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 17:04:02.000000 xrd-image-util-1.1.1/xrdimageutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-07-28 17:04:02.000000 xrd-image-util-1.1.1/xrdimageutil/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12424 2023-07-28 17:04:02.000000 xrd-image-util-1.1.1/xrdimageutil/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-28 17:04:02.000000 xrd-image-util-1.1.1/xrdimageutil/utils.py
```

### Comparing `xrd-image-util-1.1.0/LICENSE.txt` & `xrd-image-util-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.1.0/PKG-INFO` & `xrd-image-util-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrd-image-util
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utility package for handling XRD image data.
 Author-email: Henry Smith <henryjsmith12@outlook.com>
 License: Copyright (c) UChicago Argonne, LLC. All rights reserved.
         
         Copyright UChicago Argonne, LLC. This software was produced
         under U.S. Government contract DE-AC02-06CH11357 for Argonne National
         Laboratory (ANL), which is operated by UChicago Argonne, LLC for the
```

### Comparing `xrd-image-util-1.1.0/README.md` & `xrd-image-util-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.1.0/pyproject.toml` & `xrd-image-util-1.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xrd-image-util"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
     {name = "Henry Smith", email = "henryjsmith12@outlook.com"},
 ]
 description = "Utility package for handling XRD image data."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 1 - Planning",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
+dynamic = ["dependencies"]
+
+[tool.setuptools.dynamic]
+dependencies = {file = ["requirements.txt"]}
 
 [project.license]
 file = "LICENSE.txt"
 
 [project.optional-dependencies]
 test = [
     "coverage",
```

### Comparing `xrd-image-util-1.1.0/tests/test_catalog.py` & `xrd-image-util-1.1.1/tests/test_catalog.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from xrdimageutil import Catalog
+from xrdimageutil.structures import Catalog
 
 class TestCatalog:
 
     relative_path = "data/singh"
     absolute_path = os.path.abspath(path=relative_path)
     catalog_name = "test-catalog"
```

### Comparing `xrd-image-util-1.1.0/tests/test_scan.py` & `xrd-image-util-1.1.1/tests/test_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from xrdimageutil import Catalog, Scan
+from xrdimageutil.structures import Catalog, Scan
 
 class TestScan:
 
     relative_path = "data/singh"
     absolute_path = os.path.abspath(path=relative_path)
     catalog_name = "test-catalog"
```

### Comparing `xrd-image-util-1.1.0/xrd_image_util.egg-info/PKG-INFO` & `xrd-image-util-1.1.1/xrd_image_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrd-image-util
-Version: 1.1.0
+Version: 1.1.1
 Summary: Utility package for handling XRD image data.
 Author-email: Henry Smith <henryjsmith12@outlook.com>
 License: Copyright (c) UChicago Argonne, LLC. All rights reserved.
         
         Copyright UChicago Argonne, LLC. This software was produced
         under U.S. Government contract DE-AC02-06CH11357 for Argonne National
         Laboratory (ANL), which is operated by UChicago Argonne, LLC for the
```

### Comparing `xrd-image-util-1.1.0/xrdimageutil/utils.py` & `xrd-image-util-1.1.1/xrdimageutil/utils.py`

 * *Files identical despite different names*

