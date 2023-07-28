# Comparing `tmp/ign-gpao-utils-0.0.6.tar.gz` & `tmp/ign-gpao-utils-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ign-gpao-utils-0.0.6.tar", last modified: Tue Jul 25 09:09:48 2023, max compression
+gzip compressed data, was "ign-gpao-utils-0.1.0.tar", last modified: Fri Jul 28 17:29:24 2023, max compression
```

## Comparing `ign-gpao-utils-0.0.6.tar` & `ign-gpao-utils-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:48.144046 ign-gpao-utils-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 09:09:48.144046 ign-gpao-utils-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:48.140046 ign-gpao-utils-0.0.6/gpao_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/gpao_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/gpao_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/gpao_utils/interface_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/gpao_utils/utils_store.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:48.140046 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 09:09:48.000000 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 09:09:48.000000 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:09:48.000000 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 09:09:48.000000 ign-gpao-utils-0.0.6/ign_gpao_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:09:48.144046 ign-gpao-utils-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:09:48.140046 ign-gpao-utils-0.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-25 09:09:42.000000 ign-gpao-utils-0.0.6/test/test_utils_store.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:29:24.328661 ign-gpao-utils-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-28 17:29:24.328661 ign-gpao-utils-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-28 17:29:20.000000 ign-gpao-utils-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:29:24.328661 ign-gpao-utils-0.1.0/gpao_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 17:29:20.000000 ign-gpao-utils-0.1.0/gpao_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-28 17:29:20.000000 ign-gpao-utils-0.1.0/gpao_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-28 17:29:20.000000 ign-gpao-utils-0.1.0/gpao_utils/interface_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-28 17:29:20.000000 ign-gpao-utils-0.1.0/gpao_utils/utils_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-07-28 17:29:20.000000 ign-gpao-utils-0.1.0/gpao_utils/utils_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:29:24.328661 ign-gpao-utils-0.1.0/ign_gpao_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-28 17:29:24.000000 ign-gpao-utils-0.1.0/ign_gpao_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-28 17:29:24.000000 ign-gpao-utils-0.1.0/ign_gpao_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:29:24.000000 ign-gpao-utils-0.1.0/ign_gpao_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 17:29:24.000000 ign-gpao-utils-0.1.0/ign_gpao_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:29:24.328661 ign-gpao-utils-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-28 17:29:20.000000 ign-gpao-utils-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:29:24.328661 ign-gpao-utils-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-28 17:29:20.000000 ign-gpao-utils-0.1.0/test/test_utils_store.py
```

### Comparing `ign-gpao-utils-0.0.6/gpao_utils/utils_store.py` & `ign-gpao-utils-0.1.0/gpao_utils/utils_store.py`

 * *Files identical despite different names*

### Comparing `ign-gpao-utils-0.0.6/setup.py` & `ign-gpao-utils-0.1.0/setup.py`

 * *Files identical despite different names*

