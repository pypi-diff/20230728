# Comparing `tmp/mypy-boto3-braket-1.28.12.tar.gz` & `tmp/mypy-boto3-braket-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-braket-1.28.12.tar", last modified: Thu Jul 27 05:34:22 2023, max compression
+gzip compressed data, was "mypy-boto3-braket-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
```

## Comparing `mypy-boto3-braket-1.28.12.tar` & `mypy-boto3-braket-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/mypy_boto3_braket/
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-27 05:18:02.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15003 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:22.000000 mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:22.772567 mypy-boto3-braket-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:18:01.000000 mypy-boto3-braket-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.324737 mypy-boto3-braket-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-07-28 20:42:22.324737 mypy-boto3-braket-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13132 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.320737 mypy-boto3-braket-1.28.15/mypy_boto3_braket/
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12403 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10144 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17637 2023-07-28 20:20:17.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17606 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:16.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.324737 mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-07-28 20:42:22.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:22.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:22.000000 mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.324737 mypy-boto3-braket-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:20:15.000000 mypy-boto3-braket-1.28.15/setup.py
```

### Comparing `mypy-boto3-braket-1.28.12/LICENSE` & `mypy-boto3-braket-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.12/PKG-INFO` & `mypy-boto3-braket-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-braket
-Version: 1.28.12
-Summary: Type annotations for boto3.Braket 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Braket 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-braket)](https://pepy.tech/project/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,76 +338,65 @@
 ### Typed dictionaries
 
 `mypy_boto3_braket.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
-    ContainerImageOutputTypeDef,
-    ScriptModeConfigOutputTypeDef,
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
-    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
-    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
-    CreateQuantumTaskResponseTypeDef,
-    S3DataSourceOutputTypeDef,
     S3DataSourceTypeDef,
-    DeviceConfigOutputTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
-    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
-    InstanceConfigOutputTypeDef,
-    JobCheckpointConfigOutputTypeDef,
     JobEventDetailsTypeDef,
-    JobOutputDataConfigOutputTypeDef,
-    JobStoppingConditionOutputTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
-    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
-    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AlgorithmSpecificationOutputTypeDef,
     AlgorithmSpecificationTypeDef,
-    DataSourceOutputTypeDef,
+    CancelJobResponseTypeDef,
+    CancelQuantumTaskResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateQuantumTaskResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    GetQuantumTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
     SearchJobsRequestSearchJobsPaginateTypeDef,
     SearchQuantumTasksRequestRequestTypeDef,
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
-    InputFileConfigOutputTypeDef,
     InputFileConfigTypeDef,
-    GetJobResponseTypeDef,
     CreateJobRequestRequestTypeDef,
+    GetJobResponseTypeDef,
 )
 
 
-def get_structure() -> ContainerImageOutputTypeDef:
+def get_structure() -> ContainerImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-braket-1.28.12/README.md` & `mypy-boto3-braket-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-braket)](https://pepy.tech/project/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,76 +306,65 @@
 ### Typed dictionaries
 
 `mypy_boto3_braket.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
-    ContainerImageOutputTypeDef,
-    ScriptModeConfigOutputTypeDef,
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
-    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
-    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
-    CreateQuantumTaskResponseTypeDef,
-    S3DataSourceOutputTypeDef,
     S3DataSourceTypeDef,
-    DeviceConfigOutputTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
-    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
-    InstanceConfigOutputTypeDef,
-    JobCheckpointConfigOutputTypeDef,
     JobEventDetailsTypeDef,
-    JobOutputDataConfigOutputTypeDef,
-    JobStoppingConditionOutputTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
-    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
-    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AlgorithmSpecificationOutputTypeDef,
     AlgorithmSpecificationTypeDef,
-    DataSourceOutputTypeDef,
+    CancelJobResponseTypeDef,
+    CancelQuantumTaskResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateQuantumTaskResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    GetQuantumTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
     SearchJobsRequestSearchJobsPaginateTypeDef,
     SearchQuantumTasksRequestRequestTypeDef,
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
-    InputFileConfigOutputTypeDef,
     InputFileConfigTypeDef,
-    GetJobResponseTypeDef,
     CreateJobRequestRequestTypeDef,
+    GetJobResponseTypeDef,
 )
 
 
-def get_structure() -> ContainerImageOutputTypeDef:
+def get_structure() -> ContainerImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/__init__.py` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/__init__.pyi` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/__main__.py` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Braket 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Braket 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket\nOther"
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

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/client.py` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/client.pyi` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/literals.py` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/literals.pyi` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/paginator.py` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchdevicespaginator)
         """
 
 
@@ -74,15 +74,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchjobspaginator)
         """
 
 
@@ -92,13 +92,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchquantumtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchQuantumTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchquantumtaskspaginator)
         """
```

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/paginator.pyi` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchdevicespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchDevicesFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchdevicespaginator)
         """
 
 class SearchJobsPaginator(Paginator):
@@ -70,15 +70,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchjobspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchJobsFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchjobspaginator)
         """
 
 class SearchQuantumTasksPaginator(Paginator):
@@ -87,13 +87,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchquantumtaskspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SearchQuantumTasksFilterTypeDef],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchQuantumTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket.Paginator.SearchQuantumTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/paginators/#searchquantumtaskspaginator)
         """
