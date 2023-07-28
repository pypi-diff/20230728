# Comparing `tmp/harpia-1.4.tar.gz` & `tmp/harpia-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.4.tar", last modified: Thu Jul 20 06:05:54 2023, max compression
+gzip compressed data, was "harpia-1.5.tar", last modified: Fri Jul 28 18:39:47 2023, max compression
```

## Comparing `harpia-1.4.tar` & `harpia-1.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-20 06:05:54.134382 harpia-1.4/
--rw-r--r--   0 ryan       (501) staff       (20)     1061 2023-07-20 05:11:32.000000 harpia-1.4/LICENSE
--rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-20 06:05:54.133954 harpia-1.4/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      183 2023-07-20 05:15:06.000000 harpia-1.4/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-20 06:05:54.101420 harpia-1.4/harpia/
--rw-r--r--   0 ryan       (501) staff       (20)     1105 2023-07-20 05:28:30.000000 harpia-1.4/harpia/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-20 06:05:54.104127 harpia-1.4/harpia/tropomi/
--rw-r--r--   0 ryan       (501) staff       (20)     1101 2023-07-20 05:28:42.000000 harpia-1.4/harpia/tropomi/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-20 06:05:54.105141 harpia-1.4/harpia/tropomi/no2/
--rw-r--r--   0 ryan       (501) staff       (20)     1107 2023-07-20 05:29:04.000000 harpia-1.4/harpia/tropomi/no2/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     6881 2023-07-20 06:05:02.000000 harpia-1.4/harpia/tropomi/no2/converter.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-20 06:05:54.133368 harpia-1.4/harpia/tropomi/no2/lib/
--rw-r--r--   0 ryan       (501) staff       (20)  7844566 2023-07-16 20:21:38.000000 harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif
--rw-r--r--   0 ryan       (501) staff       (20)  1970880 2023-07-16 20:22:34.000000 harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif
--rw-r--r--   0 ryan       (501) staff       (20)   317616 2023-07-16 20:23:30.000000 harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif
--rw-r--r--   0 ryan       (501) staff       (20)    78826 2023-07-16 20:26:42.000000 harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif
--rw-r--r--   0 ryan       (501) staff       (20)    19984 2023-07-16 20:28:46.000000 harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-20 06:05:54.103526 harpia-1.4/harpia.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-20 06:05:54.000000 harpia-1.4/harpia.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      589 2023-07-20 06:05:54.000000 harpia-1.4/harpia.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-20 06:05:54.000000 harpia-1.4/harpia.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       49 2023-07-20 06:05:54.000000 harpia-1.4/harpia.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        7 2023-07-20 06:05:54.000000 harpia-1.4/harpia.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-20 06:05:54.134525 harpia-1.4/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2103 2023-07-20 06:05:14.000000 harpia-1.4/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.538064 harpia-1.5/
+-rw-r--r--   0 ryan       (501) staff       (20)     1061 2023-07-20 05:11:32.000000 harpia-1.5/LICENSE
+-rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-28 18:39:47.537588 harpia-1.5/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      183 2023-07-20 05:15:06.000000 harpia-1.5/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.490985 harpia-1.5/harpia/
+-rw-r--r--   0 ryan       (501) staff       (20)     1105 2023-07-20 05:28:30.000000 harpia-1.5/harpia/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.494068 harpia-1.5/harpia/tropomi/
+-rw-r--r--   0 ryan       (501) staff       (20)     1101 2023-07-20 05:28:42.000000 harpia-1.5/harpia/tropomi/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.496333 harpia-1.5/harpia/tropomi/no2/
+-rw-r--r--   0 ryan       (501) staff       (20)     1107 2023-07-20 05:29:04.000000 harpia-1.5/harpia/tropomi/no2/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6954 2023-07-28 18:37:37.000000 harpia-1.5/harpia/tropomi/no2/converter.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.536478 harpia-1.5/harpia/tropomi/no2/lib/
+-rw-r--r--   0 ryan       (501) staff       (20)  7844566 2023-07-16 20:21:38.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif
+-rw-r--r--   0 ryan       (501) staff       (20)  1970880 2023-07-16 20:22:34.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif
+-rw-r--r--   0 ryan       (501) staff       (20)   317616 2023-07-16 20:23:30.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif
+-rw-r--r--   0 ryan       (501) staff       (20)    78826 2023-07-16 20:26:42.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif
+-rw-r--r--   0 ryan       (501) staff       (20)    19984 2023-07-16 20:28:46.000000 harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-28 18:39:47.493655 harpia-1.5/harpia.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)      698 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      589 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       49 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        7 2023-07-28 18:39:47.000000 harpia-1.5/harpia.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-28 18:39:47.538229 harpia-1.5/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2103 2023-07-28 17:59:10.000000 harpia-1.5/setup.py
```

### Comparing `harpia-1.4/LICENSE` & `harpia-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.4/PKG-INFO` & `harpia-1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.4
+Version: 1.5
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.4/harpia/__init__.py` & `harpia-1.5/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.4/harpia/tropomi/__init__.py` & `harpia-1.5/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.4/harpia/tropomi/no2/__init__.py` & `harpia-1.5/harpia/tropomi/no2/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.4/harpia/tropomi/no2/converter.py` & `harpia-1.5/harpia/tropomi/no2/converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from netCDF4 import Dataset
 import pandas as pd
 import geopandas
 from rasterio.features import rasterize
 import rasterio
 import pkg_resources
 from harpia.tropomi.no2 import converter
+import gc
 
 def sat_to_df(data_file_path):
     
     file=Dataset(data_file_path, "r" , format="NETCDF4")
     
     
     qa_value=file.groups['PRODUCT'].variables['qa_value']
@@ -180,20 +181,24 @@
     if not gdf.empty:
         for res in resolution_list:
             raster_template=converter.get_raster_template('130w60w20n55n',res)
             new_raster_name=granule_end_date+'_'+res+'_'+str(qa_value_threshold)+'_raster.tif'
             new_raster=os.path.join(writing_directory, new_raster_name)
     
             rasterized=converter.gdf_to_raster(gdf,raster_template, new_raster)
-        
+            raster_template.close()
+    del df
+    del gdf
+    
+
    
 
 
 
 def converter_run(read_directory,write_directory, granule_end_date, qa_value_threshold, df_print=False):
  
-    if df_print:
-            converter.convert_to_df(read_directory,write_directory,granule_end_date,write_to_file=True)
+    #if df_print:
+    #        converter.convert_to_df(read_directory,write_directory,granule_end_date,write_to_file=True)
         
     converter.convert_to_raster(read_directory,write_directory, ['005','010','025','050','100'], granule_end_date, qa_value_threshold)
```

### Comparing `harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif` & `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif` & `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif` & `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif` & `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.4/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif` & `harpia-1.5/harpia/tropomi/no2/lib/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.4/harpia.egg-info/PKG-INFO` & `harpia-1.5/harpia.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.4
+Version: 1.5
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.4/harpia.egg-info/SOURCES.txt` & `harpia-1.5/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.4/setup.py` & `harpia-1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.4",
+    version="1.5",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```

