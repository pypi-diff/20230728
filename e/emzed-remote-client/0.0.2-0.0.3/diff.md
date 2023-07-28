# Comparing `tmp/emzed_remote_client-0.0.2.tar.gz` & `tmp/emzed_remote_client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emzed_remote_client-0.0.2.tar", last modified: Fri Jul 28 16:34:52 2023, max compression
+gzip compressed data, was "emzed_remote_client-0.0.3.tar", last modified: Fri Jul 28 18:31:19 2023, max compression
```

## Comparing `emzed_remote_client-0.0.2.tar` & `emzed_remote_client-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-07-28 16:34:52.205941 emzed_remote_client-0.0.2/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      252 2023-07-28 16:34:52.205741 emzed_remote_client-0.0.2/PKG-INFO
-drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-07-28 16:34:52.205535 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/
--rw-r--r--   0 uweschmitt   (501) staff       (20)      252 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/PKG-INFO
--rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/SOURCES.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/dependency_links.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)        6 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/requires.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)       20 2023-07-28 16:34:52.000000 emzed_remote_client-0.0.2/emzed_remote_client.egg-info/top_level.txt
--rw-r--r--   0 uweschmitt   (501) staff       (20)     6891 2023-07-28 16:32:27.000000 emzed_remote_client-0.0.2/emzed_remote_client.py
--rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-07-28 16:34:52.205992 emzed_remote_client-0.0.2/setup.cfg
--rw-r--r--   0 uweschmitt   (501) staff       (20)      860 2023-07-28 16:34:36.000000 emzed_remote_client-0.0.2/setup.py
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-07-28 18:31:19.711144 emzed_remote_client-0.0.3/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      252 2023-07-28 18:31:19.710991 emzed_remote_client-0.0.3/PKG-INFO
+drwxr-xr-x   0 uweschmitt   (501) staff       (20)        0 2023-07-28 18:31:19.710796 emzed_remote_client-0.0.3/emzed_remote_client.egg-info/
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      252 2023-07-28 18:31:19.000000 emzed_remote_client-0.0.3/emzed_remote_client.egg-info/PKG-INFO
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      245 2023-07-28 18:31:19.000000 emzed_remote_client-0.0.3/emzed_remote_client.egg-info/SOURCES.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        1 2023-07-28 18:31:19.000000 emzed_remote_client-0.0.3/emzed_remote_client.egg-info/dependency_links.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)        6 2023-07-28 18:31:19.000000 emzed_remote_client-0.0.3/emzed_remote_client.egg-info/requires.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       20 2023-07-28 18:31:19.000000 emzed_remote_client-0.0.3/emzed_remote_client.egg-info/top_level.txt
+-rw-r--r--   0 uweschmitt   (501) staff       (20)     6888 2023-07-28 17:20:51.000000 emzed_remote_client-0.0.3/emzed_remote_client.py
+-rw-r--r--   0 uweschmitt   (501) staff       (20)       38 2023-07-28 18:31:19.711184 emzed_remote_client-0.0.3/setup.cfg
+-rw-r--r--   0 uweschmitt   (501) staff       (20)      860 2023-07-28 18:31:07.000000 emzed_remote_client-0.0.3/setup.py
```

### Comparing `emzed_remote_client-0.0.2/emzed_remote_client.py` & `emzed_remote_client-0.0.3/emzed_remote_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from functools import partial
 from multiprocessing.connection import Listener
 from multiprocessing import current_process
 from pprint import pprint
 
 import numpy as np
 
+current_process()._inheriting = False
+
 BASIC_TYPES = (int, float, str, bool, bytes, type(None))
 
 REMOTE_OBJECT_PROXY = 1
 ND_ARRAY = 2
 LOCAL_OBJECT_PROXY = 3
 PICKLE = 4
 
@@ -138,15 +140,14 @@
 
 
 optimizations = {}
 
 
 def main(pipe, pipe_2):
 
-    current_process()._inheriting = False
     current_process()._identity = ()
 
     signal.signal(signal.SIGINT, signal.SIG_IGN)
 
     mapper = ClientObjectMapper(pipe_2)
 
     commands = {
```

### Comparing `emzed_remote_client-0.0.2/setup.py` & `emzed_remote_client-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import print_function
 
 import os
 import sys
 
 from setuptools import setup
 
-VERSION = (0, 0, 2)  # no need to adapt version in other locations
+VERSION = (0, 0, 3)  # no need to adapt version in other locations
 
 AUTHOR = "Uwe Schmitt"
 AUTHOR_EMAIL = "uwe.schmitt@id.ethz.ch"
 
 DESCRIPTION = "client side of emzed remote execution"
 
 LICENSE = "https://opensource.org/licenses/MIT"
```

