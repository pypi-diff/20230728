# Comparing `tmp/mypy-boto3-datapipeline-1.28.12.tar.gz` & `tmp/mypy-boto3-datapipeline-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datapipeline-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
+gzip compressed data, was "mypy-boto3-datapipeline-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
```

## Comparing `mypy-boto3-datapipeline-1.28.12.tar` & `mypy-boto3-datapipeline-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.608536 mypy-boto3-datapipeline-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-27 05:34:33.608536 mypy-boto3-datapipeline-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.604536 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19268 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19234 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:00.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.608536 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15113 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:33.000000 mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.608536 mypy-boto3-datapipeline-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:19:59.000000 mypy-boto3-datapipeline-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.572955 mypy-boto3-datapipeline-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-07-28 20:42:37.560954 mypy-boto3-datapipeline-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.552954 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16552 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-28 20:22:36.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18314 2023-07-28 20:22:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18282 2023-07-28 20:22:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.560954 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:37.000000 mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.572955 mypy-boto3-datapipeline-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:22:35.000000 mypy-boto3-datapipeline-1.28.15/setup.py
```

### Comparing `mypy-boto3-datapipeline-1.28.12/LICENSE` & `mypy-boto3-datapipeline-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.12/PKG-INFO` & `mypy-boto3-datapipeline-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.28.12
-Summary: Type annotations for boto3.DataPipeline 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,67 +331,63 @@
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
     TagTypeDef,
-    CreatePipelineOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    FieldOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
-    ParameterValueOutputTypeDef,
     InstanceIdentityTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
-    PaginatorConfigTypeDef,
-    ParameterAttributeOutputTypeDef,
     ParameterAttributeTypeDef,
-    TagOutputTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
-    QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
+    CreatePipelineOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EvaluateExpressionOutputTypeDef,
+    QueryObjectsOutputTypeDef,
+    ReportTaskProgressOutputTypeDef,
+    ReportTaskRunnerHeartbeatOutputTypeDef,
+    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    PipelineDescriptionTypeDef,
     PipelineObjectOutputTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
     ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
-    PipelineDescriptionTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
+    DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     PutPipelineDefinitionInputRequestTypeDef,
     ValidatePipelineDefinitionInputRequestTypeDef,
-    DescribePipelinesOutputTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
 )
 
 
 def get_structure() -> ParameterValueTypeDef:
```

### Comparing `mypy-boto3-datapipeline-1.28.12/README.md` & `mypy-boto3-datapipeline-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,67 +299,63 @@
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
     TagTypeDef,
-    CreatePipelineOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    FieldOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
-    ParameterValueOutputTypeDef,
     InstanceIdentityTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
-    PaginatorConfigTypeDef,
-    ParameterAttributeOutputTypeDef,
     ParameterAttributeTypeDef,
-    TagOutputTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
-    QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
+    CreatePipelineOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EvaluateExpressionOutputTypeDef,
+    QueryObjectsOutputTypeDef,
+    ReportTaskProgressOutputTypeDef,
+    ReportTaskRunnerHeartbeatOutputTypeDef,
+    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    PipelineDescriptionTypeDef,
     PipelineObjectOutputTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
     ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
-    PipelineDescriptionTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
+    DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     PutPipelineDefinitionInputRequestTypeDef,
     ValidatePipelineDefinitionInputRequestTypeDef,
-    DescribePipelinesOutputTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
 )
 
 
 def get_structure() -> ParameterValueTypeDef:
