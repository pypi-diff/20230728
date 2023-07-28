# Comparing `tmp/vdk-ingest-http-0.2.824443273.tar.gz` & `tmp/vdk-ingest-http-0.2.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-ingest-http-0.2.824443273.tar", last modified: Fri Mar 31 14:25:05 2023, max compression
+gzip compressed data, was "vdk-ingest-http-0.2.948436673.tar", last modified: Fri Jul 28 09:42:34 2023, max compression
```

## Comparing `vdk-ingest-http-0.2.824443273.tar` & `vdk-ingest-http-0.2.948436673.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:05.293145 vdk-ingest-http-0.2.824443273/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-03-31 14:25:05.293145 vdk-ingest-http-0.2.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-03-31 14:24:53.000000 vdk-ingest-http-0.2.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:25:05.293145 vdk-ingest-http-0.2.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1127 2023-03-31 14:24:57.000000 vdk-ingest-http-0.2.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:05.289145 vdk-ingest-http-0.2.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:05.289145 vdk-ingest-http-0.2.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:05.289145 vdk-ingest-http-0.2.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:05.293145 vdk-ingest-http-0.2.824443273/src/vdk/plugin/ingest_http/
--rw-rw-rw-   0 root         (0) root         (0)     3420 2023-03-31 14:24:53.000000 vdk-ingest-http-0.2.824443273/src/vdk/plugin/ingest_http/ingest_http_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)     9068 2023-03-31 14:24:53.000000 vdk-ingest-http-0.2.824443273/src/vdk/plugin/ingest_http/ingest_over_http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:05.293145 vdk-ingest-http-0.2.824443273/src/vdk_ingest_http.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2192 2023-03-31 14:25:05.000000 vdk-ingest-http-0.2.824443273/src/vdk_ingest_http.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      405 2023-03-31 14:25:05.000000 vdk-ingest-http-0.2.824443273/src/vdk_ingest_http.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:25:05.000000 vdk-ingest-http-0.2.824443273/src/vdk_ingest_http.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-03-31 14:25:05.000000 vdk-ingest-http-0.2.824443273/src/vdk_ingest_http.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-31 14:25:05.000000 vdk-ingest-http-0.2.824443273/src/vdk_ingest_http.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:25:05.000000 vdk-ingest-http-0.2.824443273/src/vdk_ingest_http.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:05.293145 vdk-ingest-http-0.2.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     9237 2023-03-31 14:24:53.000000 vdk-ingest-http-0.2.824443273/tests/test_ingest_over_http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:34.636023 vdk-ingest-http-0.2.948436673/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-28 09:42:34.636023 vdk-ingest-http-0.2.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-07-28 09:42:14.000000 vdk-ingest-http-0.2.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:34.636023 vdk-ingest-http-0.2.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1127 2023-07-28 09:42:23.000000 vdk-ingest-http-0.2.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:34.632023 vdk-ingest-http-0.2.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:34.632023 vdk-ingest-http-0.2.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:34.632023 vdk-ingest-http-0.2.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:34.632023 vdk-ingest-http-0.2.948436673/src/vdk/plugin/ingest_http/
+-rw-rw-rw-   0 root         (0) root         (0)     3420 2023-07-28 09:42:14.000000 vdk-ingest-http-0.2.948436673/src/vdk/plugin/ingest_http/ingest_http_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)     9068 2023-07-28 09:42:14.000000 vdk-ingest-http-0.2.948436673/src/vdk/plugin/ingest_http/ingest_over_http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:34.632023 vdk-ingest-http-0.2.948436673/src/vdk_ingest_http.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-07-28 09:42:34.000000 vdk-ingest-http-0.2.948436673/src/vdk_ingest_http.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      405 2023-07-28 09:42:34.000000 vdk-ingest-http-0.2.948436673/src/vdk_ingest_http.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:34.000000 vdk-ingest-http-0.2.948436673/src/vdk_ingest_http.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-07-28 09:42:34.000000 vdk-ingest-http-0.2.948436673/src/vdk_ingest_http.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-28 09:42:34.000000 vdk-ingest-http-0.2.948436673/src/vdk_ingest_http.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:34.000000 vdk-ingest-http-0.2.948436673/src/vdk_ingest_http.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:34.632023 vdk-ingest-http-0.2.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9237 2023-07-28 09:42:14.000000 vdk-ingest-http-0.2.948436673/tests/test_ingest_over_http.py
```

### Comparing `vdk-ingest-http-0.2.824443273/PKG-INFO` & `vdk-ingest-http-0.2.948436673/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-ingest-http
-Version: 0.2.824443273
+Version: 0.2.948436673
 Summary: Versatile Data Kit SDK ingestion plugin to ingest data via http requests.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-ingest-http-0.2.824443273/README.md` & `vdk-ingest-http-0.2.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-ingest-http-0.2.824443273/setup.py` & `vdk-ingest-http-0.2.948436673/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.824443273"
+__version__ = "0.2.948436673"
 
 setuptools.setup(
     name="vdk-ingest-http",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK ingestion plugin to ingest data via http requests.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-ingest-http-0.2.824443273/src/vdk/plugin/ingest_http/ingest_http_plugin.py` & `vdk-ingest-http-0.2.948436673/src/vdk/plugin/ingest_http/ingest_http_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-ingest-http-0.2.824443273/src/vdk/plugin/ingest_http/ingest_over_http.py` & `vdk-ingest-http-0.2.948436673/src/vdk/plugin/ingest_http/ingest_over_http.py`

 * *Files identical despite different names*

### Comparing `vdk-ingest-http-0.2.824443273/src/vdk_ingest_http.egg-info/PKG-INFO` & `vdk-ingest-http-0.2.948436673/src/vdk_ingest_http.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-ingest-http
-Version: 0.2.824443273
+Version: 0.2.948436673
 Summary: Versatile Data Kit SDK ingestion plugin to ingest data via http requests.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-ingest-http-0.2.824443273/tests/test_ingest_over_http.py` & `vdk-ingest-http-0.2.948436673/tests/test_ingest_over_http.py`

 * *Files identical despite different names*

