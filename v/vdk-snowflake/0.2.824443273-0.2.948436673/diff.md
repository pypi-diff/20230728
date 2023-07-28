# Comparing `tmp/vdk-snowflake-0.2.824443273.tar.gz` & `tmp/vdk-snowflake-0.2.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-snowflake-0.2.824443273.tar", last modified: Fri Mar 31 14:26:04 2023, max compression
+gzip compressed data, was "vdk-snowflake-0.2.948436673.tar", last modified: Fri Jul 28 09:43:54 2023, max compression
```

## Comparing `vdk-snowflake-0.2.824443273.tar` & `vdk-snowflake-0.2.948436673.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/
--rw-r--r--   0 root         (0) root         (0)     2236 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1635 2023-03-31 14:25:52.000000 vdk-snowflake-0.2.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1111 2023-03-31 14:25:56.000000 vdk-snowflake-0.2.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/src/vdk/plugin/snowflake/
--rw-rw-rw-   0 root         (0) root         (0)     2088 2023-03-31 14:25:52.000000 vdk-snowflake-0.2.824443273/src/vdk/plugin/snowflake/snowflake_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     3876 2023-03-31 14:25:52.000000 vdk-snowflake-0.2.824443273/src/vdk/plugin/snowflake/snowflake_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2023-03-31 14:25:52.000000 vdk-snowflake-0.2.824443273/src/vdk/plugin/snowflake/snowflake_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/src/vdk_snowflake.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2236 2023-03-31 14:26:04.000000 vdk-snowflake-0.2.824443273/src/vdk_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      478 2023-03-31 14:26:04.000000 vdk-snowflake-0.2.824443273/src/vdk_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:26:04.000000 vdk-snowflake-0.2.824443273/src/vdk_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-03-31 14:26:04.000000 vdk-snowflake-0.2.824443273/src/vdk_snowflake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       36 2023-03-31 14:26:04.000000 vdk-snowflake-0.2.824443273/src/vdk_snowflake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:26:04.000000 vdk-snowflake-0.2.824443273/src/vdk_snowflake.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.290739 vdk-snowflake-0.2.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-03-31 14:25:52.000000 vdk-snowflake-0.2.824443273/tests/test_snowflake_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     1476 2023-03-31 14:25:52.000000 vdk-snowflake-0.2.824443273/tests/test_snowflake_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1635 2023-07-28 09:43:29.000000 vdk-snowflake-0.2.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1111 2023-07-28 09:43:40.000000 vdk-snowflake-0.2.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/src/vdk/plugin/snowflake/
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2023-07-28 09:43:29.000000 vdk-snowflake-0.2.948436673/src/vdk/plugin/snowflake/snowflake_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     3876 2023-07-28 09:43:29.000000 vdk-snowflake-0.2.948436673/src/vdk/plugin/snowflake/snowflake_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2023-07-28 09:43:29.000000 vdk-snowflake-0.2.948436673/src/vdk/plugin/snowflake/snowflake_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/src/vdk_snowflake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2236 2023-07-28 09:43:54.000000 vdk-snowflake-0.2.948436673/src/vdk_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-28 09:43:54.000000 vdk-snowflake-0.2.948436673/src/vdk_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:54.000000 vdk-snowflake-0.2.948436673/src/vdk_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-28 09:43:54.000000 vdk-snowflake-0.2.948436673/src/vdk_snowflake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-28 09:43:54.000000 vdk-snowflake-0.2.948436673/src/vdk_snowflake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:54.000000 vdk-snowflake-0.2.948436673/src/vdk_snowflake.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:54.909942 vdk-snowflake-0.2.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-28 09:43:29.000000 vdk-snowflake-0.2.948436673/tests/test_snowflake_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     1476 2023-07-28 09:43:29.000000 vdk-snowflake-0.2.948436673/tests/test_snowflake_plugin.py
```

### Comparing `vdk-snowflake-0.2.824443273/PKG-INFO` & `vdk-snowflake-0.2.948436673/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-snowflake
-Version: 0.2.824443273
+Version: 0.2.948436673
 Summary: Versatile Data Kit SDK plugin provides support for snowflake databases.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-snowflake-0.2.824443273/README.md` & `vdk-snowflake-0.2.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-snowflake-0.2.824443273/setup.py` & `vdk-snowflake-0.2.948436673/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.2.824443273"
+__version__ = "0.2.948436673"
 
 setuptools.setup(
     name="vdk-snowflake",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for snowflake databases.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-snowflake-0.2.824443273/src/vdk/plugin/snowflake/snowflake_configuration.py` & `vdk-snowflake-0.2.948436673/src/vdk/plugin/snowflake/snowflake_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-snowflake-0.2.824443273/src/vdk/plugin/snowflake/snowflake_connection.py` & `vdk-snowflake-0.2.948436673/src/vdk/plugin/snowflake/snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-snowflake-0.2.824443273/src/vdk/plugin/snowflake/snowflake_plugin.py` & `vdk-snowflake-0.2.948436673/src/vdk/plugin/snowflake/snowflake_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-snowflake-0.2.824443273/src/vdk_snowflake.egg-info/PKG-INFO` & `vdk-snowflake-0.2.948436673/src/vdk_snowflake.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-snowflake
-Version: 0.2.824443273
+Version: 0.2.948436673
 Summary: Versatile Data Kit SDK plugin provides support for snowflake databases.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-snowflake-0.2.824443273/tests/test_snowflake_connection.py` & `vdk-snowflake-0.2.948436673/tests/test_snowflake_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-snowflake-0.2.824443273/tests/test_snowflake_plugin.py` & `vdk-snowflake-0.2.948436673/tests/test_snowflake_plugin.py`

 * *Files identical despite different names*