```

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__init__.py` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__init__.pyi` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/__main__.py` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataPipeline 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.DataPipeline 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline\nOther"
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

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/client.py` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/client.pyi` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/literals.py` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/literals.pyi` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/paginator.py` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,30 +56,30 @@
 
     def paginate(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#describeobjectspaginator)
         """
 
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#listpipelinespaginator)
         """
 
 
@@ -91,13 +91,13 @@
 
     def paginate(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#queryobjectspaginator)
         """
```

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/paginator.pyi` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,29 +53,29 @@
 
     def paginate(
         self,
         *,
         pipelineId: str,
         objectIds: Sequence[str],
         evaluateExpressions: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.DescribeObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#describeobjectspaginator)
         """
 
 class ListPipelinesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPipelinesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.ListPipelines.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#listpipelinespaginator)
         """
 
 class QueryObjectsPaginator(Paginator):
@@ -86,13 +86,13 @@
 
     def paginate(
         self,
         *,
         pipelineId: str,
         sphere: str,
         query: QueryTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryObjectsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline.Paginator.QueryObjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/paginators/#queryobjectspaginator)
         """
```

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/type_defs.py` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -18,71 +18,66 @@
 from .literals import OperatorTypeType, TaskStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ParameterValueTypeDef",
     "TagTypeDef",
-    "CreatePipelineOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
-    "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeObjectsInputRequestTypeDef",
     "DescribePipelinesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluateExpressionInputRequestTypeDef",
-    "EvaluateExpressionOutputTypeDef",
-    "FieldOutputTypeDef",
     "FieldTypeDef",
     "GetPipelineDefinitionInputRequestTypeDef",
-    "ParameterValueOutputTypeDef",
     "InstanceIdentityTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineIdNameTypeDef",
     "OperatorTypeDef",
-    "PaginatorConfigTypeDef",
-    "ParameterAttributeOutputTypeDef",
     "ParameterAttributeTypeDef",
-    "TagOutputTypeDef",
     "ValidationErrorTypeDef",
     "ValidationWarningTypeDef",
-    "QueryObjectsOutputTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "ReportTaskProgressOutputTypeDef",
     "ReportTaskRunnerHeartbeatInputRequestTypeDef",
-    "ReportTaskRunnerHeartbeatOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SetStatusInputRequestTypeDef",
     "SetTaskStatusInputRequestTypeDef",
     "ActivatePipelineInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreatePipelineInputRequestTypeDef",
+    "CreatePipelineOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EvaluateExpressionOutputTypeDef",
+    "QueryObjectsOutputTypeDef",
+    "ReportTaskProgressOutputTypeDef",
+    "ReportTaskRunnerHeartbeatOutputTypeDef",
+    "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    "PipelineDescriptionTypeDef",
     "PipelineObjectOutputTypeDef",
     "PipelineObjectTypeDef",
     "ReportTaskProgressInputRequestTypeDef",
     "PollForTaskInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "SelectorTypeDef",
     "ParameterObjectOutputTypeDef",
     "ParameterObjectTypeDef",
-    "PipelineDescriptionTypeDef",
     "PutPipelineDefinitionOutputTypeDef",
     "ValidatePipelineDefinitionOutputTypeDef",
+    "DescribePipelinesOutputTypeDef",
     "DescribeObjectsOutputTypeDef",
     "TaskObjectTypeDef",
     "QueryTypeDef",
     "GetPipelineDefinitionOutputTypeDef",
     "PutPipelineDefinitionInputRequestTypeDef",
     "ValidatePipelineDefinitionInputRequestTypeDef",
-    "DescribePipelinesOutputTypeDef",
     "PollForTaskOutputTypeDef",
     "QueryObjectsInputQueryObjectsPaginateTypeDef",
     "QueryObjectsInputRequestTypeDef",
 )
 
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
@@ -96,19 +91,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "pipelineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredDeactivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredDeactivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
@@ -118,52 +116,36 @@
     "_OptionalDeactivatePipelineInputRequestTypeDef",
     {
         "cancelActive": bool,
     },
     total=False,
 )
 
-
 class DeactivatePipelineInputRequestTypeDef(
     _RequiredDeactivatePipelineInputRequestTypeDef, _OptionalDeactivatePipelineInputRequestTypeDef
 ):
     pass
 
-
 DeletePipelineInputRequestTypeDef = TypedDict(
     "DeletePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 
-_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef",
-    {
-        "pipelineId": str,
-        "objectIds": Sequence[str],
-    },
-)
-_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "evaluateExpressions": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
-    _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeObjectsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
     },
 )
@@ -172,72 +154,35 @@
     {
         "evaluateExpressions": bool,
         "marker": str,
     },
     total=False,
 )
 
-
 class DescribeObjectsInputRequestTypeDef(
     _RequiredDescribeObjectsInputRequestTypeDef, _OptionalDescribeObjectsInputRequestTypeDef
 ):
     pass
 
-
 DescribePipelinesInputRequestTypeDef = TypedDict(
     "DescribePipelinesInputRequestTypeDef",
     {
         "pipelineIds": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluateExpressionInputRequestTypeDef = TypedDict(
     "EvaluateExpressionInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectId": str,
         "expression": str,
     },
 )
 
-EvaluateExpressionOutputTypeDef = TypedDict(
-    "EvaluateExpressionOutputTypeDef",
-    {
-        "evaluatedExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredFieldOutputTypeDef = TypedDict(
-    "_RequiredFieldOutputTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalFieldOutputTypeDef = TypedDict(
-    "_OptionalFieldOutputTypeDef",
-    {
-        "stringValue": str,
-        "refValue": str,
-    },
-    total=False,
-)
-
-
-class FieldOutputTypeDef(_RequiredFieldOutputTypeDef, _OptionalFieldOutputTypeDef):
-    pass
-
-
 _RequiredFieldTypeDef = TypedDict(
     "_RequiredFieldTypeDef",
     {
         "key": str,
     },
 )
 _OptionalFieldTypeDef = TypedDict(
@@ -245,66 +190,46 @@
     {
         "stringValue": str,
         "refValue": str,
     },
     total=False,
 )
 
-
 class FieldTypeDef(_RequiredFieldTypeDef, _OptionalFieldTypeDef):
     pass
 
-
 _RequiredGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredGetPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalGetPipelineDefinitionInputRequestTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
-
 class GetPipelineDefinitionInputRequestTypeDef(
     _RequiredGetPipelineDefinitionInputRequestTypeDef,
     _OptionalGetPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
-
-ParameterValueOutputTypeDef = TypedDict(
-    "ParameterValueOutputTypeDef",
-    {
-        "id": str,
-        "stringValue": str,
-    },
-)
-
 InstanceIdentityTypeDef = TypedDict(
     "InstanceIdentityTypeDef",
     {
         "document": str,
         "signature": str,
     },
     total=False,
 )
 
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "marker": str,
     },
     total=False,
 )
@@ -323,48 +248,22 @@
     {
         "type": OperatorTypeType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ParameterAttributeOutputTypeDef = TypedDict(
-    "ParameterAttributeOutputTypeDef",
-    {
-        "key": str,
-        "stringValue": str,
-    },
-)
-
 ParameterAttributeTypeDef = TypedDict(
     "ParameterAttributeTypeDef",
     {
         "key": str,
         "stringValue": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 ValidationErrorTypeDef = TypedDict(
     "ValidationErrorTypeDef",
     {
         "id": str,
         "errors": List[str],
     },
     total=False,
@@ -375,40 +274,22 @@
     {
         "id": str,
         "warnings": List[str],
     },
     total=False,
 )
 
-QueryObjectsOutputTypeDef = TypedDict(
-    "QueryObjectsOutputTypeDef",
-    {
-        "ids": List[str],
-        "marker": str,
-        "hasMoreResults": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsInputRequestTypeDef = TypedDict(
     "RemoveTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tagKeys": Sequence[str],
     },
 )
 
-ReportTaskProgressOutputTypeDef = TypedDict(
-    "ReportTaskProgressOutputTypeDef",
-    {
-        "canceled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredReportTaskRunnerHeartbeatInputRequestTypeDef",
     {
         "taskrunnerId": str,
     },
 )
 _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef = TypedDict(
@@ -416,41 +297,20 @@
     {
         "workerGroup": str,
         "hostname": str,
     },
     total=False,
 )
 
-
 class ReportTaskRunnerHeartbeatInputRequestTypeDef(
     _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef,
     _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef,
 ):
     pass
 
-
-ReportTaskRunnerHeartbeatOutputTypeDef = TypedDict(
-    "ReportTaskRunnerHeartbeatOutputTypeDef",
-    {
-        "terminate": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 SetStatusInputRequestTypeDef = TypedDict(
     "SetStatusInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
         "status": str,
     },
@@ -469,21 +329,19 @@
         "errorId": str,
         "errorMessage": str,
         "errorStackTrace": str,
     },
     total=False,
 )
 
-
 class SetTaskStatusInputRequestTypeDef(
     _RequiredSetTaskStatusInputRequestTypeDef, _OptionalSetTaskStatusInputRequestTypeDef
 ):
     pass
 
-
 _RequiredActivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredActivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalActivatePipelineInputRequestTypeDef = TypedDict(
@@ -491,21 +349,19 @@
     {
         "parameterValues": Sequence[ParameterValueTypeDef],
         "startTimestamp": Union[datetime, str],
     },
     total=False,
 )
 
-
 class ActivatePipelineInputRequestTypeDef(
     _RequiredActivatePipelineInputRequestTypeDef, _OptionalActivatePipelineInputRequestTypeDef
 ):
     pass
 
-
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -522,27 +378,126 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
+    {
+        "pipelineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EvaluateExpressionOutputTypeDef = TypedDict(
+    "EvaluateExpressionOutputTypeDef",
+    {
+        "evaluatedExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+QueryObjectsOutputTypeDef = TypedDict(
+    "QueryObjectsOutputTypeDef",
+    {
+        "ids": List[str],
+        "marker": str,
+        "hasMoreResults": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReportTaskProgressOutputTypeDef = TypedDict(
+    "ReportTaskProgressOutputTypeDef",
+    {
+        "canceled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReportTaskRunnerHeartbeatOutputTypeDef = TypedDict(
+    "ReportTaskRunnerHeartbeatOutputTypeDef",
+    {
+        "terminate": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    {
+        "pipelineId": str,
+        "objectIds": Sequence[str],
+    },
+)
+_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    {
+        "evaluateExpressions": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
+    _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
+):
+    pass
+
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredPipelineDescriptionTypeDef = TypedDict(
+    "_RequiredPipelineDescriptionTypeDef",
+    {
+        "pipelineId": str,
+        "name": str,
+        "fields": List[FieldTypeDef],
+    },
+)
+_OptionalPipelineDescriptionTypeDef = TypedDict(
+    "_OptionalPipelineDescriptionTypeDef",
+    {
+        "description": str,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+class PipelineDescriptionTypeDef(
+    _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
+):
+    pass
 
 PipelineObjectOutputTypeDef = TypedDict(
     "PipelineObjectOutputTypeDef",
     {
         "id": str,
         "name": str,
-        "fields": List[FieldOutputTypeDef],
+        "fields": List[FieldTypeDef],
     },
 )
 
 PipelineObjectTypeDef = TypedDict(
     "PipelineObjectTypeDef",
     {
         "id": str,
@@ -561,21 +516,19 @@
     "_OptionalReportTaskProgressInputRequestTypeDef",
     {
         "fields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
-
 class ReportTaskProgressInputRequestTypeDef(
     _RequiredReportTaskProgressInputRequestTypeDef, _OptionalReportTaskProgressInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPollForTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForTaskInputRequestTypeDef",
     {
         "workerGroup": str,
     },
 )
 _OptionalPollForTaskInputRequestTypeDef = TypedDict(
@@ -583,28 +536,26 @@
     {
         "hostname": str,
         "instanceIdentity": InstanceIdentityTypeDef,
     },
     total=False,
 )
 
-
 class PollForTaskInputRequestTypeDef(
     _RequiredPollForTaskInputRequestTypeDef, _OptionalPollForTaskInputRequestTypeDef
 ):
     pass
 
-
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelineIdList": List[PipelineIdNameTypeDef],
         "marker": str,
         "hasMoreResults": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SelectorTypeDef = TypedDict(
     "SelectorTypeDef",
     {
         "fieldName": str,
@@ -613,77 +564,61 @@
     total=False,
 )
 
 ParameterObjectOutputTypeDef = TypedDict(
     "ParameterObjectOutputTypeDef",
     {
         "id": str,
-        "attributes": List[ParameterAttributeOutputTypeDef],
+        "attributes": List[ParameterAttributeTypeDef],
     },
 )
 
 ParameterObjectTypeDef = TypedDict(
     "ParameterObjectTypeDef",
     {
         "id": str,
         "attributes": Sequence[ParameterAttributeTypeDef],
     },
 )
 
-_RequiredPipelineDescriptionTypeDef = TypedDict(
-    "_RequiredPipelineDescriptionTypeDef",
-    {
-        "pipelineId": str,
-        "name": str,
-        "fields": List[FieldOutputTypeDef],
-    },
-)
-_OptionalPipelineDescriptionTypeDef = TypedDict(
-    "_OptionalPipelineDescriptionTypeDef",
-    {
-        "description": str,
-        "tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class PipelineDescriptionTypeDef(
-    _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
-):
-    pass
-
-
 PutPipelineDefinitionOutputTypeDef = TypedDict(
     "PutPipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidatePipelineDefinitionOutputTypeDef = TypedDict(
     "ValidatePipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePipelinesOutputTypeDef = TypedDict(
+    "DescribePipelinesOutputTypeDef",
+    {
+        "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeObjectsOutputTypeDef = TypedDict(
     "DescribeObjectsOutputTypeDef",
     {
         "pipelineObjects": List[PipelineObjectOutputTypeDef],
         "marker": str,
         "hasMoreResults": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaskObjectTypeDef = TypedDict(
     "TaskObjectTypeDef",
     {
         "taskId": str,
@@ -703,16 +638,16 @@
 )
 
 GetPipelineDefinitionOutputTypeDef = TypedDict(
     "GetPipelineDefinitionOutputTypeDef",
     {
         "pipelineObjects": List[PipelineObjectOutputTypeDef],
         "parameterObjects": List[ParameterObjectOutputTypeDef],
-        "parameterValues": List[ParameterValueOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "parameterValues": List[ParameterValueTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredPutPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
@@ -724,22 +659,20 @@
     {
         "parameterObjects": Sequence[ParameterObjectTypeDef],
         "parameterValues": Sequence[ParameterValueTypeDef],
     },
     total=False,
 )
 
-
 class PutPipelineDefinitionInputRequestTypeDef(
     _RequiredPutPipelineDefinitionInputRequestTypeDef,
     _OptionalPutPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
         "pipelineObjects": Sequence[PipelineObjectTypeDef],
     },
 )
@@ -748,62 +681,50 @@
     {
         "parameterObjects": Sequence[ParameterObjectTypeDef],
         "parameterValues": Sequence[ParameterValueTypeDef],
     },
     total=False,
 )
 
-
 class ValidatePipelineDefinitionInputRequestTypeDef(
     _RequiredValidatePipelineDefinitionInputRequestTypeDef,
     _OptionalValidatePipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
-
-DescribePipelinesOutputTypeDef = TypedDict(
-    "DescribePipelinesOutputTypeDef",
-    {
-        "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef = TypedDict(
     "_RequiredQueryObjectsInputQueryObjectsPaginateTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
 _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef = TypedDict(
     "_OptionalQueryObjectsInputQueryObjectsPaginateTypeDef",
     {
         "query": QueryTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class QueryObjectsInputQueryObjectsPaginateTypeDef(
     _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef,
     _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredQueryObjectsInputRequestTypeDef = TypedDict(
     "_RequiredQueryObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
@@ -813,12 +734,11 @@
         "query": QueryTypeDef,
         "marker": str,
         "limit": int,
     },
     total=False,
 )
 
-
 class QueryObjectsInputRequestTypeDef(
     _RequiredQueryObjectsInputRequestTypeDef, _OptionalQueryObjectsInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline/type_defs.pyi` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,70 +18,67 @@
 from .literals import OperatorTypeType, TaskStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ParameterValueTypeDef",
     "TagTypeDef",
