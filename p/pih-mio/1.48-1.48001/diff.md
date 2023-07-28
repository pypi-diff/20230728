# Comparing `tmp/pih_mio-1.48.tar.gz` & `tmp/pih_mio-1.48001.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih_mio-1.48.tar", last modified: Fri Jul 28 09:14:52 2023, max compression
+gzip compressed data, was "pih_mio-1.48001.tar", last modified: Fri Jul 28 09:16:20 2023, max compression
```

## Comparing `pih_mio-1.48.tar` & `pih_mio-1.48001.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 09:14:51.509624 pih_mio-1.48/
-drwxrwxrwx   0        0        0        0 2023-07-28 09:14:51.853349 pih_mio-1.48/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0   165160 2023-07-28 09:13:23.000000 pih_mio-1.48/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      276 2023-07-28 09:14:52.259593 pih_mio-1.48/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-28 09:14:52.009607 pih_mio-1.48/pih_MIO.egg-info/
--rw-rw-rw-   0        0        0      276 2023-07-28 09:14:50.000000 pih_mio-1.48/pih_MIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      463 2023-07-28 09:14:51.000000 pih_mio-1.48/pih_MIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 09:14:50.000000 pih_mio-1.48/pih_MIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-07-28 09:14:50.000000 pih_mio-1.48/pih_MIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-28 09:14:50.000000 pih_mio-1.48/pih_MIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48/pih_mio_setup.py
--rw-rw-rw-   0        0        0       42 2023-07-28 09:14:52.275218 pih_mio-1.48/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-28 09:16:20.504282 pih_mio-1.48001/
+drwxrwxrwx   0        0        0        0 2023-07-28 09:16:20.535545 pih_mio-1.48001/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih_mio-1.48001/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0   165160 2023-07-28 09:13:23.000000 pih_mio-1.48001/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      686 2023-07-17 12:20:25.000000 pih_mio-1.48001/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9200 2023-07-23 04:55:02.000000 pih_mio-1.48001/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih_mio-1.48001/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-07-28 09:16:20.958198 pih_mio-1.48001/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-28 09:16:20.895689 pih_mio-1.48001/pih_MIO.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-07-28 09:16:19.000000 pih_mio-1.48001/pih_MIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2023-07-28 09:16:20.000000 pih_mio-1.48001/pih_MIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:16:19.000000 pih_mio-1.48001/pih_MIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-28 09:16:20.000000 pih_mio-1.48001/pih_MIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-28 09:16:20.000000 pih_mio-1.48001/pih_MIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1501 2023-07-28 09:13:59.000000 pih_mio-1.48001/pih_mio_setup.py
+-rw-rw-rw-   0        0        0       42 2023-07-28 09:16:20.958198 pih_mio-1.48001/setup.cfg
```

### Comparing `pih_mio-1.48/MobileHelperCore/api.py` & `pih_mio-1.48001/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48/MobileHelperCore/service.py` & `pih_mio-1.48001/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48/MobileHelperCore/service_api.py` & `pih_mio-1.48001/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48/MobileHelperCore/tools.py` & `pih_mio-1.48001/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih_mio-1.48/pih_mio_setup.py` & `pih_mio-1.48001/pih_mio_setup.py`

 * *Files identical despite different names*

