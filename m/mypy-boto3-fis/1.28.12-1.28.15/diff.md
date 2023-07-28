# Comparing `tmp/mypy-boto3-fis-1.28.12.tar.gz` & `tmp/mypy-boto3-fis-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fis-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
+gzip compressed data, was "mypy-boto3-fis-1.28.15.tar", last modified: Fri Jul 28 20:42:49 2023, max compression
```

## Comparing `mypy-boto3-fis-1.28.12.tar` & `mypy-boto3-fis-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.344508 mypy-boto3-fis-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-07-27 05:34:42.344508 mypy-boto3-fis-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.344508 mypy-boto3-fis-1.28.12/mypy_boto3_fis/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23899 2023-07-27 05:22:21.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23876 2023-07-27 05:22:20.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.344508 mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-07-27 05:34:42.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 05:34:42.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:42.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:42.000000 mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.344508 mypy-boto3-fis-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:22:19.000000 mypy-boto3-fis-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.701123 mypy-boto3-fis-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-07-28 20:42:49.701123 mypy-boto3-fis-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.689122 mypy-boto3-fis-1.28.15/mypy_boto3_fis/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-07-28 20:25:56.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-07-28 20:25:56.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23871 2023-07-28 20:25:56.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23848 2023-07-28 20:25:56.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.701123 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14477 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:49.000000 mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:49.701123 mypy-boto3-fis-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:25:55.000000 mypy-boto3-fis-1.28.15/setup.py
```

### Comparing `mypy-boto3-fis-1.28.12/LICENSE` & `mypy-boto3-fis-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.12/PKG-INFO` & `mypy-boto3-fis-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fis
-Version: 1.28.12
-Summary: Type annotations for boto3.FIS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fis)](https://pepy.tech/project/mypy-boto3-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FIS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[boto3.FIS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,14 +302,15 @@
 from mypy_boto3_fis.type_defs import (
     ActionParameterTypeDef,
     ActionTargetTypeDef,
     CreateExperimentTemplateActionInputTypeDef,
     ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
     ExperimentTemplateS3LogConfigurationInputTypeDef,
     CreateExperimentTemplateStopConditionInputTypeDef,
+    ResponseMetadataTypeDef,
     ExperimentTemplateTargetInputFilterTypeDef,
     DeleteExperimentTemplateRequestRequestTypeDef,
     ExperimentActionStateTypeDef,
     ExperimentCloudWatchLogsLogConfigurationTypeDef,
     ExperimentS3LogConfigurationTypeDef,
     ExperimentStateTypeDef,
     ExperimentStopConditionTypeDef,
@@ -324,29 +325,28 @@
     GetExperimentRequestRequestTypeDef,
     GetExperimentTemplateRequestRequestTypeDef,
     GetTargetResourceTypeRequestRequestTypeDef,
     ListActionsRequestRequestTypeDef,
     ListExperimentTemplatesRequestRequestTypeDef,
     ListExperimentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetResourceTypesRequestRequestTypeDef,
     TargetResourceTypeSummaryTypeDef,
-    ResponseMetadataTypeDef,
     StartExperimentRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetResourceTypeParameterTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExperimentTemplateActionInputItemTypeDef,
     UpdateExperimentTemplateStopConditionInputTypeDef,
     ActionSummaryTypeDef,
     ActionTypeDef,
     CreateExperimentTemplateLogConfigurationInputTypeDef,
     UpdateExperimentTemplateLogConfigurationInputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateExperimentTemplateTargetInputTypeDef,
     UpdateExperimentTemplateTargetInputTypeDef,
     ExperimentActionTypeDef,
     ExperimentLogConfigurationTypeDef,
     ExperimentSummaryTypeDef,
     ExperimentTargetTypeDef,
     ExperimentTemplateLogConfigurationTypeDef,
```

### Comparing `mypy-boto3-fis-1.28.12/README.md` & `mypy-boto3-fis-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fis)](https://pepy.tech/project/mypy-boto3-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FIS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[boto3.FIS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,14 +270,15 @@
 from mypy_boto3_fis.type_defs import (
     ActionParameterTypeDef,
     ActionTargetTypeDef,
     CreateExperimentTemplateActionInputTypeDef,
     ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
     ExperimentTemplateS3LogConfigurationInputTypeDef,
     CreateExperimentTemplateStopConditionInputTypeDef,
+    ResponseMetadataTypeDef,
     ExperimentTemplateTargetInputFilterTypeDef,
     DeleteExperimentTemplateRequestRequestTypeDef,
     ExperimentActionStateTypeDef,
     ExperimentCloudWatchLogsLogConfigurationTypeDef,
     ExperimentS3LogConfigurationTypeDef,
     ExperimentStateTypeDef,
     ExperimentStopConditionTypeDef,
@@ -292,29 +293,28 @@
     GetExperimentRequestRequestTypeDef,
     GetExperimentTemplateRequestRequestTypeDef,
     GetTargetResourceTypeRequestRequestTypeDef,
     ListActionsRequestRequestTypeDef,
     ListExperimentTemplatesRequestRequestTypeDef,
     ListExperimentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetResourceTypesRequestRequestTypeDef,
     TargetResourceTypeSummaryTypeDef,
-    ResponseMetadataTypeDef,
     StartExperimentRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetResourceTypeParameterTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExperimentTemplateActionInputItemTypeDef,
     UpdateExperimentTemplateStopConditionInputTypeDef,
     ActionSummaryTypeDef,
     ActionTypeDef,
     CreateExperimentTemplateLogConfigurationInputTypeDef,
     UpdateExperimentTemplateLogConfigurationInputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateExperimentTemplateTargetInputTypeDef,
     UpdateExperimentTemplateTargetInputTypeDef,
     ExperimentActionTypeDef,
     ExperimentLogConfigurationTypeDef,
     ExperimentSummaryTypeDef,
     ExperimentTargetTypeDef,
     ExperimentTemplateLogConfigurationTypeDef,
```

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis/__main__.py` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FIS 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.FIS 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS\nOther"
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

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis/client.py` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis/client.pyi` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis/literals.py` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis/literals.pyi` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis/type_defs.py` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 __all__ = (
     "ActionParameterTypeDef",
     "ActionTargetTypeDef",
     "CreateExperimentTemplateActionInputTypeDef",
     "ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef",
     "ExperimentTemplateS3LogConfigurationInputTypeDef",
     "CreateExperimentTemplateStopConditionInputTypeDef",
+    "ResponseMetadataTypeDef",
     "ExperimentTemplateTargetInputFilterTypeDef",
     "DeleteExperimentTemplateRequestRequestTypeDef",
     "ExperimentActionStateTypeDef",
     "ExperimentCloudWatchLogsLogConfigurationTypeDef",
     "ExperimentS3LogConfigurationTypeDef",
     "ExperimentStateTypeDef",
     "ExperimentStopConditionTypeDef",
@@ -48,29 +49,28 @@
     "GetExperimentRequestRequestTypeDef",
     "GetExperimentTemplateRequestRequestTypeDef",
     "GetTargetResourceTypeRequestRequestTypeDef",
     "ListActionsRequestRequestTypeDef",
     "ListExperimentTemplatesRequestRequestTypeDef",
     "ListExperimentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTargetResourceTypesRequestRequestTypeDef",
     "TargetResourceTypeSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "StartExperimentRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetResourceTypeParameterTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExperimentTemplateActionInputItemTypeDef",
     "UpdateExperimentTemplateStopConditionInputTypeDef",
     "ActionSummaryTypeDef",
     "ActionTypeDef",
     "CreateExperimentTemplateLogConfigurationInputTypeDef",
     "UpdateExperimentTemplateLogConfigurationInputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateExperimentTemplateTargetInputTypeDef",
     "UpdateExperimentTemplateTargetInputTypeDef",
     "ExperimentActionTypeDef",
     "ExperimentLogConfigurationTypeDef",
     "ExperimentSummaryTypeDef",
     "ExperimentTargetTypeDef",
     "ExperimentTemplateLogConfigurationTypeDef",
@@ -184,14 +184,25 @@
 class CreateExperimentTemplateStopConditionInputTypeDef(
     _RequiredCreateExperimentTemplateStopConditionInputTypeDef,
     _OptionalCreateExperimentTemplateStopConditionInputTypeDef,
 ):
     pass
 
 
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
 ExperimentTemplateTargetInputFilterTypeDef = TypedDict(
     "ExperimentTemplateTargetInputFilterTypeDef",
     {
         "path": str,
         "values": Sequence[str],
     },
 )
@@ -373,22 +384,14 @@
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
 ListTargetResourceTypesRequestRequestTypeDef = TypedDict(
     "ListTargetResourceTypesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -399,25 +402,14 @@
     {
         "resourceType": str,
         "description": str,
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
 _RequiredStartExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredStartExperimentRequestRequestTypeDef",
     {
         "clientToken": str,
         "experimentTemplateId": str,
     },
 )
@@ -567,14 +559,22 @@
         "cloudWatchLogsConfiguration": ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
         "s3Configuration": ExperimentTemplateS3LogConfigurationInputTypeDef,
         "logSchemaVersion": int,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateExperimentTemplateTargetInputTypeDef = TypedDict(
     "_RequiredCreateExperimentTemplateTargetInputTypeDef",
     {
         "resourceType": str,
         "selectionMode": str,
     },
 )
@@ -684,15 +684,15 @@
 )
 
 ListExperimentTemplatesResponseTypeDef = TypedDict(
     "ListExperimentTemplatesResponseTypeDef",
     {
         "experimentTemplates": List[ExperimentTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExperimentTemplateTargetTypeDef = TypedDict(
     "ExperimentTemplateTargetTypeDef",
     {
         "resourceType": str,
@@ -706,15 +706,15 @@
 )
 
 ListTargetResourceTypesResponseTypeDef = TypedDict(
     "ListTargetResourceTypesResponseTypeDef",
     {
         "targetResourceTypes": List[TargetResourceTypeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetResourceTypeTypeDef = TypedDict(
     "TargetResourceTypeTypeDef",
     {
         "resourceType": str,
@@ -725,23 +725,23 @@
 )
 
 ListActionsResponseTypeDef = TypedDict(
     "ListActionsResponseTypeDef",
     {
         "actions": List[ActionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetActionResponseTypeDef = TypedDict(
     "GetActionResponseTypeDef",
     {
         "action": ActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExperimentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentTemplateRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -797,15 +797,15 @@
 
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExperimentTypeDef = TypedDict(
     "ExperimentTypeDef",
     {
         "id": str,
@@ -841,66 +841,66 @@
     total=False,
 )
 
 GetTargetResourceTypeResponseTypeDef = TypedDict(
     "GetTargetResourceTypeResponseTypeDef",
     {
         "targetResourceType": TargetResourceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartExperimentResponseTypeDef = TypedDict(
     "StartExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopExperimentResponseTypeDef = TypedDict(
     "StopExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExperimentTemplateResponseTypeDef = TypedDict(
     "CreateExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteExperimentTemplateResponseTypeDef = TypedDict(
     "DeleteExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExperimentTemplateResponseTypeDef = TypedDict(
     "GetExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateExperimentTemplateResponseTypeDef = TypedDict(
     "UpdateExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis/type_defs.pyi` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 __all__ = (
     "ActionParameterTypeDef",
     "ActionTargetTypeDef",
     "CreateExperimentTemplateActionInputTypeDef",
     "ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef",
     "ExperimentTemplateS3LogConfigurationInputTypeDef",
     "CreateExperimentTemplateStopConditionInputTypeDef",
+    "ResponseMetadataTypeDef",
     "ExperimentTemplateTargetInputFilterTypeDef",
     "DeleteExperimentTemplateRequestRequestTypeDef",
     "ExperimentActionStateTypeDef",
     "ExperimentCloudWatchLogsLogConfigurationTypeDef",
     "ExperimentS3LogConfigurationTypeDef",
     "ExperimentStateTypeDef",
     "ExperimentStopConditionTypeDef",
@@ -47,29 +48,28 @@
     "GetExperimentRequestRequestTypeDef",
     "GetExperimentTemplateRequestRequestTypeDef",
     "GetTargetResourceTypeRequestRequestTypeDef",
     "ListActionsRequestRequestTypeDef",
     "ListExperimentTemplatesRequestRequestTypeDef",
     "ListExperimentsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTargetResourceTypesRequestRequestTypeDef",
     "TargetResourceTypeSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "StartExperimentRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TargetResourceTypeParameterTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateExperimentTemplateActionInputItemTypeDef",
     "UpdateExperimentTemplateStopConditionInputTypeDef",
     "ActionSummaryTypeDef",
     "ActionTypeDef",
     "CreateExperimentTemplateLogConfigurationInputTypeDef",
     "UpdateExperimentTemplateLogConfigurationInputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateExperimentTemplateTargetInputTypeDef",
     "UpdateExperimentTemplateTargetInputTypeDef",
     "ExperimentActionTypeDef",
     "ExperimentLogConfigurationTypeDef",
     "ExperimentSummaryTypeDef",
     "ExperimentTargetTypeDef",
     "ExperimentTemplateLogConfigurationTypeDef",
@@ -177,14 +177,25 @@
 
 class CreateExperimentTemplateStopConditionInputTypeDef(
     _RequiredCreateExperimentTemplateStopConditionInputTypeDef,
     _OptionalCreateExperimentTemplateStopConditionInputTypeDef,
 ):
     pass
 
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
 ExperimentTemplateTargetInputFilterTypeDef = TypedDict(
     "ExperimentTemplateTargetInputFilterTypeDef",
     {
         "path": str,
         "values": Sequence[str],
     },
 )
@@ -366,22 +377,14 @@
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
 ListTargetResourceTypesRequestRequestTypeDef = TypedDict(
     "ListTargetResourceTypesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -392,25 +395,14 @@
     {
         "resourceType": str,
         "description": str,
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
 _RequiredStartExperimentRequestRequestTypeDef = TypedDict(
     "_RequiredStartExperimentRequestRequestTypeDef",
     {
         "clientToken": str,
         "experimentTemplateId": str,
     },
 )
@@ -552,14 +544,22 @@
         "cloudWatchLogsConfiguration": ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
         "s3Configuration": ExperimentTemplateS3LogConfigurationInputTypeDef,
         "logSchemaVersion": int,
     },
     total=False,
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateExperimentTemplateTargetInputTypeDef = TypedDict(
     "_RequiredCreateExperimentTemplateTargetInputTypeDef",
     {
         "resourceType": str,
         "selectionMode": str,
     },
 )
@@ -665,15 +665,15 @@
 )
 
 ListExperimentTemplatesResponseTypeDef = TypedDict(
     "ListExperimentTemplatesResponseTypeDef",
     {
         "experimentTemplates": List[ExperimentTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExperimentTemplateTargetTypeDef = TypedDict(
     "ExperimentTemplateTargetTypeDef",
     {
         "resourceType": str,
@@ -687,15 +687,15 @@
 )
 
 ListTargetResourceTypesResponseTypeDef = TypedDict(
     "ListTargetResourceTypesResponseTypeDef",
     {
         "targetResourceTypes": List[TargetResourceTypeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetResourceTypeTypeDef = TypedDict(
     "TargetResourceTypeTypeDef",
     {
         "resourceType": str,
@@ -706,23 +706,23 @@
 )
 
 ListActionsResponseTypeDef = TypedDict(
     "ListActionsResponseTypeDef",
     {
         "actions": List[ActionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetActionResponseTypeDef = TypedDict(
     "GetActionResponseTypeDef",
     {
         "action": ActionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExperimentTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExperimentTemplateRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -774,15 +774,15 @@
     pass
 
 ListExperimentsResponseTypeDef = TypedDict(
     "ListExperimentsResponseTypeDef",
     {
         "experiments": List[ExperimentSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExperimentTypeDef = TypedDict(
     "ExperimentTypeDef",
     {
         "id": str,
@@ -818,66 +818,66 @@
     total=False,
 )
 
 GetTargetResourceTypeResponseTypeDef = TypedDict(
     "GetTargetResourceTypeResponseTypeDef",
     {
         "targetResourceType": TargetResourceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExperimentResponseTypeDef = TypedDict(
     "GetExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartExperimentResponseTypeDef = TypedDict(
     "StartExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopExperimentResponseTypeDef = TypedDict(
     "StopExperimentResponseTypeDef",
     {
         "experiment": ExperimentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateExperimentTemplateResponseTypeDef = TypedDict(
     "CreateExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteExperimentTemplateResponseTypeDef = TypedDict(
     "DeleteExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExperimentTemplateResponseTypeDef = TypedDict(
     "GetExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateExperimentTemplateResponseTypeDef = TypedDict(
     "UpdateExperimentTemplateResponseTypeDef",
     {
         "experimentTemplate": ExperimentTemplateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/PKG-INFO` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fis
-Version: 1.28.12
-Summary: Type annotations for boto3.FIS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fis.svg?color=blue)](https://pypi.org/project/mypy-boto3-fis)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fis)](https://pepy.tech/project/mypy-boto3-fis)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FIS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
+[boto3.FIS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fis.html#FIS)
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
 [mypy-boto3-fis docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,14 +302,15 @@
 from mypy_boto3_fis.type_defs import (
     ActionParameterTypeDef,
     ActionTargetTypeDef,
     CreateExperimentTemplateActionInputTypeDef,
     ExperimentTemplateCloudWatchLogsLogConfigurationInputTypeDef,
     ExperimentTemplateS3LogConfigurationInputTypeDef,
     CreateExperimentTemplateStopConditionInputTypeDef,
+    ResponseMetadataTypeDef,
     ExperimentTemplateTargetInputFilterTypeDef,
     DeleteExperimentTemplateRequestRequestTypeDef,
     ExperimentActionStateTypeDef,
     ExperimentCloudWatchLogsLogConfigurationTypeDef,
     ExperimentS3LogConfigurationTypeDef,
     ExperimentStateTypeDef,
     ExperimentStopConditionTypeDef,
@@ -324,29 +325,28 @@
     GetExperimentRequestRequestTypeDef,
     GetExperimentTemplateRequestRequestTypeDef,
     GetTargetResourceTypeRequestRequestTypeDef,
     ListActionsRequestRequestTypeDef,
     ListExperimentTemplatesRequestRequestTypeDef,
     ListExperimentsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetResourceTypesRequestRequestTypeDef,
     TargetResourceTypeSummaryTypeDef,
-    ResponseMetadataTypeDef,
     StartExperimentRequestRequestTypeDef,
     StopExperimentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TargetResourceTypeParameterTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateExperimentTemplateActionInputItemTypeDef,
     UpdateExperimentTemplateStopConditionInputTypeDef,
     ActionSummaryTypeDef,
     ActionTypeDef,
     CreateExperimentTemplateLogConfigurationInputTypeDef,
     UpdateExperimentTemplateLogConfigurationInputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateExperimentTemplateTargetInputTypeDef,
     UpdateExperimentTemplateTargetInputTypeDef,
     ExperimentActionTypeDef,
     ExperimentLogConfigurationTypeDef,
     ExperimentSummaryTypeDef,
     ExperimentTargetTypeDef,
     ExperimentTemplateLogConfigurationTypeDef,
```

### Comparing `mypy-boto3-fis-1.28.12/mypy_boto3_fis.egg-info/SOURCES.txt` & `mypy-boto3-fis-1.28.15/mypy_boto3_fis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fis-1.28.12/setup.py` & `mypy-boto3-fis-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fis",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_fis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FIS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.FIS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

