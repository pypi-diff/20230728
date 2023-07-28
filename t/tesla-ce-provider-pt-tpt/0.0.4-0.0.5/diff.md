# Comparing `tmp/tesla-ce-provider-pt-tpt-0.0.4.tar.gz` & `tmp/tesla-ce-provider-pt-tpt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesla-ce-provider-pt-tpt-0.0.4.tar", last modified: Tue Jul 25 15:14:16 2023, max compression
+gzip compressed data, was "tesla-ce-provider-pt-tpt-0.0.5.tar", last modified: Fri Jul 28 17:40:17 2023, max compression
```

## Comparing `tesla-ce-provider-pt-tpt-0.0.4.tar` & `tesla-ce-provider-pt-tpt-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.349770 tesla-ce-provider-pt-tpt-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-25 15:14:16.349770 tesla-ce-provider-pt-tpt-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 15:14:16.349770 tesla-ce-provider-pt-tpt-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-25 15:14:16.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tests/test_validation_tpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/data/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 15:14:15.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/data/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/tpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.345771 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 15:14:16.349770 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/base_tpt_lib_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/invalid_api_url.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/invalid_secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/request_failed.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-25 15:14:07.000000 tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/timeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.113679 tesla-ce-provider-pt-tpt-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-28 17:40:17.113679 tesla-ce-provider-pt-tpt-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 17:40:17.113679 tesla-ce-provider-pt-tpt-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.109679 tesla-ce-provider-pt-tpt-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.109679 tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-07-28 17:40:17.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-28 17:40:17.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 17:40:17.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-28 17:40:17.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 17:40:17.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.109679 tesla-ce-provider-pt-tpt-0.0.5/src/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tests/test_validation_tpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.109679 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.109679 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 17:40:16.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/data/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.113679 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/provider/tpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/provider/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.113679 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 17:40:17.113679 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/base_tpt_lib_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/invalid_api_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/invalid_secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/request_failed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-28 17:40:09.000000 tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/timeout.py
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/LICENSE` & `tesla-ce-provider-pt-tpt-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/PKG-INFO` & `tesla-ce-provider-pt-tpt-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-pt-tpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: TeSLA CE Plagiarism Provider
 Home-page: https://tesla-ce.github.io
 Author: Roger Muñoz Bernaus
 Author-email: rmunozber@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-pt-tpt/
 Project-URL: Source, https://github.com/tesla-ce/provider-pt-tpt
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/README.md` & `tesla-ce-provider-pt-tpt-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/requirements.txt` & `tesla-ce-provider-pt-tpt-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/setup.py` & `tesla-ce-provider-pt-tpt-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/PKG-INFO` & `tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesla-ce-provider-pt-tpt
-Version: 0.0.4
+Version: 0.0.5
 Summary: TeSLA CE Plagiarism Provider
 Home-page: https://tesla-ce.github.io
 Author: Roger Muñoz Bernaus
 Author-email: rmunozber@uoc.edu
 License: UNKNOWN
 Project-URL: Documentation, https://tesla-ce.github.io/provider-pt-tpt/
 Project-URL: Source, https://github.com/tesla-ce/provider-pt-tpt
```

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/SOURCES.txt` & `tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tesla_ce_provider_pt_tpt.egg-info/requires.txt` & `tesla-ce-provider-pt-tpt-0.0.5/src/tesla_ce_provider_pt_tpt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tests/__init__.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tests/conftest.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tests/test_validation_tpt.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tests/test_validation_tpt.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tests/utils.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tests/utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/__init__.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/__init__.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/tpt.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/provider/tpt.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/provider/utils.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/provider/utils.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/__init__.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/base_tpt_lib_exception.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/base_tpt_lib_exception.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/invalid_api_url.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/invalid_api_url.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/invalid_secret.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/invalid_secret.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/request_failed.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/request_failed.py`

 * *Files identical despite different names*

### Comparing `tesla-ce-provider-pt-tpt-0.0.4/src/tpt/tpt_lib/exceptions/timeout.py` & `tesla-ce-provider-pt-tpt-0.0.5/src/tpt/tpt_lib/exceptions/timeout.py`

 * *Files identical despite different names*

