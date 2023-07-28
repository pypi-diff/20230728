# Comparing `tmp/mypy-boto3-timestream-query-1.28.12.tar.gz` & `tmp/mypy-boto3-timestream-query-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-query-1.28.12.tar", last modified: Thu Jul 27 11:49:46 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-query-1.28.15.tar", last modified: Fri Jul 28 20:43:52 2023, max compression
```

## Comparing `mypy-boto3-timestream-query-1.28.12.tar` & `mypy-boto3-timestream-query-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.485435 mypy-boto3-timestream-query-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-27 11:49:46.481435 mypy-boto3-timestream-query-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14343 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.473435 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-27 11:47:58.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-27 11:47:58.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-27 11:48:00.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-27 11:48:00.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-27 11:47:58.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-27 11:47:58.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24008 2023-07-27 11:48:00.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23967 2023-07-27 11:48:00.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:46.481435 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15865 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-27 11:49:46.000000 mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:46.485435 mypy-boto3-timestream-query-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-27 11:47:57.000000 mypy-boto3-timestream-query-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.589985 mypy-boto3-timestream-query-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-28 20:43:52.585985 mypy-boto3-timestream-query-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.577985 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13143 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21640 2023-07-28 20:40:37.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:52.585985 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-28 20:43:52.000000 mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:52.589985 mypy-boto3-timestream-query-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-28 20:40:36.000000 mypy-boto3-timestream-query-1.28.15/setup.py
```

### Comparing `mypy-boto3-timestream-query-1.28.12/LICENSE` & `mypy-boto3-timestream-query-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/PKG-INFO` & `mypy-boto3-timestream-query-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.28.12
-Summary: Type annotations for boto3.TimestreamQuery 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.TimestreamQuery 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,57 +348,49 @@
     ScheduleConfigurationTypeDef,
     TagTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
-    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
     PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    SnsConfigurationOutputTypeDef,
     SnsConfigurationTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ScheduleConfigurationOutputTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
     CancelQueryResponseTypeDef,
     CreateScheduledQueryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
-    ErrorReportConfigurationOutputTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
     ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     QueryRequestQueryPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MixedMeasureMappingOutputTypeDef,
-    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
-    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
     TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
```

### Comparing `mypy-boto3-timestream-query-1.28.12/README.md` & `mypy-boto3-timestream-query-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,57 +316,49 @@
     ScheduleConfigurationTypeDef,
     TagTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
-    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
     PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    SnsConfigurationOutputTypeDef,
     SnsConfigurationTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ScheduleConfigurationOutputTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
     CancelQueryResponseTypeDef,
     CreateScheduledQueryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
-    ErrorReportConfigurationOutputTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
     ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     QueryRequestQueryPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MixedMeasureMappingOutputTypeDef,
-    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
-    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
     TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