-    "CreatePipelineOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DeactivatePipelineInputRequestTypeDef",
     "DeletePipelineInputRequestTypeDef",
-    "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeObjectsInputRequestTypeDef",
     "DescribePipelinesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluateExpressionInputRequestTypeDef",
-    "EvaluateExpressionOutputTypeDef",
-    "FieldOutputTypeDef",
     "FieldTypeDef",
     "GetPipelineDefinitionInputRequestTypeDef",
-    "ParameterValueOutputTypeDef",
     "InstanceIdentityTypeDef",
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
     "ListPipelinesInputRequestTypeDef",
     "PipelineIdNameTypeDef",
     "OperatorTypeDef",
-    "PaginatorConfigTypeDef",
-    "ParameterAttributeOutputTypeDef",
     "ParameterAttributeTypeDef",
-    "TagOutputTypeDef",
     "ValidationErrorTypeDef",
     "ValidationWarningTypeDef",
-    "QueryObjectsOutputTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "ReportTaskProgressOutputTypeDef",
     "ReportTaskRunnerHeartbeatInputRequestTypeDef",
-    "ReportTaskRunnerHeartbeatOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SetStatusInputRequestTypeDef",
     "SetTaskStatusInputRequestTypeDef",
     "ActivatePipelineInputRequestTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreatePipelineInputRequestTypeDef",
