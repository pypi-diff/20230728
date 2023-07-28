# Comparing `tmp/general-superstaq-0.4.7.tar.gz` & `tmp/general-superstaq-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "general-superstaq-0.4.7.tar", last modified: Wed Jul 26 21:52:18 2023, max compression
+gzip compressed data, was "general-superstaq-0.4.8.tar", last modified: Fri Jul 28 17:44:10 2023, max compression
```

## Comparing `general-superstaq-0.4.7.tar` & `general-superstaq-0.4.8.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:18.479673 general-superstaq-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-26 21:52:18.479673 general-superstaq-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:18.479673 general-superstaq-0.4.7/general_superstaq/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/_init_vars.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/_version_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:18.479673 general-superstaq-0.4.7/general_superstaq/check/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/all_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/check_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/coverage_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/flake8_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/format_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/mypy_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/pylint_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/pytest_.py
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/check/requirements.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/qubo.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/qubo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/resource_estimate.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/resource_estimate_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/serialization_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20517 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/superstaq_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24366 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/superstaq_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/superstaq_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/superstaq_exceptions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/general_superstaq/validation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 21:52:18.479673 general-superstaq-0.4.7/general_superstaq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-26 21:52:18.000000 general-superstaq-0.4.7/general_superstaq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-26 21:52:18.000000 general-superstaq-0.4.7/general_superstaq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 21:52:18.000000 general-superstaq-0.4.7/general_superstaq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-26 21:52:18.000000 general-superstaq-0.4.7/general_superstaq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-26 21:52:18.000000 general-superstaq-0.4.7/general_superstaq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-26 21:51:58.000000 general-superstaq-0.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-26 21:52:18.479673 general-superstaq-0.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:10.084422 general-superstaq-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 17:44:10.084422 general-superstaq-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:10.080422 general-superstaq-0.4.8/general_superstaq/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/_init_vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/_version_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:10.084422 general-superstaq-0.4.8/general_superstaq/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/all_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/check_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/checks-pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/coverage_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/flake8_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/format_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/mypy_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/pylint_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/pytest_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/check/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/qubo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/qubo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/resource_estimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/resource_estimate_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/serialization_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23178 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/superstaq_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25714 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/superstaq_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/superstaq_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/superstaq_exceptions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/general_superstaq/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:44:10.080422 general-superstaq-0.4.8/general_superstaq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 17:44:10.000000 general-superstaq-0.4.8/general_superstaq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-28 17:43:49.000000 general-superstaq-0.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:44:10.084422 general-superstaq-0.4.8/setup.cfg
```

### Comparing `general-superstaq-0.4.7/PKG-INFO` & `general-superstaq-0.4.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-superstaq
-Version: 0.4.7
+Version: 0.4.8
 Summary: The general module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `general-superstaq-0.4.7/general_superstaq/__init__.py` & `general-superstaq-0.4.8/general_superstaq/__init__.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/all_.py` & `general-superstaq-0.4.8/general_superstaq/check/all_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/build_docs.py` & `general-superstaq-0.4.8/general_superstaq/check/build_docs.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/check_utils.py` & `general-superstaq-0.4.8/general_superstaq/check/check_utils.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/configs.py` & `general-superstaq-0.4.8/general_superstaq/check/configs.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/coverage_.py` & `general-superstaq-0.4.8/general_superstaq/check/coverage_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/flake8_.py` & `general-superstaq-0.4.8/general_superstaq/check/flake8_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/format_.py` & `general-superstaq-0.4.8/general_superstaq/check/format_.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,19 @@
 
     parsed_args, args_to_pass_isort = parser.parse_known_intermixed_args(args)
     files = check_utils.extract_files(parsed_args, include, exclude, silent)
     if not files:
         return 0
 
     diff_check_args = ["--diff", "--check"] if not parsed_args.apply else []
+
+    args_to_pass_black = ["--config", "pyproject.toml"]
     returncode_black = subprocess.call(
-        ["python", "-m", "black", *files, *diff_check_args], cwd=check_utils.root_dir
+        ["python", "-m", "black", *files, *diff_check_args, *args_to_pass_black],
+        cwd=check_utils.root_dir,
     )
 
     if returncode_black > 1:
         # this only occurs if black could not parse a file (for example due to a syntax error)
         return returncode_black
 
     args_to_pass_isort += ["--resolve-all-configs", f"--config-root={check_utils.root_dir}"]
```

