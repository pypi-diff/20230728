# Comparing `tmp/alpaka-job-coverage-1.3.5.tar.gz` & `tmp/alpaka-job-coverage-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpaka-job-coverage-1.3.5.tar", last modified: Thu Jul 20 15:01:25 2023, max compression
+gzip compressed data, was "alpaka-job-coverage-1.3.6.tar", last modified: Fri Jul 28 05:46:19 2023, max compression
```

## Comparing `alpaka-job-coverage-1.3.5.tar` & `alpaka-job-coverage-1.3.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.516089 alpaka-job-coverage-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-20 15:01:25.516089 alpaka-job-coverage-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:01:25.516089 alpaka-job-coverage-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.512088 alpaka-job-coverage-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.512088 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_backend_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_compiler_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_compiler_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_software_dependency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/main_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.512088 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 15:01:25.000000 alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:01:25.516089 alpaka-job-coverage-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_compiler_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    41654 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_cuda_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_hipcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_single_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-20 15:01:03.000000 alpaka-job-coverage-1.3.5/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.740753 alpaka-job-coverage-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-28 05:46:19.740753 alpaka-job-coverage-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 05:46:19.740753 alpaka-job-coverage-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.736753 alpaka-job-coverage-1.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.736753 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_backend_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_compiler_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_compiler_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_software_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/main_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11681 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.736753 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 05:46:19.000000 alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 05:46:19.740753 alpaka-job-coverage-1.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_compiler_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41676 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_cuda_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12280 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_hipcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3134 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_single_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-28 05:46:00.000000 alpaka-job-coverage-1.3.6/version.txt
```

### Comparing `alpaka-job-coverage-1.3.5/LICENSE` & `alpaka-job-coverage-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/PKG-INFO` & `alpaka-job-coverage-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.5
+Version: 1.3.6
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.3.5/README.md` & `alpaka-job-coverage-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/setup.py` & `alpaka-job-coverage-1.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_backend_version.py` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_backend_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,14 +120,19 @@
         ) and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, ">", "11.2"):
             return False
 
         if row_check_version(
             row, DEVICE_COMPILER, "<=", "15"
         ) and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, ">", "11.5"):
             return False
+        
+        if row_check_version(
+            row, DEVICE_COMPILER, "<=", "16"
+        ) and row_check_backend_version(row, ALPAKA_ACC_GPU_CUDA_ENABLE, ">", "11.5"):
+            return False
 
     ###########################
     ## hipcc device compiler
     ###########################
 
     # the HIP backend needs to be enabled and has the same version number
     if row_check_name(row, DEVICE_COMPILER, "==", HIPCC):
```

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_compiler_name.py` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_compiler_name.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_compiler_version.py` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_compiler_version.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/filter_software_dependency.py` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/filter_software_dependency.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/globals.py` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/globals.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/main_functions.py` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/main_functions.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage/util.py` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage/util.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/PKG-INFO` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpaka-job-coverage
-Version: 1.3.5
+Version: 1.3.6
 Summary: The library provides everything needed to generate a sparse combination matrix for alpaca-based projects, including a set of general-purpose combination rules.
 Home-page: https://github.com/alpaka-group/alpaka-job-matrix-library
 Author: Simeon Ehrig
 Author-email: s.ehrig@hzdr.de
 Project-URL: Bug Tracker, https://github.com/alpaka-group/alpaka-job-matrix-library/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `alpaka-job-coverage-1.3.5/src/alpaka_job_coverage.egg-info/SOURCES.txt` & `alpaka-job-coverage-1.3.6/src/alpaka_job_coverage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/tests/test_compiler_names.py` & `alpaka-job-coverage-1.3.6/tests/test_compiler_names.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/tests/test_cuda_sdk.py` & `alpaka-job-coverage-1.3.6/tests/test_cuda_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -819,14 +819,15 @@
             9: 10.1,
             10: 10.1,
             11: 11.0,
             12: 11.0,
             13: 11.2,
             14: 11.5,
             15: 11.5,
+            16: 11.5,
         }
 
         for clang_version in supported_versions.keys():
             for cuda_version in cuda_versions:
                 comb = [
                     (CLANG_CUDA, str(clang_version)),
                     (CLANG_CUDA, str(clang_version)),
```

### Comparing `alpaka-job-coverage-1.3.5/tests/test_hipcc.py` & `alpaka-job-coverage-1.3.6/tests/test_hipcc.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/tests/test_single_rules.py` & `alpaka-job-coverage-1.3.6/tests/test_single_rules.py`

 * *Files identical despite different names*

### Comparing `alpaka-job-coverage-1.3.5/tests/test_util.py` & `alpaka-job-coverage-1.3.6/tests/test_util.py`

 * *Files identical despite different names*

