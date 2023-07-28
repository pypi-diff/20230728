# Comparing `tmp/vdk-notebook-0.1.914806943.tar.gz` & `tmp/vdk-notebook-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-notebook-0.1.914806943.tar", last modified: Wed Jun 28 13:44:31 2023, max compression
+gzip compressed data, was "vdk-notebook-0.1.948436673.tar", last modified: Fri Jul 28 09:43:19 2023, max compression
```

## Comparing `vdk-notebook-0.1.914806943.tar` & `vdk-notebook-0.1.948436673.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/
--rw-r--r--   0 root         (0) root         (0)     1804 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-28 13:44:17.000000 vdk-notebook-0.1.914806943/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-06-28 13:44:21.000000 vdk-notebook-0.1.914806943/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/src/vdk/plugin/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/
--rw-rw-rw-   0 root         (0) root         (0)      522 2023-06-28 13:44:17.000000 vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/cell.py
--rw-rw-rw-   0 root         (0) root         (0)     4289 2023-06-28 13:44:17.000000 vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/notebook.py
--rw-rw-rw-   0 root         (0) root         (0)     4452 2023-06-28 13:44:17.000000 vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/notebook_based_step.py
--rw-rw-rw-   0 root         (0) root         (0)     2008 2023-06-28 13:44:17.000000 vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/notebook_plugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/src/vdk_notebook.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1804 2023-06-28 13:44:31.000000 vdk-notebook-0.1.914806943/src/vdk_notebook.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      439 2023-06-28 13:44:31.000000 vdk-notebook-0.1.914806943/src/vdk_notebook.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-28 13:44:31.000000 vdk-notebook-0.1.914806943/src/vdk_notebook.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-06-28 13:44:31.000000 vdk-notebook-0.1.914806943/src/vdk_notebook.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-06-28 13:44:31.000000 vdk-notebook-0.1.914806943/src/vdk_notebook.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-06-28 13:44:31.000000 vdk-notebook-0.1.914806943/src/vdk_notebook.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-28 13:44:31.500340 vdk-notebook-0.1.914806943/tests/
--rw-rw-rw-   0 root         (0) root         (0)     2608 2023-06-28 13:44:17.000000 vdk-notebook-0.1.914806943/tests/test_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:19.340386 vdk-notebook-0.1.948436673/
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-07-28 09:43:19.340386 vdk-notebook-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2023-07-28 09:42:58.000000 vdk-notebook-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:43:19.340386 vdk-notebook-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-07-28 09:43:07.000000 vdk-notebook-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:19.336386 vdk-notebook-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:19.336386 vdk-notebook-0.1.948436673/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:19.336386 vdk-notebook-0.1.948436673/src/vdk/plugin/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:19.336386 vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/
+-rw-rw-rw-   0 root         (0) root         (0)      522 2023-07-28 09:42:58.000000 vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/cell.py
+-rw-rw-rw-   0 root         (0) root         (0)     4289 2023-07-28 09:42:58.000000 vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/notebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     4452 2023-07-28 09:42:58.000000 vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/notebook_based_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     2008 2023-07-28 09:42:58.000000 vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/notebook_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:19.336386 vdk-notebook-0.1.948436673/src/vdk_notebook.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1804 2023-07-28 09:43:19.000000 vdk-notebook-0.1.948436673/src/vdk_notebook.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      439 2023-07-28 09:43:19.000000 vdk-notebook-0.1.948436673/src/vdk_notebook.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:43:19.000000 vdk-notebook-0.1.948436673/src/vdk_notebook.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-07-28 09:43:19.000000 vdk-notebook-0.1.948436673/src/vdk_notebook.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-28 09:43:19.000000 vdk-notebook-0.1.948436673/src/vdk_notebook.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-28 09:43:19.000000 vdk-notebook-0.1.948436673/src/vdk_notebook.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:43:19.336386 vdk-notebook-0.1.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2608 2023-07-28 09:42:58.000000 vdk-notebook-0.1.948436673/tests/test_plugin.py
```

### Comparing `vdk-notebook-0.1.914806943/PKG-INFO` & `vdk-notebook-0.1.948436673/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-notebook
-Version: 0.1.914806943
+Version: 0.1.948436673
 Summary: A VDK plugin for working with notebooks
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-notebook-0.1.914806943/README.md` & `vdk-notebook-0.1.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-notebook-0.1.914806943/setup.py` & `vdk-notebook-0.1.948436673/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.1.914806943"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-notebook",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="A VDK plugin for working with notebooks",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/cell.py` & `vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/cell.py`

 * *Files identical despite different names*

### Comparing `vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/notebook.py` & `vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/notebook_based_step.py` & `vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/notebook_based_step.py`

 * *Files identical despite different names*

### Comparing `vdk-notebook-0.1.914806943/src/vdk/plugin/notebook/notebook_plugin.py` & `vdk-notebook-0.1.948436673/src/vdk/plugin/notebook/notebook_plugin.py`

 * *Files identical despite different names*

### Comparing `vdk-notebook-0.1.914806943/src/vdk_notebook.egg-info/PKG-INFO` & `vdk-notebook-0.1.948436673/src/vdk_notebook.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-notebook
-Version: 0.1.914806943
+Version: 0.1.948436673
 Summary: A VDK plugin for working with notebooks
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-notebook-0.1.914806943/tests/test_plugin.py` & `vdk-notebook-0.1.948436673/tests/test_plugin.py`

 * *Files identical despite different names*