```

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__init__.py` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__init__.pyi` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/__main__.py` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamQuery 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.TimestreamQuery 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/client.py` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/client.pyi` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/literals.py` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/literals.pyi` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/paginator.py` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/paginator.pyi` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/type_defs.py` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -29,69 +29,60 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
     "RowTypeDef",
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
-    "DimensionMappingOutputTypeDef",
     "DimensionMappingTypeDef",
-    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ExecutionStatsTypeDef",
     "PaginatorConfigTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "MultiMeasureAttributeMappingOutputTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
-    "SnsConfigurationOutputTypeDef",
     "SnsConfigurationTypeDef",
     "ParameterMappingTypeDef",
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
-    "ScheduleConfigurationOutputTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
     "CancelQueryResponseTypeDef",
     "CreateScheduledQueryResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
-    "ErrorReportConfigurationOutputTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "QueryRequestQueryPaginateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MixedMeasureMappingOutputTypeDef",
-    "MultiMeasureMappingsOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
-    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
     "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
@@ -132,19 +123,17 @@
     "_OptionalColumnInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class ColumnInfoTypeDef(_RequiredColumnInfoTypeDef, _OptionalColumnInfoTypeDef):
     pass
 
-
 ScheduleConfigurationTypeDef = TypedDict(
     "ScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
@@ -163,15 +152,15 @@
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
-        "Value": "DatumTypeDef",
+        "Value": Dict[str, Any],
     },
 )
 
 DeleteScheduledQueryRequestRequestTypeDef = TypedDict(
     "DeleteScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
@@ -189,52 +178,22 @@
 DescribeScheduledQueryRequestRequestTypeDef = TypedDict(
     "DescribeScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
     },
 )
 
-DimensionMappingOutputTypeDef = TypedDict(
-    "DimensionMappingOutputTypeDef",
-    {
-        "Name": str,
-        "DimensionValueType": Literal["VARCHAR"],
-    },
-)
-
 DimensionMappingTypeDef = TypedDict(
     "DimensionMappingTypeDef",
     {
         "Name": str,
         "DimensionValueType": Literal["VARCHAR"],
     },
 )
 
-_RequiredS3ConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalS3ConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3ConfigurationOutputTypeDef",
-    {
-        "ObjectKeyPrefix": str,
-        "EncryptionOption": S3EncryptionOptionType,
-    },
-    total=False,
-)
-
-
-class S3ConfigurationOutputTypeDef(
-    _RequiredS3ConfigurationOutputTypeDef, _OptionalS3ConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredS3ConfigurationTypeDef = TypedDict(
     "_RequiredS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ConfigurationTypeDef = TypedDict(
@@ -242,19 +201,17 @@
     {
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
     },
     total=False,
 )
 
-
 class S3ConfigurationTypeDef(_RequiredS3ConfigurationTypeDef, _OptionalS3ConfigurationTypeDef):
     pass
 
-
 S3ReportLocationTypeDef = TypedDict(
     "S3ReportLocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
@@ -271,22 +228,20 @@
     "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class ExecuteScheduledQueryRequestRequestTypeDef(
     _RequiredExecuteScheduledQueryRequestRequestTypeDef,
     _OptionalExecuteScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
-
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": int,
         "DataWrites": int,
         "BytesMetered": int,
         "RecordsIngested": int,
@@ -325,53 +280,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-_RequiredMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureAttributeMappingOutputTypeDef",
-    {
-        "SourceColumn": str,
-        "MeasureValueType": ScalarMeasureValueTypeType,
-    },
-)
-_OptionalMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureAttributeMappingOutputTypeDef",
-    {
-        "TargetMultiMeasureAttributeName": str,
-    },
-    total=False,
-)
-
-
-class MultiMeasureAttributeMappingOutputTypeDef(
-    _RequiredMultiMeasureAttributeMappingOutputTypeDef,
-    _OptionalMultiMeasureAttributeMappingOutputTypeDef,
-):
-    pass
-
-
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
 )
@@ -379,28 +301,19 @@
     "_OptionalMultiMeasureAttributeMappingTypeDef",
     {
         "TargetMultiMeasureAttributeName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-
-SnsConfigurationOutputTypeDef = TypedDict(
-    "SnsConfigurationOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
-
 SnsConfigurationTypeDef = TypedDict(
     "SnsConfigurationTypeDef",
     {
         "TopicArn": str,
     },
 )
 
@@ -422,21 +335,19 @@
     "_OptionalPrepareQueryRequestRequestTypeDef",
     {
         "ValidateOnly": bool,
     },
     total=False,
 )
 
-
 class PrepareQueryRequestRequestTypeDef(
     _RequiredPrepareQueryRequestRequestTypeDef, _OptionalPrepareQueryRequestRequestTypeDef
 ):
     pass
 
-
 SelectColumnTypeDef = TypedDict(
     "SelectColumnTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
         "DatabaseName": str,
         "TableName": str,
@@ -457,38 +368,29 @@
         "ClientToken": str,
         "NextToken": str,
         "MaxRows": int,
     },
     total=False,
 )
 
-
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
-
 QueryStatusTypeDef = TypedDict(
     "QueryStatusTypeDef",
     {
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
     },
     total=False,
 )
 
-ScheduleConfigurationOutputTypeDef = TypedDict(
-    "ScheduleConfigurationOutputTypeDef",
-    {
-        "ScheduleExpression": str,
-    },
-)
-
 TimestreamDestinationTypeDef = TypedDict(
     "TimestreamDestinationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
     total=False,
@@ -540,14 +442,23 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -568,21 +479,14 @@
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ErrorReportConfigurationOutputTypeDef = TypedDict(
-    "ErrorReportConfigurationOutputTypeDef",
-    {
-        "S3Configuration": S3ConfigurationOutputTypeDef,
-    },
-)
-
 ErrorReportConfigurationTypeDef = TypedDict(
     "ErrorReportConfigurationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
 )
 
@@ -612,22 +516,20 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
-
 _RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
     "_RequiredQueryRequestQueryPaginateTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
@@ -635,75 +537,41 @@
     {
         "ClientToken": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class QueryRequestQueryPaginateTypeDef(
     _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
 ):
     pass
 
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingOutputTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
     "_OptionalMixedMeasureMappingOutputTypeDef",
     {
         "MeasureName": str,
         "SourceColumn": str,
         "TargetMeasureName": str,
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
 class MixedMeasureMappingOutputTypeDef(
     _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
 ):
     pass
 
-
-_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureMappingsOutputTypeDef",
-    {
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
-    },
-)
-_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureMappingsOutputTypeDef",
-    {
-        "TargetMultiMeasureName": str,
-    },
-    total=False,
-)
-
-
-class MultiMeasureMappingsOutputTypeDef(
-    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
-):
-    pass
-
-
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -713,20 +581,37 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
 
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
@@ -734,28 +619,19 @@
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
-
-NotificationConfigurationOutputTypeDef = TypedDict(
-    "NotificationConfigurationOutputTypeDef",
-    {
-        "SnsConfiguration": SnsConfigurationOutputTypeDef,
-    },
-)
-
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "SnsConfiguration": SnsConfigurationTypeDef,
     },
 )
 
@@ -804,34 +680,32 @@
 
 _RequiredTimestreamConfigurationOutputTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationOutputTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
-        "DimensionMappings": List[DimensionMappingOutputTypeDef],
+        "DimensionMappings": List[DimensionMappingTypeDef],
     },
 )
 _OptionalTimestreamConfigurationOutputTypeDef = TypedDict(
     "_OptionalTimestreamConfigurationOutputTypeDef",
     {
         "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
         "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class TimestreamConfigurationOutputTypeDef(
     _RequiredTimestreamConfigurationOutputTypeDef, _OptionalTimestreamConfigurationOutputTypeDef
 ):
     pass
 
-
 _RequiredTimestreamConfigurationTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -843,47 +717,43 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class TimestreamConfigurationTypeDef(
     _RequiredTimestreamConfigurationTypeDef, _OptionalTimestreamConfigurationTypeDef
 ):
     pass
 
-
 _RequiredScheduledQueryTypeDef = TypedDict(
     "_RequiredScheduledQueryTypeDef",
     {
         "Arn": str,
         "Name": str,
         "State": ScheduledQueryStateType,
     },
 )
 _OptionalScheduledQueryTypeDef = TypedDict(
     "_OptionalScheduledQueryTypeDef",
     {
         "CreationTime": datetime,
         "PreviousInvocationTime": datetime,
         "NextInvocationTime": datetime,
-        "ErrorReportConfiguration": ErrorReportConfigurationOutputTypeDef,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
         "TargetDestination": TargetDestinationTypeDef,
         "LastRunStatus": ScheduledQueryRunStatusType,
     },
     total=False,
 )
 
-
 class ScheduledQueryTypeDef(_RequiredScheduledQueryTypeDef, _OptionalScheduledQueryTypeDef):
     pass
 
-
 TargetConfigurationOutputTypeDef = TypedDict(
     "TargetConfigurationOutputTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
     },
 )
 
@@ -906,41 +776,39 @@
 _RequiredScheduledQueryDescriptionTypeDef = TypedDict(
     "_RequiredScheduledQueryDescriptionTypeDef",
     {
         "Arn": str,
         "Name": str,
         "QueryString": str,
         "State": ScheduledQueryStateType,
-        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
-        "NotificationConfiguration": NotificationConfigurationOutputTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
 )
 _OptionalScheduledQueryDescriptionTypeDef = TypedDict(
     "_OptionalScheduledQueryDescriptionTypeDef",
     {
         "CreationTime": datetime,
         "PreviousInvocationTime": datetime,
         "NextInvocationTime": datetime,
         "TargetConfiguration": TargetConfigurationOutputTypeDef,
         "ScheduledQueryExecutionRoleArn": str,
         "KmsKeyId": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationOutputTypeDef,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
         "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
         "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-
 class ScheduledQueryDescriptionTypeDef(
     _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
 ):
     pass
 
-
 _RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
         "Name": str,
         "QueryString": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
@@ -955,22 +823,20 @@
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class CreateScheduledQueryRequestRequestTypeDef(
     _RequiredCreateScheduledQueryRequestRequestTypeDef,
     _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query/type_defs.pyi` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,68 +29,61 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
     "RowTypeDef",
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
-    "DimensionMappingOutputTypeDef",
     "DimensionMappingTypeDef",
