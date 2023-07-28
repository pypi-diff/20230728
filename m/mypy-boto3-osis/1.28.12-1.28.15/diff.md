# Comparing `tmp/mypy-boto3-osis-1.28.12.tar.gz` & `tmp/mypy-boto3-osis-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-osis-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
+gzip compressed data, was "mypy-boto3-osis-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
```

## Comparing `mypy-boto3-osis-1.28.12.tar` & `mypy-boto3-osis-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-osis-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-27 11:49:21.793132 mypy-boto3-osis-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11876 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.785132 mypy-boto3-osis-1.28.12/mypy_boto3_osis/
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-07-27 11:41:08.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.793132 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 11:49:21.000000 mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.793132 mypy-boto3-osis-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-27 11:41:07.000000 mypy-boto3-osis-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.925606 mypy-boto3-osis-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-28 20:43:24.921606 mypy-boto3-osis-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.921606 mypy-boto3-osis-1.28.15/mypy_boto3_osis/
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11080 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8344 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10908 2023-07-28 20:33:07.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10899 2023-07-28 20:33:07.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.921606 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:24.000000 mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.925606 mypy-boto3-osis-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 20:33:06.000000 mypy-boto3-osis-1.28.15/setup.py
```

### Comparing `mypy-boto3-osis-1.28.12/LICENSE` & `mypy-boto3-osis-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.12/PKG-INFO` & `mypy-boto3-osis-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.28.12
-Summary: Type annotations for boto3.OpenSearchIngestion 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,42 +299,39 @@
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
-    CloudWatchLogDestinationOutputTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
     ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PipelineStatusReasonTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
     VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
-    LogPublishingOptionsOutputTypeDef,
     LogPublishingOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     VpcEndpointTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
```

### Comparing `mypy-boto3-osis-1.28.12/README.md` & `mypy-boto3-osis-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,42 +267,39 @@
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
-    CloudWatchLogDestinationOutputTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
     ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PipelineStatusReasonTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
     VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
-    LogPublishingOptionsOutputTypeDef,
     LogPublishingOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     VpcEndpointTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
