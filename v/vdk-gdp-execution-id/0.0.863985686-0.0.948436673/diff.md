# Comparing `tmp/vdk-gdp-execution-id-0.0.863985686.tar.gz` & `tmp/vdk-gdp-execution-id-0.0.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-gdp-execution-id-0.0.863985686.tar", last modified: Thu May 11 07:40:01 2023, max compression
+gzip compressed data, was "vdk-gdp-execution-id-0.0.948436673.tar", last modified: Fri Jul 28 09:42:36 2023, max compression
```

## Comparing `vdk-gdp-execution-id-0.0.863985686.tar` & `vdk-gdp-execution-id-0.0.948436673.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/
--rw-r--r--   0 root         (0) root         (0)     3780 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3095 2023-05-11 07:39:48.000000 vdk-gdp-execution-id-0.0.863985686/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1229 2023-05-11 07:39:52.000000 vdk-gdp-execution-id-0.0.863985686/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/
--rw-rw-rw-   0 root         (0) root         (0)      824 2023-05-11 07:39:48.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     2322 2023-05-11 07:39:48.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-11 07:40:01.973032 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3780 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       92 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-11 07:40:01.000000 vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.694751 vdk-gdp-execution-id-0.0.948436673/
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-28 09:42:36.694751 vdk-gdp-execution-id-0.0.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3095 2023-07-28 09:42:13.000000 vdk-gdp-execution-id-0.0.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:36.694751 vdk-gdp-execution-id-0.0.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2023-07-28 09:42:23.000000 vdk-gdp-execution-id-0.0.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.690751 vdk-gdp-execution-id-0.0.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.690751 vdk-gdp-execution-id-0.0.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.690751 vdk-gdp-execution-id-0.0.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.690751 vdk-gdp-execution-id-0.0.948436673/src/vdk/plugin/gdp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.690751 vdk-gdp-execution-id-0.0.948436673/src/vdk/plugin/gdp/execution_id/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2023-07-28 09:42:13.000000 vdk-gdp-execution-id-0.0.948436673/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     2322 2023-07-28 09:42:13.000000 vdk-gdp-execution-id-0.0.948436673/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:36.690751 vdk-gdp-execution-id-0.0.948436673/src/vdk_gdp_execution_id.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-28 09:42:36.000000 vdk-gdp-execution-id-0.0.948436673/src/vdk_gdp_execution_id.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      433 2023-07-28 09:42:36.000000 vdk-gdp-execution-id-0.0.948436673/src/vdk_gdp_execution_id.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:36.000000 vdk-gdp-execution-id-0.0.948436673/src/vdk_gdp_execution_id.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-07-28 09:42:36.000000 vdk-gdp-execution-id-0.0.948436673/src/vdk_gdp_execution_id.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 09:42:36.000000 vdk-gdp-execution-id-0.0.948436673/src/vdk_gdp_execution_id.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:36.000000 vdk-gdp-execution-id-0.0.948436673/src/vdk_gdp_execution_id.egg-info/top_level.txt
```

### Comparing `vdk-gdp-execution-id-0.0.863985686/PKG-INFO` & `vdk-gdp-execution-id-0.0.948436673/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-gdp-execution-id
-Version: 0.0.863985686
+Version: 0.0.948436673
 Summary: This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset with the execution ID detected during data job run.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-gdp-execution-id-0.0.863985686/README.md` & `vdk-gdp-execution-id-0.0.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-gdp-execution-id-0.0.863985686/setup.py` & `vdk-gdp-execution-id-0.0.948436673/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
-__version__ = "0.0.863985686"
+__version__ = "0.0.948436673"
 
 setuptools.setup(
     name="vdk-gdp-execution-id",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset "
     "with the execution ID detected during data job run.",
```

### Comparing `vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py` & `vdk-gdp-execution-id-0.0.948436673/src/vdk/plugin/gdp/execution_id/gdp_execution_id_configuration.py`

 * *Files identical despite different names*

### Comparing `vdk-gdp-execution-id-0.0.863985686/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py` & `vdk-gdp-execution-id-0.0.948436673/src/vdk/plugin/gdp/execution_id/gdp_execution_id_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-gdp-execution-id-0.0.863985686/src/vdk_gdp_execution_id.egg-info/PKG-INFO` & `vdk-gdp-execution-id-0.0.948436673/src/vdk_gdp_execution_id.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-gdp-execution-id
-Version: 0.0.863985686
+Version: 0.0.948436673
 Summary: This Versatile Data Kit SDK plugin is a Generative Data Pack, that expands each ingested dataset with the execution ID detected during data job run.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

