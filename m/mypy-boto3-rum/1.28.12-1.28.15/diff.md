# Comparing `tmp/mypy-boto3-rum-1.28.12.tar.gz` & `tmp/mypy-boto3-rum-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-rum-1.28.12.tar", last modified: Thu Jul 27 11:49:33 2023, max compression
+gzip compressed data, was "mypy-boto3-rum-1.28.15.tar", last modified: Fri Jul 28 20:43:37 2023, max compression
```

## Comparing `mypy-boto3-rum-1.28.12.tar` & `mypy-boto3-rum-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/mypy_boto3_rum/
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21433 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:45:01.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15235 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:32.000000 mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:33.077239 mypy-boto3-rum-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 11:45:00.000000 mypy-boto3-rum-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.213775 mypy-boto3-rum-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-28 20:43:37.213775 mypy-boto3-rum-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.209775 mypy-boto3-rum-1.28.15/mypy_boto3_rum/
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16581 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21247 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-07-28 20:37:28.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:27.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:37.213775 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:37.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:36.000000 mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:37.213775 mypy-boto3-rum-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:37:24.000000 mypy-boto3-rum-1.28.15/setup.py
```

### Comparing `mypy-boto3-rum-1.28.12/LICENSE` & `mypy-boto3-rum-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/PKG-INFO` & `mypy-boto3-rum-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudWatchRUM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,24 +342,23 @@
 
 ```python
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
-    CustomEventsOutputTypeDef,
+    CustomEventsTypeDef,
     MetricDefinitionRequestOutputTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
-    CustomEventsTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
     GetAppMonitorRequestRequestTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
@@ -367,28 +366,28 @@
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateAppMonitorRequestRequestTypeDef,
+    UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     GetAppMonitorDataResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    CreateAppMonitorRequestRequestTypeDef,
-    UpdateAppMonitorRequestRequestTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
```

### Comparing `mypy-boto3-rum-1.28.12/README.md` & `mypy-boto3-rum-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,24 +310,23 @@
 
 ```python
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
-    CustomEventsOutputTypeDef,
+    CustomEventsTypeDef,
     MetricDefinitionRequestOutputTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
-    CustomEventsTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
     GetAppMonitorRequestRequestTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
@@ -335,28 +334,28 @@
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateAppMonitorRequestRequestTypeDef,
+    UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     GetAppMonitorDataResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    CreateAppMonitorRequestRequestTypeDef,
-    UpdateAppMonitorRequestRequestTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
```

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/__init__.py` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/__init__.pyi` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/__main__.py` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudWatchRUM 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudWatchRUM 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM\nOther"
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

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/client.py` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/client.pyi` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/literals.py` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/literals.pyi` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/paginator.py` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/paginator.pyi` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/type_defs.py` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,23 @@
 
 
 __all__ = (
     "AppMonitorConfigurationOutputTypeDef",
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
-    "CustomEventsOutputTypeDef",
+    "CustomEventsTypeDef",
     "MetricDefinitionRequestOutputTypeDef",
     "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
-    "CustomEventsTypeDef",
     "CwLogTypeDef",
     "DeleteAppMonitorRequestRequestTypeDef",
     "DeleteRumMetricsDestinationRequestRequestTypeDef",
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
@@ -49,28 +48,28 @@
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RumEventTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateAppMonitorRequestRequestTypeDef",
+    "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     "CreateAppMonitorResponseTypeDef",
     "GetAppMonitorDataResponseTypeDef",
     "ListAppMonitorsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    "CreateAppMonitorRequestRequestTypeDef",
-    "UpdateAppMonitorRequestRequestTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
     "PutRumEventsRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
@@ -127,16 +126,16 @@
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
     },
     total=False,
 )
 