+    "CreatePipelineOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "EvaluateExpressionOutputTypeDef",
+    "QueryObjectsOutputTypeDef",
+    "ReportTaskProgressOutputTypeDef",
+    "ReportTaskRunnerHeartbeatOutputTypeDef",
+    "DescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    "PipelineDescriptionTypeDef",
     "PipelineObjectOutputTypeDef",
     "PipelineObjectTypeDef",
     "ReportTaskProgressInputRequestTypeDef",
     "PollForTaskInputRequestTypeDef",
     "ListPipelinesOutputTypeDef",
     "SelectorTypeDef",
     "ParameterObjectOutputTypeDef",
     "ParameterObjectTypeDef",
-    "PipelineDescriptionTypeDef",
     "PutPipelineDefinitionOutputTypeDef",
     "ValidatePipelineDefinitionOutputTypeDef",
+    "DescribePipelinesOutputTypeDef",
     "DescribeObjectsOutputTypeDef",
     "TaskObjectTypeDef",
     "QueryTypeDef",
     "GetPipelineDefinitionOutputTypeDef",
     "PutPipelineDefinitionInputRequestTypeDef",
     "ValidatePipelineDefinitionInputRequestTypeDef",
-    "DescribePipelinesOutputTypeDef",
     "PollForTaskOutputTypeDef",
     "QueryObjectsInputQueryObjectsPaginateTypeDef",
     "QueryObjectsInputRequestTypeDef",
 )
 
 ParameterValueTypeDef = TypedDict(
     "ParameterValueTypeDef",
@@ -95,19 +92,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-CreatePipelineOutputTypeDef = TypedDict(
-    "CreatePipelineOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "pipelineId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredDeactivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredDeactivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
@@ -117,48 +117,38 @@
     "_OptionalDeactivatePipelineInputRequestTypeDef",
     {
         "cancelActive": bool,
     },
     total=False,
 )
 
+
 class DeactivatePipelineInputRequestTypeDef(
     _RequiredDeactivatePipelineInputRequestTypeDef, _OptionalDeactivatePipelineInputRequestTypeDef
 ):
     pass
 
+
 DeletePipelineInputRequestTypeDef = TypedDict(
     "DeletePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 
-_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef",
-    {
-        "pipelineId": str,
-        "objectIds": Sequence[str],
-    },
-)
-_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "evaluateExpressions": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
-    _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
-    _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeObjectsInputRequestTypeDef = TypedDict(
     "_RequiredDescribeObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
     },
 )
