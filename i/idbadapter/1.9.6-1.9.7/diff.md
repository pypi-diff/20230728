# Comparing `tmp/idbadapter-1.9.6.tar.gz` & `tmp/idbadapter-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.9.6.tar", last modified: Tue Jul 25 08:13:34 2023, max compression
+gzip compressed data, was "idbadapter-1.9.7.tar", last modified: Fri Jul 28 06:44:42 2023, max compression
```

## Comparing `idbadapter-1.9.6.tar` & `idbadapter-1.9.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 08:13:34.870033 idbadapter-1.9.6/
--rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.9.6/LICENSE
--rw-rw-rw-   0        0        0      697 2023-07-25 08:13:34.870033 idbadapter-1.9.6/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.9.6/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 08:13:34.861035 idbadapter-1.9.6/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-22 08:18:39.000000 idbadapter-1.9.6/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    12480 2023-07-25 07:30:55.000000 idbadapter-1.9.6/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-25 08:13:34.869036 idbadapter-1.9.6/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      697 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-25 08:13:34.000000 idbadapter-1.9.6/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 08:13:34.871033 idbadapter-1.9.6/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-07-25 08:13:32.000000 idbadapter-1.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:44:42.100642 idbadapter-1.9.7/
+-rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.7/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-07-28 06:44:42.100642 idbadapter-1.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.7/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 06:44:42.076857 idbadapter-1.9.7/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.7/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    12475 2023-07-28 06:42:43.000000 idbadapter-1.9.7/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:44:42.099563 idbadapter-1.9.7/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-28 06:44:42.102436 idbadapter-1.9.7/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-07-28 06:43:02.000000 idbadapter-1.9.7/setup.py
```

### Comparing `idbadapter-1.9.6/LICENSE` & `idbadapter-1.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.9.6/PKG-INFO` & `idbadapter-1.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.6
+Version: 1.9.7
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.6/idbadapter/schedule_loader.py` & `idbadapter-1.9.7/idbadapter/schedule_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         
         result = response.json()
         df = pd.DataFrame(result)
         return df
     
     def get_all_works_name(self):
         query = f"""
-        select DISTINCT w.name as work_name, gw.name as granulary_name, tlw.name as lvl2_name, pn.name as processed_name from works w
+        select DISTINCT w.name as name, gw.name as granulary_name, tlw.name as lvl2_name, pn.name as processed_name from works w
         join work_info wi on w.id = wi.id_work 
         join granulary_works gw on gw.id = wi.id_granulary_work 
         join typed_lvl2_works tlw on tlw.id = wi.id_typed_lvl2_work 
         join processed_works pn on pn.id = wi.id_processed_work"""
         
         df = self._execute_query(query)
         return df
```

### Comparing `idbadapter-1.9.6/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.9.7/idbadapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.6
+Version: 1.9.7
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.6/setup.py` & `idbadapter-1.9.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.9.6'
+version = '1.9.7'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.9.6',
+      version='1.9.7',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

