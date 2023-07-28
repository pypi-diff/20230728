# Comparing `tmp/awyes-10.0.6.tar.gz` & `tmp/awyes-10.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awyes-10.0.6.tar", last modified: Mon Jul 24 05:09:36 2023, max compression
+gzip compressed data, was "awyes-10.0.7.tar", last modified: Fri Jul 28 05:49:22 2023, max compression
```

## Comparing `awyes-10.0.6.tar` & `awyes-10.0.7.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:09:36.034027 awyes-10.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 05:09:36.034027 awyes-10.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-24 05:09:15.000000 awyes-10.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-24 05:09:34.000000 awyes-10.0.6/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 05:09:36.034027 awyes-10.0.6/awyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-24 05:09:35.000000 awyes-10.0.6/awyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-24 05:09:36.000000 awyes-10.0.6/awyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:09:35.000000 awyes-10.0.6/awyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 05:09:35.000000 awyes-10.0.6/awyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-24 05:09:35.000000 awyes-10.0.6/awyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 05:09:35.000000 awyes-10.0.6/awyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-24 05:09:36.034027 awyes-10.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-24 05:09:15.000000 awyes-10.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:22.898237 awyes-10.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 05:49:22.898237 awyes-10.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-28 05:49:02.000000 awyes-10.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-28 05:49:21.000000 awyes-10.0.7/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:22.898237 awyes-10.0.7/awyes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:02.000000 awyes-10.0.7/awyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-07-28 05:49:02.000000 awyes-10.0.7/awyes/awyes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-28 05:49:02.000000 awyes-10.0.7/awyes/awyes_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-28 05:49:02.000000 awyes-10.0.7/awyes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:49:22.898237 awyes-10.0.7/awyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 05:49:22.000000 awyes-10.0.7/awyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-28 05:49:22.000000 awyes-10.0.7/awyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:49:22.000000 awyes-10.0.7/awyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 05:49:22.000000 awyes-10.0.7/awyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 05:49:22.000000 awyes-10.0.7/awyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 05:49:22.000000 awyes-10.0.7/awyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 05:49:22.898237 awyes-10.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-28 05:49:02.000000 awyes-10.0.7/setup.py
```

### Comparing `awyes-10.0.6/PKG-INFO` & `awyes-10.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.0.6
+Version: 10.0.7
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.0.6/awyes.egg-info/PKG-INFO` & `awyes-10.0.7/awyes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awyes
-Version: 10.0.6
+Version: 10.0.7
 Summary: A package for easy setup and management of resources on AWS
 Home-page: https://github.com/bb-labs/awyes
 Author: Truman Purnell
 Author-email: truman.purnell@gmail.com
 Keywords: aws resources manager setup management
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `awyes-10.0.6/setup.py` & `awyes-10.0.7/setup.py`

 * *Files identical despite different names*

