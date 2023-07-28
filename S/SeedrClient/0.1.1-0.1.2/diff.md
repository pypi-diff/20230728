# Comparing `tmp/SeedrClient-0.1.1.tar.gz` & `tmp/SeedrClient-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeedrClient-0.1.1.tar", last modified: Fri Jul 28 10:38:13 2023, max compression
+gzip compressed data, was "SeedrClient-0.1.2.tar", last modified: Fri Jul 28 10:54:01 2023, max compression
```

## Comparing `SeedrClient-0.1.1.tar` & `SeedrClient-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:38:13.318719 SeedrClient-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 10:38:13.318719 SeedrClient-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 10:37:58.000000 SeedrClient-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 10:38:13.322719 SeedrClient-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-28 10:37:58.000000 SeedrClient-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:38:13.314719 SeedrClient-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:38:13.318719 SeedrClient-0.1.1/src/SeedrClient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 10:38:13.000000 SeedrClient-0.1.1/src/SeedrClient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 10:38:13.000000 SeedrClient-0.1.1/src/SeedrClient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:38:13.000000 SeedrClient-0.1.1/src/SeedrClient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 10:38:13.000000 SeedrClient-0.1.1/src/SeedrClient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 10:38:13.000000 SeedrClient-0.1.1/src/SeedrClient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:38:13.318719 SeedrClient-0.1.1/src/seedr_client/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 10:37:58.000000 SeedrClient-0.1.1/src/seedr_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 10:37:58.000000 SeedrClient-0.1.1/src/seedr_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    20325 2023-07-28 10:37:58.000000 SeedrClient-0.1.1/src/seedr_client/seedr_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/src/SeedrClient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-28 10:54:01.000000 SeedrClient-0.1.2/src/SeedrClient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 10:54:01.443942 SeedrClient-0.1.2/src/seedr_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/src/seedr_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/src/seedr_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20325 2023-07-28 10:53:44.000000 SeedrClient-0.1.2/src/seedr_client/seedr_handler.py
```

### Comparing `SeedrClient-0.1.1/PKG-INFO` & `SeedrClient-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeedrClient
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python library to interface with Seedr
 Home-page: https://github.com/Mr-Developer-X/seedr-client
 Author: Mr Developer X
 Author-email: 139059229+Mr-Developer-X@users.noreply.github.com
 Keywords: seedr,bittorrent,torrent,magnet,seedr api,seedbox
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `SeedrClient-0.1.1/setup.py` & `SeedrClient-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `SeedrClient-0.1.1/src/SeedrClient.egg-info/PKG-INFO` & `SeedrClient-0.1.2/src/SeedrClient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SeedrClient
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python library to interface with Seedr
 Home-page: https://github.com/Mr-Developer-X/seedr-client
 Author: Mr Developer X
 Author-email: 139059229+Mr-Developer-X@users.noreply.github.com
 Keywords: seedr,bittorrent,torrent,magnet,seedr api,seedbox
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `SeedrClient-0.1.1/src/seedr_client/seedr_handler.py` & `SeedrClient-0.1.2/src/seedr_client/seedr_handler.py`

 * *Files identical despite different names*

