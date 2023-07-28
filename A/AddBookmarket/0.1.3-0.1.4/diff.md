# Comparing `tmp/AddBookmarket-0.1.3.tar.gz` & `tmp/AddBookmarket-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AddBookmarket-0.1.3.tar", last modified: Fri Jul 14 08:16:09 2023, max compression
+gzip compressed data, was "AddBookmarket-0.1.4.tar", last modified: Fri Jul 28 09:50:43 2023, max compression
```

## Comparing `AddBookmarket-0.1.3.tar` & `AddBookmarket-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 08:16:09.596595 AddBookmarket-0.1.3/
-drwxrwxrwx   0        0        0        0 2023-07-14 08:16:09.573531 AddBookmarket-0.1.3/AddBookmarket/
--rw-rw-rw-   0        0        0   108032 2023-07-14 08:10:19.000000 AddBookmarket-0.1.3/AddBookmarket/AddBookmarket.pyd
--rw-rw-rw-   0        0        0        0 2023-07-13 02:45:04.000000 AddBookmarket-0.1.3/AddBookmarket/__init__.py
--rw-rw-rw-   0        0        0    71168 2023-07-14 08:10:28.000000 AddBookmarket-0.1.3/AddBookmarket/bookmarket_input.pyd
--rw-rw-rw-   0        0        0    70656 2023-07-14 08:10:37.000000 AddBookmarket-0.1.3/AddBookmarket/optimize_import.pyd
-drwxrwxrwx   0        0        0        0 2023-07-14 08:16:09.592546 AddBookmarket-0.1.3/AddBookmarket.egg-info/
--rw-rw-rw-   0        0        0      408 2023-07-14 08:16:09.000000 AddBookmarket-0.1.3/AddBookmarket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-07-14 08:16:09.000000 AddBookmarket-0.1.3/AddBookmarket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 08:16:09.000000 AddBookmarket-0.1.3/AddBookmarket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-14 08:16:09.000000 AddBookmarket-0.1.3/AddBookmarket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 AddBookmarket-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AddBookmarket-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      408 2023-07-14 08:16:09.596595 AddBookmarket-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-07-14 06:48:33.000000 AddBookmarket-0.1.3/README.md
--rw-rw-rw-   0        0        0      136 2023-07-14 08:16:09.599540 AddBookmarket-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-07-14 08:15:39.000000 AddBookmarket-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-28 09:50:43.595930 AddBookmarket-0.1.4/
+drwxrwxrwx   0        0        0        0 2023-07-28 09:50:43.583930 AddBookmarket-0.1.4/AddBookmarket/
+-rw-rw-rw-   0        0        0   108032 2023-07-28 08:37:07.000000 AddBookmarket-0.1.4/AddBookmarket/AddBookmarket.pyd
+-rw-rw-rw-   0        0        0        0 2023-07-13 02:45:04.000000 AddBookmarket-0.1.4/AddBookmarket/__init__.py
+-rw-rw-rw-   0        0        0    71168 2023-07-28 08:37:12.000000 AddBookmarket-0.1.4/AddBookmarket/bookmarket_input.pyd
+-rw-rw-rw-   0        0        0    70144 2023-07-28 08:37:23.000000 AddBookmarket-0.1.4/AddBookmarket/optimize_import.pyd
+drwxrwxrwx   0        0        0        0 2023-07-28 09:50:43.593967 AddBookmarket-0.1.4/AddBookmarket.egg-info/
+-rw-rw-rw-   0        0        0      408 2023-07-28 09:50:43.000000 AddBookmarket-0.1.4/AddBookmarket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-28 09:50:43.000000 AddBookmarket-0.1.4/AddBookmarket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-28 09:50:43.000000 AddBookmarket-0.1.4/AddBookmarket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-28 09:50:43.000000 AddBookmarket-0.1.4/AddBookmarket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       19 2023-07-05 02:27:45.000000 AddBookmarket-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 AddBookmarket-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      408 2023-07-28 09:50:43.595930 AddBookmarket-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-07-14 06:48:33.000000 AddBookmarket-0.1.4/README.md
+-rw-rw-rw-   0        0        0      136 2023-07-28 09:50:43.597935 AddBookmarket-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-07-28 08:40:29.000000 AddBookmarket-0.1.4/setup.py
```

### Comparing `AddBookmarket-0.1.3/setup.py` & `AddBookmarket-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 1
-PATCH = 3
+PATCH = 4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "AddBookmarket",
```