-    "S3ConfigurationOutputTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
     "ExecuteScheduledQueryRequestRequestTypeDef",
     "ExecutionStatsTypeDef",
     "PaginatorConfigTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "MultiMeasureAttributeMappingOutputTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
-    "SnsConfigurationOutputTypeDef",
     "SnsConfigurationTypeDef",
     "ParameterMappingTypeDef",
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
-    "ScheduleConfigurationOutputTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
     "CancelQueryResponseTypeDef",
     "CreateScheduledQueryResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
-    "ErrorReportConfigurationOutputTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
     "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "QueryRequestQueryPaginateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "MixedMeasureMappingOutputTypeDef",
-    "MultiMeasureMappingsOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
-    "NotificationConfigurationOutputTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
     "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
@@ -131,17 +124,19 @@
     "_OptionalColumnInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class ColumnInfoTypeDef(_RequiredColumnInfoTypeDef, _OptionalColumnInfoTypeDef):
     pass
 
+
 ScheduleConfigurationTypeDef = TypedDict(
     "ScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 
@@ -160,15 +155,15 @@
     },
 )
 
 TimeSeriesDataPointTypeDef = TypedDict(
     "TimeSeriesDataPointTypeDef",
     {
         "Time": str,
-        "Value": "DatumTypeDef",
+        "Value": Dict[str, Any],
     },
 )
 
 DeleteScheduledQueryRequestRequestTypeDef = TypedDict(
     "DeleteScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
@@ -186,50 +181,22 @@
 DescribeScheduledQueryRequestRequestTypeDef = TypedDict(
     "DescribeScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
     },
 )
 
