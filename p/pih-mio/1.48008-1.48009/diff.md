# Comparing `tmp/pih-mio-1.48008.tar.gz` & `tmp/pih-mio-1.48009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48008.tar", last modified: Fri Jul 28 12:43:48 2023, max compression
+gzip compressed data, was "pih-mio-1.48009.tar", last modified: Fri Jul 28 12:48:50 2023, max compression
```

## Comparing `pih-mio-1.48008.tar` & `pih-mio-1.48009.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 12:43:47.637864 pih-mio-1.48008/
-drwxrwxrwx   0        0        0        0 2023-07-28 12:43:47.684736 pih-mio-1.48008/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48008/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      206 2023-07-28 12:42:54.000000 pih-mio-1.48008/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-mio-1.48008/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      781 2023-07-28 12:36:33.000000 pih-mio-1.48008/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih-mio-1.48008/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48008/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 12:43:48.190597 pih-mio-1.48008/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 12:43:48.143725 pih-mio-1.48008/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 12:43:46.000000 pih-mio-1.48008/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-07-28 12:43:47.000000 pih-mio-1.48008/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 12:43:46.000000 pih-mio-1.48008/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-07-28 12:43:46.000000 pih-mio-1.48008/pih_MIO.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 12:43:47.000000 pih-mio-1.48008/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 12:43:47.000000 pih-mio-1.48008/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48008/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 12:43:48.190597 pih-mio-1.48008/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 12:48:49.713178 pih-mio-1.48009/
+drwxrwxrwx   0        0        0        0 2023-07-28 12:48:50.041305 pih-mio-1.48009/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48009/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      208 2023-07-28 12:47:58.000000 pih-mio-1.48009/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih-mio-1.48009/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      781 2023-07-28 12:36:33.000000 pih-mio-1.48009/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih-mio-1.48009/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48009/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 12:48:50.322547 pih-mio-1.48009/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 12:48:50.260046 pih-mio-1.48009/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 12:48:48.000000 pih-mio-1.48009/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-07-28 12:48:49.000000 pih-mio-1.48009/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 12:48:48.000000 pih-mio-1.48009/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-07-28 12:48:48.000000 pih-mio-1.48009/pih_MIO.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 12:48:49.000000 pih-mio-1.48009/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 12:48:49.000000 pih-mio-1.48009/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1644 2023-07-28 12:42:15.000000 pih-mio-1.48009/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 12:48:50.322547 pih-mio-1.48009/setup.cfg
```

### Comparing `pih-mio-1.48008/MobileHelperCore/api.py` & `pih-mio-1.48009/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48008/MobileHelperCore/service.py` & `pih-mio-1.48009/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48008/MobileHelperCore/service_api.py` & `pih-mio-1.48009/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48008/MobileHelperCore/tools.py` & `pih-mio-1.48009/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48008/pih_MIO.egg-info/SOURCES.txt` & `pih-mio-1.48009/pih_MIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48008/pih_mio_setup.py` & `pih-mio-1.48009/pih_mio_setup.py`

 * *Files identical despite different names*

