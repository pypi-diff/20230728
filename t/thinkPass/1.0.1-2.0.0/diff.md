# Comparing `tmp/thinkPass-1.0.1.tar.gz` & `tmp/thinkPass-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thinkPass-1.0.1.tar", last modified: Fri Jul 28 10:16:25 2023, max compression
+gzip compressed data, was "thinkPass-2.0.0.tar", last modified: Fri Jul 28 10:22:30 2023, max compression
```

## Comparing `thinkPass-1.0.1.tar` & `thinkPass-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 10:16:25.026912 thinkPass-1.0.1/
--rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-07-14 09:35:04.000000 thinkPass-1.0.1/LICENSE.txt
--rw-rw-r--   0 user      (1000) user      (1000)      385 2023-07-28 10:16:25.022912 thinkPass-1.0.1/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 10:16:25.026912 thinkPass-1.0.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      709 2023-07-28 10:16:14.000000 thinkPass-1.0.1/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 10:16:25.022912 thinkPass-1.0.1/thinkPass/
--rw-rw-r--   0 user      (1000) user      (1000)       30 2023-07-24 09:48:27.000000 thinkPass-1.0.1/thinkPass/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 10:16:25.022912 thinkPass-1.0.1/thinkPass/data/
--rw-rw-r--   0 user      (1000) user      (1000)       24 2023-07-18 11:04:17.000000 thinkPass-1.0.1/thinkPass/data/names.csv
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-18 11:05:29.000000 thinkPass-1.0.1/thinkPass/data/places.csv
--rw-rw-r--   0 user      (1000) user      (1000)     3167 2023-07-24 17:18:33.000000 thinkPass-1.0.1/thinkPass/passwd.py
--rw-rw-r--   0 user      (1000) user      (1000)     1896 2023-07-20 18:57:51.000000 thinkPass-1.0.1/thinkPass/testing.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 10:16:25.022912 thinkPass-1.0.1/thinkPass.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      385 2023-07-28 10:16:24.000000 thinkPass-1.0.1/thinkPass.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-28 10:16:24.000000 thinkPass-1.0.1/thinkPass.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 10:16:24.000000 thinkPass-1.0.1/thinkPass.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 10:16:24.000000 thinkPass-1.0.1/thinkPass.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 10:22:30.394643 thinkPass-2.0.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1068 2023-07-14 09:35:04.000000 thinkPass-2.0.0/LICENSE.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      385 2023-07-28 10:22:30.394643 thinkPass-2.0.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-28 10:22:30.394643 thinkPass-2.0.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      709 2023-07-28 10:22:20.000000 thinkPass-2.0.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 10:22:30.390643 thinkPass-2.0.0/thinkPass/
+-rw-rw-r--   0 user      (1000) user      (1000)       30 2023-07-24 09:48:27.000000 thinkPass-2.0.0/thinkPass/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 10:22:30.394643 thinkPass-2.0.0/thinkPass/data/
+-rw-rw-r--   0 user      (1000) user      (1000)       24 2023-07-18 11:04:17.000000 thinkPass-2.0.0/thinkPass/data/names.csv
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-18 11:05:29.000000 thinkPass-2.0.0/thinkPass/data/places.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     3167 2023-07-24 17:18:33.000000 thinkPass-2.0.0/thinkPass/passwd.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1896 2023-07-20 18:57:51.000000 thinkPass-2.0.0/thinkPass/testing.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-28 10:22:30.394643 thinkPass-2.0.0/thinkPass.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      385 2023-07-28 10:22:30.000000 thinkPass-2.0.0/thinkPass.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      266 2023-07-28 10:22:30.000000 thinkPass-2.0.0/thinkPass.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-28 10:22:30.000000 thinkPass-2.0.0/thinkPass.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-07-28 10:22:30.000000 thinkPass-2.0.0/thinkPass.egg-info/top_level.txt
```

### Comparing `thinkPass-1.0.1/LICENSE.txt` & `thinkPass-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thinkPass-1.0.1/thinkPass/passwd.py` & `thinkPass-2.0.0/thinkPass/passwd.py`

 * *Files identical despite different names*

### Comparing `thinkPass-1.0.1/thinkPass/testing.py` & `thinkPass-2.0.0/thinkPass/testing.py`

 * *Files identical despite different names*