-DimensionMappingOutputTypeDef = TypedDict(
-    "DimensionMappingOutputTypeDef",
-    {
-        "Name": str,
-        "DimensionValueType": Literal["VARCHAR"],
-    },
-)
-
 DimensionMappingTypeDef = TypedDict(
     "DimensionMappingTypeDef",
     {
         "Name": str,
         "DimensionValueType": Literal["VARCHAR"],
     },
 )
 
-_RequiredS3ConfigurationOutputTypeDef = TypedDict(
-    "_RequiredS3ConfigurationOutputTypeDef",
-    {
-        "BucketName": str,
-    },
-)
-_OptionalS3ConfigurationOutputTypeDef = TypedDict(
-    "_OptionalS3ConfigurationOutputTypeDef",
-    {
-        "ObjectKeyPrefix": str,
-        "EncryptionOption": S3EncryptionOptionType,
-    },
-    total=False,
-)
-
-class S3ConfigurationOutputTypeDef(
-    _RequiredS3ConfigurationOutputTypeDef, _OptionalS3ConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredS3ConfigurationTypeDef = TypedDict(
     "_RequiredS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ConfigurationTypeDef = TypedDict(
@@ -237,17 +204,19 @@
     {
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
     },
     total=False,
 )
 
+
 class S3ConfigurationTypeDef(_RequiredS3ConfigurationTypeDef, _OptionalS3ConfigurationTypeDef):
     pass
 
+
 S3ReportLocationTypeDef = TypedDict(
     "S3ReportLocationTypeDef",
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
@@ -264,20 +233,22 @@
     "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class ExecuteScheduledQueryRequestRequestTypeDef(
     _RequiredExecuteScheduledQueryRequestRequestTypeDef,
     _OptionalExecuteScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
+
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": int,
         "DataWrites": int,
         "BytesMetered": int,
         "RecordsIngested": int,
@@ -316,48 +287,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
-_RequiredMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureAttributeMappingOutputTypeDef",
-    {
-        "SourceColumn": str,
-        "MeasureValueType": ScalarMeasureValueTypeType,
-    },
-)
-_OptionalMultiMeasureAttributeMappingOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureAttributeMappingOutputTypeDef",
-    {
-        "TargetMultiMeasureAttributeName": str,
-    },
-    total=False,
-)
-
-class MultiMeasureAttributeMappingOutputTypeDef(
-    _RequiredMultiMeasureAttributeMappingOutputTypeDef,
-    _OptionalMultiMeasureAttributeMappingOutputTypeDef,
-):
-    pass
 
 _RequiredMultiMeasureAttributeMappingTypeDef = TypedDict(
     "_RequiredMultiMeasureAttributeMappingTypeDef",
     {
         "SourceColumn": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
@@ -366,25 +310,20 @@
     "_OptionalMultiMeasureAttributeMappingTypeDef",
     {
         "TargetMultiMeasureAttributeName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-SnsConfigurationOutputTypeDef = TypedDict(
-    "SnsConfigurationOutputTypeDef",
-    {
-        "TopicArn": str,
-    },
-)
 
 SnsConfigurationTypeDef = TypedDict(
     "SnsConfigurationTypeDef",
     {
         "TopicArn": str,
     },
 )
@@ -407,19 +346,21 @@
     "_OptionalPrepareQueryRequestRequestTypeDef",
     {
         "ValidateOnly": bool,
     },
     total=False,
 )
 
+
 class PrepareQueryRequestRequestTypeDef(
     _RequiredPrepareQueryRequestRequestTypeDef, _OptionalPrepareQueryRequestRequestTypeDef
 ):
     pass
 
+
 SelectColumnTypeDef = TypedDict(
     "SelectColumnTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
         "DatabaseName": str,
         "TableName": str,
@@ -440,36 +381,31 @@
         "ClientToken": str,
         "NextToken": str,
         "MaxRows": int,
     },
     total=False,
 )
 