### Comparing `general-superstaq-0.4.7/general_superstaq/check/mypy_.py` & `general-superstaq-0.4.8/general_superstaq/check/mypy_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/pylint_.py` & `general-superstaq-0.4.8/general_superstaq/check/pylint_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/pytest_.py` & `general-superstaq-0.4.8/general_superstaq/check/pytest_.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/check/requirements.py` & `general-superstaq-0.4.8/general_superstaq/check/requirements.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/qubo.py` & `general-superstaq-0.4.8/general_superstaq/qubo.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/qubo_test.py` & `general-superstaq-0.4.8/general_superstaq/qubo_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/resource_estimate.py` & `general-superstaq-0.4.8/general_superstaq/resource_estimate.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/serialization.py` & `general-superstaq-0.4.8/general_superstaq/serialization.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/service.py` & `general-superstaq-0.4.8/general_superstaq/service.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/service_test.py` & `general-superstaq-0.4.8/general_superstaq/service_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/superstaq_client.py` & `general-superstaq-0.4.8/general_superstaq/superstaq_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -380,14 +380,86 @@
             "files": files,
             "num_qubits": int(num_qubits),
             "depth": int(depth),
             "circuit_return_type": circuit_return_type,
         }
         return self.post_request("/supercheq", json_dict)
 
