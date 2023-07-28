# Comparing `tmp/xrd-image-util-1.1.2.tar.gz` & `tmp/xrd-image-util-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrd-image-util-1.1.2.tar", last modified: Fri Jul 28 17:12:19 2023, max compression
+gzip compressed data, was "xrd-image-util-1.1.3.tar", last modified: Fri Jul 28 17:15:36 2023, max compression
```

## Comparing `xrd-image-util-1.1.2.tar` & `xrd-image-util-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:12:19.442224 xrd-image-util-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-28 17:12:08.000000 xrd-image-util-1.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-28 17:12:19.442224 xrd-image-util-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-28 17:12:08.000000 xrd-image-util-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-28 17:12:09.000000 xrd-image-util-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-28 17:12:09.000000 xrd-image-util-1.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:12:19.442224 xrd-image-util-1.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:12:19.442224 xrd-image-util-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-28 17:12:09.000000 xrd-image-util-1.1.2/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 17:12:09.000000 xrd-image-util-1.1.2/tests/test_scan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:12:19.442224 xrd-image-util-1.1.2/xrd_image_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-28 17:12:19.000000 xrd-image-util-1.1.2/xrd_image_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-28 17:12:19.000000 xrd-image-util-1.1.2/xrd_image_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:12:19.000000 xrd-image-util-1.1.2/xrd_image_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 17:12:19.000000 xrd-image-util-1.1.2/xrd_image_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 17:12:19.000000 xrd-image-util-1.1.2/xrd_image_util.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:12:19.442224 xrd-image-util-1.1.2/xrdimageutil/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 17:12:09.000000 xrd-image-util-1.1.2/xrdimageutil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-07-28 17:12:09.000000 xrd-image-util-1.1.2/xrdimageutil/roi.py
--rw-r--r--   0 runner    (1001) docker     (123)    12423 2023-07-28 17:12:09.000000 xrd-image-util-1.1.2/xrdimageutil/structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-28 17:12:09.000000 xrd-image-util-1.1.2/xrdimageutil/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:15:36.035112 xrd-image-util-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-28 17:15:20.000000 xrd-image-util-1.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-28 17:15:36.035112 xrd-image-util-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-28 17:15:20.000000 xrd-image-util-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-28 17:15:21.000000 xrd-image-util-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-28 17:15:21.000000 xrd-image-util-1.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:15:36.035112 xrd-image-util-1.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:15:36.031112 xrd-image-util-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-07-28 17:15:21.000000 xrd-image-util-1.1.3/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-28 17:15:21.000000 xrd-image-util-1.1.3/tests/test_scan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:15:36.035112 xrd-image-util-1.1.3/xrd_image_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-07-28 17:15:36.000000 xrd-image-util-1.1.3/xrd_image_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-28 17:15:36.000000 xrd-image-util-1.1.3/xrd_image_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:15:36.000000 xrd-image-util-1.1.3/xrd_image_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-28 17:15:36.000000 xrd-image-util-1.1.3/xrd_image_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 17:15:36.000000 xrd-image-util-1.1.3/xrd_image_util.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:15:36.035112 xrd-image-util-1.1.3/xrdimageutil/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-28 17:15:21.000000 xrd-image-util-1.1.3/xrdimageutil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-07-28 17:15:21.000000 xrd-image-util-1.1.3/xrdimageutil/roi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-07-28 17:15:21.000000 xrd-image-util-1.1.3/xrdimageutil/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-07-28 17:15:21.000000 xrd-image-util-1.1.3/xrdimageutil/utils.py
```

### Comparing `xrd-image-util-1.1.2/LICENSE.txt` & `xrd-image-util-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.1.2/PKG-INFO` & `xrd-image-util-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrd-image-util
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utility package for handling XRD image data.
 Author-email: Henry Smith <henryjsmith12@outlook.com>
 License: Copyright (c) UChicago Argonne, LLC. All rights reserved.
         
         Copyright UChicago Argonne, LLC. This software was produced
         under U.S. Government contract DE-AC02-06CH11357 for Argonne National
         Laboratory (ANL), which is operated by UChicago Argonne, LLC for the
```

### Comparing `xrd-image-util-1.1.2/README.md` & `xrd-image-util-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.1.2/pyproject.toml` & `xrd-image-util-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xrd-image-util"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
     {name = "Henry Smith", email = "henryjsmith12@outlook.com"},
 ]
 description = "Utility package for handling XRD image data."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `xrd-image-util-1.1.2/tests/test_catalog.py` & `xrd-image-util-1.1.3/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.1.2/tests/test_scan.py` & `xrd-image-util-1.1.3/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.1.2/xrd_image_util.egg-info/PKG-INFO` & `xrd-image-util-1.1.3/xrd_image_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrd-image-util
-Version: 1.1.2
+Version: 1.1.3
 Summary: Utility package for handling XRD image data.
 Author-email: Henry Smith <henryjsmith12@outlook.com>
 License: Copyright (c) UChicago Argonne, LLC. All rights reserved.
         
         Copyright UChicago Argonne, LLC. This software was produced
         under U.S. Government contract DE-AC02-06CH11357 for Argonne National
         Laboratory (ANL), which is operated by UChicago Argonne, LLC for the
```

### Comparing `xrd-image-util-1.1.2/xrdimageutil/roi.py` & `xrd-image-util-1.1.3/xrdimageutil/roi.py`

 * *Files identical despite different names*

### Comparing `xrd-image-util-1.1.2/xrdimageutil/structures.py` & `xrd-image-util-1.1.3/xrdimageutil/structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import databroker
 import numpy as np
 from prettytable import PrettyTable
 import pyqtgraph as pg
 import xrayutilities as xu
 
 from xrdimageutil import utils
-from xrdimageutil.gui.image_data_widget import ScanImageDataGUI
 
 
 class Catalog:
     """
     An interface for databroker's BlueskyCatalog class.
     
     .. index:: Catalog
@@ -394,14 +393,16 @@
         else:
             return self.bluesky_run.primary.metadata["dims"]["time"]
 
     def view_image_data(self) -> None:
         """
         Displays Scan image data in an interactive GUI.
         """
+
+        from xrdimageutil.gui.image_data_widget import ScanImageDataGUI
         
         self.app = pg.mkQApp()
         self.gui_window = ScanImageDataGUI(scan=self)
         self.gui_window.raise_()
         self.gui_window.show()
         self.gui_window.raise_()
         self.app.exec_()
```

### Comparing `xrd-image-util-1.1.2/xrdimageutil/utils.py` & `xrd-image-util-1.1.3/xrdimageutil/utils.py`

 * *Files identical despite different names*