+
 class QueryRequestRequestTypeDef(
     _RequiredQueryRequestRequestTypeDef, _OptionalQueryRequestRequestTypeDef
 ):
     pass
 
+
 QueryStatusTypeDef = TypedDict(
     "QueryStatusTypeDef",
     {
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
     },
     total=False,
 )
 
-ScheduleConfigurationOutputTypeDef = TypedDict(
-    "ScheduleConfigurationOutputTypeDef",
-    {
-        "ScheduleExpression": str,
-    },
-)
-
 TimestreamDestinationTypeDef = TypedDict(
     "TimestreamDestinationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
     total=False,
@@ -521,14 +457,23 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -549,21 +494,14 @@
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ErrorReportConfigurationOutputTypeDef = TypedDict(
-    "ErrorReportConfigurationOutputTypeDef",
-    {
-        "S3Configuration": S3ConfigurationOutputTypeDef,
-    },
-)
-
 ErrorReportConfigurationTypeDef = TypedDict(
     "ErrorReportConfigurationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
     },
 )
 
@@ -593,20 +531,22 @@
     "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
     _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
 ):
     pass
 
+
 _RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
     "_RequiredQueryRequestQueryPaginateTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
@@ -614,68 +554,44 @@
     {
         "ClientToken": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class QueryRequestQueryPaginateTypeDef(
     _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
 _RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingOutputTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
     "_OptionalMixedMeasureMappingOutputTypeDef",
     {
         "MeasureName": str,
         "SourceColumn": str,
         "TargetMeasureName": str,
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingOutputTypeDef(
     _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
 ):
     pass
 
-_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_RequiredMultiMeasureMappingsOutputTypeDef",
-    {
-        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingOutputTypeDef],
-    },
-)
-_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
-    "_OptionalMultiMeasureMappingsOutputTypeDef",
-    {
-        "TargetMultiMeasureName": str,
-    },
-    total=False,
-)
-
-class MultiMeasureMappingsOutputTypeDef(
-    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
-):
-    pass
 
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
@@ -686,44 +602,62 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
+
+
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
-NotificationConfigurationOutputTypeDef = TypedDict(
-    "NotificationConfigurationOutputTypeDef",
-    {
-        "SnsConfiguration": SnsConfigurationOutputTypeDef,
-    },
-)
 
 NotificationConfigurationTypeDef = TypedDict(
     "NotificationConfigurationTypeDef",
     {
         "SnsConfiguration": SnsConfigurationTypeDef,
     },
 )
@@ -773,32 +707,34 @@
 
 _RequiredTimestreamConfigurationOutputTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationOutputTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
