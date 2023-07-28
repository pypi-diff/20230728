# Comparing `tmp/mcemtools-0.8.2.tar.gz` & `tmp/mcemtools-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.8.2.tar", last modified: Fri Jul 28 03:54:01 2023, max compression
+gzip compressed data, was "mcemtools-0.8.3.tar", last modified: Fri Jul 28 04:07:37 2023, max compression
```

## Comparing `mcemtools-0.8.2.tar` & `mcemtools-0.8.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.432038 mcemtools-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-28 03:53:51.000000 mcemtools-0.8.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-28 03:53:51.000000 mcemtools-0.8.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-28 03:53:51.000000 mcemtools-0.8.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 03:53:51.000000 mcemtools-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 03:53:51.000000 mcemtools-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-28 03:54:01.432038 mcemtools-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-28 03:53:51.000000 mcemtools-0.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.428038 mcemtools-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.428038 mcemtools-0.8.2/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.432038 mcemtools-0.8.2/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 03:53:51.000000 mcemtools-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-28 03:54:01.432038 mcemtools-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-28 03:53:51.000000 mcemtools-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.432038 mcemtools-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:07:37.659253 mcemtools-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-28 04:07:27.000000 mcemtools-0.8.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-28 04:07:27.000000 mcemtools-0.8.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-28 04:07:27.000000 mcemtools-0.8.3/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 04:07:27.000000 mcemtools-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 04:07:27.000000 mcemtools-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-28 04:07:37.659253 mcemtools-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-28 04:07:27.000000 mcemtools-0.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:07:37.655253 mcemtools-0.8.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 04:07:27.000000 mcemtools-0.8.3/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:07:37.655253 mcemtools-0.8.3/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 04:07:27.000000 mcemtools-0.8.3/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-28 04:07:27.000000 mcemtools-0.8.3/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 04:07:27.000000 mcemtools-0.8.3/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-28 04:07:27.000000 mcemtools-0.8.3/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-07-28 04:07:27.000000 mcemtools-0.8.3/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-28 04:07:27.000000 mcemtools-0.8.3/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-28 04:07:27.000000 mcemtools-0.8.3/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:07:37.655253 mcemtools-0.8.3/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-28 04:07:37.000000 mcemtools-0.8.3/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-28 04:07:37.000000 mcemtools-0.8.3/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:07:37.000000 mcemtools-0.8.3/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 04:07:37.000000 mcemtools-0.8.3/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 04:07:37.000000 mcemtools-0.8.3/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 04:07:37.000000 mcemtools-0.8.3/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 04:07:37.000000 mcemtools-0.8.3/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 04:07:27.000000 mcemtools-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-28 04:07:37.659253 mcemtools-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-28 04:07:27.000000 mcemtools-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 04:07:37.659253 mcemtools-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 04:07:27.000000 mcemtools-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 04:07:27.000000 mcemtools-0.8.3/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-28 04:07:27.000000 mcemtools-0.8.3/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-28 04:07:27.000000 mcemtools-0.8.3/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-28 04:07:27.000000 mcemtools-0.8.3/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-28 04:07:27.000000 mcemtools-0.8.3/tests/test_transforms.py
```

### Comparing `mcemtools-0.8.2/CONTRIBUTING.rst` & `mcemtools-0.8.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/HISTORY.rst` & `mcemtools-0.8.3/HISTORY.rst`

 * *Files 22% similar despite different names*

```diff
@@ -43,10 +43,14 @@
 * napari based GUI is added to mcemtools.
 * bianary files can be read too.
 
 0.8.1 (2023-07-27)
 ------------------
 * viewer_4D is a lot more concise and bug free.
 
-0.8.1 (2023-07-27)
+0.8.2 (2023-07-27)
+------------------
+* by pressing i, you get shapes info, m shows the mask and F5 updates the mask.
+
+0.8.3 (2023-07-28)
 ------------------
