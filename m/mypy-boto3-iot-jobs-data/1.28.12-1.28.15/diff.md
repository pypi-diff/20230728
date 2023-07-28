# Comparing `tmp/mypy-boto3-iot-jobs-data-1.28.12.tar.gz` & `tmp/mypy-boto3-iot-jobs-data-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-jobs-data-1.28.12.tar", last modified: Thu Jul 27 05:34:48 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-jobs-data-1.28.15.tar", last modified: Fri Jul 28 20:42:58 2023, max compression
```

## Comparing `mypy-boto3-iot-jobs-data-1.28.12.tar` & `mypy-boto3-iot-jobs-data-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.748485 mypy-boto3-iot-jobs-data-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-07-27 05:34:48.748485 mypy-boto3-iot-jobs-data-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.744485 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5343 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.748485 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-07-27 05:34:48.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:48.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:48.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:48.000000 mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:48.748485 mypy-boto3-iot-jobs-data-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-27 05:23:53.000000 mypy-boto3-iot-jobs-data-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:58.793248 mypy-boto3-iot-jobs-data-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-07-28 20:42:58.785247 mypy-boto3-iot-jobs-data-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11137 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:58.785247 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-28 20:28:11.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-07-28 20:28:11.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:58.785247 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-07-28 20:42:58.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 20:42:58.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:58.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:58.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:58.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:58.000000 mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:58.793248 mypy-boto3-iot-jobs-data-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-28 20:28:10.000000 mypy-boto3-iot-jobs-data-1.28.15/setup.py
```

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/LICENSE` & `mypy-boto3-iot-jobs-data-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/PKG-INFO` & `mypy-boto3-iot-jobs-data-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-jobs-data
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTJobsDataPlane 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTJobsDataPlane 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-jobs-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-jobs-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-jobs-data)](https://pepy.tech/project/mypy-boto3-iot-jobs-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTJobsDataPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
+[boto3.IoTJobsDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-jobs-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,18 +300,18 @@
 `mypy_boto3_iot_jobs_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_jobs_data.type_defs import (
     DescribeJobExecutionRequestRequestTypeDef,
     JobExecutionTypeDef,
+    ResponseMetadataTypeDef,
     GetPendingJobExecutionsRequestRequestTypeDef,
     JobExecutionSummaryTypeDef,
     JobExecutionStateTypeDef,
-    ResponseMetadataTypeDef,
     StartNextPendingJobExecutionRequestRequestTypeDef,
     UpdateJobExecutionRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     StartNextPendingJobExecutionResponseTypeDef,
     GetPendingJobExecutionsResponseTypeDef,
     UpdateJobExecutionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/README.md` & `mypy-boto3-iot-jobs-data-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-jobs-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-jobs-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-jobs-data)](https://pepy.tech/project/mypy-boto3-iot-jobs-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTJobsDataPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
+[boto3.IoTJobsDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-jobs-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -268,18 +268,18 @@
 `mypy_boto3_iot_jobs_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_jobs_data.type_defs import (
     DescribeJobExecutionRequestRequestTypeDef,
     JobExecutionTypeDef,
+    ResponseMetadataTypeDef,
     GetPendingJobExecutionsRequestRequestTypeDef,
     JobExecutionSummaryTypeDef,
     JobExecutionStateTypeDef,
-    ResponseMetadataTypeDef,
     StartNextPendingJobExecutionRequestRequestTypeDef,
     UpdateJobExecutionRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     StartNextPendingJobExecutionResponseTypeDef,
     GetPendingJobExecutionsResponseTypeDef,
     UpdateJobExecutionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/__main__.py` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTJobsDataPlane 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTJobsDataPlane 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.12")
+    print("1.28.15")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/client.py` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/client.pyi` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/literals.py` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/literals.pyi` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/type_defs.py` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,21 @@
 from .literals import JobExecutionStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DescribeJobExecutionRequestRequestTypeDef",
     "JobExecutionTypeDef",
+    "ResponseMetadataTypeDef",
     "GetPendingJobExecutionsRequestRequestTypeDef",
     "JobExecutionSummaryTypeDef",
     "JobExecutionStateTypeDef",
-    "ResponseMetadataTypeDef",
     "StartNextPendingJobExecutionRequestRequestTypeDef",
     "UpdateJobExecutionRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "StartNextPendingJobExecutionResponseTypeDef",
     "GetPendingJobExecutionsResponseTypeDef",
     "UpdateJobExecutionResponseTypeDef",
 )
@@ -49,22 +48,20 @@
     {
         "includeJobDocument": bool,
         "executionNumber": int,
     },
     total=False,
 )
 
-
 class DescribeJobExecutionRequestRequestTypeDef(
     _RequiredDescribeJobExecutionRequestRequestTypeDef,
     _OptionalDescribeJobExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 JobExecutionTypeDef = TypedDict(
     "JobExecutionTypeDef",
     {
         "jobId": str,
         "thingName": str,
         "status": JobExecutionStatusType,
         "statusDetails": Dict[str, str],
@@ -75,14 +72,25 @@
         "versionNumber": int,
         "executionNumber": int,
         "jobDocument": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 GetPendingJobExecutionsRequestRequestTypeDef = TypedDict(
     "GetPendingJobExecutionsRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
@@ -105,25 +113,14 @@
         "status": JobExecutionStatusType,
         "statusDetails": Dict[str, str],
         "versionNumber": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredStartNextPendingJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartNextPendingJobExecutionRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalStartNextPendingJobExecutionRequestRequestTypeDef = TypedDict(
@@ -131,22 +128,20 @@
     {
         "statusDetails": Mapping[str, str],
         "stepTimeoutInMinutes": int,
     },
     total=False,
 )
 
-
 class StartNextPendingJobExecutionRequestRequestTypeDef(
     _RequiredStartNextPendingJobExecutionRequestRequestTypeDef,
     _OptionalStartNextPendingJobExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobExecutionRequestRequestTypeDef",
     {
         "jobId": str,
         "thingName": str,
         "status": JobExecutionStatusType,
     },
@@ -160,48 +155,46 @@
         "includeJobExecutionState": bool,
         "includeJobDocument": bool,
         "executionNumber": int,
     },
     total=False,
 )
 
-
 class UpdateJobExecutionRequestRequestTypeDef(
     _RequiredUpdateJobExecutionRequestRequestTypeDef,
     _OptionalUpdateJobExecutionRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeJobExecutionResponseTypeDef = TypedDict(
     "DescribeJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartNextPendingJobExecutionResponseTypeDef = TypedDict(
     "StartNextPendingJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPendingJobExecutionsResponseTypeDef = TypedDict(
     "GetPendingJobExecutionsResponseTypeDef",
     {
         "inProgressJobs": List[JobExecutionSummaryTypeDef],
         "queuedJobs": List[JobExecutionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobExecutionResponseTypeDef = TypedDict(
     "UpdateJobExecutionResponseTypeDef",
     {
         "executionState": JobExecutionStateTypeDef,
         "jobDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data/type_defs.pyi` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,22 @@
 from .literals import JobExecutionStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "DescribeJobExecutionRequestRequestTypeDef",
     "JobExecutionTypeDef",
+    "ResponseMetadataTypeDef",
     "GetPendingJobExecutionsRequestRequestTypeDef",
     "JobExecutionSummaryTypeDef",
     "JobExecutionStateTypeDef",
-    "ResponseMetadataTypeDef",
     "StartNextPendingJobExecutionRequestRequestTypeDef",
     "UpdateJobExecutionRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
     "StartNextPendingJobExecutionResponseTypeDef",
     "GetPendingJobExecutionsResponseTypeDef",
     "UpdateJobExecutionResponseTypeDef",
 )
@@ -48,20 +49,22 @@
     {
         "includeJobDocument": bool,
         "executionNumber": int,
     },
     total=False,
 )
 
