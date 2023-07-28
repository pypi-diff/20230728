# Comparing `tmp/RdQxbAPI-0.1.2.tar.gz` & `tmp/RdQxbAPI-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RdQxbAPI-0.1.2.tar", last modified: Mon Jul 17 05:50:09 2023, max compression
+gzip compressed data, was "RdQxbAPI-0.1.3.tar", last modified: Fri Jul 28 06:48:12 2023, max compression
```

## Comparing `RdQxbAPI-0.1.2.tar` & `RdQxbAPI-0.1.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.381457 RdQxbAPI-0.1.2/
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 RdQxbAPI-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 RdQxbAPI-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      374 2023-07-17 05:50:09.381457 RdQxbAPI-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0       17 2023-07-05 02:28:57.000000 RdQxbAPI-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.332258 RdQxbAPI-0.1.2/RdQxbAPI/
-drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.372005 RdQxbAPI-0.1.2/RdQxbAPI/Function/
--rw-rw-rw-   0        0        0    83456 2023-07-05 02:09:39.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIgsgd.pyd
--rw-rw-rw-   0        0        0   113152 2023-07-05 02:09:45.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIphone.pyd
--rw-rw-rw-   0        0        0   177152 2023-07-05 02:09:53.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIqylt.pyd
--rw-rw-rw-   0        0        0   115200 2023-07-05 02:09:59.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIysglf.pyd
--rw-rw-rw-   0        0        0   139264 2023-07-05 02:10:06.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/QxbAPIzyrytz.pyd
--rw-rw-rw-   0        0        0        0 2023-06-25 08:05:06.000000 RdQxbAPI-0.1.2/RdQxbAPI/Function/__init__.py
--rw-rw-rw-   0        0        0   155136 2023-07-17 05:46:51.000000 RdQxbAPI-0.1.2/RdQxbAPI/RdqxbAPI.pyd
-drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.377005 RdQxbAPI-0.1.2/RdQxbAPI/UI/
--rw-rw-rw-   0        0        0        0 2023-06-25 08:04:41.000000 RdQxbAPI-0.1.2/RdQxbAPI/UI/__init__.py
--rw-rw-rw-   0        0        0    80384 2023-07-05 02:10:12.000000 RdQxbAPI-0.1.2/RdQxbAPI/UI/qxbUI.pyd
--rw-rw-rw-   0        0        0        0 2023-06-25 09:28:39.000000 RdQxbAPI-0.1.2/RdQxbAPI/__init__.py
--rw-rw-rw-   0        0        0    69632 2023-07-05 02:09:33.000000 RdQxbAPI-0.1.2/RdQxbAPI/optionDb.pyd
-drwxrwxrwx   0        0        0        0 2023-07-17 05:50:09.346004 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/
--rw-rw-rw-   0        0        0      374 2023-07-17 05:50:09.000000 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      490 2023-07-17 05:50:09.000000 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 05:50:09.000000 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 05:50:09.000000 RdQxbAPI-0.1.2/RdQxbAPI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-07-17 05:50:09.383453 RdQxbAPI-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1005 2023-07-17 05:50:03.000000 RdQxbAPI-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 06:48:12.340318 RdQxbAPI-0.1.3/
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 RdQxbAPI-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 RdQxbAPI-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      374 2023-07-28 06:48:12.341319 RdQxbAPI-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0       17 2023-07-05 02:28:57.000000 RdQxbAPI-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-07-28 06:48:12.291317 RdQxbAPI-0.1.3/RdQxbAPI/
+drwxrwxrwx   0        0        0        0 2023-07-28 06:48:12.330316 RdQxbAPI-0.1.3/RdQxbAPI/Function/
+-rw-rw-rw-   0        0        0    83456 2023-07-05 02:09:39.000000 RdQxbAPI-0.1.3/RdQxbAPI/Function/QxbAPIgsgd.pyd
+-rw-rw-rw-   0        0        0   113152 2023-07-05 02:09:45.000000 RdQxbAPI-0.1.3/RdQxbAPI/Function/QxbAPIphone.pyd
+-rw-rw-rw-   0        0        0   177152 2023-07-05 02:09:53.000000 RdQxbAPI-0.1.3/RdQxbAPI/Function/QxbAPIqylt.pyd
+-rw-rw-rw-   0        0        0   115200 2023-07-05 02:09:59.000000 RdQxbAPI-0.1.3/RdQxbAPI/Function/QxbAPIysglf.pyd
+-rw-rw-rw-   0        0        0   139264 2023-07-05 02:10:06.000000 RdQxbAPI-0.1.3/RdQxbAPI/Function/QxbAPIzyrytz.pyd
+-rw-rw-rw-   0        0        0        0 2023-06-25 08:05:06.000000 RdQxbAPI-0.1.3/RdQxbAPI/Function/__init__.py
+-rw-rw-rw-   0        0        0   157184 2023-07-28 06:42:34.000000 RdQxbAPI-0.1.3/RdQxbAPI/RdQxbAPI.pyd
+drwxrwxrwx   0        0        0        0 2023-07-28 06:48:12.335320 RdQxbAPI-0.1.3/RdQxbAPI/UI/
+-rw-rw-rw-   0        0        0        0 2023-06-25 08:04:41.000000 RdQxbAPI-0.1.3/RdQxbAPI/UI/__init__.py
+-rw-rw-rw-   0        0        0    80384 2023-07-05 02:10:12.000000 RdQxbAPI-0.1.3/RdQxbAPI/UI/qxbUI.pyd
+-rw-rw-rw-   0        0        0        0 2023-06-25 09:28:39.000000 RdQxbAPI-0.1.3/RdQxbAPI/__init__.py
+-rw-rw-rw-   0        0        0    69632 2023-07-05 02:09:33.000000 RdQxbAPI-0.1.3/RdQxbAPI/optionDb.pyd
+drwxrwxrwx   0        0        0        0 2023-07-28 06:48:12.304322 RdQxbAPI-0.1.3/RdQxbAPI.egg-info/
+-rw-rw-rw-   0        0        0      374 2023-07-28 06:48:12.000000 RdQxbAPI-0.1.3/RdQxbAPI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      490 2023-07-28 06:48:12.000000 RdQxbAPI-0.1.3/RdQxbAPI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 06:48:12.000000 RdQxbAPI-0.1.3/RdQxbAPI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-28 06:48:12.000000 RdQxbAPI-0.1.3/RdQxbAPI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-07-28 06:48:12.342317 RdQxbAPI-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1005 2023-07-28 06:44:57.000000 RdQxbAPI-0.1.3/setup.py
```

### Comparing `RdQxbAPI-0.1.2/setup.py` & `RdQxbAPI-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 2
+PATCH = 3
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "RdQxbAPI",
```