-* by pressing i, you get shapes info, m shows the mask and F5 updates the mask.
+* critical bug was fixed in viewer_4D
```

### Comparing `mcemtools-0.8.2/LICENSE` & `mcemtools-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/PKG-INFO` & `mcemtools-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.2
+Version: 0.8.3
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -109,10 +109,14 @@
 * napari based GUI is added to mcemtools.
 * bianary files can be read too.
 
 0.8.1 (2023-07-27)
 ------------------
 * viewer_4D is a lot more concise and bug free.
 
-0.8.1 (2023-07-27)
+0.8.2 (2023-07-27)
 ------------------
 * by pressing i, you get shapes info, m shows the mask and F5 updates the mask.
+
+0.8.3 (2023-07-28)
+------------------
+* critical bug was fixed in viewer_4D
```

### Comparing `mcemtools-0.8.2/README.rst` & `mcemtools-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/docs/Makefile` & `mcemtools-0.8.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/docs/conf.py` & `mcemtools-0.8.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/docs/installation.rst` & `mcemtools-0.8.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/docs/make.bat` & `mcemtools-0.8.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/mcemtools/__init__.py` & `mcemtools-0.8.3/mcemtools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'Alireza.Sadri@monash.edu'
-__version__ = '0.8.2'
+__version__ = '0.8.3'
 
 from .analysis import pyMSSE, cross_correlation_4D, SymmSTEM
 from .analysis import centre_of_mass_4D, sum_4D
 
 from .masking import annular_mask, image_by_windows, markimage, mask2D_to_4D
 
 from .tensor_svd import svd_fit, svd_eval
```

### Comparing `mcemtools-0.8.2/mcemtools/analysis.py` & `mcemtools-0.8.3/mcemtools/analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/mcemtools/masking.py` & `mcemtools-0.8.3/mcemtools/masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/mcemtools/mcemtools.py` & `mcemtools-0.8.3/mcemtools/mcemtools.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     elif(size/(y*x) == 8):
         d_type = '>f8'
     #Read data and reshape as required.
     return np.reshape(np.fromfile(filename, dtype = d_type),(y,x))
 
 class viewer_4D:
     def __init__(self, data4D, 
-                 statistics_4D = sum4D, logger = print):
+                 statistics_4D = sum_4D, logger = print):
         import napari
         self.data4D = data4D
         self.statistics_4D = statistics_4D
         self.logger = logger
 
         self.data4D_shape = self.data4D.shape
         self.data4D_shape_list = np.array(self.data4D_shape)
```

### Comparing `mcemtools-0.8.2/mcemtools/tensor_svd.py` & `mcemtools-0.8.3/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/mcemtools/transforms.py` & `mcemtools-0.8.3/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.8.3/mcemtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.2
+Version: 0.8.3
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -109,10 +109,14 @@
 * napari based GUI is added to mcemtools.
 * bianary files can be read too.
 
 0.8.1 (2023-07-27)
 ------------------
 * viewer_4D is a lot more concise and bug free.
 
-0.8.1 (2023-07-27)
+0.8.2 (2023-07-27)
 ------------------
 * by pressing i, you get shapes info, m shows the mask and F5 updates the mask.
+
+0.8.3 (2023-07-28)
+------------------
+* critical bug was fixed in viewer_4D
```

### Comparing `mcemtools-0.8.2/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.8.3/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/setup.py` & `mcemtools-0.8.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.8.2'
+__version__ = '0.8.3'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
```

### Comparing `mcemtools-0.8.2/tests/test_analysis.py` & `mcemtools-0.8.3/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/tests/test_masking.py` & `mcemtools-0.8.3/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/tests/test_mcemtools.py` & `mcemtools-0.8.3/tests/test_mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/tests/test_tensor_svd.py` & `mcemtools-0.8.3/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.2/tests/test_transforms.py` & `mcemtools-0.8.3/tests/test_transforms.py`

 * *Files identical despite different names*

