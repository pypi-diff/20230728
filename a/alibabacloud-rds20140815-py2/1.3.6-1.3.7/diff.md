# Comparing `tmp/alibabacloud_rds20140815_py2-1.3.6.tar.gz` & `tmp/alibabacloud_rds20140815_py2-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.3.6.tar", last modified: Thu Jul 27 15:10:23 2023, max compression
+gzip compressed data, was "dist/alibabacloud_rds20140815_py2-1.3.7.tar", last modified: Fri Jul 28 15:10:29 2023, max compression
```

## Comparing `alibabacloud_rds20140815_py2-1.3.6.tar` & `alibabacloud_rds20140815_py2-1.3.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/
--rw-r--r--   0 root         (0) root         (0)     2691 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815/__init__.py
--rw-r--r--   0 root         (0) root         (0)   779383 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815/client.py
--rw-r--r--   0 root         (0) root         (0)  2654015 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2472 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      440 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-27 15:10:23.000000 alibabacloud_rds20140815_py2-1.3.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2903 2023-07-27 15:10:22.000000 alibabacloud_rds20140815_py2-1.3.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   779383 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815/client.py
+-rw-r--r--   0 root         (0) root         (0)  2654015 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2472 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      440 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2903 2023-07-28 15:10:29.000000 alibabacloud_rds20140815_py2-1.3.7/setup.py
```

### Comparing `alibabacloud_rds20140815_py2-1.3.6/ChangeLog.md` & `alibabacloud_rds20140815_py2-1.3.7/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2023-07-27 Version: 1.3.6
+- Fix bug ram.
+- Add minor version error.
+- Support to select the minor version of the kernel when the modify instance error reports that the kernel version does not support it.
+
 2023-07-25 Version: 1.3.5
 - Add error code.
 - Support System param.
 
 2023-07-24 Version: 1.3.4
 - Add error code.
 - Add error code for CreateDBNodes.
```

### Comparing `alibabacloud_rds20140815_py2-1.3.6/LICENSE` & `alibabacloud_rds20140815_py2-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.3.6/PKG-INFO` & `alibabacloud_rds20140815_py2-1.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_rds20140815_py2
-Version: 1.3.6
+Version: 1.3.7
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.3.6/README-CN.md` & `alibabacloud_rds20140815_py2-1.3.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.3.6/README.md` & `alibabacloud_rds20140815_py2-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815/client.py` & `alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815/models.py` & `alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_rds20140815_py2-1.3.6/alibabacloud_rds20140815_py2.egg-info/PKG-INFO` & `alibabacloud_rds20140815_py2-1.3.7/alibabacloud_rds20140815_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-rds20140815-py2
-Version: 1.3.6
+Version: 1.3.7
 Summary: Alibaba Cloud rds (20140815) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_rds20140815_py2-1.3.6/setup.py` & `alibabacloud_rds20140815_py2-1.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_rds20140815_py2.
 
-Created on 27/07/2023
+Created on 28/07/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_rds20140815"
 NAME = "alibabacloud_rds20140815_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud rds (20140815) SDK Library for Python2"
```

