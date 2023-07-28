# Comparing `tmp/pih-mio-1.48011.tar.gz` & `tmp/pih-mio-1.48012.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48011.tar", last modified: Fri Jul 28 13:09:14 2023, max compression
+gzip compressed data, was "pih-mio-1.48012.tar", last modified: Fri Jul 28 13:14:07 2023, max compression
```

## Comparing `pih-mio-1.48011.tar` & `pih-mio-1.48012.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 13:09:13.613616 pih-mio-1.48011/
-drwxrwxrwx   0        0        0        0 2023-07-28 13:09:13.644867 pih-mio-1.48011/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48011/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      225 2023-07-28 13:07:08.000000 pih-mio-1.48011/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-mio-1.48011/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      781 2023-07-28 12:36:33.000000 pih-mio-1.48011/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9217 2023-07-28 13:09:01.000000 pih-mio-1.48011/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48011/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 13:09:14.191735 pih-mio-1.48011/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 13:09:14.144860 pih-mio-1.48011/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 13:09:12.000000 pih-mio-1.48011/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-28 13:09:13.000000 pih-mio-1.48011/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 13:09:12.000000 pih-mio-1.48011/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-28 13:09:12.000000 pih-mio-1.48011/pih_MIO.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 13:09:13.000000 pih-mio-1.48011/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 13:09:13.000000 pih-mio-1.48011/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48011/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 13:09:14.207367 pih-mio-1.48011/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 13:14:06.977972 pih-mio-1.48012/
+drwxrwxrwx   0        0        0        0 2023-07-28 13:14:07.307916 pih-mio-1.48012/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48012/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      236 2023-07-28 13:12:31.000000 pih-mio-1.48012/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-mio-1.48012/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      781 2023-07-28 12:36:33.000000 pih-mio-1.48012/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9217 2023-07-28 13:09:01.000000 pih-mio-1.48012/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48012/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 13:14:07.698558 pih-mio-1.48012/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 13:14:07.604825 pih-mio-1.48012/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 13:14:06.000000 pih-mio-1.48012/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48012/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 13:14:07.745486 pih-mio-1.48012/setup.cfg
```

### Comparing `pih-mio-1.48011/MobileHelperCore/api.py` & `pih-mio-1.48012/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48011/MobileHelperCore/service.py` & `pih-mio-1.48012/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48011/MobileHelperCore/service_api.py` & `pih-mio-1.48012/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48011/MobileHelperCore/tools.py` & `pih-mio-1.48012/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48011/pih_MIO.egg-info/SOURCES.txt` & `pih-mio-1.48012/pih_MIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48011/pih_mio_setup.py` & `pih-mio-1.48012/pih_mio_setup.py`

 * *Files identical despite different names*

