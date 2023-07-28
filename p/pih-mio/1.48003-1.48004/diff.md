# Comparing `tmp/pih_mio-1.48003.tar.gz` & `tmp/pih_mio-1.48004.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih_mio-1.48003.tar", last modified: Fri Jul 28 09:31:16 2023, max compression
+gzip compressed data, was "pih_mio-1.48004.tar", last modified: Fri Jul 28 11:54:41 2023, max compression
```

## Comparing `pih_mio-1.48003.tar` & `pih_mio-1.48004.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 09:31:16.208093 pih_mio-1.48003/
-drwxrwxrwx   0        0        0        0 2023-07-28 09:31:16.473712 pih_mio-1.48003/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48003/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih_mio-1.48003/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48003/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48003/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48003/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-07-28 09:31:16.708106 pih_mio-1.48003/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 09:31:16.629944 pih_mio-1.48003/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      279 2023-07-28 09:31:15.000000 pih_mio-1.48003/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-07-28 09:31:16.000000 pih_mio-1.48003/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 09:31:15.000000 pih_mio-1.48003/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 09:31:15.000000 pih_mio-1.48003/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 09:31:15.000000 pih_mio-1.48003/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48003/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 09:31:16.724055 pih_mio-1.48003/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 11:54:41.467131 pih_mio-1.48004/
+drwxrwxrwx   0        0        0        0 2023-07-28 11:54:41.499020 pih_mio-1.48004/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48004/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-07-28 11:53:03.000000 pih_mio-1.48004/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165201 2023-07-28 09:30:54.000000 pih_mio-1.48004/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48004/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48004/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48004/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 11:54:41.967779 pih_mio-1.48004/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 11:54:41.889654 pih_mio-1.48004/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 11:54:40.000000 pih_mio-1.48004/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      492 2023-07-28 11:54:41.000000 pih_mio-1.48004/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 11:54:40.000000 pih_mio-1.48004/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 11:54:40.000000 pih_mio-1.48004/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 11:54:40.000000 pih_mio-1.48004/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48004/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 11:54:41.983403 pih_mio-1.48004/setup.cfg
```

### Comparing `pih_mio-1.48003/MobileHelperCore/api.py` & `pih_mio-1.48004/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48003/MobileHelperCore/service.py` & `pih_mio-1.48004/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48003/MobileHelperCore/service_api.py` & `pih_mio-1.48004/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48003/MobileHelperCore/tools.py` & `pih_mio-1.48004/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48003/pih_mio_setup.py` & `pih_mio-1.48004/pih_mio_setup.py`

 * *Files identical despite different names*

