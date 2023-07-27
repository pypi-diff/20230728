# Comparing `tmp/climatePy-0.4.35.tar.gz` & `tmp/climatePy-0.4.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climatePy-0.4.35.tar", last modified: Tue Jul 18 17:09:07 2023, max compression
+gzip compressed data, was "climatePy-0.4.37.tar", last modified: Thu Jul 27 23:48:46 2023, max compression
```

## Comparing `climatePy-0.4.35.tar` & `climatePy-0.4.37.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.926550 climatePy-0.4.35/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-18 17:09:04.000000 climatePy-0.4.35/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-18 17:09:07.922550 climatePy-0.4.35/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-18 17:09:04.000000 climatePy-0.4.35/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.878549 climatePy-0.4.35/climatePy/
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_climatepy_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    63216 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_dap.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_netrc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    39285 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    32241 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.882550 climatePy-0.4.35/climatePy/data/
--rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-18 17:09:04.000000 climatePy-0.4.35/climatePy/data/catalog.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.882550 climatePy-0.4.35/climatePy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 17:09:07.000000 climatePy-0.4.35/climatePy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:09:07.926550 climatePy-0.4.35/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-18 17:09:06.000000 climatePy-0.4.35/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:07.922550 climatePy-0.4.35/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:09:04.000000 climatePy-0.4.35/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-18 17:09:04.000000 climatePy-0.4.35/tests/test_extract_sites.py
--rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-18 17:09:04.000000 climatePy-0.4.35/tests/test_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-18 17:09:04.000000 climatePy-0.4.35/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.580408 climatePy-0.4.37/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-27 23:48:43.000000 climatePy-0.4.37/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-27 23:48:46.580408 climatePy-0.4.37/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-07-27 23:48:43.000000 climatePy-0.4.37/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.536408 climatePy-0.4.37/climatePy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22670 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_climatepy_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63328 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_dap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_netrc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39286 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32241 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.536408 climatePy-0.4.37/climatePy/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 45897655 2023-07-27 23:48:43.000000 climatePy-0.4.37/climatePy/data/catalog.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.536408 climatePy-0.4.37/climatePy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 23:48:46.000000 climatePy-0.4.37/climatePy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:48:46.580408 climatePy-0.4.37/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-27 23:48:45.000000 climatePy-0.4.37/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:46.580408 climatePy-0.4.37/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:48:43.000000 climatePy-0.4.37/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-27 23:48:43.000000 climatePy-0.4.37/tests/test_extract_sites.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43960 2023-07-27 23:48:43.000000 climatePy-0.4.37/tests/test_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-27 23:48:43.000000 climatePy-0.4.37/tests/test_utils.py
```

### Comparing `climatePy-0.4.35/LICENSE` & `climatePy-0.4.37/LICENSE`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/PKG-INFO` & `climatePy-0.4.37/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.35
+Version: 0.4.37
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
+Author-email: anguswatters@gmail.com, mikecp11@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `climatePy-0.4.35/README.md` & `climatePy-0.4.37/README.md`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/climatePy/__init__.py` & `climatePy-0.4.37/climatePy/__init__.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/climatePy/_climatepy_filter.py` & `climatePy-0.4.37/climatePy/_climatepy_filter.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/climatePy/_dap.py` & `climatePy-0.4.37/climatePy/_dap.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,34 +480,34 @@
             if k in kwargs:
                     matched_args[k] = kwargs[k]
             elif args:
                     matched_args[k] = args[0]
                     args = args[1:]
             else:
                     matched_args[k] = v.default
+                    
     return matched_args
 
 def climatepy_dap(*args, verbose = False, **kwargs):
 
         """ClimatePy DAP (DAP).
         
         This is an internal function that works to take varied argument inputs and appropriatly match 
         them to climatepy_filter() and dap_crop() functions. 
+
         Args:
             *args: Positional arguments to be matched with parameters of `climatepy_filter` and `dap_crop`.
             verbose (bool, optional): Whether to print verbose output during DAP operations. Defaults to False.
             **kwargs: Keyword arguments to be matched with parameters of `climatepy_filter` and `dap_crop`.
-
         Returns:
             dict: A dictionary containing the matched arguments for DAP operations.
-
         """
 
         # get matching arguments for climatepy_filter function
-        matches1            = match_args(climatepy_filter.climatepy_filter, *args, **kwargs)
+        matches1 = match_args(climatepy_filter.climatepy_filter, *args, **kwargs)
 
         # get catalog from climatepy_filter
         x = climatepy_filter.climatepy_filter(**matches1)
 
         # add catalog to list of arguments that'll be passed to dap
         matches1['catalog'] = x
 
@@ -523,25 +523,26 @@
 
         if verbose: 
             print("dap_matches: ", dap_matches)
 
         return dap_matches
 
 def var_to_da(var, dap_row):
+
     """Converts a variable to an xarray DataArray with coordinate reference system (CRS).
 
     Args:
         var (numpy.ndarray): The variable to be converted to a DataArray.
         dap_row (pandas.Series): A pandas Series containing metadata information.
-
+        
     Returns:
         xarray.DataArray: The variable converted to a DataArray with CRS included.
 
     """
-
+    
     # var = get_data(dap_row)
     # dap_row = dap_row
 
     # dates = pd.to_datetime(dates)
     dates = pd.date_range(
         start   = dap_row['startDate'], 
         end     = dap_row['endDate'], 
@@ -617,21 +618,22 @@
         var = var.transpose(dap_row["Y_name"], dap_row["X_name"], dap_row["T_name"])
         # var2 = var.transpose(dap_row["T_name"], dap_row["X_name"],  dap_row["Y_name"])
     
     # Create the DataArray with the CRS included
     r = xr.DataArray(
         var,
         coords = {
-            'y': -1*np.linspace(ymin, ymax, dap_row['nrows'], endpoint=False),
+            'y': np.linspace(ymax, ymin, dap_row['nrows'], endpoint=False),
+            # 'y': -1*np.linspace(ymin, ymax, dap_row['nrows'], endpoint=False),
             'x': np.linspace(xmin, xmax, dap_row['ncols'], endpoint=False),
             'time': dates,
             'crs': dap_row['crs']
-        },
-        dims=['y', 'x', 'time']
-        )
+            },
+            dims=['y', 'x', 'time']
+            )
 
     # if toptobottom is True, flip the data vertically
     if dap_row['toptobottom']:
 
         # vertically flip each 2D array
         flipped_data = np.flip(r.values, axis=0)
         # flipped_data = np.flipud(r.values)
```