```

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis/__main__.py` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchIngestion 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.OpenSearchIngestion 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion\nOther"
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

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis/client.py` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis/client.pyi` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis/literals.py` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis/literals.pyi` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis/type_defs.py` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,42 +25,39 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ChangeProgressStageTypeDef",
-    "CloudWatchLogDestinationOutputTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
     "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "GetPipelineBlueprintRequestRequestTypeDef",
     "PipelineBlueprintTypeDef",
     "GetPipelineChangeProgressRequestRequestTypeDef",
     "GetPipelineRequestRequestTypeDef",
     "PipelineBlueprintSummaryTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "PipelineStatusReasonTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
     "VpcOptionsOutputTypeDef",
     "ChangeProgressStatusTypeDef",
-    "LogPublishingOptionsOutputTypeDef",
     "LogPublishingOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
     "VpcEndpointTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
@@ -79,21 +76,14 @@
         "Status": ChangeProgressStageStatusesType,
         "Description": str,
         "LastUpdatedAt": datetime,
     },
     total=False,
 )
 
-CloudWatchLogDestinationOutputTypeDef = TypedDict(
-    "CloudWatchLogDestinationOutputTypeDef",
-    {
-        "LogGroup": str,
-    },
-)
-
 CloudWatchLogDestinationTypeDef = TypedDict(
     "CloudWatchLogDestinationTypeDef",
     {
         "LogGroup": str,
     },
 )
 
@@ -192,22 +182,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PipelineStatusReasonTypeDef = TypedDict(
     "PipelineStatusReasonTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
@@ -275,23 +257,14 @@
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
     },
     total=False,
 )
 
-LogPublishingOptionsOutputTypeDef = TypedDict(
-    "LogPublishingOptionsOutputTypeDef",
-    {
-        "IsLoggingEnabled": bool,
-        "CloudWatchLogDestination": CloudWatchLogDestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 LogPublishingOptionsTypeDef = TypedDict(
     "LogPublishingOptionsTypeDef",
     {
         "IsLoggingEnabled": bool,
         "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
     },
     total=False,
@@ -301,14 +274,22 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetPipelineBlueprintResponseTypeDef = TypedDict(
     "GetPipelineBlueprintResponseTypeDef",
     {
         "Blueprint": PipelineBlueprintTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -317,22 +298,14 @@
     "ListPipelineBlueprintsResponseTypeDef",
     {
         "Blueprints": List[PipelineBlueprintSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PipelineSummaryTypeDef = TypedDict(
     "PipelineSummaryTypeDef",
     {
         "Status": PipelineStatusType,
         "StatusReason": PipelineStatusReasonTypeDef,
         "PipelineName": str,
         "PipelineArn": str,
@@ -439,15 +412,15 @@
         "MaxUnits": int,
         "Status": PipelineStatusType,
         "StatusReason": PipelineStatusReasonTypeDef,
         "PipelineConfigurationBody": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "IngestEndpointUrls": List[str],
-        "LogPublishingOptions": LogPublishingOptionsOutputTypeDef,
+        "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcEndpoints": List[VpcEndpointTypeDef],
     },
     total=False,
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
```

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis/type_defs.pyi` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -24,42 +24,39 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ChangeProgressStageTypeDef",
-    "CloudWatchLogDestinationOutputTypeDef",
     "CloudWatchLogDestinationTypeDef",
     "TagTypeDef",
     "VpcOptionsTypeDef",
     "ResponseMetadataTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "GetPipelineBlueprintRequestRequestTypeDef",
     "PipelineBlueprintTypeDef",
     "GetPipelineChangeProgressRequestRequestTypeDef",
     "GetPipelineRequestRequestTypeDef",
     "PipelineBlueprintSummaryTypeDef",
     "ListPipelinesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "PipelineStatusReasonTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
     "VpcOptionsOutputTypeDef",
     "ChangeProgressStatusTypeDef",
-    "LogPublishingOptionsOutputTypeDef",
     "LogPublishingOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
     "VpcEndpointTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
     "ListPipelinesResponseTypeDef",
@@ -78,21 +75,14 @@
         "Status": ChangeProgressStageStatusesType,
         "Description": str,
         "LastUpdatedAt": datetime,
     },
     total=False,
 )
 
-CloudWatchLogDestinationOutputTypeDef = TypedDict(
-    "CloudWatchLogDestinationOutputTypeDef",
-    {
-        "LogGroup": str,
-    },
-)
-
 CloudWatchLogDestinationTypeDef = TypedDict(
     "CloudWatchLogDestinationTypeDef",
     {
         "LogGroup": str,
     },
 )
 
@@ -189,22 +179,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PipelineStatusReasonTypeDef = TypedDict(
     "PipelineStatusReasonTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
@@ -270,23 +252,14 @@
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
     },
     total=False,
 )
 
-LogPublishingOptionsOutputTypeDef = TypedDict(
-    "LogPublishingOptionsOutputTypeDef",
-    {
-        "IsLoggingEnabled": bool,
-        "CloudWatchLogDestination": CloudWatchLogDestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 LogPublishingOptionsTypeDef = TypedDict(
     "LogPublishingOptionsTypeDef",
     {
         "IsLoggingEnabled": bool,
         "CloudWatchLogDestination": CloudWatchLogDestinationTypeDef,
     },
     total=False,
@@ -296,14 +269,22 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetPipelineBlueprintResponseTypeDef = TypedDict(
     "GetPipelineBlueprintResponseTypeDef",
     {
         "Blueprint": PipelineBlueprintTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -312,22 +293,14 @@
     "ListPipelineBlueprintsResponseTypeDef",
     {
         "Blueprints": List[PipelineBlueprintSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PipelineSummaryTypeDef = TypedDict(
     "PipelineSummaryTypeDef",
     {
         "Status": PipelineStatusType,
         "StatusReason": PipelineStatusReasonTypeDef,
         "PipelineName": str,
         "PipelineArn": str,
@@ -430,15 +403,15 @@
         "MaxUnits": int,
         "Status": PipelineStatusType,
         "StatusReason": PipelineStatusReasonTypeDef,
         "PipelineConfigurationBody": str,
         "CreatedAt": datetime,
         "LastUpdatedAt": datetime,
         "IngestEndpointUrls": List[str],
-        "LogPublishingOptions": LogPublishingOptionsOutputTypeDef,
+        "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcEndpoints": List[VpcEndpointTypeDef],
     },
     total=False,
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
```

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/PKG-INFO` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-osis
-Version: 1.28.12
-Summary: Type annotations for boto3.OpenSearchIngestion 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-osis.svg?color=blue)](https://pypi.org/project/mypy-boto3-osis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-osis)](https://pepy.tech/project/mypy-boto3-osis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchIngestion 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
+[boto3.OpenSearchIngestion 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion)
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
 [mypy-boto3-osis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,42 +299,39 @@
 
 `mypy_boto3_osis.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_osis.type_defs import (
     ChangeProgressStageTypeDef,
-    CloudWatchLogDestinationOutputTypeDef,
     CloudWatchLogDestinationTypeDef,
     TagTypeDef,
     VpcOptionsTypeDef,
     ResponseMetadataTypeDef,
     DeletePipelineRequestRequestTypeDef,
     GetPipelineBlueprintRequestRequestTypeDef,
     PipelineBlueprintTypeDef,
     GetPipelineChangeProgressRequestRequestTypeDef,
     GetPipelineRequestRequestTypeDef,
     PipelineBlueprintSummaryTypeDef,
     ListPipelinesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     PipelineStatusReasonTypeDef,
     StartPipelineRequestRequestTypeDef,
     StopPipelineRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ValidatePipelineRequestRequestTypeDef,
     ValidationMessageTypeDef,
     VpcOptionsOutputTypeDef,
     ChangeProgressStatusTypeDef,
-    LogPublishingOptionsOutputTypeDef,
     LogPublishingOptionsTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     GetPipelineBlueprintResponseTypeDef,
     ListPipelineBlueprintsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     PipelineSummaryTypeDef,
     ValidatePipelineResponseTypeDef,
     VpcEndpointTypeDef,
     GetPipelineChangeProgressResponseTypeDef,
     CreatePipelineRequestRequestTypeDef,
     UpdatePipelineRequestRequestTypeDef,
     ListPipelinesResponseTypeDef,
```

### Comparing `mypy-boto3-osis-1.28.12/mypy_boto3_osis.egg-info/SOURCES.txt` & `mypy-boto3-osis-1.28.15/mypy_boto3_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-osis-1.28.12/setup.py` & `mypy-boto3-osis-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-osis",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchIngestion 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.OpenSearchIngestion 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