@@ -167,68 +157,37 @@
     {
         "evaluateExpressions": bool,
         "marker": str,
     },
     total=False,
 )
 
+
 class DescribeObjectsInputRequestTypeDef(
     _RequiredDescribeObjectsInputRequestTypeDef, _OptionalDescribeObjectsInputRequestTypeDef
 ):
     pass
 
+
 DescribePipelinesInputRequestTypeDef = TypedDict(
     "DescribePipelinesInputRequestTypeDef",
     {
         "pipelineIds": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluateExpressionInputRequestTypeDef = TypedDict(
     "EvaluateExpressionInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectId": str,
         "expression": str,
     },
 )
 
-EvaluateExpressionOutputTypeDef = TypedDict(
-    "EvaluateExpressionOutputTypeDef",
-    {
-        "evaluatedExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredFieldOutputTypeDef = TypedDict(
-    "_RequiredFieldOutputTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalFieldOutputTypeDef = TypedDict(
-    "_OptionalFieldOutputTypeDef",
-    {
-        "stringValue": str,
-        "refValue": str,
-    },
-    total=False,
-)
-
-class FieldOutputTypeDef(_RequiredFieldOutputTypeDef, _OptionalFieldOutputTypeDef):
-    pass
-
 _RequiredFieldTypeDef = TypedDict(
     "_RequiredFieldTypeDef",
     {
         "key": str,
     },
 )
 _OptionalFieldTypeDef = TypedDict(
@@ -236,62 +195,50 @@
     {
         "stringValue": str,
         "refValue": str,
     },
     total=False,
 )
 
+
 class FieldTypeDef(_RequiredFieldTypeDef, _OptionalFieldTypeDef):
     pass
 
+
 _RequiredGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredGetPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalGetPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_OptionalGetPipelineDefinitionInputRequestTypeDef",
     {
         "version": str,
     },
     total=False,
 )
 
+
 class GetPipelineDefinitionInputRequestTypeDef(
     _RequiredGetPipelineDefinitionInputRequestTypeDef,
     _OptionalGetPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
-ParameterValueOutputTypeDef = TypedDict(
-    "ParameterValueOutputTypeDef",
-    {
-        "id": str,
-        "stringValue": str,
-    },
-)
 
 InstanceIdentityTypeDef = TypedDict(
     "InstanceIdentityTypeDef",
     {
         "document": str,
         "signature": str,
     },
     total=False,
 )
 
-ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesInputListPipelinesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesInputRequestTypeDef = TypedDict(
     "ListPipelinesInputRequestTypeDef",
     {
         "marker": str,
     },
     total=False,
 )
@@ -310,48 +257,22 @@
     {
         "type": OperatorTypeType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
-ParameterAttributeOutputTypeDef = TypedDict(
-    "ParameterAttributeOutputTypeDef",
-    {
-        "key": str,
-        "stringValue": str,
-    },
-)
-
 ParameterAttributeTypeDef = TypedDict(
     "ParameterAttributeTypeDef",
     {
         "key": str,
         "stringValue": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 ValidationErrorTypeDef = TypedDict(
     "ValidationErrorTypeDef",
     {
         "id": str,
         "errors": List[str],
     },
     total=False,
@@ -362,40 +283,22 @@
     {
         "id": str,
         "warnings": List[str],
     },
     total=False,
 )
 
-QueryObjectsOutputTypeDef = TypedDict(
-    "QueryObjectsOutputTypeDef",
-    {
-        "ids": List[str],
-        "marker": str,
-        "hasMoreResults": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RemoveTagsInputRequestTypeDef = TypedDict(
     "RemoveTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tagKeys": Sequence[str],
     },
 )
 
-ReportTaskProgressOutputTypeDef = TypedDict(
-    "ReportTaskProgressOutputTypeDef",
-    {
-        "canceled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef = TypedDict(
     "_RequiredReportTaskRunnerHeartbeatInputRequestTypeDef",
     {
         "taskrunnerId": str,
     },
 )
 _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef = TypedDict(
@@ -403,38 +306,21 @@
     {
         "workerGroup": str,
         "hostname": str,
     },
     total=False,
 )
 
+
 class ReportTaskRunnerHeartbeatInputRequestTypeDef(
     _RequiredReportTaskRunnerHeartbeatInputRequestTypeDef,
     _OptionalReportTaskRunnerHeartbeatInputRequestTypeDef,
 ):
     pass
 
-ReportTaskRunnerHeartbeatOutputTypeDef = TypedDict(
-    "ReportTaskRunnerHeartbeatOutputTypeDef",
-    {
-        "terminate": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 
 SetStatusInputRequestTypeDef = TypedDict(
     "SetStatusInputRequestTypeDef",
     {
         "pipelineId": str,
         "objectIds": Sequence[str],
         "status": str,
@@ -454,19 +340,21 @@
         "errorId": str,
         "errorMessage": str,
         "errorStackTrace": str,
     },
     total=False,
 )
 
+
 class SetTaskStatusInputRequestTypeDef(
     _RequiredSetTaskStatusInputRequestTypeDef, _OptionalSetTaskStatusInputRequestTypeDef
 ):
     pass
 
+
 _RequiredActivatePipelineInputRequestTypeDef = TypedDict(
     "_RequiredActivatePipelineInputRequestTypeDef",
     {
         "pipelineId": str,
     },
 )
 _OptionalActivatePipelineInputRequestTypeDef = TypedDict(
@@ -474,19 +362,21 @@
     {
         "parameterValues": Sequence[ParameterValueTypeDef],
         "startTimestamp": Union[datetime, str],
     },
     total=False,
 )
 
+
 class ActivatePipelineInputRequestTypeDef(
     _RequiredActivatePipelineInputRequestTypeDef, _OptionalActivatePipelineInputRequestTypeDef
 ):
     pass
 
+
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "pipelineId": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -503,25 +393,132 @@
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreatePipelineInputRequestTypeDef(
     _RequiredCreatePipelineInputRequestTypeDef, _OptionalCreatePipelineInputRequestTypeDef
 ):
     pass
 
+
+CreatePipelineOutputTypeDef = TypedDict(
+    "CreatePipelineOutputTypeDef",
+    {
+        "pipelineId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EvaluateExpressionOutputTypeDef = TypedDict(
+    "EvaluateExpressionOutputTypeDef",
+    {
+        "evaluatedExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+QueryObjectsOutputTypeDef = TypedDict(
+    "QueryObjectsOutputTypeDef",
+    {
+        "ids": List[str],
+        "marker": str,
+        "hasMoreResults": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReportTaskProgressOutputTypeDef = TypedDict(
+    "ReportTaskProgressOutputTypeDef",
+    {
+        "canceled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ReportTaskRunnerHeartbeatOutputTypeDef = TypedDict(
+    "ReportTaskRunnerHeartbeatOutputTypeDef",
+    {
+        "terminate": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    {
+        "pipelineId": str,
+        "objectIds": Sequence[str],
+    },
+)
+_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef",
+    {
+        "evaluateExpressions": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeObjectsInputDescribeObjectsPaginateTypeDef(
+    _RequiredDescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    _OptionalDescribeObjectsInputDescribeObjectsPaginateTypeDef,
+):
+    pass
+
+
+ListPipelinesInputListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesInputListPipelinesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredPipelineDescriptionTypeDef = TypedDict(
+    "_RequiredPipelineDescriptionTypeDef",
+    {
+        "pipelineId": str,
+        "name": str,
+        "fields": List[FieldTypeDef],
+    },
+)
+_OptionalPipelineDescriptionTypeDef = TypedDict(
+    "_OptionalPipelineDescriptionTypeDef",
+    {
+        "description": str,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PipelineDescriptionTypeDef(
+    _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
+):
+    pass
+
+
 PipelineObjectOutputTypeDef = TypedDict(
     "PipelineObjectOutputTypeDef",
     {
         "id": str,
         "name": str,
-        "fields": List[FieldOutputTypeDef],
+        "fields": List[FieldTypeDef],
     },
 )
 
 PipelineObjectTypeDef = TypedDict(
     "PipelineObjectTypeDef",
     {
         "id": str,
@@ -540,19 +537,21 @@
     "_OptionalReportTaskProgressInputRequestTypeDef",
     {
         "fields": Sequence[FieldTypeDef],
     },
     total=False,
 )
 
+
 class ReportTaskProgressInputRequestTypeDef(
     _RequiredReportTaskProgressInputRequestTypeDef, _OptionalReportTaskProgressInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPollForTaskInputRequestTypeDef = TypedDict(
     "_RequiredPollForTaskInputRequestTypeDef",
     {
         "workerGroup": str,
     },
 )
 _OptionalPollForTaskInputRequestTypeDef = TypedDict(
@@ -560,26 +559,28 @@
     {
         "hostname": str,
         "instanceIdentity": InstanceIdentityTypeDef,
     },
     total=False,
 )
 
+
 class PollForTaskInputRequestTypeDef(
     _RequiredPollForTaskInputRequestTypeDef, _OptionalPollForTaskInputRequestTypeDef
 ):
     pass
 
+
 ListPipelinesOutputTypeDef = TypedDict(
     "ListPipelinesOutputTypeDef",
     {
         "pipelineIdList": List[PipelineIdNameTypeDef],
         "marker": str,
         "hasMoreResults": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SelectorTypeDef = TypedDict(
     "SelectorTypeDef",
     {
         "fieldName": str,
@@ -588,75 +589,61 @@
     total=False,
 )
 
 ParameterObjectOutputTypeDef = TypedDict(
     "ParameterObjectOutputTypeDef",
     {
         "id": str,
-        "attributes": List[ParameterAttributeOutputTypeDef],
+        "attributes": List[ParameterAttributeTypeDef],
     },
 )
 
 ParameterObjectTypeDef = TypedDict(
     "ParameterObjectTypeDef",
     {
         "id": str,
         "attributes": Sequence[ParameterAttributeTypeDef],
     },
 )
 
-_RequiredPipelineDescriptionTypeDef = TypedDict(
-    "_RequiredPipelineDescriptionTypeDef",
-    {
-        "pipelineId": str,
-        "name": str,
-        "fields": List[FieldOutputTypeDef],
-    },
-)
-_OptionalPipelineDescriptionTypeDef = TypedDict(
-    "_OptionalPipelineDescriptionTypeDef",
-    {
-        "description": str,
-        "tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-class PipelineDescriptionTypeDef(
-    _RequiredPipelineDescriptionTypeDef, _OptionalPipelineDescriptionTypeDef
-):
-    pass
-
 PutPipelineDefinitionOutputTypeDef = TypedDict(
     "PutPipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ValidatePipelineDefinitionOutputTypeDef = TypedDict(
     "ValidatePipelineDefinitionOutputTypeDef",
     {
         "validationErrors": List[ValidationErrorTypeDef],
         "validationWarnings": List[ValidationWarningTypeDef],
         "errored": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePipelinesOutputTypeDef = TypedDict(
+    "DescribePipelinesOutputTypeDef",
+    {
+        "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeObjectsOutputTypeDef = TypedDict(
     "DescribeObjectsOutputTypeDef",
     {
         "pipelineObjects": List[PipelineObjectOutputTypeDef],
         "marker": str,
         "hasMoreResults": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TaskObjectTypeDef = TypedDict(
     "TaskObjectTypeDef",
     {
         "taskId": str,
@@ -676,16 +663,16 @@
 )
 
 GetPipelineDefinitionOutputTypeDef = TypedDict(
     "GetPipelineDefinitionOutputTypeDef",
     {
         "pipelineObjects": List[PipelineObjectOutputTypeDef],
         "parameterObjects": List[ParameterObjectOutputTypeDef],
-        "parameterValues": List[ParameterValueOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "parameterValues": List[ParameterValueTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutPipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredPutPipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
@@ -697,20 +684,22 @@
     {
         "parameterObjects": Sequence[ParameterObjectTypeDef],
         "parameterValues": Sequence[ParameterValueTypeDef],
     },
     total=False,
 )
 
+
 class PutPipelineDefinitionInputRequestTypeDef(
     _RequiredPutPipelineDefinitionInputRequestTypeDef,
     _OptionalPutPipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredValidatePipelineDefinitionInputRequestTypeDef = TypedDict(
     "_RequiredValidatePipelineDefinitionInputRequestTypeDef",
     {
         "pipelineId": str,
         "pipelineObjects": Sequence[PipelineObjectTypeDef],
     },
 )
@@ -719,58 +708,54 @@
     {
         "parameterObjects": Sequence[ParameterObjectTypeDef],
         "parameterValues": Sequence[ParameterValueTypeDef],
     },
     total=False,
 )
 
+
 class ValidatePipelineDefinitionInputRequestTypeDef(
     _RequiredValidatePipelineDefinitionInputRequestTypeDef,
     _OptionalValidatePipelineDefinitionInputRequestTypeDef,
 ):
     pass
 
-DescribePipelinesOutputTypeDef = TypedDict(
-    "DescribePipelinesOutputTypeDef",
-    {
-        "pipelineDescriptionList": List[PipelineDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 PollForTaskOutputTypeDef = TypedDict(
     "PollForTaskOutputTypeDef",
     {
         "taskObject": TaskObjectTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef = TypedDict(
     "_RequiredQueryObjectsInputQueryObjectsPaginateTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
 _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef = TypedDict(
     "_OptionalQueryObjectsInputQueryObjectsPaginateTypeDef",
     {
         "query": QueryTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class QueryObjectsInputQueryObjectsPaginateTypeDef(
     _RequiredQueryObjectsInputQueryObjectsPaginateTypeDef,
     _OptionalQueryObjectsInputQueryObjectsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredQueryObjectsInputRequestTypeDef = TypedDict(
     "_RequiredQueryObjectsInputRequestTypeDef",
     {
         "pipelineId": str,
         "sphere": str,
     },
 )
@@ -780,11 +765,12 @@
         "query": QueryTypeDef,
         "marker": str,
         "limit": int,
     },
     total=False,
 )
 
+
 class QueryObjectsInputRequestTypeDef(
     _RequiredQueryObjectsInputRequestTypeDef, _OptionalQueryObjectsInputRequestTypeDef
 ):
     pass
```

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/PKG-INFO` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datapipeline
-Version: 1.28.12
-Summary: Type annotations for boto3.DataPipeline 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datapipeline.svg?color=blue)](https://pypi.org/project/mypy-boto3-datapipeline)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datapipeline)](https://pepy.tech/project/mypy-boto3-datapipeline)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataPipeline 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
+[boto3.DataPipeline 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datapipeline.html#DataPipeline)
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
 [mypy-boto3-datapipeline docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datapipeline/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,67 +331,63 @@
 `mypy_boto3_datapipeline.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_datapipeline.type_defs import (
     ParameterValueTypeDef,
     TagTypeDef,
-    CreatePipelineOutputTypeDef,
+    ResponseMetadataTypeDef,
     DeactivatePipelineInputRequestTypeDef,
     DeletePipelineInputRequestTypeDef,
-    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeObjectsInputRequestTypeDef,
     DescribePipelinesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluateExpressionInputRequestTypeDef,
-    EvaluateExpressionOutputTypeDef,
-    FieldOutputTypeDef,
     FieldTypeDef,
     GetPipelineDefinitionInputRequestTypeDef,
-    ParameterValueOutputTypeDef,
     InstanceIdentityTypeDef,
-    ListPipelinesInputListPipelinesPaginateTypeDef,
     ListPipelinesInputRequestTypeDef,
     PipelineIdNameTypeDef,
     OperatorTypeDef,
-    PaginatorConfigTypeDef,
-    ParameterAttributeOutputTypeDef,
     ParameterAttributeTypeDef,
-    TagOutputTypeDef,
     ValidationErrorTypeDef,
     ValidationWarningTypeDef,
-    QueryObjectsOutputTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ReportTaskProgressOutputTypeDef,
     ReportTaskRunnerHeartbeatInputRequestTypeDef,
-    ReportTaskRunnerHeartbeatOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetStatusInputRequestTypeDef,
     SetTaskStatusInputRequestTypeDef,
     ActivatePipelineInputRequestTypeDef,
     AddTagsInputRequestTypeDef,
     CreatePipelineInputRequestTypeDef,
+    CreatePipelineOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    EvaluateExpressionOutputTypeDef,
+    QueryObjectsOutputTypeDef,
+    ReportTaskProgressOutputTypeDef,
+    ReportTaskRunnerHeartbeatOutputTypeDef,
+    DescribeObjectsInputDescribeObjectsPaginateTypeDef,
+    ListPipelinesInputListPipelinesPaginateTypeDef,
+    PipelineDescriptionTypeDef,
     PipelineObjectOutputTypeDef,
     PipelineObjectTypeDef,
     ReportTaskProgressInputRequestTypeDef,
     PollForTaskInputRequestTypeDef,
     ListPipelinesOutputTypeDef,
     SelectorTypeDef,
     ParameterObjectOutputTypeDef,
     ParameterObjectTypeDef,
-    PipelineDescriptionTypeDef,
     PutPipelineDefinitionOutputTypeDef,
     ValidatePipelineDefinitionOutputTypeDef,
+    DescribePipelinesOutputTypeDef,
     DescribeObjectsOutputTypeDef,
     TaskObjectTypeDef,
     QueryTypeDef,
     GetPipelineDefinitionOutputTypeDef,
     PutPipelineDefinitionInputRequestTypeDef,
     ValidatePipelineDefinitionInputRequestTypeDef,
-    DescribePipelinesOutputTypeDef,
     PollForTaskOutputTypeDef,
     QueryObjectsInputQueryObjectsPaginateTypeDef,
     QueryObjectsInputRequestTypeDef,
 )
 
 
 def get_structure() -> ParameterValueTypeDef:
```

### Comparing `mypy-boto3-datapipeline-1.28.12/mypy_boto3_datapipeline.egg-info/SOURCES.txt` & `mypy-boto3-datapipeline-1.28.15/mypy_boto3_datapipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datapipeline-1.28.12/setup.py` & `mypy-boto3-datapipeline-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datapipeline",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_datapipeline"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DataPipeline 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.DataPipeline 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