-        "DimensionMappings": List[DimensionMappingOutputTypeDef],
+        "DimensionMappings": List[DimensionMappingTypeDef],
     },
 )
 _OptionalTimestreamConfigurationOutputTypeDef = TypedDict(
     "_OptionalTimestreamConfigurationOutputTypeDef",
     {
         "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
         "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class TimestreamConfigurationOutputTypeDef(
     _RequiredTimestreamConfigurationOutputTypeDef, _OptionalTimestreamConfigurationOutputTypeDef
 ):
     pass
 
+
 _RequiredTimestreamConfigurationTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -810,43 +746,47 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class TimestreamConfigurationTypeDef(
     _RequiredTimestreamConfigurationTypeDef, _OptionalTimestreamConfigurationTypeDef
 ):
     pass
 
+
 _RequiredScheduledQueryTypeDef = TypedDict(
     "_RequiredScheduledQueryTypeDef",
     {
         "Arn": str,
         "Name": str,
         "State": ScheduledQueryStateType,
     },
 )
 _OptionalScheduledQueryTypeDef = TypedDict(
     "_OptionalScheduledQueryTypeDef",
     {
         "CreationTime": datetime,
         "PreviousInvocationTime": datetime,
         "NextInvocationTime": datetime,
-        "ErrorReportConfiguration": ErrorReportConfigurationOutputTypeDef,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
         "TargetDestination": TargetDestinationTypeDef,
         "LastRunStatus": ScheduledQueryRunStatusType,
     },
     total=False,
 )
 
+
 class ScheduledQueryTypeDef(_RequiredScheduledQueryTypeDef, _OptionalScheduledQueryTypeDef):
     pass
 
+
 TargetConfigurationOutputTypeDef = TypedDict(
     "TargetConfigurationOutputTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
     },
 )
 
@@ -869,39 +809,41 @@
 _RequiredScheduledQueryDescriptionTypeDef = TypedDict(
     "_RequiredScheduledQueryDescriptionTypeDef",
     {
         "Arn": str,
         "Name": str,
         "QueryString": str,
         "State": ScheduledQueryStateType,
-        "ScheduleConfiguration": ScheduleConfigurationOutputTypeDef,
-        "NotificationConfiguration": NotificationConfigurationOutputTypeDef,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
+        "NotificationConfiguration": NotificationConfigurationTypeDef,
     },
 )
 _OptionalScheduledQueryDescriptionTypeDef = TypedDict(
     "_OptionalScheduledQueryDescriptionTypeDef",
     {
         "CreationTime": datetime,
         "PreviousInvocationTime": datetime,
         "NextInvocationTime": datetime,
         "TargetConfiguration": TargetConfigurationOutputTypeDef,
         "ScheduledQueryExecutionRoleArn": str,
         "KmsKeyId": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationOutputTypeDef,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
         "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
         "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
+
 class ScheduledQueryDescriptionTypeDef(
     _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
 ):
     pass
 
+
 _RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
         "Name": str,
         "QueryString": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
@@ -916,20 +858,22 @@
         "ClientToken": str,
         "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class CreateScheduledQueryRequestRequestTypeDef(
     _RequiredCreateScheduledQueryRequestRequestTypeDef,
     _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/PKG-INFO` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-query
-Version: 1.28.12
-Summary: Type annotations for boto3.TimestreamQuery 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.TimestreamQuery 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-query.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-timestream-query)](https://pepy.tech/project/mypy-boto3-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamQuery 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
+[boto3.TimestreamQuery 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [mypy-boto3-timestream-query docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_query/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,57 +348,49 @@
     ScheduleConfigurationTypeDef,
     TagTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
-    DimensionMappingOutputTypeDef,
     DimensionMappingTypeDef,
-    S3ConfigurationOutputTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
     ExecuteScheduledQueryRequestRequestTypeDef,
     ExecutionStatsTypeDef,
     PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MultiMeasureAttributeMappingOutputTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    SnsConfigurationOutputTypeDef,
     SnsConfigurationTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ScheduleConfigurationOutputTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
     CancelQueryResponseTypeDef,
     CreateScheduledQueryResponseTypeDef,
     EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
-    ErrorReportConfigurationOutputTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
     ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
     ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     QueryRequestQueryPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     MixedMeasureMappingOutputTypeDef,
-    MultiMeasureMappingsOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
-    NotificationConfigurationOutputTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
     TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
```

### Comparing `mypy-boto3-timestream-query-1.28.12/mypy_boto3_timestream_query.egg-info/SOURCES.txt` & `mypy-boto3-timestream-query-1.28.15/mypy_boto3_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-query-1.28.12/setup.py` & `mypy-boto3-timestream-query-1.28.15/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-timestream-query",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamQuery 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.TimestreamQuery 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