-CustomEventsOutputTypeDef = TypedDict(
-    "CustomEventsOutputTypeDef",
+CustomEventsTypeDef = TypedDict(
+    "CustomEventsTypeDef",
     {
         "Status": CustomEventsStatusType,
     },
     total=False,
 )
 
 _RequiredMetricDefinitionRequestOutputTypeDef = TypedDict(
@@ -288,22 +287,14 @@
 class BatchGetRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchGetRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
 
-CustomEventsTypeDef = TypedDict(
-    "CustomEventsTypeDef",
-    {
-        "Status": CustomEventsStatusType,
-    },
-    total=False,
-)
-
 CwLogTypeDef = TypedDict(
     "CwLogTypeDef",
     {
         "CwLogEnabled": bool,
         "CwLogGroup": str,
     },
     total=False,
@@ -490,14 +481,63 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppMonitorRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+    },
+)
+_OptionalCreateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppMonitorRequestRequestTypeDef",
+    {
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
+        "CwLogEnabled": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateAppMonitorRequestRequestTypeDef(
+    _RequiredCreateAppMonitorRequestRequestTypeDef, _OptionalCreateAppMonitorRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppMonitorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppMonitorRequestRequestTypeDef",
+    {
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
+        "CwLogEnabled": bool,
+        "Domain": str,
+    },
+    total=False,
+)
+
+
+class UpdateAppMonitorRequestRequestTypeDef(
+    _RequiredUpdateAppMonitorRequestRequestTypeDef, _OptionalUpdateAppMonitorRequestRequestTypeDef
+):
+    pass
+
+
 BatchCreateRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "MetricDefinition": MetricDefinitionRequestOutputTypeDef,
     },
@@ -655,63 +695,14 @@
 class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
     _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
 ):
     pass
 
 
-_RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppMonitorRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-    },
-)
-_OptionalCreateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppMonitorRequestRequestTypeDef",
-    {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
-        "CustomEvents": CustomEventsTypeDef,
-        "CwLogEnabled": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateAppMonitorRequestRequestTypeDef(
-    _RequiredCreateAppMonitorRequestRequestTypeDef, _OptionalCreateAppMonitorRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppMonitorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppMonitorRequestRequestTypeDef",
-    {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
-        "CustomEvents": CustomEventsTypeDef,
-        "CwLogEnabled": bool,
-        "Domain": str,
-    },
-    total=False,
-)
-
-
-class UpdateAppMonitorRequestRequestTypeDef(
-    _RequiredUpdateAppMonitorRequestRequestTypeDef, _OptionalUpdateAppMonitorRequestRequestTypeDef
-):
-    pass
-
-
 DataStorageTypeDef = TypedDict(
     "DataStorageTypeDef",
     {
         "CwLog": CwLogTypeDef,
     },
     total=False,
 )
@@ -794,15 +785,15 @@
 )
 
 AppMonitorTypeDef = TypedDict(
     "AppMonitorTypeDef",
     {
         "AppMonitorConfiguration": AppMonitorConfigurationOutputTypeDef,
         "Created": str,
-        "CustomEvents": CustomEventsOutputTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
         "DataStorage": DataStorageTypeDef,
         "Domain": str,
         "Id": str,
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
         "Tags": Dict[str, str],
```

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum/type_defs.pyi` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,23 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AppMonitorConfigurationOutputTypeDef",
     "AppMonitorConfigurationTypeDef",
     "AppMonitorDetailsTypeDef",
     "AppMonitorSummaryTypeDef",
-    "CustomEventsOutputTypeDef",
+    "CustomEventsTypeDef",
     "MetricDefinitionRequestOutputTypeDef",
     "MetricDefinitionRequestTypeDef",
     "MetricDefinitionTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteRumMetricDefinitionsErrorTypeDef",
     "BatchDeleteRumMetricDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "BatchGetRumMetricDefinitionsRequestRequestTypeDef",
-    "CustomEventsTypeDef",
     "CwLogTypeDef",
     "DeleteAppMonitorRequestRequestTypeDef",
     "DeleteRumMetricsDestinationRequestRequestTypeDef",
     "QueryFilterTypeDef",
     "TimeRangeTypeDef",
     "GetAppMonitorRequestRequestTypeDef",
     "ListAppMonitorsRequestRequestTypeDef",
@@ -48,28 +47,28 @@
     "MetricDestinationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "RumEventTypeDef",
     "UserDetailsTypeDef",
     "PutRumMetricsDestinationRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateAppMonitorRequestRequestTypeDef",
+    "UpdateAppMonitorRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     "BatchCreateRumMetricDefinitionsRequestRequestTypeDef",
     "UpdateRumMetricDefinitionRequestRequestTypeDef",
     "BatchGetRumMetricDefinitionsResponseTypeDef",
     "CreateAppMonitorResponseTypeDef",
     "GetAppMonitorDataResponseTypeDef",
     "ListAppMonitorsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "BatchDeleteRumMetricDefinitionsResponseTypeDef",
     "BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef",
     "ListAppMonitorsRequestListAppMonitorsPaginateTypeDef",
     "ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef",
-    "CreateAppMonitorRequestRequestTypeDef",
-    "UpdateAppMonitorRequestRequestTypeDef",
     "DataStorageTypeDef",
     "GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef",
     "GetAppMonitorDataRequestRequestTypeDef",
     "ListRumMetricsDestinationsResponseTypeDef",
     "PutRumEventsRequestRequestTypeDef",
     "BatchCreateRumMetricDefinitionsResponseTypeDef",
     "AppMonitorTypeDef",
@@ -126,16 +125,16 @@
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
     },
     total=False,
 )
 
