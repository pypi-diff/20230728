# Comparing `tmp/vdk-ipython-0.1.919227134.tar.gz` & `tmp/vdk-ipython-0.1.948436673.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vdk-ipython-0.1.919227134.tar", last modified: Mon Jul  3 12:04:37 2023, max compression
+gzip compressed data, was "vdk-ipython-0.1.948436673.tar", last modified: Fri Jul 28 09:42:42 2023, max compression
```

## Comparing `vdk-ipython-0.1.919227134.tar` & `vdk-ipython-0.1.948436673.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:04:37.699095 vdk-ipython-0.1.919227134/
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-03 12:04:37.699095 vdk-ipython-0.1.919227134/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-03 12:04:22.000000 vdk-ipython-0.1.919227134/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-03 12:04:37.699095 vdk-ipython-0.1.919227134/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1035 2023-07-03 12:04:27.000000 vdk-ipython-0.1.919227134/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:04:37.695095 vdk-ipython-0.1.919227134/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:04:37.699095 vdk-ipython-0.1.919227134/src/vdk_ipython.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2298 2023-07-03 12:04:37.000000 vdk-ipython-0.1.919227134/src/vdk_ipython.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      275 2023-07-03 12:04:37.000000 vdk-ipython-0.1.919227134/src/vdk_ipython.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:04:37.000000 vdk-ipython-0.1.919227134/src/vdk_ipython.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-07-03 12:04:37.000000 vdk-ipython-0.1.919227134/src/vdk_ipython.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-07-03 12:04:37.000000 vdk-ipython-0.1.919227134/src/vdk_ipython.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 12:04:37.000000 vdk-ipython-0.1.919227134/src/vdk_ipython.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 12:04:37.699095 vdk-ipython-0.1.919227134/tests/
--rw-rw-rw-   0 root         (0) root         (0)     9998 2023-07-03 12:04:22.000000 vdk-ipython-0.1.919227134/tests/test_plugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-07-28 09:42:19.000000 vdk-ipython-0.1.948436673/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1035 2023-07-28 09:42:29.000000 vdk-ipython-0.1.948436673/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2298 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 09:42:42.000000 vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 09:42:42.594514 vdk-ipython-0.1.948436673/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     9998 2023-07-28 09:42:19.000000 vdk-ipython-0.1.948436673/tests/test_plugin.py
```

### Comparing `vdk-ipython-0.1.919227134/PKG-INFO` & `vdk-ipython-0.1.948436673/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-ipython
-Version: 0.1.919227134
+Version: 0.1.948436673
 Summary: Ipython extension for VDK
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-ipython-0.1.919227134/README.md` & `vdk-ipython-0.1.948436673/README.md`

 * *Files identical despite different names*

### Comparing `vdk-ipython-0.1.919227134/setup.py` & `vdk-ipython-0.1.948436673/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright 2021-2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 import pathlib
 
 import setuptools
 
 
-__version__ = "0.1.919227134"
+__version__ = "0.1.948436673"
 
 setuptools.setup(
     name="vdk-ipython",
     version=__version__,
     url="https://github.com/vmware/versatile-data-kit",
     description="Ipython extension for VDK",
     long_description=pathlib.Path("README.md").read_text(),
```

### Comparing `vdk-ipython-0.1.919227134/src/vdk_ipython.egg-info/PKG-INFO` & `vdk-ipython-0.1.948436673/src/vdk_ipython.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-ipython
-Version: 0.1.919227134
+Version: 0.1.948436673
 Summary: Ipython extension for VDK
 Home-page: https://github.com/vmware/versatile-data-kit
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `vdk-ipython-0.1.919227134/tests/test_plugin.py` & `vdk-ipython-0.1.948436673/tests/test_plugin.py`

 * *Files identical despite different names*

