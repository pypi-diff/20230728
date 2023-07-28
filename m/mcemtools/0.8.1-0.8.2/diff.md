# Comparing `tmp/mcemtools-0.8.1.tar.gz` & `tmp/mcemtools-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcemtools-0.8.1.tar", last modified: Thu Jul 27 13:34:58 2023, max compression
+gzip compressed data, was "mcemtools-0.8.2.tar", last modified: Fri Jul 28 03:54:01 2023, max compression
```

## Comparing `mcemtools-0.8.1.tar` & `mcemtools-0.8.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.850114 mcemtools-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-27 13:34:46.000000 mcemtools-0.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-27 13:34:46.000000 mcemtools-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-27 13:34:46.000000 mcemtools-0.8.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-27 13:34:46.000000 mcemtools-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-27 13:34:46.000000 mcemtools-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-27 13:34:58.850114 mcemtools-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-27 13:34:46.000000 mcemtools-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.846114 mcemtools-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/mcemtools.denoise.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/mcemtools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-27 13:34:46.000000 mcemtools-0.8.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.846114 mcemtools-0.8.1/mcemtools/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)    10313 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-27 13:34:46.000000 mcemtools-0.8.1/mcemtools/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.846114 mcemtools-0.8.1/mcemtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-27 13:34:58.000000 mcemtools-0.8.1/mcemtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 13:34:46.000000 mcemtools-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-27 13:34:58.850114 mcemtools-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-27 13:34:46.000000 mcemtools-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 13:34:58.850114 mcemtools-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_mcemtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_tensor_svd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-27 13:34:46.000000 mcemtools-0.8.1/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.432038 mcemtools-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-28 03:53:51.000000 mcemtools-0.8.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-07-28 03:53:51.000000 mcemtools-0.8.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-28 03:53:51.000000 mcemtools-0.8.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 03:53:51.000000 mcemtools-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-28 03:53:51.000000 mcemtools-0.8.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-28 03:54:01.432038 mcemtools-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-28 03:53:51.000000 mcemtools-0.8.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.428038 mcemtools-0.8.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/mcemtools.denoise.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/mcemtools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 03:53:51.000000 mcemtools-0.8.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.428038 mcemtools-0.8.2/mcemtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-07-28 03:53:51.000000 mcemtools-0.8.2/mcemtools/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.432038 mcemtools-0.8.2/mcemtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 03:54:01.000000 mcemtools-0.8.2/mcemtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-28 03:53:51.000000 mcemtools-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-28 03:54:01.432038 mcemtools-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-28 03:53:51.000000 mcemtools-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:54:01.432038 mcemtools-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_mcemtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_tensor_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-28 03:53:51.000000 mcemtools-0.8.2/tests/test_transforms.py
```

### Comparing `mcemtools-0.8.1/CONTRIBUTING.rst` & `mcemtools-0.8.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/HISTORY.rst` & `mcemtools-0.8.2/HISTORY.rst`

 * *Files 7% similar despite different names*

```diff
@@ -41,8 +41,12 @@
 ------------------
 * markimage bug is fixed really as US version of centre is center.
 * napari based GUI is added to mcemtools.
 * bianary files can be read too.
 
 0.8.1 (2023-07-27)
 ------------------
-* viewer_4D is a lot more concise and bug free.
+* viewer_4D is a lot more concise and bug free.
+
+0.8.1 (2023-07-27)
+------------------
+* by pressing i, you get shapes info, m shows the mask and F5 updates the mask.
```

### Comparing `mcemtools-0.8.1/LICENSE` & `mcemtools-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/PKG-INFO` & `mcemtools-0.8.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.1
+Version: 0.8.2
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -108,7 +108,11 @@
 * markimage bug is fixed really as US version of centre is center.
 * napari based GUI is added to mcemtools.
 * bianary files can be read too.
 
 0.8.1 (2023-07-27)
 ------------------
 * viewer_4D is a lot more concise and bug free.