-CustomEventsOutputTypeDef = TypedDict(
-    "CustomEventsOutputTypeDef",
+CustomEventsTypeDef = TypedDict(
+    "CustomEventsTypeDef",
     {
         "Status": CustomEventsStatusType,
     },
     total=False,
 )
 
 _RequiredMetricDefinitionRequestOutputTypeDef = TypedDict(
@@ -277,22 +276,14 @@
 
 class BatchGetRumMetricDefinitionsRequestRequestTypeDef(
     _RequiredBatchGetRumMetricDefinitionsRequestRequestTypeDef,
     _OptionalBatchGetRumMetricDefinitionsRequestRequestTypeDef,
 ):
     pass
 
-CustomEventsTypeDef = TypedDict(
-    "CustomEventsTypeDef",
-    {
-        "Status": CustomEventsStatusType,
-    },
-    total=False,
-)
-
 CwLogTypeDef = TypedDict(
     "CwLogTypeDef",
     {
         "CwLogEnabled": bool,
         "CwLogGroup": str,
     },
     total=False,
@@ -469,14 +460,59 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+_RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateAppMonitorRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "Name": str,
+    },
+)
+_OptionalCreateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateAppMonitorRequestRequestTypeDef",
+    {
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
+        "CwLogEnabled": bool,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateAppMonitorRequestRequestTypeDef(
+    _RequiredCreateAppMonitorRequestRequestTypeDef, _OptionalCreateAppMonitorRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateAppMonitorRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalUpdateAppMonitorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateAppMonitorRequestRequestTypeDef",
+    {
+        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
+        "CwLogEnabled": bool,
+        "Domain": str,
+    },
+    total=False,
+)
+
+class UpdateAppMonitorRequestRequestTypeDef(
+    _RequiredUpdateAppMonitorRequestRequestTypeDef, _OptionalUpdateAppMonitorRequestRequestTypeDef
+):
+    pass
+
 BatchCreateRumMetricDefinitionsErrorTypeDef = TypedDict(
     "BatchCreateRumMetricDefinitionsErrorTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
         "MetricDefinition": MetricDefinitionRequestOutputTypeDef,
     },
@@ -626,59 +662,14 @@
 
 class ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef(
     _RequiredListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
     _OptionalListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
 ):
     pass
 
-_RequiredCreateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateAppMonitorRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "Name": str,
-    },
-)
-_OptionalCreateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateAppMonitorRequestRequestTypeDef",
-    {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
-        "CustomEvents": CustomEventsTypeDef,
-        "CwLogEnabled": bool,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateAppMonitorRequestRequestTypeDef(
-    _RequiredCreateAppMonitorRequestRequestTypeDef, _OptionalCreateAppMonitorRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateAppMonitorRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalUpdateAppMonitorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateAppMonitorRequestRequestTypeDef",
-    {
-        "AppMonitorConfiguration": AppMonitorConfigurationTypeDef,
-        "CustomEvents": CustomEventsTypeDef,
-        "CwLogEnabled": bool,
-        "Domain": str,
-    },
-    total=False,
-)
-
-class UpdateAppMonitorRequestRequestTypeDef(
-    _RequiredUpdateAppMonitorRequestRequestTypeDef, _OptionalUpdateAppMonitorRequestRequestTypeDef
-):
-    pass
-
 DataStorageTypeDef = TypedDict(
     "DataStorageTypeDef",
     {
         "CwLog": CwLogTypeDef,
     },
     total=False,
 )
@@ -757,15 +748,15 @@
 )
 
 AppMonitorTypeDef = TypedDict(
     "AppMonitorTypeDef",
     {
         "AppMonitorConfiguration": AppMonitorConfigurationOutputTypeDef,
         "Created": str,
-        "CustomEvents": CustomEventsOutputTypeDef,
+        "CustomEvents": CustomEventsTypeDef,
         "DataStorage": DataStorageTypeDef,
         "Domain": str,
         "Id": str,
         "LastModified": str,
         "Name": str,
         "State": StateEnumType,
         "Tags": Dict[str, str],
```

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/PKG-INFO` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-rum
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudWatchRUM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-rum.svg?color=blue)](https://pypi.org/project/mypy-boto3-rum)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-rum)](https://pepy.tech/project/mypy-boto3-rum)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudWatchRUM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
+[boto3.CloudWatchRUM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rum.html#CloudWatchRUM)
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
 [mypy-boto3-rum docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_rum/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,24 +342,23 @@
 
 ```python
 from mypy_boto3_rum.type_defs import (
     AppMonitorConfigurationOutputTypeDef,
     AppMonitorConfigurationTypeDef,
     AppMonitorDetailsTypeDef,
     AppMonitorSummaryTypeDef,
-    CustomEventsOutputTypeDef,
+    CustomEventsTypeDef,
     MetricDefinitionRequestOutputTypeDef,
     MetricDefinitionRequestTypeDef,
     MetricDefinitionTypeDef,
     ResponseMetadataTypeDef,
     BatchDeleteRumMetricDefinitionsErrorTypeDef,
     BatchDeleteRumMetricDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
     BatchGetRumMetricDefinitionsRequestRequestTypeDef,
-    CustomEventsTypeDef,
     CwLogTypeDef,
     DeleteAppMonitorRequestRequestTypeDef,
     DeleteRumMetricsDestinationRequestRequestTypeDef,
     QueryFilterTypeDef,
     TimeRangeTypeDef,
     GetAppMonitorRequestRequestTypeDef,
     ListAppMonitorsRequestRequestTypeDef,
@@ -367,28 +366,28 @@
     MetricDestinationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     RumEventTypeDef,
     UserDetailsTypeDef,
     PutRumMetricsDestinationRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateAppMonitorRequestRequestTypeDef,
+    UpdateAppMonitorRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsErrorTypeDef,
     BatchCreateRumMetricDefinitionsRequestRequestTypeDef,
     UpdateRumMetricDefinitionRequestRequestTypeDef,
     BatchGetRumMetricDefinitionsResponseTypeDef,
     CreateAppMonitorResponseTypeDef,
     GetAppMonitorDataResponseTypeDef,
     ListAppMonitorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     BatchDeleteRumMetricDefinitionsResponseTypeDef,
     BatchGetRumMetricDefinitionsRequestBatchGetRumMetricDefinitionsPaginateTypeDef,
     ListAppMonitorsRequestListAppMonitorsPaginateTypeDef,
     ListRumMetricsDestinationsRequestListRumMetricsDestinationsPaginateTypeDef,
-    CreateAppMonitorRequestRequestTypeDef,
-    UpdateAppMonitorRequestRequestTypeDef,
     DataStorageTypeDef,
     GetAppMonitorDataRequestGetAppMonitorDataPaginateTypeDef,
     GetAppMonitorDataRequestRequestTypeDef,
     ListRumMetricsDestinationsResponseTypeDef,
     PutRumEventsRequestRequestTypeDef,
     BatchCreateRumMetricDefinitionsResponseTypeDef,
     AppMonitorTypeDef,
```

### Comparing `mypy-boto3-rum-1.28.12/mypy_boto3_rum.egg-info/SOURCES.txt` & `mypy-boto3-rum-1.28.15/mypy_boto3_rum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-rum-1.28.12/setup.py` & `mypy-boto3-rum-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-rum",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_rum"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudWatchRUM 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.CloudWatchRUM 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