+    def submit_dfe(
+        self,
+        circuit_1: Dict[str, str],
+        target_1: str,
+        circuit_2: Dict[str, str],
+        target_2: str,
+        num_random_bases: int,
+        shots: int,
+        **kwargs: Any,
+    ) -> List[str]:
+        """Performs a POST request on the `/dfe_post` endpoint.
+
+        Args:
+            circuit_1: Serialized circuit that prepares the first state for the protocol.
+            target_1: Target to prepare the first state on.
+            circuit_2: Serialized circuit that prepares the second state for the protocol.
+            target_2: Target to prepare the second state on.
+            num_random_bases: Number of random bases to measure the states on.
+            shots: Number of shots per random basis.
+            kwargs: Other execution parameters.
+                - tag: Tag for all jobs submitted for this protocol.
+                - lifespan: How long to store the jobs submitted for in days (only works with right
+                permissions).
+                - method: Which type of method to execute the circuits with.
+
+        Returns:
+            A list of size two with the ids for the RMT jobs created; these ids should be passed to
+            `process_dfe` to get back the fidelity estimation.
+
+        Raises:
+            ValueError: If any of the targets passed are not valid.
+            SuperstaqServerException: if the request fails.
+        """
+        gss.validation.validate_target(target_1)
+        gss.validation.validate_target(target_2)
+
+        state_1 = {**circuit_1, "target": target_1}
+        state_2 = {**circuit_2, "target": target_2}
+
+        json_dict: Dict[str, Any] = {
+            "state_1": state_1,
+            "state_2": state_2,
+            "shots": int(shots),
+            "n_bases": int(num_random_bases),
+        }
+
+        if kwargs:
+            json_dict["options"] = json.dumps(kwargs)
+        return self.post_request("/dfe_post", json_dict)
+
+    def process_dfe(self, job_ids: List[str]) -> float:
+        """Performs a POST request on the `/dfe_fetch` endpoint.
+
+        Args:
+            job_ids: A list of job ids returned by a call to `submit_dfe`.
+
+        Returns:
+            The estimated fidelity between the two states as a float.
+
+        Raises:
+            ValueError: If `job_ids` is not of size two.
+            SuperstaqServerException: If the request fails.
+        """
+        if len(job_ids) != 2:
+            raise ValueError("`job_ids` must contain exactly two job ids.")
+
+        json_dict = {
+            "job_id_1": job_ids[0],
+            "job_id_2": job_ids[1],
+        }
+        return self.post_request("/dfe_fetch", json_dict)
+
     def target_info(self, target: str) -> Dict[str, Any]:
         """Makes a POST request to the /target_info endpoint.
 
         Uses the Superstaq API to request information about `target`.
 
         Args:
             target: A string representing the device to get information about.
```

### Comparing `general-superstaq-0.4.7/general_superstaq/superstaq_client_test.py` & `general-superstaq-0.4.8/general_superstaq/superstaq_client_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -604,14 +604,63 @@
         headers=EXPECTED_HEADERS,
         json=expected_json,
         verify=False,
     )
 
 
 @mock.patch("requests.post")
+def test_superstaq_client_dfe(mock_post: mock.MagicMock) -> None:
+    client = gss.superstaq_client._SuperstaqClient(
+        client_name="general-superstaq",
+        remote_host="http://example.com",
+        api_key="to_my_heart",
+    )
+    client.submit_dfe(
+        circuit_1={"Hello": "World"},
+        target_1="ss_example_qpu",
+        circuit_2={"Hello": "World"},
+        target_2="ss_example_qpu",
+        num_random_bases=5,
+        shots=100,
+        lifespan=10,
+    )
+
+    state = {
+        "Hello": "World",
+        "target": "ss_example_qpu",
+    }
+    expected_json = {
+        "state_1": state,
+        "state_2": state,
+        "shots": 100,
+        "n_bases": 5,
+        "options": json.dumps({"lifespan": 10}),
+    }
+
+    mock_post.assert_called_with(
+        f"http://example.com/{API_VERSION}/dfe_post",
+        headers=EXPECTED_HEADERS,
+        json=expected_json,
+        verify=False,
+    )
+
+    client.process_dfe(["id1", "id2"])
+    expected_json = {"job_id_1": "id1", "job_id_2": "id2"}
+    mock_post.assert_called_with(
+        f"http://example.com/{API_VERSION}/dfe_fetch",
+        headers=EXPECTED_HEADERS,
+        json=expected_json,
+        verify=False,
+    )
+
+    with pytest.raises(ValueError, match="must contain exactly two job ids"):
+        client.process_dfe(["1", "2", "3"])
+
+
+@mock.patch("requests.post")
 def test_superstaq_client_ibmq_set_token(mock_post: mock.MagicMock) -> None:
     client = gss.superstaq_client._SuperstaqClient(
         client_name="general-superstaq",
         remote_host="http://example.com",
         api_key="to_my_heart",
     )
```

### Comparing `general-superstaq-0.4.7/general_superstaq/superstaq_exceptions.py` & `general-superstaq-0.4.8/general_superstaq/superstaq_exceptions.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/superstaq_exceptions_test.py` & `general-superstaq-0.4.8/general_superstaq/superstaq_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/typing.py` & `general-superstaq-0.4.8/general_superstaq/typing.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/validation.py` & `general-superstaq-0.4.8/general_superstaq/validation.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq/validation_test.py` & `general-superstaq-0.4.8/general_superstaq/validation_test.py`

 * *Files identical despite different names*

### Comparing `general-superstaq-0.4.7/general_superstaq.egg-info/PKG-INFO` & `general-superstaq-0.4.8/general_superstaq.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: general-superstaq
-Version: 0.4.7
+Version: 0.4.8
 Summary: The general module that provides tools and access to Superstaq.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache 2
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `general-superstaq-0.4.7/general_superstaq.egg-info/SOURCES.txt` & `general-superstaq-0.4.8/general_superstaq.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 general_superstaq.egg-info/dependency_links.txt
 general_superstaq.egg-info/requires.txt
 general_superstaq.egg-info/top_level.txt
 general_superstaq/check/__init__.py
 general_superstaq/check/all_.py
 general_superstaq/check/build_docs.py
 general_superstaq/check/check_utils.py
+general_superstaq/check/checks-pyproject.toml
 general_superstaq/check/configs.py
 general_superstaq/check/coverage_.py
 general_superstaq/check/flake8_.py
 general_superstaq/check/format_.py
 general_superstaq/check/mypy_.py
 general_superstaq/check/pylint_.py
 general_superstaq/check/pytest_.py
```

### Comparing `general-superstaq-0.4.7/pyproject.toml` & `general-superstaq-0.4.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 include = ["general_superstaq*"]
 
 [tool.setuptools.package-data]
-general_superstaq = ["py.typed"]
+general_superstaq = ["py.typed", "check/checks-pyproject.toml"]
 
 [tool.setuptools.dynamic.version]
 attr = "general_superstaq._version.__version__"
 
 [tool.setuptools.dynamic.dependencies]
 file = ["requirements.txt"]
```

