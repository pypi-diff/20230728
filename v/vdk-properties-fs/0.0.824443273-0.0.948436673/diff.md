# Comparing `tmp/vdk-properties-fs-0.0.824443273.tar.gz` & `tmp/vdk-properties-fs-0.0.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-properties-fs-0.0.824443273.tar", last modified: Fri Mar 31 14:26:04 2023, max compression
+gzip compressed data, was "vdk-properties-fs-0.0.948436673.tar", last modified: Fri Jul 28 09:43:20 2023, max compression
```

## Comparing `vdk-properties-fs-0.0.824443273.tar` & `vdk-properties-fs-0.0.948436673.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.452617 vdk-properties-fs-0.0.824443273/
--rw-r--r--   0 root         (0) root         (0)     1798 2023-03-31 14:26:04.452617 vdk-properties-fs-0.0.824443273/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-03-31 14:25:52.000000 vdk-properties-fs-0.0.824443273/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-31 14:26:04.452617 vdk-properties-fs-0.0.824443273/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1179 2023-03-31 14:25:55.000000 vdk-properties-fs-0.0.824443273/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.448617 vdk-properties-fs-0.0.824443273/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.448617 vdk-properties-fs-0.0.824443273/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.448617 vdk-properties-fs-0.0.824443273/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.448617 vdk-properties-fs-0.0.824443273/src/vdk/plugin/properties_fs/
--rw-rw-rw-   0 root         (0) root         (0)     2638 2023-03-31 14:25:52.000000 vdk-properties-fs-0.0.824443273/src/vdk/plugin/properties_fs/fs_properties_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1507 2023-03-31 14:25:52.000000 vdk-properties-fs-0.0.824443273/src/vdk/plugin/properties_fs/fs_properties_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.452617 vdk-properties-fs-0.0.824443273/src/vdk_properties_fs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1798 2023-03-31 14:26:04.000000 vdk-properties-fs-0.0.824443273/src/vdk_properties_fs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      431 2023-03-31 14:26:04.000000 vdk-properties-fs-0.0.824443273/src/vdk_properties_fs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-31 14:26:04.000000 vdk-properties-fs-0.0.824443273/src/vdk_properties_fs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       83 2023-03-31 14:26:04.000000 vdk-properties-fs-0.0.824443273/src/vdk_properties_fs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-31 14:26:04.000000 vdk-properties-fs-0.0.824443273/src/vdk_properties_fs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-03-31 14:26:04.000000 vdk-properties-fs-0.0.824443273/src/vdk_properties_fs.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-31 14:26:04.452617 vdk-properties-fs-0.0.824443273/tests/
--rw-rw-rw-   0 root         (0) root         (0)     3004 2023-03-31 14:25:52.000000 vdk-properties-fs-0.0.824443273/tests/test_fs_properties_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-07-28 09:42:59.000000 vdk-properties-fs-0.0.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2023-07-28 09:43:08.000000 vdk-properties-fs-0.0.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/src/vdk/plugin/properties_fs/
+-rw-rw-rw-   0 root         (0) root         (0)     2638 2023-07-28 09:42:59.000000 vdk-properties-fs-0.0.948436673/src/vdk/plugin/properties_fs/fs_properties_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1507 2023-07-28 09:42:59.000000 vdk-properties-fs-0.0.948436673/src/vdk/plugin/properties_fs/fs_properties_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/src/vdk_properties_fs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1798 2023-07-28 09:43:20.000000 vdk-properties-fs-0.0.948436673/src/vdk_properties_fs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      431 2023-07-28 09:43:20.000000 vdk-properties-fs-0.0.948436673/src/vdk_properties_fs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:20.000000 vdk-properties-fs-0.0.948436673/src/vdk_properties_fs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-07-28 09:43:20.000000 vdk-properties-fs-0.0.948436673/src/vdk_properties_fs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 09:43:20.000000 vdk-properties-fs-0.0.948436673/src/vdk_properties_fs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:20.000000 vdk-properties-fs-0.0.948436673/src/vdk_properties_fs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:20.099291 vdk-properties-fs-0.0.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3004 2023-07-28 09:42:59.000000 vdk-properties-fs-0.0.948436673/tests/test_fs_properties_plugin.py
```

### Comparing `vdk-properties-fs-0.0.824443273/PKG-INFO` & `vdk-properties-fs-0.0.948436673/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-properties-fs
-Version: 0.0.824443273
+Version: 0.0.948436673
 Summary: Versatile Data Kit SDK plugin provides support for Properties API client that uses local FS storage.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-properties-fs-0.0.824443273/README.md` & `vdk-properties-fs-0.0.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-properties-fs-0.0.824443273/setup.py` & `vdk-properties-fs-0.0.948436673/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.0.824443273"
+__version__ = "0.0.948436673"
 
 setuptools.setup(
     name="vdk-properties-fs",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Versatile Data Kit SDK plugin provides support for Properties API client that uses local FS storage.",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-properties-fs-0.0.824443273/src/vdk/plugin/properties_fs/fs_properties_client.py` & `vdk-properties-fs-0.0.948436673/src/vdk/plugin/properties_fs/fs_properties_client.py`

 * *Files identical despite different names*

### Comparing `vdk-properties-fs-0.0.824443273/src/vdk/plugin/properties_fs/fs_properties_plugin.py` & `vdk-properties-fs-0.0.948436673/src/vdk/plugin/properties_fs/fs_properties_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-properties-fs-0.0.824443273/src/vdk_properties_fs.egg-info/PKG-INFO` & `vdk-properties-fs-0.0.948436673/src/vdk_properties_fs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-properties-fs
-Version: 0.0.824443273
+Version: 0.0.948436673
 Summary: Versatile Data Kit SDK plugin provides support for Properties API client that uses local FS storage.
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-properties-fs-0.0.824443273/tests/test_fs_properties_plugin.py` & `vdk-properties-fs-0.0.948436673/tests/test_fs_properties_plugin.py`

 * *Files identical despite different names*

