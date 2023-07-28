# Comparing `tmp/emzed_remote_client-0.0.1.tar.gz` & `tmp/emzed_remote_client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emzed_remote_client-0.0.1.tar", last modified: Fri Jul 28 06:27:40 2023, max compression
+gzip compressed data, was "emzed_remote_client-0.0.2.tar", last modified: Fri Jul 28 16:34:52 2023, max compression
```

## Comparing `emzed_remote_client-0.0.1.tar` & `emzed_remote_client-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-07-28 06:27:40.341631 emzed_remote_client-0.0.1/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      252 2023-07-28 06:27:40.341426 emzed_remote_client-0.0.1/PKG-INFO
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-07-28 06:27:40.341169 emzed_remote_client-0.0.1/emzed_remote_client.egg-info/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      252 2023-07-28 06:27:40.000000 emzed_remote_client-0.0.1/emzed_remote_client.egg-info/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2023-07-28 06:27:40.000000 emzed_remote_client-0.0.1/emzed_remote_client.egg-info/SOURCES.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-07-28 06:27:40.000000 emzed_remote_client-0.0.1/emzed_remote_client.egg-info/dependency_links.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        6 2023-07-28 06:27:40.000000 emzed_remote_client-0.0.1/emzed_remote_client.egg-info/requires.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)       20 2023-07-28 06:27:40.000000 emzed_remote_client-0.0.1/emzed_remote_client.egg-info/top_level.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)     5383 2023-07-27 17:33:59.000000 emzed_remote_client-0.0.1/emzed_remote_client.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-07-28 06:27:40.341688 emzed_remote_client-0.0.1/setup.cfg
--rw-r--r--   0 uweschmitt   (501) staff       (20)      860 2023-07-28 06:26:38.000000 emzed_remote_client-0.0.1/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-07-28 16:34:52.205941 emzed_remote_client-0.0.2/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      252 2023-07-28 16:34:52.205741 emzed_remote_client-0.0.2/PKG-INFO
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-07-28 16:34:52.205535 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      252 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/SOURCES.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/dependency_links.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        6 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/requires.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       20 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/top_level.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6891 2023-07-28 16:32:27.000000 emzed_remote_client-0.0.2/emzed_remote_client.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-07-28 16:34:52.205992 emzed_remote_client-0.0.2/setup.cfg
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      860 2023-07-28 16:34:36.000000 emzed_remote_client-0.0.2/setup.py
```

### Comparing `emzed_remote_client-0.0.1/setup.py` & `emzed_remote_client-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import print_function
 
 import os
 import sys
 
 from setuptools import setup
 
-VERSION = (0, 0, 1)  # no need to adapt version in other locations
+VERSION = (0, 0, 2)  # no need to adapt version in other locations
 
 AUTHOR = "Uwe Schmitt"
 AUTHOR_EMAIL = "uwe.schmitt@id.ethz.ch"
 
 DESCRIPTION = "client side of emzed remote execution"
 
 LICENSE = "https://opensource.org/licenses/MIT"
```