+
 class DescribeJobExecutionRequestRequestTypeDef(
     _RequiredDescribeJobExecutionRequestRequestTypeDef,
     _OptionalDescribeJobExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 JobExecutionTypeDef = TypedDict(
     "JobExecutionTypeDef",
     {
         "jobId": str,
         "thingName": str,
         "status": JobExecutionStatusType,
         "statusDetails": Dict[str, str],
@@ -72,14 +75,25 @@
         "versionNumber": int,
         "executionNumber": int,
         "jobDocument": str,
     },
     total=False,
 )
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 GetPendingJobExecutionsRequestRequestTypeDef = TypedDict(
     "GetPendingJobExecutionsRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
@@ -102,25 +116,14 @@
         "status": JobExecutionStatusType,
         "statusDetails": Dict[str, str],
         "versionNumber": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredStartNextPendingJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartNextPendingJobExecutionRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalStartNextPendingJobExecutionRequestRequestTypeDef = TypedDict(
@@ -128,20 +131,22 @@
     {
         "statusDetails": Mapping[str, str],
         "stepTimeoutInMinutes": int,
     },
     total=False,
 )
 
+
 class StartNextPendingJobExecutionRequestRequestTypeDef(
     _RequiredStartNextPendingJobExecutionRequestRequestTypeDef,
     _OptionalStartNextPendingJobExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobExecutionRequestRequestTypeDef",
     {
         "jobId": str,
         "thingName": str,
         "status": JobExecutionStatusType,
     },
@@ -155,46 +160,48 @@
         "includeJobExecutionState": bool,
         "includeJobDocument": bool,
         "executionNumber": int,
     },
     total=False,
 )
 
+
 class UpdateJobExecutionRequestRequestTypeDef(
     _RequiredUpdateJobExecutionRequestRequestTypeDef,
     _OptionalUpdateJobExecutionRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeJobExecutionResponseTypeDef = TypedDict(
     "DescribeJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartNextPendingJobExecutionResponseTypeDef = TypedDict(
     "StartNextPendingJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPendingJobExecutionsResponseTypeDef = TypedDict(
     "GetPendingJobExecutionsResponseTypeDef",
     {
         "inProgressJobs": List[JobExecutionSummaryTypeDef],
         "queuedJobs": List[JobExecutionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobExecutionResponseTypeDef = TypedDict(
     "UpdateJobExecutionResponseTypeDef",
     {
         "executionState": JobExecutionStateTypeDef,
         "jobDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/PKG-INFO` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot-jobs-data
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTJobsDataPlane 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTJobsDataPlane 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot-jobs-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot-jobs-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot-jobs-data)](https://pepy.tech/project/mypy-boto3-iot-jobs-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTJobsDataPlane 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
+[boto3.IoTJobsDataPlane 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot-jobs-data.html#IoTJobsDataPlane)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.15.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.16.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-iot-jobs-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot_jobs_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,18 +300,18 @@
 `mypy_boto3_iot_jobs_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot_jobs_data.type_defs import (
     DescribeJobExecutionRequestRequestTypeDef,
     JobExecutionTypeDef,
+    ResponseMetadataTypeDef,
     GetPendingJobExecutionsRequestRequestTypeDef,
     JobExecutionSummaryTypeDef,
     JobExecutionStateTypeDef,
-    ResponseMetadataTypeDef,
     StartNextPendingJobExecutionRequestRequestTypeDef,
     UpdateJobExecutionRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
     StartNextPendingJobExecutionResponseTypeDef,
     GetPendingJobExecutionsResponseTypeDef,
     UpdateJobExecutionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/mypy_boto3_iot_jobs_data.egg-info/SOURCES.txt` & `mypy-boto3-iot-jobs-data-1.28.15/mypy_boto3_iot_jobs_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-jobs-data-1.28.12/setup.py` & `mypy-boto3-iot-jobs-data-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot-jobs-data",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iot_jobs_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTJobsDataPlane 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IoTJobsDataPlane 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