```

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/type_defs.py` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for braket service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_braket.type_defs import ContainerImageOutputTypeDef
+    from mypy_boto3_braket.type_defs import ContainerImageTypeDef
 
-    data: ContainerImageOutputTypeDef = {...}
+    data: ContainerImageTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -31,103 +31,63 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ContainerImageOutputTypeDef",
-    "ScriptModeConfigOutputTypeDef",
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "CancelJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
-    "CancelQuantumTaskResponseTypeDef",
     "DeviceConfigTypeDef",
     "InstanceConfigTypeDef",
     "JobCheckpointConfigTypeDef",
     "JobOutputDataConfigTypeDef",
     "JobStoppingConditionTypeDef",
-    "CreateJobResponseTypeDef",
     "CreateQuantumTaskRequestRequestTypeDef",
-    "CreateQuantumTaskResponseTypeDef",
-    "S3DataSourceOutputTypeDef",
     "S3DataSourceTypeDef",
-    "DeviceConfigOutputTypeDef",
     "DeviceSummaryTypeDef",
     "GetDeviceRequestRequestTypeDef",
-    "GetDeviceResponseTypeDef",
     "GetJobRequestRequestTypeDef",
-    "InstanceConfigOutputTypeDef",
-    "JobCheckpointConfigOutputTypeDef",
     "JobEventDetailsTypeDef",
-    "JobOutputDataConfigOutputTypeDef",
-    "JobStoppingConditionOutputTypeDef",
     "GetQuantumTaskRequestRequestTypeDef",
-    "GetQuantumTaskResponseTypeDef",
     "JobSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "QuantumTaskSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchDevicesFilterTypeDef",
     "SearchJobsFilterTypeDef",
     "SearchQuantumTasksFilterTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AlgorithmSpecificationOutputTypeDef",
     "AlgorithmSpecificationTypeDef",
-    "DataSourceOutputTypeDef",
+    "CancelJobResponseTypeDef",
+    "CancelQuantumTaskResponseTypeDef",
+    "CreateJobResponseTypeDef",
+    "CreateQuantumTaskResponseTypeDef",
+    "GetDeviceResponseTypeDef",
+    "GetQuantumTaskResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DataSourceTypeDef",
     "SearchDevicesResponseTypeDef",
     "SearchJobsResponseTypeDef",
     "SearchQuantumTasksResponseTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchJobsRequestRequestTypeDef",
     "SearchJobsRequestSearchJobsPaginateTypeDef",
     "SearchQuantumTasksRequestRequestTypeDef",
     "SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
-    "InputFileConfigOutputTypeDef",
     "InputFileConfigTypeDef",
-    "GetJobResponseTypeDef",
     "CreateJobRequestRequestTypeDef",
+    "GetJobResponseTypeDef",
 )
 
-ContainerImageOutputTypeDef = TypedDict(
-    "ContainerImageOutputTypeDef",
-    {
-        "uri": str,
-    },
-)
-
-_RequiredScriptModeConfigOutputTypeDef = TypedDict(
-    "_RequiredScriptModeConfigOutputTypeDef",
-    {
-        "entryPoint": str,
-        "s3Uri": str,
-    },
-)
-_OptionalScriptModeConfigOutputTypeDef = TypedDict(
-    "_OptionalScriptModeConfigOutputTypeDef",
-    {
-        "compressionType": CompressionTypeType,
-    },
-    total=False,
-)
-
-
-class ScriptModeConfigOutputTypeDef(
-    _RequiredScriptModeConfigOutputTypeDef, _OptionalScriptModeConfigOutputTypeDef
-):
-    pass
-
-
 ContainerImageTypeDef = TypedDict(
     "ContainerImageTypeDef",
     {
         "uri": str,
     },
 )
 
@@ -154,40 +114,33 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "cancellationStatus": CancellationStatusType,
-        "jobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelQuantumTaskRequestRequestTypeDef = TypedDict(
     "CancelQuantumTaskRequestRequestTypeDef",
     {
         "clientToken": str,
         "quantumTaskArn": str,
     },
 )
 