+
+0.8.1 (2023-07-27)
+------------------
+* by pressing i, you get shapes info, m shows the mask and F5 updates the mask.
```

### Comparing `mcemtools-0.8.1/README.rst` & `mcemtools-0.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/docs/Makefile` & `mcemtools-0.8.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/docs/conf.py` & `mcemtools-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/docs/installation.rst` & `mcemtools-0.8.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/docs/make.bat` & `mcemtools-0.8.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/mcemtools/__init__.py` & `mcemtools-0.8.2/mcemtools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for mcemtools."""
 
 __author__ = """Alireza Sadri"""
 __email__ = 'Alireza.Sadri@monash.edu'
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 from .analysis import pyMSSE, cross_correlation_4D, SymmSTEM
 from .analysis import centre_of_mass_4D, sum_4D
 
 from .masking import annular_mask, image_by_windows, markimage, mask2D_to_4D
 
 from .tensor_svd import svd_fit, svd_eval
```

### Comparing `mcemtools-0.8.1/mcemtools/analysis.py` & `mcemtools-0.8.2/mcemtools/analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/mcemtools/masking.py` & `mcemtools-0.8.2/mcemtools/masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/mcemtools/mcemtools.py` & `mcemtools-0.8.2/mcemtools/mcemtools.py`

 * *Files 6% similar despite different names*

```diff
@@ -103,55 +103,59 @@
         d_type = '>f4'
     elif(size/(y*x) == 8):
         d_type = '>f8'
     #Read data and reshape as required.
     return np.reshape(np.fromfile(filename, dtype = d_type),(y,x))
 
 class viewer_4D:
-    def __init__(self, data4D, logger = print):
+    def __init__(self, data4D, 
+                 statistics_4D = sum4D, logger = print):
         import napari
         self.data4D = data4D
+        self.statistics_4D = statistics_4D
+        self.logger = logger
+
         self.data4D_shape = self.data4D.shape
         self.data4D_shape_list = np.array(self.data4D_shape)
-        self.viewers_list = [napari.Viewer(), napari.Viewer()]
-        self.viewers_list[0].add_image(self.data4D.sum(1).sum(0).squeeze())
-        self.viewers_list[1].add_image(self.data4D.sum(3).sum(2).squeeze())
 
         self.viewers_list[0].bind_key(
-            key = 'Control-i', func = self.print_shape_info)
+            key = 'i', func = self.print_shape_info)
         self.viewers_list[1].bind_key(
-            key = 'Control-i', func = self.print_shape_info)
+            key = 'i', func = self.print_shape_info)
         
         self.viewers_list[0].bind_key(
-            key = 'Control-Shift-s', func = self.save)
+            key = 'm', func = self.show_mask)
         self.viewers_list[1].bind_key(
-            key = 'Control-Shift-s', func = self.save)
+            key = 'm', func = self.show_mask)
         
         self.viewers_list[0].bind_key(
             key = 'F5', func = self.update_by_masked_sum_4D)
         self.viewers_list[1].bind_key(
             key = 'F5', func = self.update_by_masked_sum_4D)
         self.viewers_list[0].mouse_drag_callbacks.append(self.mouse_drag_event)
         self.viewers_list[1].mouse_drag_callbacks.append(self.mouse_drag_event)
         
         self.mask2D_list = []
         self.mask2D_list.append(np.ones(
             (self.data4D_shape[2], self.data4D_shape[3]), dtype='int8'))
         self.mask2D_list.append(np.ones(
             (self.data4D_shape[0], self.data4D_shape[1]), dtype='int8'))
-        self.logger = logger
+
+        STEM_img, PACBED = self.statistics_4D(self.data4D)
+        self.viewers_list = [napari.Viewer(), napari.Viewer()]
+        self.viewers_list[0].add_image(PACBED)
+        self.viewers_list[1].add_image(STEM_img)
+        
         napari.run()
     
-    def save(self, viewer):
-        if isinstance(self.logger, lognflow):
-            assert self.logger, 'logger does not point to a valid directory.'
-            self.logger.log_imshow('masks/mask2D_0', self.mask2D_list[0])
-            self.logger.log_single('masks/mask2D_0', self.mask2D_list[0])
-            self.logger.log_imshow('masks/mask2D_1', self.mask2D_list[1])
-            self.logger.log_single('masks/mask2D_1', self.mask2D_list[1])
+    def show_mask(self, viewer):
+        self.update_by_masked_sum_4D(viewer)
+        viewer_index = self.viewers_list.index(viewer)
+        plt.figure(), plt.imshow(self.mask2D_list[viewer_index])
+        plt.title(f'mask for viewer {viewer_index}'), plt.show()
     
     def get_mask2D(self, shape_layer, mask_shape):
         from skimage.draw import polygon2mask
         from scipy.ndimage import binary_dilation, binary_fill_holes
         mask2D = np.zeros(mask_shape, dtype='int8')
         
         label2D = shape_layer.to_labels(mask_shape)
@@ -206,20 +210,20 @@
             data4D_shape_select = viewer.layers[0].data.shape
             mask2D = self.get_mask2D(viewer.layers[1], data4D_shape_select)
             if( (self.mask2D_list[viewer_index] != mask2D).sum()>0):
                 self.mask2D_list.__setitem__(viewer_index, mask2D.copy())
                 mask4D = np.zeros(self.data4D_shape, dtype='int8')
                 if(viewer_index == 0):
                     mask4D[:, :, mask2D==1] = 1
-                    STEM_img, PACBED = sum_4D(self.data4D, mask4D)
+                    STEM_img, PACBED = self.statistics_4D(self.data4D, mask4D)
                     self.viewers_list[1].layers[0].data = STEM_img
                     self.logger('STEM image updated')
                 if(viewer_index == 1):
                     mask4D[mask2D==1, :, :] = 1
-                    STEM_img, PACBED = sum_4D(self.data4D, mask4D)
+                    STEM_img, PACBED = self.statistics_4D(self.data4D, mask4D)
                     self.viewers_list[0].layers[0].data = PACBED
                     self.logger('PACBED image updated')
 
     def mouse_drag_event(self, viewer, event):
         dragged = False
         yield
         while event.type == 'mouse_move':
```

### Comparing `mcemtools-0.8.1/mcemtools/tensor_svd.py` & `mcemtools-0.8.2/mcemtools/tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/mcemtools/transforms.py` & `mcemtools-0.8.2/mcemtools/transforms.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/mcemtools.egg-info/PKG-INFO` & `mcemtools-0.8.2/mcemtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcemtools
-Version: 0.8.1
+Version: 0.8.2
 Summary: State of the art analysis tools for electron microscopy
 Home-page: https://github.com/arsadri/mcemtools
 Author: Alireza Sadri
 Author-email: Alireza.Sadri@monash.edu
 License: MIT license
 Keywords: mcemtools
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -108,7 +108,11 @@
 * markimage bug is fixed really as US version of centre is center.
 * napari based GUI is added to mcemtools.
 * bianary files can be read too.
 
 0.8.1 (2023-07-27)
 ------------------
 * viewer_4D is a lot more concise and bug free.
+
+0.8.1 (2023-07-27)
+------------------
+* by pressing i, you get shapes info, m shows the mask and F5 updates the mask.
```

### Comparing `mcemtools-0.8.1/mcemtools.egg-info/SOURCES.txt` & `mcemtools-0.8.2/mcemtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/setup.py` & `mcemtools-0.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 
 """The setup script."""
 
 from setuptools import setup, find_packages
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
```

### Comparing `mcemtools-0.8.1/tests/test_analysis.py` & `mcemtools-0.8.2/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/tests/test_masking.py` & `mcemtools-0.8.2/tests/test_masking.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/tests/test_mcemtools.py` & `mcemtools-0.8.2/tests/test_mcemtools.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/tests/test_tensor_svd.py` & `mcemtools-0.8.2/tests/test_tensor_svd.py`

 * *Files identical despite different names*

### Comparing `mcemtools-0.8.1/tests/test_transforms.py` & `mcemtools-0.8.2/tests/test_transforms.py`

 * *Files identical despite different names*

