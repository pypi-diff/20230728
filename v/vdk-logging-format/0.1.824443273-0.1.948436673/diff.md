# Comparing `tmp/vdk-logging-format-0.1.824443273.tar.gz` & `tmp/vdk-logging-format-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-logging-format-0.1.824443273.tar", last modified: Fri Mar 31 14:25:59 2023, max compression
+gzip compressed data, was "vdk-logging-format-0.1.948436673.tar", last modified: Fri Jul 28 09:42:41 2023, max compression
```

## Comparing `vdk-logging-format-0.1.824443273.tar` & `vdk-logging-format-0.1.948436673.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/
--rw-r--r--   0 root         (0) root         (0)     4976 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4373 2023-03-31 14:25:47.000000 vdk-logging-format-0.1.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-03-31 14:25:51.000000 vdk-logging-format-0.1.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/src/vdk/plugin/logging_format/
--rw-rw-rw-   0 root         (0) root         (0)     3878 2023-03-31 14:25:47.000000 vdk-logging-format-0.1.824443273/src/vdk/plugin/logging_format/logging_format.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/src/vdk_logging_format.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4976 2023-03-31 14:25:59.000000 vdk-logging-format-0.1.824443273/src/vdk_logging_format.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      371 2023-03-31 14:25:59.000000 vdk-logging-format-0.1.824443273/src/vdk_logging_format.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:25:59.000000 vdk-logging-format-0.1.824443273/src/vdk_logging_format.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-03-31 14:25:59.000000 vdk-logging-format-0.1.824443273/src/vdk_logging_format.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-31 14:25:59.000000 vdk-logging-format-0.1.824443273/src/vdk_logging_format.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:25:59.000000 vdk-logging-format-0.1.824443273/src/vdk_logging_format.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:25:59.573151 vdk-logging-format-0.1.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-03-31 14:25:47.000000 vdk-logging-format-0.1.824443273/tests/test_logging_json.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/
+-rw-r--r--   0 root         (0) root         (0)     4976 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2023-07-28 09:42:19.000000 vdk-logging-format-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-28 09:42:28.000000 vdk-logging-format-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/src/vdk/plugin/logging_format/
+-rw-rw-rw-   0 root         (0) root         (0)     3878 2023-07-28 09:42:19.000000 vdk-logging-format-0.1.948436673/src/vdk/plugin/logging_format/logging_format.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/src/vdk_logging_format.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4976 2023-07-28 09:42:41.000000 vdk-logging-format-0.1.948436673/src/vdk_logging_format.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      371 2023-07-28 09:42:41.000000 vdk-logging-format-0.1.948436673/src/vdk_logging_format.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:41.000000 vdk-logging-format-0.1.948436673/src/vdk_logging_format.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-07-28 09:42:41.000000 vdk-logging-format-0.1.948436673/src/vdk_logging_format.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 09:42:41.000000 vdk-logging-format-0.1.948436673/src/vdk_logging_format.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:42:41.000000 vdk-logging-format-0.1.948436673/src/vdk_logging_format.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:41.163223 vdk-logging-format-0.1.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-07-28 09:42:19.000000 vdk-logging-format-0.1.948436673/tests/test_logging_json.py
```

### Comparing `vdk-logging-format-0.1.824443273/PKG-INFO` & `vdk-logging-format-0.1.948436673/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-logging-format
-Version: 0.1.824443273
+Version: 0.1.948436673
 Summary: Versatile Data Kit SDK plugin that configures logging output format.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-logging-format-0.1.824443273/README.md` & `vdk-logging-format-0.1.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-logging-format-0.1.824443273/setup.py` & `vdk-logging-format-0.1.948436673/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.1.824443273"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-logging-format",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin that configures logging output format.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-logging-format-0.1.824443273/src/vdk/plugin/logging_format/logging_format.py` & `vdk-logging-format-0.1.948436673/src/vdk/plugin/logging_format/logging_format.py`

 * *Files identical despite different names*

### Comparing `vdk-logging-format-0.1.824443273/src/vdk_logging_format.egg-info/PKG-INFO` & `vdk-logging-format-0.1.948436673/src/vdk_logging_format.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-logging-format
-Version: 0.1.824443273
+Version: 0.1.948436673
 Summary: Versatile Data Kit SDK plugin that configures logging output format.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-logging-format-0.1.824443273/tests/test_logging_json.py` & `vdk-logging-format-0.1.948436673/tests/test_logging_json.py`

 * *Files identical despite different names*

