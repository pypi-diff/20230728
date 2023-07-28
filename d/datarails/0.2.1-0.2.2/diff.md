# Comparing `tmp/datarails-0.2.1.tar.gz` & `tmp/datarails-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datarails-0.2.1.tar", last modified: Fri Jul 28 13:39:38 2023, max compression
+gzip compressed data, was "datarails-0.2.2.tar", last modified: Fri Jul 28 13:50:03 2023, max compression
```

## Comparing `datarails-0.2.1.tar` & `datarails-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:39:38.016716 datarails-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:39:38.016716 datarails-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:39:18.000000 datarails-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:39:38.016716 datarails-0.2.1/datarails/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 13:39:18.000000 datarails-0.2.1/datarails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-28 13:39:18.000000 datarails-0.2.1/datarails/databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 13:39:18.000000 datarails-0.2.1/datarails/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-28 13:39:18.000000 datarails-0.2.1/datarails/step.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 13:39:18.000000 datarails-0.2.1/datarails/type_vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:39:38.016716 datarails-0.2.1/datarails.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:39:38.000000 datarails-0.2.1/datarails.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-28 13:39:38.000000 datarails-0.2.1/datarails.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:39:38.000000 datarails-0.2.1/datarails.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 13:39:38.000000 datarails-0.2.1/datarails.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 13:39:38.000000 datarails-0.2.1/datarails.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 13:39:18.000000 datarails-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:39:38.016716 datarails-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 13:39:18.000000 datarails-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:39:38.016716 datarails-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-28 13:39:18.000000 datarails-0.2.1/tests/test_databox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-28 13:39:18.000000 datarails-0.2.1/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 13:39:18.000000 datarails-0.2.1/tests/test_step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:03.254701 datarails-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:50:03.254701 datarails-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 13:49:39.000000 datarails-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:03.254701 datarails-0.2.2/datarails/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 13:49:39.000000 datarails-0.2.2/datarails/type_vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:03.254701 datarails-0.2.2/datarails.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 13:50:03.000000 datarails-0.2.2/datarails.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-28 13:49:39.000000 datarails-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:50:03.254701 datarails-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 13:49:39.000000 datarails-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:50:03.254701 datarails-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-28 13:49:39.000000 datarails-0.2.2/tests/test_databox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-28 13:49:39.000000 datarails-0.2.2/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 13:49:39.000000 datarails-0.2.2/tests/test_step.py
```

### Comparing `datarails-0.2.1/datarails/databox.py` & `datarails-0.2.2/datarails/databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.1/datarails/runner.py` & `datarails-0.2.2/datarails/runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.1/datarails/step.py` & `datarails-0.2.2/datarails/step.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.1/pyproject.toml` & `datarails-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "datarails"
-version = "0.2.1"
+version = "0.2.2"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `datarails-0.2.1/tests/test_databox.py` & `datarails-0.2.2/tests/test_databox.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.1/tests/test_runner.py` & `datarails-0.2.2/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `datarails-0.2.1/tests/test_step.py` & `datarails-0.2.2/tests/test_step.py`

 * *Files identical despite different names*