-CancelQuantumTaskResponseTypeDef = TypedDict(
-    "CancelQuantumTaskResponseTypeDef",
-    {
-        "cancellationStatus": CancellationStatusType,
-        "quantumTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceConfigTypeDef = TypedDict(
     "DeviceConfigTypeDef",
     {
         "device": str,
     },
 )
 
@@ -257,22 +210,14 @@
     "JobStoppingConditionTypeDef",
     {
         "maxRuntimeInSeconds": int,
     },
     total=False,
 )
 
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateQuantumTaskRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuantumTaskRequestRequestTypeDef",
     {
         "action": str,
         "clientToken": str,
         "deviceArn": str,
         "outputS3Bucket": str,
@@ -293,43 +238,21 @@
 
 class CreateQuantumTaskRequestRequestTypeDef(
     _RequiredCreateQuantumTaskRequestRequestTypeDef, _OptionalCreateQuantumTaskRequestRequestTypeDef
 ):
     pass
 
 
-CreateQuantumTaskResponseTypeDef = TypedDict(
-    "CreateQuantumTaskResponseTypeDef",
-    {
-        "quantumTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-S3DataSourceOutputTypeDef = TypedDict(
-    "S3DataSourceOutputTypeDef",
-    {
-        "s3Uri": str,
-    },
-)
-
 S3DataSourceTypeDef = TypedDict(
     "S3DataSourceTypeDef",
     {
         "s3Uri": str,
     },
 )
 
-DeviceConfigOutputTypeDef = TypedDict(
-    "DeviceConfigOutputTypeDef",
-    {
-        "device": str,
-    },
-)
-
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "deviceArn": str,
         "deviceName": str,
         "deviceStatus": DeviceStatusType,
         "deviceType": DeviceTypeType,
@@ -340,142 +263,38 @@
 GetDeviceRequestRequestTypeDef = TypedDict(
     "GetDeviceRequestRequestTypeDef",
     {
         "deviceArn": str,
     },
 )
 
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
-    {
-        "deviceArn": str,
-        "deviceCapabilities": str,
-        "deviceName": str,
-        "deviceStatus": DeviceStatusType,
-        "deviceType": DeviceTypeType,
-        "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
-_RequiredInstanceConfigOutputTypeDef = TypedDict(
-    "_RequiredInstanceConfigOutputTypeDef",
-    {
-        "instanceType": InstanceTypeType,
-        "volumeSizeInGb": int,
-    },
-)
-_OptionalInstanceConfigOutputTypeDef = TypedDict(
-    "_OptionalInstanceConfigOutputTypeDef",
-    {
-        "instanceCount": int,
-    },
-    total=False,
-)
-
-
-class InstanceConfigOutputTypeDef(
-    _RequiredInstanceConfigOutputTypeDef, _OptionalInstanceConfigOutputTypeDef
-):
-    pass
-
-
-_RequiredJobCheckpointConfigOutputTypeDef = TypedDict(
-    "_RequiredJobCheckpointConfigOutputTypeDef",
-    {
-        "s3Uri": str,
-    },
-)
-_OptionalJobCheckpointConfigOutputTypeDef = TypedDict(
-    "_OptionalJobCheckpointConfigOutputTypeDef",
-    {
-        "localPath": str,
-    },
-    total=False,
-)
-
-
-class JobCheckpointConfigOutputTypeDef(
-    _RequiredJobCheckpointConfigOutputTypeDef, _OptionalJobCheckpointConfigOutputTypeDef
-):
-    pass
-
-
 JobEventDetailsTypeDef = TypedDict(
     "JobEventDetailsTypeDef",
     {
         "eventType": JobEventTypeType,
         "message": str,
         "timeOfEvent": datetime,
     },
     total=False,
 )
 
-_RequiredJobOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredJobOutputDataConfigOutputTypeDef",
-    {
-        "s3Path": str,
-    },
-)
-_OptionalJobOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalJobOutputDataConfigOutputTypeDef",
-    {
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class JobOutputDataConfigOutputTypeDef(
-    _RequiredJobOutputDataConfigOutputTypeDef, _OptionalJobOutputDataConfigOutputTypeDef
-):
-    pass
-
-
-JobStoppingConditionOutputTypeDef = TypedDict(
-    "JobStoppingConditionOutputTypeDef",
-    {
-        "maxRuntimeInSeconds": int,
-    },
-    total=False,
-)
-
 GetQuantumTaskRequestRequestTypeDef = TypedDict(
     "GetQuantumTaskRequestRequestTypeDef",
     {
         "quantumTaskArn": str,
     },
 )
 
-GetQuantumTaskResponseTypeDef = TypedDict(
-    "GetQuantumTaskResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "deviceArn": str,
-        "deviceParameters": str,
-        "endedAt": datetime,
-        "failureReason": str,
-        "jobArn": str,
-        "outputS3Bucket": str,
-        "outputS3Directory": str,
-        "quantumTaskArn": str,
-        "shots": int,
-        "status": QuantumTaskStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredJobSummaryTypeDef = TypedDict(
     "_RequiredJobSummaryTypeDef",
     {
         "createdAt": datetime,
         "device": str,
         "jobArn": str,
         "jobName": str,
@@ -500,22 +319,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -546,25 +357,14 @@
 
 class QuantumTaskSummaryTypeDef(
     _RequiredQuantumTaskSummaryTypeDef, _OptionalQuantumTaskSummaryTypeDef
 ):
     pass
 
 
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
 SearchDevicesFilterTypeDef = TypedDict(
     "SearchDevicesFilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
 )
@@ -599,36 +399,94 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-AlgorithmSpecificationOutputTypeDef = TypedDict(
-    "AlgorithmSpecificationOutputTypeDef",
-    {
-        "containerImage": ContainerImageOutputTypeDef,
-        "scriptModeConfig": ScriptModeConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 AlgorithmSpecificationTypeDef = TypedDict(
     "AlgorithmSpecificationTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
         "scriptModeConfig": ScriptModeConfigTypeDef,
     },
     total=False,
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "jobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelQuantumTaskResponseTypeDef = TypedDict(
+    "CancelQuantumTaskResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "quantumTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateQuantumTaskResponseTypeDef = TypedDict(
+    "CreateQuantumTaskResponseTypeDef",
+    {
+        "quantumTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
+    {
+        "deviceArn": str,
+        "deviceCapabilities": str,
+        "deviceName": str,
+        "deviceStatus": DeviceStatusType,
+        "deviceType": DeviceTypeType,
+        "providerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQuantumTaskResponseTypeDef = TypedDict(
+    "GetQuantumTaskResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "deviceArn": str,
+        "deviceParameters": str,
+        "endedAt": datetime,
+        "failureReason": str,
+        "jobArn": str,
+        "outputS3Bucket": str,
+        "outputS3Directory": str,
+        "quantumTaskArn": str,
+        "shots": int,
+        "status": QuantumTaskStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "s3DataSource": S3DataSourceOutputTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "s3DataSource": S3DataSourceTypeDef,
@@ -636,33 +494,33 @@
 )
 
 SearchDevicesResponseTypeDef = TypedDict(
     "SearchDevicesResponseTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchJobsResponseTypeDef = TypedDict(
     "SearchJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchQuantumTasksResponseTypeDef = TypedDict(
     "SearchQuantumTasksResponseTypeDef",
     {
         "nextToken": str,
         "quantumTasks": List[QuantumTaskSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestRequestTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
@@ -689,15 +547,15 @@
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
     },
 )
 _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchDevicesRequestSearchDevicesPaginateTypeDef(
     _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef,
@@ -733,15 +591,15 @@
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_OptionalSearchJobsRequestSearchJobsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchJobsRequestSearchJobsPaginateTypeDef(
     _RequiredSearchJobsRequestSearchJobsPaginateTypeDef,
@@ -778,49 +636,27 @@
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(
     _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
 ):
     pass
 
 
-_RequiredInputFileConfigOutputTypeDef = TypedDict(
-    "_RequiredInputFileConfigOutputTypeDef",
-    {
-        "channelName": str,
-        "dataSource": DataSourceOutputTypeDef,
-    },
-)
-_OptionalInputFileConfigOutputTypeDef = TypedDict(
-    "_OptionalInputFileConfigOutputTypeDef",
-    {
-        "contentType": str,
-    },
-    total=False,
-)
-
-
-class InputFileConfigOutputTypeDef(
-    _RequiredInputFileConfigOutputTypeDef, _OptionalInputFileConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredInputFileConfigTypeDef = TypedDict(
     "_RequiredInputFileConfigTypeDef",
     {
         "channelName": str,
         "dataSource": DataSourceTypeDef,
     },
 )
@@ -833,40 +669,14 @@
 )
 
 
 class InputFileConfigTypeDef(_RequiredInputFileConfigTypeDef, _OptionalInputFileConfigTypeDef):
     pass
 
 
-GetJobResponseTypeDef = TypedDict(
-    "GetJobResponseTypeDef",
-    {
-        "algorithmSpecification": AlgorithmSpecificationOutputTypeDef,
-        "billableDuration": int,
-        "checkpointConfig": JobCheckpointConfigOutputTypeDef,
-        "createdAt": datetime,
-        "deviceConfig": DeviceConfigOutputTypeDef,
-        "endedAt": datetime,
-        "events": List[JobEventDetailsTypeDef],
-        "failureReason": str,
-        "hyperParameters": Dict[str, str],
-        "inputDataConfig": List[InputFileConfigOutputTypeDef],
-        "instanceConfig": InstanceConfigOutputTypeDef,
-        "jobArn": str,
-        "jobName": str,
-        "outputDataConfig": JobOutputDataConfigOutputTypeDef,
-        "roleArn": str,
-        "startedAt": datetime,
-        "status": JobPrimaryStatusType,
-        "stoppingCondition": JobStoppingConditionOutputTypeDef,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "algorithmSpecification": AlgorithmSpecificationTypeDef,
         "clientToken": str,
         "deviceConfig": DeviceConfigTypeDef,
         "instanceConfig": InstanceConfigTypeDef,
@@ -888,7 +698,34 @@
 )
 
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
+
+
+GetJobResponseTypeDef = TypedDict(
+    "GetJobResponseTypeDef",
+    {
+        "algorithmSpecification": AlgorithmSpecificationTypeDef,
+        "billableDuration": int,
+        "checkpointConfig": JobCheckpointConfigTypeDef,
+        "createdAt": datetime,
+        "deviceConfig": DeviceConfigTypeDef,
+        "endedAt": datetime,
+        "events": List[JobEventDetailsTypeDef],
+        "failureReason": str,
+        "hyperParameters": Dict[str, str],
+        "inputDataConfig": List[InputFileConfigTypeDef],
+        "instanceConfig": InstanceConfigTypeDef,
+        "jobArn": str,
+        "jobName": str,
+        "outputDataConfig": JobOutputDataConfigTypeDef,
+        "roleArn": str,
+        "startedAt": datetime,
+        "status": JobPrimaryStatusType,
+        "stoppingCondition": JobStoppingConditionTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket/type_defs.pyi` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for braket service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_braket.type_defs import ContainerImageOutputTypeDef
+    from mypy_boto3_braket.type_defs import ContainerImageTypeDef
 
-    data: ContainerImageOutputTypeDef = {...}
+    data: ContainerImageTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -30,101 +30,63 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ContainerImageOutputTypeDef",
-    "ScriptModeConfigOutputTypeDef",
     "ContainerImageTypeDef",
     "ScriptModeConfigTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "CancelJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelQuantumTaskRequestRequestTypeDef",
-    "CancelQuantumTaskResponseTypeDef",
     "DeviceConfigTypeDef",
     "InstanceConfigTypeDef",
     "JobCheckpointConfigTypeDef",
     "JobOutputDataConfigTypeDef",
     "JobStoppingConditionTypeDef",
-    "CreateJobResponseTypeDef",
     "CreateQuantumTaskRequestRequestTypeDef",
-    "CreateQuantumTaskResponseTypeDef",
-    "S3DataSourceOutputTypeDef",
     "S3DataSourceTypeDef",
-    "DeviceConfigOutputTypeDef",
     "DeviceSummaryTypeDef",
     "GetDeviceRequestRequestTypeDef",
-    "GetDeviceResponseTypeDef",
     "GetJobRequestRequestTypeDef",
-    "InstanceConfigOutputTypeDef",
-    "JobCheckpointConfigOutputTypeDef",
     "JobEventDetailsTypeDef",
-    "JobOutputDataConfigOutputTypeDef",
-    "JobStoppingConditionOutputTypeDef",
     "GetQuantumTaskRequestRequestTypeDef",
-    "GetQuantumTaskResponseTypeDef",
     "JobSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PaginatorConfigTypeDef",
     "QuantumTaskSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchDevicesFilterTypeDef",
     "SearchJobsFilterTypeDef",
     "SearchQuantumTasksFilterTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "AlgorithmSpecificationOutputTypeDef",
     "AlgorithmSpecificationTypeDef",
-    "DataSourceOutputTypeDef",
+    "CancelJobResponseTypeDef",
+    "CancelQuantumTaskResponseTypeDef",
+    "CreateJobResponseTypeDef",
+    "CreateQuantumTaskResponseTypeDef",
+    "GetDeviceResponseTypeDef",
+    "GetQuantumTaskResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "DataSourceTypeDef",
     "SearchDevicesResponseTypeDef",
     "SearchJobsResponseTypeDef",
     "SearchQuantumTasksResponseTypeDef",
     "SearchDevicesRequestRequestTypeDef",
     "SearchDevicesRequestSearchDevicesPaginateTypeDef",
     "SearchJobsRequestRequestTypeDef",
     "SearchJobsRequestSearchJobsPaginateTypeDef",
     "SearchQuantumTasksRequestRequestTypeDef",
     "SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
-    "InputFileConfigOutputTypeDef",
     "InputFileConfigTypeDef",
-    "GetJobResponseTypeDef",
     "CreateJobRequestRequestTypeDef",
+    "GetJobResponseTypeDef",
 )
 
-ContainerImageOutputTypeDef = TypedDict(
-    "ContainerImageOutputTypeDef",
-    {
-        "uri": str,
-    },
-)
-
-_RequiredScriptModeConfigOutputTypeDef = TypedDict(
-    "_RequiredScriptModeConfigOutputTypeDef",
-    {
-        "entryPoint": str,
-        "s3Uri": str,
-    },
-)
-_OptionalScriptModeConfigOutputTypeDef = TypedDict(
-    "_OptionalScriptModeConfigOutputTypeDef",
-    {
-        "compressionType": CompressionTypeType,
-    },
-    total=False,
-)
-
-class ScriptModeConfigOutputTypeDef(
-    _RequiredScriptModeConfigOutputTypeDef, _OptionalScriptModeConfigOutputTypeDef
-):
-    pass
-
 ContainerImageTypeDef = TypedDict(
     "ContainerImageTypeDef",
     {
         "uri": str,
     },
 )
 
@@ -149,40 +111,33 @@
 CancelJobRequestRequestTypeDef = TypedDict(
     "CancelJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "cancellationStatus": CancellationStatusType,
-        "jobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelQuantumTaskRequestRequestTypeDef = TypedDict(
     "CancelQuantumTaskRequestRequestTypeDef",
     {
         "clientToken": str,
         "quantumTaskArn": str,
     },
 )
 
-CancelQuantumTaskResponseTypeDef = TypedDict(
-    "CancelQuantumTaskResponseTypeDef",
-    {
-        "cancellationStatus": CancellationStatusType,
-        "quantumTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceConfigTypeDef = TypedDict(
     "DeviceConfigTypeDef",
     {
         "device": str,
     },
 )
 
@@ -246,22 +201,14 @@
     "JobStoppingConditionTypeDef",
     {
         "maxRuntimeInSeconds": int,
     },
     total=False,
 )
 
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateQuantumTaskRequestRequestTypeDef = TypedDict(
     "_RequiredCreateQuantumTaskRequestRequestTypeDef",
     {
         "action": str,
         "clientToken": str,
         "deviceArn": str,
         "outputS3Bucket": str,
@@ -280,43 +227,21 @@
 )
 
 class CreateQuantumTaskRequestRequestTypeDef(
     _RequiredCreateQuantumTaskRequestRequestTypeDef, _OptionalCreateQuantumTaskRequestRequestTypeDef
 ):
     pass
 
-CreateQuantumTaskResponseTypeDef = TypedDict(
-    "CreateQuantumTaskResponseTypeDef",
-    {
-        "quantumTaskArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-S3DataSourceOutputTypeDef = TypedDict(
-    "S3DataSourceOutputTypeDef",
-    {
-        "s3Uri": str,
-    },
-)
-
 S3DataSourceTypeDef = TypedDict(
     "S3DataSourceTypeDef",
     {
         "s3Uri": str,
     },
 )
 
-DeviceConfigOutputTypeDef = TypedDict(
-    "DeviceConfigOutputTypeDef",
-    {
-        "device": str,
-    },
-)
-
 DeviceSummaryTypeDef = TypedDict(
     "DeviceSummaryTypeDef",
     {
         "deviceArn": str,
         "deviceName": str,
         "deviceStatus": DeviceStatusType,
         "deviceType": DeviceTypeType,
@@ -327,136 +252,38 @@
 GetDeviceRequestRequestTypeDef = TypedDict(
     "GetDeviceRequestRequestTypeDef",
     {
         "deviceArn": str,
     },
 )
 
-GetDeviceResponseTypeDef = TypedDict(
-    "GetDeviceResponseTypeDef",
-    {
-        "deviceArn": str,
-        "deviceCapabilities": str,
-        "deviceName": str,
-        "deviceStatus": DeviceStatusType,
-        "deviceType": DeviceTypeType,
-        "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetJobRequestRequestTypeDef = TypedDict(
     "GetJobRequestRequestTypeDef",
     {
         "jobArn": str,
     },
 )
 
-_RequiredInstanceConfigOutputTypeDef = TypedDict(
-    "_RequiredInstanceConfigOutputTypeDef",
-    {
-        "instanceType": InstanceTypeType,
-        "volumeSizeInGb": int,
-    },
-)
-_OptionalInstanceConfigOutputTypeDef = TypedDict(
-    "_OptionalInstanceConfigOutputTypeDef",
-    {
-        "instanceCount": int,
-    },
-    total=False,
-)
-
-class InstanceConfigOutputTypeDef(
-    _RequiredInstanceConfigOutputTypeDef, _OptionalInstanceConfigOutputTypeDef
-):
-    pass
-
-_RequiredJobCheckpointConfigOutputTypeDef = TypedDict(
-    "_RequiredJobCheckpointConfigOutputTypeDef",
-    {
-        "s3Uri": str,
-    },
-)
-_OptionalJobCheckpointConfigOutputTypeDef = TypedDict(
-    "_OptionalJobCheckpointConfigOutputTypeDef",
-    {
-        "localPath": str,
-    },
-    total=False,
-)
-
-class JobCheckpointConfigOutputTypeDef(
-    _RequiredJobCheckpointConfigOutputTypeDef, _OptionalJobCheckpointConfigOutputTypeDef
-):
-    pass
-
 JobEventDetailsTypeDef = TypedDict(
     "JobEventDetailsTypeDef",
     {
         "eventType": JobEventTypeType,
         "message": str,
         "timeOfEvent": datetime,
     },
     total=False,
 )
 
-_RequiredJobOutputDataConfigOutputTypeDef = TypedDict(
-    "_RequiredJobOutputDataConfigOutputTypeDef",
-    {
-        "s3Path": str,
-    },
-)
-_OptionalJobOutputDataConfigOutputTypeDef = TypedDict(
-    "_OptionalJobOutputDataConfigOutputTypeDef",
-    {
-        "kmsKeyId": str,
-    },
-    total=False,
-)
-
-class JobOutputDataConfigOutputTypeDef(
-    _RequiredJobOutputDataConfigOutputTypeDef, _OptionalJobOutputDataConfigOutputTypeDef
-):
-    pass
-
-JobStoppingConditionOutputTypeDef = TypedDict(
-    "JobStoppingConditionOutputTypeDef",
-    {
-        "maxRuntimeInSeconds": int,
-    },
-    total=False,
-)
-
 GetQuantumTaskRequestRequestTypeDef = TypedDict(
     "GetQuantumTaskRequestRequestTypeDef",
     {
         "quantumTaskArn": str,
     },
 )
 
-GetQuantumTaskResponseTypeDef = TypedDict(
-    "GetQuantumTaskResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "deviceArn": str,
-        "deviceParameters": str,
-        "endedAt": datetime,
-        "failureReason": str,
-        "jobArn": str,
-        "outputS3Bucket": str,
-        "outputS3Directory": str,
-        "quantumTaskArn": str,
-        "shots": int,
-        "status": QuantumTaskStatusType,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredJobSummaryTypeDef = TypedDict(
     "_RequiredJobSummaryTypeDef",
     {
         "createdAt": datetime,
         "device": str,
         "jobArn": str,
         "jobName": str,
@@ -479,22 +306,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -523,25 +342,14 @@
 )
 
 class QuantumTaskSummaryTypeDef(
     _RequiredQuantumTaskSummaryTypeDef, _OptionalQuantumTaskSummaryTypeDef
 ):
     pass
 
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
 SearchDevicesFilterTypeDef = TypedDict(
     "SearchDevicesFilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
 )
@@ -576,36 +384,94 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-AlgorithmSpecificationOutputTypeDef = TypedDict(
-    "AlgorithmSpecificationOutputTypeDef",
-    {
-        "containerImage": ContainerImageOutputTypeDef,
-        "scriptModeConfig": ScriptModeConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 AlgorithmSpecificationTypeDef = TypedDict(
     "AlgorithmSpecificationTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
         "scriptModeConfig": ScriptModeConfigTypeDef,
     },
     total=False,
 )
 
-DataSourceOutputTypeDef = TypedDict(
-    "DataSourceOutputTypeDef",
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "jobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelQuantumTaskResponseTypeDef = TypedDict(
+    "CancelQuantumTaskResponseTypeDef",
+    {
+        "cancellationStatus": CancellationStatusType,
+        "quantumTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateQuantumTaskResponseTypeDef = TypedDict(
+    "CreateQuantumTaskResponseTypeDef",
+    {
+        "quantumTaskArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeviceResponseTypeDef = TypedDict(
+    "GetDeviceResponseTypeDef",
+    {
+        "deviceArn": str,
+        "deviceCapabilities": str,
+        "deviceName": str,
+        "deviceStatus": DeviceStatusType,
+        "deviceType": DeviceTypeType,
+        "providerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetQuantumTaskResponseTypeDef = TypedDict(
+    "GetQuantumTaskResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "deviceArn": str,
+        "deviceParameters": str,
+        "endedAt": datetime,
+        "failureReason": str,
+        "jobArn": str,
+        "outputS3Bucket": str,
+        "outputS3Directory": str,
+        "quantumTaskArn": str,
+        "shots": int,
+        "status": QuantumTaskStatusType,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "s3DataSource": S3DataSourceOutputTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "s3DataSource": S3DataSourceTypeDef,
@@ -613,33 +479,33 @@
 )
 
 SearchDevicesResponseTypeDef = TypedDict(
     "SearchDevicesResponseTypeDef",
     {
         "devices": List[DeviceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchJobsResponseTypeDef = TypedDict(
     "SearchJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchQuantumTasksResponseTypeDef = TypedDict(
     "SearchQuantumTasksResponseTypeDef",
     {
         "nextToken": str,
         "quantumTasks": List[QuantumTaskSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchDevicesRequestRequestTypeDef",
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
@@ -664,15 +530,15 @@
     {
         "filters": Sequence[SearchDevicesFilterTypeDef],
     },
 )
 _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef = TypedDict(
     "_OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchDevicesRequestSearchDevicesPaginateTypeDef(
     _RequiredSearchDevicesRequestSearchDevicesPaginateTypeDef,
     _OptionalSearchDevicesRequestSearchDevicesPaginateTypeDef,
@@ -704,15 +570,15 @@
     {
         "filters": Sequence[SearchJobsFilterTypeDef],
     },
 )
 _OptionalSearchJobsRequestSearchJobsPaginateTypeDef = TypedDict(
     "_OptionalSearchJobsRequestSearchJobsPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchJobsRequestSearchJobsPaginateTypeDef(
     _RequiredSearchJobsRequestSearchJobsPaginateTypeDef,
     _OptionalSearchJobsRequestSearchJobsPaginateTypeDef,
@@ -745,45 +611,25 @@
     {
         "filters": Sequence[SearchQuantumTasksFilterTypeDef],
     },
 )
 _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef = TypedDict(
     "_OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef(
     _RequiredSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
     _OptionalSearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
 ):
     pass
 
-_RequiredInputFileConfigOutputTypeDef = TypedDict(
-    "_RequiredInputFileConfigOutputTypeDef",
-    {
-        "channelName": str,
-        "dataSource": DataSourceOutputTypeDef,
-    },
-)
-_OptionalInputFileConfigOutputTypeDef = TypedDict(
-    "_OptionalInputFileConfigOutputTypeDef",
-    {
-        "contentType": str,
-    },
-    total=False,
-)
-
-class InputFileConfigOutputTypeDef(
-    _RequiredInputFileConfigOutputTypeDef, _OptionalInputFileConfigOutputTypeDef
-):
-    pass
-
 _RequiredInputFileConfigTypeDef = TypedDict(
     "_RequiredInputFileConfigTypeDef",
     {
         "channelName": str,
         "dataSource": DataSourceTypeDef,
     },
 )
@@ -794,40 +640,14 @@
     },
     total=False,
 )
 
 class InputFileConfigTypeDef(_RequiredInputFileConfigTypeDef, _OptionalInputFileConfigTypeDef):
     pass
 
-GetJobResponseTypeDef = TypedDict(
-    "GetJobResponseTypeDef",
-    {
-        "algorithmSpecification": AlgorithmSpecificationOutputTypeDef,
-        "billableDuration": int,
-        "checkpointConfig": JobCheckpointConfigOutputTypeDef,
-        "createdAt": datetime,
-        "deviceConfig": DeviceConfigOutputTypeDef,
-        "endedAt": datetime,
-        "events": List[JobEventDetailsTypeDef],
-        "failureReason": str,
-        "hyperParameters": Dict[str, str],
-        "inputDataConfig": List[InputFileConfigOutputTypeDef],
-        "instanceConfig": InstanceConfigOutputTypeDef,
-        "jobArn": str,
-        "jobName": str,
-        "outputDataConfig": JobOutputDataConfigOutputTypeDef,
-        "roleArn": str,
-        "startedAt": datetime,
-        "status": JobPrimaryStatusType,
-        "stoppingCondition": JobStoppingConditionOutputTypeDef,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "algorithmSpecification": AlgorithmSpecificationTypeDef,
         "clientToken": str,
         "deviceConfig": DeviceConfigTypeDef,
         "instanceConfig": InstanceConfigTypeDef,
@@ -848,7 +668,33 @@
     total=False,
 )
 
 class CreateJobRequestRequestTypeDef(
     _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
 ):
     pass
+
+GetJobResponseTypeDef = TypedDict(
+    "GetJobResponseTypeDef",
+    {
+        "algorithmSpecification": AlgorithmSpecificationTypeDef,
+        "billableDuration": int,
+        "checkpointConfig": JobCheckpointConfigTypeDef,
+        "createdAt": datetime,
+        "deviceConfig": DeviceConfigTypeDef,
+        "endedAt": datetime,
+        "events": List[JobEventDetailsTypeDef],
+        "failureReason": str,
+        "hyperParameters": Dict[str, str],
+        "inputDataConfig": List[InputFileConfigTypeDef],
+        "instanceConfig": InstanceConfigTypeDef,
+        "jobArn": str,
+        "jobName": str,
+        "outputDataConfig": JobOutputDataConfigTypeDef,
+        "roleArn": str,
+        "startedAt": datetime,
+        "status": JobPrimaryStatusType,
+        "stoppingCondition": JobStoppingConditionTypeDef,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/PKG-INFO` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-braket
-Version: 1.28.12
-Summary: Type annotations for boto3.Braket 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Braket 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-braket.svg?color=blue)](https://pypi.org/project/mypy-boto3-braket)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-braket)](https://pepy.tech/project/mypy-boto3-braket)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Braket 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
+[boto3.Braket 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/braket.html#Braket)
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
 [mypy-boto3-braket docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_braket/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,76 +338,65 @@
 ### Typed dictionaries
 
 `mypy_boto3_braket.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_braket.type_defs import (
-    ContainerImageOutputTypeDef,
-    ScriptModeConfigOutputTypeDef,
     ContainerImageTypeDef,
     ScriptModeConfigTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     CancelQuantumTaskRequestRequestTypeDef,
-    CancelQuantumTaskResponseTypeDef,
     DeviceConfigTypeDef,
     InstanceConfigTypeDef,
     JobCheckpointConfigTypeDef,
     JobOutputDataConfigTypeDef,
     JobStoppingConditionTypeDef,
-    CreateJobResponseTypeDef,
     CreateQuantumTaskRequestRequestTypeDef,
-    CreateQuantumTaskResponseTypeDef,
-    S3DataSourceOutputTypeDef,
     S3DataSourceTypeDef,
-    DeviceConfigOutputTypeDef,
     DeviceSummaryTypeDef,
     GetDeviceRequestRequestTypeDef,
-    GetDeviceResponseTypeDef,
     GetJobRequestRequestTypeDef,
-    InstanceConfigOutputTypeDef,
-    JobCheckpointConfigOutputTypeDef,
     JobEventDetailsTypeDef,
-    JobOutputDataConfigOutputTypeDef,
-    JobStoppingConditionOutputTypeDef,
     GetQuantumTaskRequestRequestTypeDef,
-    GetQuantumTaskResponseTypeDef,
     JobSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     QuantumTaskSummaryTypeDef,
-    ResponseMetadataTypeDef,
     SearchDevicesFilterTypeDef,
     SearchJobsFilterTypeDef,
     SearchQuantumTasksFilterTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    AlgorithmSpecificationOutputTypeDef,
     AlgorithmSpecificationTypeDef,
-    DataSourceOutputTypeDef,
+    CancelJobResponseTypeDef,
+    CancelQuantumTaskResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateQuantumTaskResponseTypeDef,
+    GetDeviceResponseTypeDef,
+    GetQuantumTaskResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     DataSourceTypeDef,
     SearchDevicesResponseTypeDef,
     SearchJobsResponseTypeDef,
     SearchQuantumTasksResponseTypeDef,
     SearchDevicesRequestRequestTypeDef,
     SearchDevicesRequestSearchDevicesPaginateTypeDef,
     SearchJobsRequestRequestTypeDef,
     SearchJobsRequestSearchJobsPaginateTypeDef,
     SearchQuantumTasksRequestRequestTypeDef,
     SearchQuantumTasksRequestSearchQuantumTasksPaginateTypeDef,
-    InputFileConfigOutputTypeDef,
     InputFileConfigTypeDef,
-    GetJobResponseTypeDef,
     CreateJobRequestRequestTypeDef,
+    GetJobResponseTypeDef,
 )
 
 
-def get_structure() -> ContainerImageOutputTypeDef:
+def get_structure() -> ContainerImageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-braket-1.28.12/mypy_boto3_braket.egg-info/SOURCES.txt` & `mypy-boto3-braket-1.28.15/mypy_boto3_braket.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-braket-1.28.12/setup.py` & `mypy-boto3-braket-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-braket",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_braket"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Braket 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Braket 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

