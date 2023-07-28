# Comparing `tmp/vdk-csv-0.1.824443273.tar.gz` & `tmp/vdk-csv-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-csv-0.1.824443273.tar", last modified: Fri Mar 31 14:25:18 2023, max compression
+gzip compressed data, was "vdk-csv-0.1.948436673.tar", last modified: Fri Jul 28 09:42:36 2023, max compression
```

## Comparing `vdk-csv-0.1.824443273.tar` & `vdk-csv-0.1.948436673.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/
--rw-r--r--   0 root         (0) root         (0)     1163 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      562 2023-03-31 14:25:06.000000 vdk-csv-0.1.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1059 2023-03-31 14:25:09.000000 vdk-csv-0.1.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/src/vdk/plugin/csv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/src/vdk/plugin/csv/csv_export_job/
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-03-31 14:25:06.000000 vdk-csv-0.1.824443273/src/vdk/plugin/csv/csv_export_job/csv_export_step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/src/vdk/plugin/csv/csv_ingest_job/
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-03-31 14:25:06.000000 vdk-csv-0.1.824443273/src/vdk/plugin/csv/csv_ingest_job/csv_ingest_step.py
--rw-rw-rw-   0 root         (0) root         (0)     4450 2023-03-31 14:25:06.000000 vdk-csv-0.1.824443273/src/vdk/plugin/csv/csv_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:18.479767 vdk-csv-0.1.824443273/src/vdk_csv.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1163 2023-03-31 14:25:18.000000 vdk-csv-0.1.824443273/src/vdk_csv.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2023-03-31 14:25:18.000000 vdk-csv-0.1.824443273/src/vdk_csv.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:25:18.000000 vdk-csv-0.1.824443273/src/vdk_csv.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-03-31 14:25:18.000000 vdk-csv-0.1.824443273/src/vdk_csv.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-03-31 14:25:18.000000 vdk-csv-0.1.824443273/src/vdk_csv.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:25:18.000000 vdk-csv-0.1.824443273/src/vdk_csv.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      562 2023-07-28 09:42:13.000000 vdk-csv-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2023-07-28 09:42:23.000000 vdk-csv-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/src/vdk/plugin/csv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/src/vdk/plugin/csv/csv_export_job/
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-07-28 09:42:13.000000 vdk-csv-0.1.948436673/src/vdk/plugin/csv/csv_export_job/csv_export_step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/src/vdk/plugin/csv/csv_ingest_job/
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-28 09:42:13.000000 vdk-csv-0.1.948436673/src/vdk/plugin/csv/csv_ingest_job/csv_ingest_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4450 2023-07-28 09:42:13.000000 vdk-csv-0.1.948436673/src/vdk/plugin/csv/csv_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.507214 vdk-csv-0.1.948436673/src/vdk_csv.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-07-28 09:42:36.000000 vdk-csv-0.1.948436673/src/vdk_csv.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-07-28 09:42:36.000000 vdk-csv-0.1.948436673/src/vdk_csv.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:36.000000 vdk-csv-0.1.948436673/src/vdk_csv.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       53 2023-07-28 09:42:36.000000 vdk-csv-0.1.948436673/src/vdk_csv.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-28 09:42:36.000000 vdk-csv-0.1.948436673/src/vdk_csv.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:36.000000 vdk-csv-0.1.948436673/src/vdk_csv.egg-info/top_level.txt
```

### Comparing `vdk-csv-0.1.824443273/PKG-INFO` & `vdk-csv-0.1.948436673/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-csv
-Version: 0.1.824443273
+Version: 0.1.948436673
 Summary: Versatile Data Kit SDK CSV plugin to ingest, export, or manipulate csv files.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-csv-0.1.824443273/README.md` & `vdk-csv-0.1.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-csv-0.1.824443273/setup.py` & `vdk-csv-0.1.948436673/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.1.824443273"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-csv",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK CSV plugin to ingest, export, or manipulate csv files.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-csv-0.1.824443273/src/vdk/plugin/csv/csv_export_job/csv_export_step.py` & `vdk-csv-0.1.948436673/src/vdk/plugin/csv/csv_export_job/csv_export_step.py`

 * *Files identical despite different names*

### Comparing `vdk-csv-0.1.824443273/src/vdk/plugin/csv/csv_ingest_job/csv_ingest_step.py` & `vdk-csv-0.1.948436673/src/vdk/plugin/csv/csv_ingest_job/csv_ingest_step.py`

 * *Files identical despite different names*

### Comparing `vdk-csv-0.1.824443273/src/vdk/plugin/csv/csv_plugin.py` & `vdk-csv-0.1.948436673/src/vdk/plugin/csv/csv_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-csv-0.1.824443273/src/vdk_csv.egg-info/PKG-INFO` & `vdk-csv-0.1.948436673/src/vdk_csv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-csv
-Version: 0.1.824443273
+Version: 0.1.948436673
 Summary: Versatile Data Kit SDK CSV plugin to ingest, export, or manipulate csv files.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

