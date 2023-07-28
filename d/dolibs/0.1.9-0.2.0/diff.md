# Comparing `tmp/dolibs-0.1.9.tar.gz` & `tmp/dolibs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolibs-0.1.9.tar", last modified: Mon Jun 12 09:33:37 2023, max compression
+gzip compressed data, was "dolibs-0.2.0.tar", last modified: Fri Jul 28 09:52:29 2023, max compression
```

## Comparing `dolibs-0.1.9.tar` & `dolibs-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-12 09:33:37.242982 dolibs-0.1.9/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-12 09:33:37.242851 dolibs-0.1.9/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)     1152 2023-05-03 10:26:07.000000 dolibs-0.1.9/README.md
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-12 09:33:37.241933 dolibs-0.1.9/dolibs/
--rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.1.9/dolibs/__init__.py
--rw-r--r--   0 leandro    (501) staff       (20)     4592 2023-06-12 09:33:01.000000 dolibs-0.1.9/dolibs/dewpoint.py
--rw-r--r--   0 leandro    (501) staff       (20)     4591 2023-05-03 09:47:15.000000 dolibs-0.1.9/dolibs/skintemp.py
-drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-06-12 09:33:37.242638 dolibs-0.1.9/dolibs.egg-info/
--rw-r--r--   0 leandro    (501) staff       (20)      298 2023-06-12 09:33:37.000000 dolibs-0.1.9/dolibs.egg-info/PKG-INFO
--rw-r--r--   0 leandro    (501) staff       (20)      224 2023-06-12 09:33:37.000000 dolibs-0.1.9/dolibs.egg-info/SOURCES.txt
--rw-r--r--   0 leandro    (501) staff       (20)        1 2023-06-12 09:33:37.000000 dolibs-0.1.9/dolibs.egg-info/dependency_links.txt
--rw-r--r--   0 leandro    (501) staff       (20)       71 2023-06-12 09:33:37.000000 dolibs-0.1.9/dolibs.egg-info/requires.txt
--rw-r--r--   0 leandro    (501) staff       (20)        7 2023-06-12 09:33:37.000000 dolibs-0.1.9/dolibs.egg-info/top_level.txt
--rw-r--r--   0 leandro    (501) staff       (20)       38 2023-06-12 09:33:37.243031 dolibs-0.1.9/setup.cfg
--rw-r--r--   0 leandro    (501) staff       (20)      599 2023-06-12 09:33:31.000000 dolibs-0.1.9/setup.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-28 09:52:29.997799 dolibs-0.2.0/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-07-28 09:52:29.997658 dolibs-0.2.0/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)     1152 2023-05-03 10:26:07.000000 dolibs-0.2.0/README.md
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-28 09:52:29.996412 dolibs-0.2.0/dolibs/
+-rw-r--r--   0 leandro    (501) staff       (20)        0 2023-04-12 09:31:04.000000 dolibs-0.2.0/dolibs/__init__.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4532 2023-06-20 17:32:50.000000 dolibs-0.2.0/dolibs/dewpoint.py
+-rw-r--r--   0 leandro    (501) staff       (20)     4527 2023-06-20 17:32:50.000000 dolibs-0.2.0/dolibs/skintemp.py
+drwxr-xr-x   0 leandro    (501) staff       (20)        0 2023-07-28 09:52:29.997392 dolibs-0.2.0/dolibs.egg-info/
+-rw-r--r--   0 leandro    (501) staff       (20)      298 2023-07-28 09:52:29.000000 dolibs-0.2.0/dolibs.egg-info/PKG-INFO
+-rw-r--r--   0 leandro    (501) staff       (20)      224 2023-07-28 09:52:29.000000 dolibs-0.2.0/dolibs.egg-info/SOURCES.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        1 2023-07-28 09:52:29.000000 dolibs-0.2.0/dolibs.egg-info/dependency_links.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       71 2023-07-28 09:52:29.000000 dolibs-0.2.0/dolibs.egg-info/requires.txt
+-rw-r--r--   0 leandro    (501) staff       (20)        7 2023-07-28 09:52:29.000000 dolibs-0.2.0/dolibs.egg-info/top_level.txt
+-rw-r--r--   0 leandro    (501) staff       (20)       38 2023-07-28 09:52:29.997855 dolibs-0.2.0/setup.cfg
+-rw-r--r--   0 leandro    (501) staff       (20)      599 2023-07-28 09:48:53.000000 dolibs-0.2.0/setup.py
```

### Comparing `dolibs-0.1.9/README.md` & `dolibs-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `dolibs-0.1.9/dolibs/dewpoint.py` & `dolibs-0.2.0/dolibs/dewpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         ds = xr.open_dataset(nc_file).load()
 
         print('Calculate daily temperature and transform in Celsius')
         daily_data = ds.resample(time='d').mean()
         daily_data_celsius = daily_data.d2m - 273.15
 
         print('Start cube elaboration')
-        #always skip last retrieved day cause it could be incomplete
+        
         for i in range((len(daily_data_celsius))):
             dout = daily_data_celsius[i,:,:]
             dout.rio.write_crs("EPSG:4326", inplace=True).rio.to_raster(nc_file+'_out_'+str((i+1))+'.tiff')
             #set file and form data for post call
 
             files_in = {
                 'file': (nc_file+'_out_'+str((i+1))+'.tiff', open(nc_file+'_out_'+str((i+1))+'.tiff', 'rb'),'multipart/form-data'),
```

### Comparing `dolibs-0.1.9/dolibs/skintemp.py` & `dolibs-0.2.0/dolibs/skintemp.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,16 +50,16 @@
         ds = xr.open_dataset(nc_file).load()
 
         print('Calculate daily temperature and transform in Celsius')
         daily_data = ds.resample(time='d').mean()
         daily_data_celsius = daily_data.skt - 273.15
 
         print('Start cube elaboration')
-        #always skip last retrieved day cause it could be incomplete
-        for i in range((len(daily_data_celsius) - 1)):
+        
+        for i in range((len(daily_data_celsius))):
             dout = daily_data_celsius[i,:,:]
             dout.rio.write_crs("EPSG:4326", inplace=True).rio.to_raster(nc_file+'_out_'+str((i+1))+'.tiff')
             #set file and form data for post call
 
             files_in = {
                 'file': (nc_file+'_out_'+str((i+1))+'.tiff', open(nc_file+'_out_'+str((i+1))+'.tiff', 'rb'),'multipart/form-data'),
                 'year': str(year_in),
```

### Comparing `dolibs-0.1.9/setup.py` & `dolibs-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 setup(
     name='dolibs',
     packages=find_packages(include=['dolibs']),
-    version='0.1.9',
+    version='0.2.0',
     url='https://github.com/n3tmaster/ERA5_procedures',
     description='Library for importing ERA5 Copernicus data into Drought Observatory platform',
     author='Leandro Rocchi - CNR',
     author_email='leandro.rocchi@cnr.it',
     license='MIT',
     install_requires=['cdsapi','scipy','netcdf4','rioxarray','numpy','xarray','sqlalchemy','psycopg2-binary'],
     setup_requires=['pytest-runner'],
```

