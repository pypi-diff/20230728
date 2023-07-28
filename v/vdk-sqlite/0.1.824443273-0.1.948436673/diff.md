# Comparing `tmp/vdk-sqlite-0.1.824443273.tar.gz` & `tmp/vdk-sqlite-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-sqlite-0.1.824443273.tar", last modified: Fri Mar 31 14:26:05 2023, max compression
+gzip compressed data, was "vdk-sqlite-0.1.948436673.tar", last modified: Fri Jul 28 09:43:53 2023, max compression
```

## Comparing `vdk-sqlite-0.1.824443273.tar` & `vdk-sqlite-0.1.948436673.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/
--rw-r--r--   0 root         (0) root         (0)       62 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1450 2023-03-31 14:25:52.000000 vdk-sqlite-0.1.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-03-31 14:25:55.000000 vdk-sqlite-0.1.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/
--rw-rw-rw-   0 root         (0) root         (0)    10113 2023-03-31 14:25:52.000000 vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/ingest_to_sqlite.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2023-03-31 14:25:52.000000 vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/sqlite_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-03-31 14:25:52.000000 vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/sqlite_connection.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-03-31 14:25:52.000000 vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/sqlite_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/src/vdk_sqlite.egg-info/
--rw-r--r--   0 root         (0) root         (0)       62 2023-03-31 14:26:05.000000 vdk-sqlite-0.1.824443273/src/vdk_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      446 2023-03-31 14:26:05.000000 vdk-sqlite-0.1.824443273/src/vdk_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:26:05.000000 vdk-sqlite-0.1.824443273/src/vdk_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       62 2023-03-31 14:26:05.000000 vdk-sqlite-0.1.824443273/src/vdk_sqlite.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-31 14:26:05.000000 vdk-sqlite-0.1.824443273/src/vdk_sqlite.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:26:05.000000 vdk-sqlite-0.1.824443273/src/vdk_sqlite.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:05.297152 vdk-sqlite-0.1.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     5223 2023-03-31 14:25:52.000000 vdk-sqlite-0.1.824443273/tests/test_sqlite_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1450 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-28 09:43:37.000000 vdk-sqlite-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.229933 vdk-sqlite-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.229933 vdk-sqlite-0.1.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.229933 vdk-sqlite-0.1.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.229933 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/
+-rw-rw-rw-   0 root         (0) root         (0)    10113 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/ingest_to_sqlite.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_connection.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      446 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:53.000000 vdk-sqlite-0.1.948436673/src/vdk_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:53.233933 vdk-sqlite-0.1.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5223 2023-07-28 09:43:27.000000 vdk-sqlite-0.1.948436673/tests/test_sqlite_plugin.py
```

### Comparing `vdk-sqlite-0.1.824443273/README.md` & `vdk-sqlite-0.1.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.824443273/setup.py` & `vdk-sqlite-0.1.948436673/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # SPDX-License-Identifier: Apache-2.0
 import setuptools
 
 """
 Builds a package with the help of setuptools in order for this package to be imported in other projects
 """
 
-__version__ = "0.1.824443273"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-sqlite",
     version=__version__,
     install_requires=["vdk-core", "tabulate"],
     package_dir={"": "src"},
     packages=setuptools.find_namespace_packages(where="src"),
```

### Comparing `vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/ingest_to_sqlite.py` & `vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/ingest_to_sqlite.py`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/sqlite_configuration.py` & `vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/sqlite_connection.py` & `vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_connection.py`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.824443273/src/vdk/plugin/sqlite/sqlite_plugin.py` & `vdk-sqlite-0.1.948436673/src/vdk/plugin/sqlite/sqlite_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-sqlite-0.1.824443273/tests/test_sqlite_plugin.py` & `vdk-sqlite-0.1.948436673/tests/test_sqlite_plugin.py`

 * *Files identical despite different names*

