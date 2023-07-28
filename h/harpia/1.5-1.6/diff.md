# Comparing `tmp/harpia-1.5.tar.gz` & `tmp/harpia-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.5.tar", last modified: Fri Jul 28 18:39:47 2023, max compression
+gzip compressed data, was "harpia-1.6.tar", last modified: Fri Jul 28 19:42:55 2023, max compression
```

## Comparing `harpia-1.5.tar` & `harpia-1.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.538064 harpia-1.5/
--rw-r--r--   0 ryan       (501) staff       (20)     1061 2023-07-20 05:11:32.000000 harpia-1.5/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-28 18:39:47.537588 harpia-1.5/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      183 2023-07-20 05:15:06.000000 harpia-1.5/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.490985 harpia-1.5/harpia/
--rw-r--r--   0 ryan       (501) staff       (20)     1105 2023-07-20 05:28:30.000000 harpia-1.5/harpia/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.494068 harpia-1.5/harpia/tropomi/
--rw-r--r--   0 ryan       (501) staff       (20)     1101 2023-07-20 05:28:42.000000 harpia-1.5/harpia/tropomi/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.496333 harpia-1.5/harpia/tropomi/no2/
--rw-r--r--   0 ryan       (501) staff       (20)     1107 2023-07-20 05:29:04.000000 harpia-1.5/harpia/tropomi/no2/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     6954 2023-07-28 18:37:37.000000 harpia-1.5/harpia/tropomi/no2/converter.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.536478 harpia-1.5/harpia/tropomi/no2/lib/
--rw-r--r--   0 ryan       (501) staff       (20)  7844566 2023-07-16 20:21:38.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif
--rw-r--r--   0 ryan       (501) staff       (20)  1970880 2023-07-16 20:22:34.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif
--rw-r--r--   0 ryan       (501) staff       (20)   317616 2023-07-16 20:23:30.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif
--rw-r--r--   0 ryan       (501) staff       (20)    78826 2023-07-16 20:26:42.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif
--rw-r--r--   0 ryan       (501) staff       (20)    19984 2023-07-16 20:28:46.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.493655 harpia-1.5/harpia.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      589 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       49 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        7 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-28 18:39:47.538229 harpia-1.5/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2103 2023-07-28 17:59:10.000000 harpia-1.5/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.387645 harpia-1.6/
+-rw-r--r--   0 ryan       (501) staff       (20)     1061 2023-07-20 05:11:32.000000 harpia-1.6/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-28 19:42:55.386942 harpia-1.6/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      183 2023-07-20 05:15:06.000000 harpia-1.6/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.341464 harpia-1.6/harpia/
+-rw-r--r--   0 ryan       (501) staff       (20)     1105 2023-07-20 05:28:30.000000 harpia-1.6/harpia/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.343566 harpia-1.6/harpia/tropomi/
+-rw-r--r--   0 ryan       (501) staff       (20)     1101 2023-07-20 05:28:42.000000 harpia-1.6/harpia/tropomi/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.344452 harpia-1.6/harpia/tropomi/no2/
+-rw-r--r--   0 ryan       (501) staff       (20)     1107 2023-07-20 05:29:04.000000 harpia-1.6/harpia/tropomi/no2/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6945 2023-07-28 19:40:27.000000 harpia-1.6/harpia/tropomi/no2/converter.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.385701 harpia-1.6/harpia/tropomi/no2/lib/
+-rw-r--r--   0 ryan       (501) staff       (20)  7844566 2023-07-16 20:21:38.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif
+-rw-r--r--   0 ryan       (501) staff       (20)  1970880 2023-07-16 20:22:34.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif
+-rw-r--r--   0 ryan       (501) staff       (20)   317616 2023-07-16 20:23:30.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif
+-rw-r--r--   0 ryan       (501) staff       (20)    78826 2023-07-16 20:26:42.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif
+-rw-r--r--   0 ryan       (501) staff       (20)    19984 2023-07-16 20:28:46.000000 harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 19:42:55.343116 harpia-1.6/harpia.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      589 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       49 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        7 2023-07-28 19:42:55.000000 harpia-1.6/harpia.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-28 19:42:55.387793 harpia-1.6/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2103 2023-07-28 19:40:41.000000 harpia-1.6/setup.py
```

### Comparing `harpia-1.5/LICENSE` & `harpia-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.5/PKG-INFO` & `harpia-1.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.5
+Version: 1.6
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.5/harpia/__init__.py` & `harpia-1.6/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.5/harpia/tropomi/__init__.py` & `harpia-1.6/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.5/harpia/tropomi/no2/__init__.py` & `harpia-1.6/harpia/tropomi/no2/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.5/harpia/tropomi/no2/converter.py` & `harpia-1.6/harpia/tropomi/no2/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from netCDF4 import Dataset
 import pandas as pd
 import geopandas
 from rasterio.features import rasterize
 import rasterio
 import pkg_resources
 from harpia.tropomi.no2 import converter
-import gc
+
 
 def sat_to_df(data_file_path):
     
     file=Dataset(data_file_path, "r" , format="NETCDF4")
     
     
     qa_value=file.groups['PRODUCT'].variables['qa_value']
```

### Comparing `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif` & `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif` & `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif` & `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif` & `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif` & `harpia-1.6/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.5/harpia.egg-info/PKG-INFO` & `harpia-1.6/harpia.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.5
+Version: 1.6
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.5/harpia.egg-info/SOURCES.txt` & `harpia-1.6/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.5/setup.py` & `harpia-1.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.5",
+    version="1.6",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```