### Comparing `climatePy-0.4.35/climatePy/_extract_sites.py` & `climatePy-0.4.37/climatePy/_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/climatePy/_netrc_utils.py` & `climatePy-0.4.37/climatePy/_netrc_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/climatePy/_shortcuts.py` & `climatePy-0.4.37/climatePy/_shortcuts.py`

 * *Files 0% similar despite different names*

```diff
@@ -509,14 +509,15 @@
             verbose   = verbose
             )
         
         return dap_data
     
     return dap_data
 
+
 # --------------------
 # ---- getLivneh ----
 # --------------------
 
 def getLivneh(
         AOI       = None,
         varname   = None,
```

### Comparing `climatePy-0.4.35/climatePy/_utils.py` & `climatePy-0.4.37/climatePy/_utils.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/climatePy/data/catalog.csv` & `climatePy-0.4.37/climatePy/data/catalog.csv`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/climatePy.egg-info/PKG-INFO` & `climatePy-0.4.37/climatePy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: climatePy
-Version: 0.4.35
+Version: 0.4.37
 Summary: A Python package for getting point and gridded climate data by AOI
 Author: Angus Watters, Mike Johnson
+Author-email: anguswatters@gmail.com, mikecp11@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `climatePy-0.4.35/setup.py` & `climatePy-0.4.37/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="climatePy",                         # pkg name
     # version="0.0.4.24",                        # version
-    version='0.4.35',
+    version='0.4.37',
     author="Angus Watters, Mike Johnson",     # authors
+    author_email = "anguswatters@gmail.com, mikecp11@gmail.com",
     description="A Python package for getting point and gridded climate data by AOI",
     long_description=long_description,      # long description is read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # python modules to install
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],          
     python_requires='>=3.6',               # min python version required 
     # py_modules=["climatePy"],             #  python package name
     # package_dir={'':'climatePy/src'},     #  source code directory of package
     # package_dir={'':'src/climatePy'},     #  source code directory of package
     # package_dir={'':'/climatePy'},     #  source code directory of package
-    install_requires=['pandas', 'geopandas', 'shapely', 'pyproj', 'rasterio', 'xarray', 'rtree', 'numpy',
+    install_requires=['pandas', 'geopandas', 'shapely', 'pyproj', 'rasterio', 'xarray', 'rioxarray', 'rtree', 'numpy',
                     'netCDF4', 'joblib'], # dependencies
     include_package_data=True, 
     package_data={'': ['data/*.csv']}     # include catalog csv dataset
     # package_data={'src/climatePy': ['src/data/*']}
     )
```

### Comparing `climatePy-0.4.35/tests/test_extract_sites.py` & `climatePy-0.4.37/tests/test_extract_sites.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/tests/test_shortcuts.py` & `climatePy-0.4.37/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `climatePy-0.4.35/tests/test_utils.py` & `climatePy-0.4.37/tests/test_utils.py`

 * *Files identical despite different names*

