# Comparing `tmp/txdpy-4.5.4.tar.gz` & `tmp/txdpy-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\txdpy-4.5.4.tar", last modified: Tue Jan 17 08:10:03 2023, max compression
+gzip compressed data, was "dist\txdpy-6.0.0.tar", last modified: Fri Jul 28 08:19:04 2023, max compression
```

## Comparing `txdpy-4.5.4.tar` & `txdpy-6.0.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-01-17 08:10:03.000000 txdpy-4.5.4/
--rw-rw-rw-   0        0        0      191 2023-01-17 08:10:03.000000 txdpy-4.5.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-01-17 08:10:03.000000 txdpy-4.5.4/setup.cfg
--rw-rw-rw-   0        0        0      370 2023-01-17 08:07:04.000000 txdpy-4.5.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-17 08:10:03.000000 txdpy-4.5.4/txdpy/
--rw-rw-rw-   0        0        0     2548 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/PyReBf.py
--rw-rw-rw-   0        0        0    39935 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/URLjoin.py
--rw-rw-rw-   0        0        0     1388 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/__init__.py
--rw-rw-rw-   0        0        0     3102 2023-01-17 07:55:05.000000 txdpy-4.5.4/txdpy/easyreq.py
--rw-rw-rw-   0        0        0     1340 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/excel_easy.py
--rw-rw-rw-   0        0        0     2104 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/get_key.py
--rw-rw-rw-   0        0        0     1594 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/list_processing.py
--rw-rw-rw-   0        0        0     1515 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/lookup.py
--rw-rw-rw-   0        0        0     6334 2023-01-17 07:55:05.000000 txdpy-4.5.4/txdpy/pytmysql.py
--rw-rw-rw-   0        0        0     3000 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/requests_operation.py
--rw-rw-rw-   0        0        0      811 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/str_category.py
--rw-rw-rw-   0        0        0     3672 2023-01-17 02:54:55.000000 txdpy-4.5.4/txdpy/uc_easy.py
-drwxrwxrwx   0        0        0        0 2023-01-17 08:10:03.000000 txdpy-4.5.4/txdpy.egg-info/
--rw-rw-rw-   0        0        0      191 2023-01-17 08:10:03.000000 txdpy-4.5.4/txdpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-01-17 08:10:03.000000 txdpy-4.5.4/txdpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-17 08:10:03.000000 txdpy-4.5.4/txdpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2023-01-17 08:10:03.000000 txdpy-4.5.4/txdpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-01-17 08:10:03.000000 txdpy-4.5.4/txdpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-28 08:19:04.000000 txdpy-6.0.0/
+-rw-rw-rw-   0        0        0      191 2023-07-28 08:19:04.000000 txdpy-6.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-07-28 08:19:04.000000 txdpy-6.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      370 2023-07-28 08:17:27.000000 txdpy-6.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:19:04.000000 txdpy-6.0.0/txdpy/
+-rw-rw-rw-   0        0        0     2548 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/PyReBf.py
+-rw-rw-rw-   0        0        0    39935 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/URLjoin.py
+-rw-rw-rw-   0        0        0     2439 2023-07-28 08:15:54.000000 txdpy-6.0.0/txdpy/__init__.py
+-rw-rw-rw-   0        0        0    43672 2023-07-28 08:17:27.000000 txdpy-6.0.0/txdpy/bk_179.py
+-rw-rw-rw-   0        0        0     3102 2023-01-17 07:55:05.000000 txdpy-6.0.0/txdpy/easyreq.py
+-rw-rw-rw-   0        0        0     1340 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/excel_easy.py
+-rw-rw-rw-   0        0        0     2104 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/get_key.py
+-rw-rw-rw-   0        0        0     1594 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/list_processing.py
+-rw-rw-rw-   0        0        0     1515 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/lookup.py
+-rw-rw-rw-   0        0        0     6334 2023-01-17 07:55:05.000000 txdpy-6.0.0/txdpy/pytmysql.py
+-rw-rw-rw-   0        0        0     3000 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/requests_operation.py
+-rw-rw-rw-   0        0        0      811 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/str_category.py
+-rw-rw-rw-   0        0        0     3672 2023-01-17 02:54:55.000000 txdpy-6.0.0/txdpy/uc_easy.py
+drwxrwxrwx   0        0        0        0 2023-07-28 08:19:04.000000 txdpy-6.0.0/txdpy.egg-info/
+-rw-rw-rw-   0        0        0      191 2023-07-28 08:19:04.000000 txdpy-6.0.0/txdpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-07-28 08:19:04.000000 txdpy-6.0.0/txdpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 08:19:04.000000 txdpy-6.0.0/txdpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       97 2023-07-28 08:19:04.000000 txdpy-6.0.0/txdpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-28 08:19:04.000000 txdpy-6.0.0/txdpy.egg-info/top_level.txt
```

### Comparing `txdpy-4.5.4/txdpy/PyReBf.py` & `txdpy-6.0.0/txdpy/PyReBf.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/URLjoin.py` & `txdpy-6.0.0/txdpy/URLjoin.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/easyreq.py` & `txdpy-6.0.0/txdpy/easyreq.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/excel_easy.py` & `txdpy-6.0.0/txdpy/excel_easy.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/get_key.py` & `txdpy-6.0.0/txdpy/get_key.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/list_processing.py` & `txdpy-6.0.0/txdpy/list_processing.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/lookup.py` & `txdpy-6.0.0/txdpy/lookup.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/pytmysql.py` & `txdpy-6.0.0/txdpy/pytmysql.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/requests_operation.py` & `txdpy-6.0.0/txdpy/requests_operation.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/str_category.py` & `txdpy-6.0.0/txdpy/str_category.py`

 * *Files identical despite different names*

### Comparing `txdpy-4.5.4/txdpy/uc_easy.py` & `txdpy-6.0.0/txdpy/uc_easy.py`

 * *Files identical despite different names*

