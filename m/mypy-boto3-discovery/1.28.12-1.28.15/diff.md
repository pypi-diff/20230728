# Comparing `tmp/mypy-boto3-discovery-1.28.12.tar.gz` & `tmp/mypy-boto3-discovery-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-discovery-1.28.12.tar", last modified: Thu Jul 27 05:34:34 2023, max compression
+gzip compressed data, was "mypy-boto3-discovery-1.28.15.tar", last modified: Fri Jul 28 20:42:38 2023, max compression
```

## Comparing `mypy-boto3-discovery-1.28.12.tar` & `mypy-boto3-discovery-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.916532 mypy-boto3-discovery-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-07-27 05:34:34.916532 mypy-boto3-discovery-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.916532 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-07-27 05:20:17.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-07-27 05:20:17.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8307 2023-07-27 05:20:17.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-07-27 05:20:17.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25179 2023-07-27 05:20:17.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-07-27 05:20:17.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.916532 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-07-27 05:34:34.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:34.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:34.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:34.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:34.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:34.000000 mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:34.916532 mypy-boto3-discovery-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-27 05:20:16.000000 mypy-boto3-discovery-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.100962 mypy-boto3-discovery-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-07-28 20:42:38.096962 mypy-boto3-discovery-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15573 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.088962 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22908 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10347 2023-07-28 20:23:00.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-07-28 20:23:00.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25129 2023-07-28 20:23:01.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25108 2023-07-28 20:23:00.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.096962 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17086 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:37.000000 mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:38.100962 mypy-boto3-discovery-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-28 20:22:59.000000 mypy-boto3-discovery-1.28.15/setup.py
```

### Comparing `mypy-boto3-discovery-1.28.12/LICENSE` & `mypy-boto3-discovery-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.12/PKG-INFO` & `mypy-boto3-discovery-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-discovery
-Version: 1.28.12
-Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,65 +363,65 @@
 ```python
 from mypy_boto3_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
     BatchDeleteImportDataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ConfigurationTagTypeDef,
     ContinuousExportDescriptionTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
     TagTypeDef,
     CustomerAgentInfoTypeDef,
     CustomerAgentlessCollectorInfoTypeDef,
     CustomerConnectorInfoTypeDef,
     CustomerMeCollectorInfoTypeDef,
     DeleteApplicationsRequestRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeConfigurationsRequestRequestTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
     DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsRequestRequestTypeDef,
     ExportInfoTypeDef,
     ExportFilterTypeDef,
     ImportTaskFilterTypeDef,
     ImportTaskTypeDef,
     TagFilterTypeDef,
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
-    ExportConfigurationsResponseTypeDef,
     OrderByElementTypeDef,
-    ListConfigurationsResponseTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartContinuousExportResponseTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    StartExportTaskResponseTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
-    StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeConfigurationsResponseTypeDef,
+    ExportConfigurationsResponseTypeDef,
+    ListConfigurationsResponseTypeDef,
+    StartContinuousExportResponseTypeDef,
+    StartDataCollectionByAgentIdsResponseTypeDef,
+    StartExportTaskResponseTypeDef,
+    StopContinuousExportResponseTypeDef,
+    StopDataCollectionByAgentIdsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DescribeContinuousExportsResponseTypeDef,
     CreateTagsRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
     DescribeAgentsRequestRequestTypeDef,
+    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
+    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
+    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
     DescribeImportTasksRequestRequestTypeDef,
     DescribeImportTasksResponseTypeDef,
     StartImportTaskResponseTypeDef,
```

### Comparing `mypy-boto3-discovery-1.28.12/README.md` & `mypy-boto3-discovery-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,65 +331,65 @@
 ```python
 from mypy_boto3_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
     BatchDeleteImportDataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ConfigurationTagTypeDef,
     ContinuousExportDescriptionTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
     TagTypeDef,
     CustomerAgentInfoTypeDef,
     CustomerAgentlessCollectorInfoTypeDef,
     CustomerConnectorInfoTypeDef,
     CustomerMeCollectorInfoTypeDef,
     DeleteApplicationsRequestRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeConfigurationsRequestRequestTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
     DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsRequestRequestTypeDef,
     ExportInfoTypeDef,
     ExportFilterTypeDef,
     ImportTaskFilterTypeDef,
     ImportTaskTypeDef,
     TagFilterTypeDef,
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
-    ExportConfigurationsResponseTypeDef,
     OrderByElementTypeDef,
-    ListConfigurationsResponseTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartContinuousExportResponseTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    StartExportTaskResponseTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
-    StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeConfigurationsResponseTypeDef,
+    ExportConfigurationsResponseTypeDef,
+    ListConfigurationsResponseTypeDef,
+    StartContinuousExportResponseTypeDef,
+    StartDataCollectionByAgentIdsResponseTypeDef,
+    StartExportTaskResponseTypeDef,
+    StopContinuousExportResponseTypeDef,
+    StopDataCollectionByAgentIdsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DescribeContinuousExportsResponseTypeDef,
     CreateTagsRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
     DescribeAgentsRequestRequestTypeDef,
+    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
+    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
+    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
     DescribeImportTasksRequestRequestTypeDef,
     DescribeImportTasksResponseTypeDef,
     StartImportTaskResponseTypeDef,
```

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/__init__.py` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/__init__.pyi` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/__main__.py` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationDiscoveryService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ApplicationDiscoveryService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService\nOther"
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

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/client.py` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/client.pyi` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/literals.py` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/literals.pyi` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/paginator.py` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -75,45 +75,45 @@
     """
 
     def paginate(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeagentspaginator)
         """
 
 
 class DescribeContinuousExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describecontinuousexportspaginator)
     """
 
     def paginate(
-        self, *, exportIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeContinuousExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describecontinuousexportspaginator)
         """
 
 
 class DescribeExportConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeexportconfigurationspaginator)
     """
 
     def paginate(
-        self, *, exportIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeExportConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeexportconfigurationspaginator)
         """
 
 
@@ -124,15 +124,15 @@
     """
 
     def paginate(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeexporttaskspaginator)
         """
 
 
@@ -142,15 +142,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describetagspaginator)
         """
 
 
@@ -162,13 +162,13 @@
 
     def paginate(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         orderBy: Sequence[OrderByElementTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#listconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/paginator.pyi` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/paginator.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -72,43 +72,43 @@
     """
 
     def paginate(
         self,
         *,
         agentIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAgentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeAgents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeagentspaginator)
         """
 
 class DescribeContinuousExportsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describecontinuousexportspaginator)
     """
 
     def paginate(
-        self, *, exportIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeContinuousExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeContinuousExports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describecontinuousexportspaginator)
         """
 
 class DescribeExportConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeexportconfigurationspaginator)
     """
 
     def paginate(
-        self, *, exportIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, exportIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeExportConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeexportconfigurationspaginator)
         """
 
 class DescribeExportTasksPaginator(Paginator):
@@ -118,15 +118,15 @@
     """
 
     def paginate(
         self,
         *,
         exportIds: Sequence[str] = ...,
         filters: Sequence[ExportFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeExportTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeExportTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describeexporttaskspaginator)
         """
 
 class DescribeTagsPaginator(Paginator):
@@ -135,15 +135,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describetagspaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[TagFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.DescribeTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#describetagspaginator)
         """
 
 class ListConfigurationsPaginator(Paginator):
@@ -154,13 +154,13 @@
 
     def paginate(
         self,
         *,
         configurationType: ConfigurationItemTypeType,
         filters: Sequence[FilterTypeDef] = ...,
         orderBy: Sequence[OrderByElementTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService.Paginator.ListConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/paginators/#listconfigurationspaginator)
         """
```

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/type_defs.py` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -35,72 +35,71 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AgentConfigurationStatusTypeDef",
     "AgentNetworkInfoTypeDef",
     "AssociateConfigurationItemsToApplicationRequestRequestTypeDef",
     "BatchDeleteImportDataErrorTypeDef",
     "BatchDeleteImportDataRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ConfigurationTagTypeDef",
     "ContinuousExportDescriptionTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
     "TagTypeDef",
     "CustomerAgentInfoTypeDef",
     "CustomerAgentlessCollectorInfoTypeDef",
     "CustomerConnectorInfoTypeDef",
     "CustomerMeCollectorInfoTypeDef",
     "DeleteApplicationsRequestRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeConfigurationsRequestRequestTypeDef",
-    "DescribeConfigurationsResponseTypeDef",
-    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
     "DescribeContinuousExportsRequestRequestTypeDef",
-    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
     "DescribeExportConfigurationsRequestRequestTypeDef",
     "ExportInfoTypeDef",
     "ExportFilterTypeDef",
     "ImportTaskFilterTypeDef",
     "ImportTaskTypeDef",
     "TagFilterTypeDef",
     "DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef",
     "ReservedInstanceOptionsTypeDef",
     "UsageMetricBasisTypeDef",
-    "ExportConfigurationsResponseTypeDef",
     "OrderByElementTypeDef",
-    "ListConfigurationsResponseTypeDef",
     "ListServerNeighborsRequestRequestTypeDef",
     "NeighborConnectionDetailTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartContinuousExportResponseTypeDef",
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
-    "StartExportTaskResponseTypeDef",
     "StartImportTaskRequestRequestTypeDef",
     "StopContinuousExportRequestRequestTypeDef",
-    "StopContinuousExportResponseTypeDef",
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "StartDataCollectionByAgentIdsResponseTypeDef",
-    "StopDataCollectionByAgentIdsResponseTypeDef",
     "AgentInfoTypeDef",
     "BatchDeleteImportDataResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "DescribeConfigurationsResponseTypeDef",
+    "ExportConfigurationsResponseTypeDef",
+    "ListConfigurationsResponseTypeDef",
+    "StartContinuousExportResponseTypeDef",
+    "StartDataCollectionByAgentIdsResponseTypeDef",
+    "StartExportTaskResponseTypeDef",
+    "StopContinuousExportResponseTypeDef",
+    "StopDataCollectionByAgentIdsResponseTypeDef",
     "DescribeTagsResponseTypeDef",
     "DescribeContinuousExportsResponseTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "GetDiscoverySummaryResponseTypeDef",
-    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
     "DescribeAgentsRequestRequestTypeDef",
+    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
+    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
     "DescribeExportConfigurationsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     "DescribeExportTasksRequestRequestTypeDef",
     "DescribeImportTasksRequestRequestTypeDef",
     "DescribeImportTasksResponseTypeDef",
     "StartImportTaskResponseTypeDef",
@@ -155,14 +154,25 @@
 BatchDeleteImportDataRequestRequestTypeDef = TypedDict(
     "BatchDeleteImportDataRequestRequestTypeDef",
     {
         "importTaskIds": Sequence[str],
     },
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
 ConfigurationTagTypeDef = TypedDict(
     "ConfigurationTagTypeDef",
     {
         "configurationType": ConfigurationItemTypeType,
         "configurationId": str,
         "key": str,
         "value": str,
@@ -196,29 +206,19 @@
     "_OptionalCreateApplicationRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
@@ -287,57 +287,41 @@
     {
         "name": str,
         "values": Sequence[str],
         "condition": str,
     },
 )
 
-DescribeConfigurationsRequestRequestTypeDef = TypedDict(
-    "DescribeConfigurationsRequestRequestTypeDef",
-    {
-        "configurationIds": Sequence[str],
-    },
-)
-
-DescribeConfigurationsResponseTypeDef = TypedDict(
-    "DescribeConfigurationsResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "configurations": List[Dict[str, str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = TypedDict(
-    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+DescribeConfigurationsRequestRequestTypeDef = TypedDict(
+    "DescribeConfigurationsRequestRequestTypeDef",
     {
-        "exportIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "configurationIds": Sequence[str],
     },
-    total=False,
 )
 
 DescribeContinuousExportsRequestRequestTypeDef = TypedDict(
     "DescribeContinuousExportsRequestRequestTypeDef",
     {
         "exportIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
-    {
-        "exportIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeExportConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeExportConfigurationsRequestRequestTypeDef",
     {
         "exportIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -360,19 +344,17 @@
         "isTruncated": bool,
         "requestedStartTime": datetime,
         "requestedEndTime": datetime,
     },
     total=False,
 )
 
-
 class ExportInfoTypeDef(_RequiredExportInfoTypeDef, _OptionalExportInfoTypeDef):
     pass
 
-
 ExportFilterTypeDef = TypedDict(
     "ExportFilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
         "condition": str,
     },
@@ -437,50 +419,31 @@
     {
         "name": str,
         "percentageAdjust": float,
     },
     total=False,
 )
 
-ExportConfigurationsResponseTypeDef = TypedDict(
-    "ExportConfigurationsResponseTypeDef",
-    {
-        "exportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOrderByElementTypeDef = TypedDict(
     "_RequiredOrderByElementTypeDef",
     {
         "fieldName": str,
     },
 )
 _OptionalOrderByElementTypeDef = TypedDict(
     "_OptionalOrderByElementTypeDef",
     {
         "sortOrder": orderStringType,
     },
     total=False,
 )
 
-
 class OrderByElementTypeDef(_RequiredOrderByElementTypeDef, _OptionalOrderByElementTypeDef):
     pass
 
-
-ListConfigurationsResponseTypeDef = TypedDict(
-    "ListConfigurationsResponseTypeDef",
-    {
-        "configurations": List[Dict[str, str]],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListServerNeighborsRequestRequestTypeDef = TypedDict(
     "_RequiredListServerNeighborsRequestRequestTypeDef",
     {
         "configurationId": str,
     },
 )
 _OptionalListServerNeighborsRequestRequestTypeDef = TypedDict(
@@ -490,22 +453,20 @@
         "neighborConfigurationIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListServerNeighborsRequestRequestTypeDef(
     _RequiredListServerNeighborsRequestRequestTypeDef,
     _OptionalListServerNeighborsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredNeighborConnectionDetailTypeDef = TypedDict(
     "_RequiredNeighborConnectionDetailTypeDef",
     {
         "sourceServerId": str,
         "destinationServerId": str,
         "connectionsCount": int,
     },
@@ -515,69 +476,26 @@
     {
         "destinationPort": int,
         "transportProtocol": str,
     },
     total=False,
 )
 
-
 class NeighborConnectionDetailTypeDef(
     _RequiredNeighborConnectionDetailTypeDef, _OptionalNeighborConnectionDetailTypeDef
 ):
     pass
 
-
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
-StartContinuousExportResponseTypeDef = TypedDict(
-    "StartContinuousExportResponseTypeDef",
-    {
-        "exportId": str,
-        "s3Bucket": str,
-        "startTime": datetime,
-        "dataSource": Literal["AGENT"],
-        "schemaStorageConfig": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
-StartExportTaskResponseTypeDef = TypedDict(
-    "StartExportTaskResponseTypeDef",
-    {
-        "exportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportTaskRequestRequestTypeDef",
     {
         "name": str,
         "importUrl": str,
     },
 )
@@ -585,37 +503,26 @@
     "_OptionalStartImportTaskRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
-
 class StartImportTaskRequestRequestTypeDef(
     _RequiredStartImportTaskRequestRequestTypeDef, _OptionalStartImportTaskRequestRequestTypeDef
 ):
     pass
 
-
 StopContinuousExportRequestRequestTypeDef = TypedDict(
     "StopContinuousExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
-StopContinuousExportResponseTypeDef = TypedDict(
-    "StopContinuousExportResponseTypeDef",
-    {
-        "startTime": datetime,
-        "stopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
@@ -630,37 +537,19 @@
     {
         "name": str,
         "description": str,
     },
     total=False,
 )
 
-
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-
-StartDataCollectionByAgentIdsResponseTypeDef = TypedDict(
-    "StartDataCollectionByAgentIdsResponseTypeDef",
-    {
-        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StopDataCollectionByAgentIdsResponseTypeDef = TypedDict(
-    "StopDataCollectionByAgentIdsResponseTypeDef",
-    {
-        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AgentInfoTypeDef = TypedDict(
     "AgentInfoTypeDef",
     {
         "agentId": str,
         "hostName": str,
         "agentNetworkInfoList": List[AgentNetworkInfoTypeDef],
         "connectorId": str,
@@ -674,33 +563,111 @@
     total=False,
 )
 
 BatchDeleteImportDataResponseTypeDef = TypedDict(
     "BatchDeleteImportDataResponseTypeDef",
     {
         "errors": List[BatchDeleteImportDataErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationsResponseTypeDef = TypedDict(
+    "DescribeConfigurationsResponseTypeDef",
+    {
+        "configurations": List[Dict[str, str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportConfigurationsResponseTypeDef = TypedDict(
+    "ExportConfigurationsResponseTypeDef",
+    {
+        "exportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationsResponseTypeDef = TypedDict(
+    "ListConfigurationsResponseTypeDef",
+    {
+        "configurations": List[Dict[str, str]],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartContinuousExportResponseTypeDef = TypedDict(
+    "StartContinuousExportResponseTypeDef",
+    {
+        "exportId": str,
+        "s3Bucket": str,
+        "startTime": datetime,
+        "dataSource": Literal["AGENT"],
+        "schemaStorageConfig": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDataCollectionByAgentIdsResponseTypeDef = TypedDict(
+    "StartDataCollectionByAgentIdsResponseTypeDef",
+    {
+        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExportTaskResponseTypeDef = TypedDict(
+    "StartExportTaskResponseTypeDef",
+    {
+        "exportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopContinuousExportResponseTypeDef = TypedDict(
+    "StopContinuousExportResponseTypeDef",
+    {
+        "startTime": datetime,
+        "stopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDataCollectionByAgentIdsResponseTypeDef = TypedDict(
+    "StopDataCollectionByAgentIdsResponseTypeDef",
+    {
+        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "tags": List[ConfigurationTagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousExportsResponseTypeDef = TypedDict(
     "DescribeContinuousExportsResponseTypeDef",
     {
         "descriptions": List[ContinuousExportDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "configurationIds": Sequence[str],
@@ -718,81 +685,97 @@
     "_OptionalDeleteTagsRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class DeleteTagsRequestRequestTypeDef(
     _RequiredDeleteTagsRequestRequestTypeDef, _OptionalDeleteTagsRequestRequestTypeDef
 ):
     pass
 
-
 GetDiscoverySummaryResponseTypeDef = TypedDict(
     "GetDiscoverySummaryResponseTypeDef",
     {
         "servers": int,
         "applications": int,
         "serversMappedToApplications": int,
         "serversMappedtoTags": int,
         "agentSummary": CustomerAgentInfoTypeDef,
         "connectorSummary": CustomerConnectorInfoTypeDef,
         "meCollectorSummary": CustomerMeCollectorInfoTypeDef,
         "agentlessCollectorSummary": CustomerAgentlessCollectorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAgentsRequestDescribeAgentsPaginateTypeDef = TypedDict(
-    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
+DescribeAgentsRequestRequestTypeDef = TypedDict(
+    "DescribeAgentsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "maxResults": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-DescribeAgentsRequestRequestTypeDef = TypedDict(
-    "DescribeAgentsRequestRequestTypeDef",
+DescribeAgentsRequestDescribeAgentsPaginateTypeDef = TypedDict(
+    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
     {
         "agentIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
-        "maxResults": int,
-        "nextToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = TypedDict(
+    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+    {
+        "exportIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
+    {
+        "exportIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeExportConfigurationsResponseTypeDef = TypedDict(
     "DescribeExportConfigurationsResponseTypeDef",
     {
         "exportsInfo": List[ExportInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportTasksResponseTypeDef = TypedDict(
     "DescribeExportTasksResponseTypeDef",
     {
         "exportsInfo": List[ExportInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
     "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     {
         "exportIds": Sequence[str],
         "filters": Sequence[ExportFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeExportTasksRequestRequestTypeDef = TypedDict(
     "DescribeExportTasksRequestRequestTypeDef",
     {
@@ -815,31 +798,31 @@
 )
 
 DescribeImportTasksResponseTypeDef = TypedDict(
     "DescribeImportTasksResponseTypeDef",
     {
         "nextToken": str,
         "tasks": List[ImportTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportTaskResponseTypeDef = TypedDict(
     "StartImportTaskResponseTypeDef",
     {
         "task": ImportTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     {
         "filters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
@@ -871,27 +854,25 @@
     },
 )
 _OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
     "_OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
         "orderBy": Sequence[OrderByElementTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListConfigurationsRequestListConfigurationsPaginateTypeDef(
     _RequiredListConfigurationsRequestListConfigurationsPaginateTypeDef,
     _OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListConfigurationsRequestRequestTypeDef",
     {
         "configurationType": ConfigurationItemTypeType,
     },
 )
 _OptionalListConfigurationsRequestRequestTypeDef = TypedDict(
@@ -901,38 +882,36 @@
         "maxResults": int,
         "nextToken": str,
         "orderBy": Sequence[OrderByElementTypeDef],
     },
     total=False,
 )
 
-
 class ListConfigurationsRequestRequestTypeDef(
     _RequiredListConfigurationsRequestRequestTypeDef,
     _OptionalListConfigurationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListServerNeighborsResponseTypeDef = TypedDict(
     "ListServerNeighborsResponseTypeDef",
     {
         "neighbors": List[NeighborConnectionDetailTypeDef],
         "nextToken": str,
         "knownDependencyCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAgentsResponseTypeDef = TypedDict(
     "DescribeAgentsResponseTypeDef",
     {
         "agentsInfo": List[AgentInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportPreferencesTypeDef = TypedDict(
     "ExportPreferencesTypeDef",
     {
         "ec2RecommendationsPreferences": Ec2RecommendationsExportPreferencesTypeDef,
```

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery/type_defs.pyi` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,71 +35,72 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AgentConfigurationStatusTypeDef",
     "AgentNetworkInfoTypeDef",
     "AssociateConfigurationItemsToApplicationRequestRequestTypeDef",
     "BatchDeleteImportDataErrorTypeDef",
     "BatchDeleteImportDataRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ConfigurationTagTypeDef",
     "ContinuousExportDescriptionTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
     "TagTypeDef",
     "CustomerAgentInfoTypeDef",
     "CustomerAgentlessCollectorInfoTypeDef",
     "CustomerConnectorInfoTypeDef",
     "CustomerMeCollectorInfoTypeDef",
     "DeleteApplicationsRequestRequestTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeConfigurationsRequestRequestTypeDef",
-    "DescribeConfigurationsResponseTypeDef",
-    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
     "DescribeContinuousExportsRequestRequestTypeDef",
-    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
     "DescribeExportConfigurationsRequestRequestTypeDef",
     "ExportInfoTypeDef",
     "ExportFilterTypeDef",
     "ImportTaskFilterTypeDef",
     "ImportTaskTypeDef",
     "TagFilterTypeDef",
     "DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef",
     "ReservedInstanceOptionsTypeDef",
     "UsageMetricBasisTypeDef",
-    "ExportConfigurationsResponseTypeDef",
     "OrderByElementTypeDef",
-    "ListConfigurationsResponseTypeDef",
     "ListServerNeighborsRequestRequestTypeDef",
     "NeighborConnectionDetailTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartContinuousExportResponseTypeDef",
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
-    "StartExportTaskResponseTypeDef",
     "StartImportTaskRequestRequestTypeDef",
     "StopContinuousExportRequestRequestTypeDef",
-    "StopContinuousExportResponseTypeDef",
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "StartDataCollectionByAgentIdsResponseTypeDef",
-    "StopDataCollectionByAgentIdsResponseTypeDef",
     "AgentInfoTypeDef",
     "BatchDeleteImportDataResponseTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "DescribeConfigurationsResponseTypeDef",
+    "ExportConfigurationsResponseTypeDef",
+    "ListConfigurationsResponseTypeDef",
+    "StartContinuousExportResponseTypeDef",
+    "StartDataCollectionByAgentIdsResponseTypeDef",
+    "StartExportTaskResponseTypeDef",
+    "StopContinuousExportResponseTypeDef",
+    "StopDataCollectionByAgentIdsResponseTypeDef",
     "DescribeTagsResponseTypeDef",
     "DescribeContinuousExportsResponseTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "GetDiscoverySummaryResponseTypeDef",
-    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
     "DescribeAgentsRequestRequestTypeDef",
+    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
+    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
     "DescribeExportConfigurationsResponseTypeDef",
     "DescribeExportTasksResponseTypeDef",
     "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     "DescribeExportTasksRequestRequestTypeDef",
     "DescribeImportTasksRequestRequestTypeDef",
     "DescribeImportTasksResponseTypeDef",
     "StartImportTaskResponseTypeDef",
@@ -154,14 +155,25 @@
 BatchDeleteImportDataRequestRequestTypeDef = TypedDict(
     "BatchDeleteImportDataRequestRequestTypeDef",
     {
         "importTaskIds": Sequence[str],
     },
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
 ConfigurationTagTypeDef = TypedDict(
     "ConfigurationTagTypeDef",
     {
         "configurationType": ConfigurationItemTypeType,
         "configurationId": str,
         "key": str,
         "value": str,
@@ -195,26 +207,20 @@
     "_OptionalCreateApplicationRequestRequestTypeDef",
     {
         "description": str,
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "configurationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
@@ -284,57 +290,41 @@
     {
         "name": str,
         "values": Sequence[str],
         "condition": str,
     },
 )
 
-DescribeConfigurationsRequestRequestTypeDef = TypedDict(
-    "DescribeConfigurationsRequestRequestTypeDef",
-    {
-        "configurationIds": Sequence[str],
-    },
-)
-
-DescribeConfigurationsResponseTypeDef = TypedDict(
-    "DescribeConfigurationsResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "configurations": List[Dict[str, str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = TypedDict(
-    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+DescribeConfigurationsRequestRequestTypeDef = TypedDict(
+    "DescribeConfigurationsRequestRequestTypeDef",
     {
-        "exportIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "configurationIds": Sequence[str],
     },
-    total=False,
 )
 
 DescribeContinuousExportsRequestRequestTypeDef = TypedDict(
     "DescribeContinuousExportsRequestRequestTypeDef",
     {
         "exportIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
-    {
-        "exportIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeExportConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeExportConfigurationsRequestRequestTypeDef",
     {
         "exportIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -357,17 +347,19 @@
         "isTruncated": bool,
         "requestedStartTime": datetime,
         "requestedEndTime": datetime,
     },
     total=False,
 )
 
+
 class ExportInfoTypeDef(_RequiredExportInfoTypeDef, _OptionalExportInfoTypeDef):
     pass
 
+
 ExportFilterTypeDef = TypedDict(
     "ExportFilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
         "condition": str,
     },
@@ -432,47 +424,32 @@
     {
         "name": str,
         "percentageAdjust": float,
     },
     total=False,
 )
 
-ExportConfigurationsResponseTypeDef = TypedDict(
-    "ExportConfigurationsResponseTypeDef",
-    {
-        "exportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredOrderByElementTypeDef = TypedDict(
     "_RequiredOrderByElementTypeDef",
     {
         "fieldName": str,
     },
 )
 _OptionalOrderByElementTypeDef = TypedDict(
     "_OptionalOrderByElementTypeDef",
     {
         "sortOrder": orderStringType,
     },
     total=False,
 )
 
+
 class OrderByElementTypeDef(_RequiredOrderByElementTypeDef, _OptionalOrderByElementTypeDef):
     pass
 
-ListConfigurationsResponseTypeDef = TypedDict(
-    "ListConfigurationsResponseTypeDef",
-    {
-        "configurations": List[Dict[str, str]],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredListServerNeighborsRequestRequestTypeDef = TypedDict(
     "_RequiredListServerNeighborsRequestRequestTypeDef",
     {
         "configurationId": str,
     },
 )
@@ -483,20 +460,22 @@
         "neighborConfigurationIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListServerNeighborsRequestRequestTypeDef(
     _RequiredListServerNeighborsRequestRequestTypeDef,
     _OptionalListServerNeighborsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredNeighborConnectionDetailTypeDef = TypedDict(
     "_RequiredNeighborConnectionDetailTypeDef",
     {
         "sourceServerId": str,
         "destinationServerId": str,
         "connectionsCount": int,
     },
@@ -506,67 +485,28 @@
     {
         "destinationPort": int,
         "transportProtocol": str,
     },
     total=False,
 )
 
+
 class NeighborConnectionDetailTypeDef(
     _RequiredNeighborConnectionDetailTypeDef, _OptionalNeighborConnectionDetailTypeDef
 ):
     pass
 
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
-StartContinuousExportResponseTypeDef = TypedDict(
-    "StartContinuousExportResponseTypeDef",
-    {
-        "exportId": str,
-        "s3Bucket": str,
-        "startTime": datetime,
-        "dataSource": Literal["AGENT"],
-        "schemaStorageConfig": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 StartDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StartDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
-StartExportTaskResponseTypeDef = TypedDict(
-    "StartExportTaskResponseTypeDef",
-    {
-        "exportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartImportTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartImportTaskRequestRequestTypeDef",
     {
         "name": str,
         "importUrl": str,
     },
 )
@@ -574,35 +514,28 @@
     "_OptionalStartImportTaskRequestRequestTypeDef",
     {
         "clientRequestToken": str,
     },
     total=False,
 )
 
+
 class StartImportTaskRequestRequestTypeDef(
     _RequiredStartImportTaskRequestRequestTypeDef, _OptionalStartImportTaskRequestRequestTypeDef
 ):
     pass
 
+
 StopContinuousExportRequestRequestTypeDef = TypedDict(
     "StopContinuousExportRequestRequestTypeDef",
     {
         "exportId": str,
     },
 )
 
-StopContinuousExportResponseTypeDef = TypedDict(
-    "StopContinuousExportResponseTypeDef",
-    {
-        "startTime": datetime,
-        "stopTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDataCollectionByAgentIdsRequestRequestTypeDef = TypedDict(
     "StopDataCollectionByAgentIdsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
     },
 )
 
@@ -617,34 +550,20 @@
     {
         "name": str,
         "description": str,
     },
     total=False,
 )
 
+
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-StartDataCollectionByAgentIdsResponseTypeDef = TypedDict(
-    "StartDataCollectionByAgentIdsResponseTypeDef",
-    {
-        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StopDataCollectionByAgentIdsResponseTypeDef = TypedDict(
-    "StopDataCollectionByAgentIdsResponseTypeDef",
-    {
-        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 AgentInfoTypeDef = TypedDict(
     "AgentInfoTypeDef",
     {
         "agentId": str,
         "hostName": str,
         "agentNetworkInfoList": List[AgentNetworkInfoTypeDef],
@@ -659,33 +578,111 @@
     total=False,
 )
 
 BatchDeleteImportDataResponseTypeDef = TypedDict(
     "BatchDeleteImportDataResponseTypeDef",
     {
         "errors": List[BatchDeleteImportDataErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "configurationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeConfigurationsResponseTypeDef = TypedDict(
+    "DescribeConfigurationsResponseTypeDef",
+    {
+        "configurations": List[Dict[str, str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportConfigurationsResponseTypeDef = TypedDict(
+    "ExportConfigurationsResponseTypeDef",
+    {
+        "exportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListConfigurationsResponseTypeDef = TypedDict(
+    "ListConfigurationsResponseTypeDef",
+    {
+        "configurations": List[Dict[str, str]],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartContinuousExportResponseTypeDef = TypedDict(
+    "StartContinuousExportResponseTypeDef",
+    {
+        "exportId": str,
+        "s3Bucket": str,
+        "startTime": datetime,
+        "dataSource": Literal["AGENT"],
+        "schemaStorageConfig": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDataCollectionByAgentIdsResponseTypeDef = TypedDict(
+    "StartDataCollectionByAgentIdsResponseTypeDef",
+    {
+        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartExportTaskResponseTypeDef = TypedDict(
+    "StartExportTaskResponseTypeDef",
+    {
+        "exportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopContinuousExportResponseTypeDef = TypedDict(
+    "StopContinuousExportResponseTypeDef",
+    {
+        "startTime": datetime,
+        "stopTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDataCollectionByAgentIdsResponseTypeDef = TypedDict(
+    "StopDataCollectionByAgentIdsResponseTypeDef",
+    {
+        "agentsConfigurationStatus": List[AgentConfigurationStatusTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "tags": List[ConfigurationTagTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeContinuousExportsResponseTypeDef = TypedDict(
     "DescribeContinuousExportsResponseTypeDef",
     {
         "descriptions": List[ContinuousExportDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "configurationIds": Sequence[str],
@@ -703,79 +700,99 @@
     "_OptionalDeleteTagsRequestRequestTypeDef",
     {
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class DeleteTagsRequestRequestTypeDef(
     _RequiredDeleteTagsRequestRequestTypeDef, _OptionalDeleteTagsRequestRequestTypeDef
 ):
     pass
 
+
 GetDiscoverySummaryResponseTypeDef = TypedDict(
     "GetDiscoverySummaryResponseTypeDef",
     {
         "servers": int,
         "applications": int,
         "serversMappedToApplications": int,
         "serversMappedtoTags": int,
         "agentSummary": CustomerAgentInfoTypeDef,
         "connectorSummary": CustomerConnectorInfoTypeDef,
         "meCollectorSummary": CustomerMeCollectorInfoTypeDef,
         "agentlessCollectorSummary": CustomerAgentlessCollectorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAgentsRequestDescribeAgentsPaginateTypeDef = TypedDict(
-    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
+DescribeAgentsRequestRequestTypeDef = TypedDict(
+    "DescribeAgentsRequestRequestTypeDef",
     {
         "agentIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "maxResults": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-DescribeAgentsRequestRequestTypeDef = TypedDict(
-    "DescribeAgentsRequestRequestTypeDef",
+DescribeAgentsRequestDescribeAgentsPaginateTypeDef = TypedDict(
+    "DescribeAgentsRequestDescribeAgentsPaginateTypeDef",
     {
         "agentIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
-        "maxResults": int,
-        "nextToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef = TypedDict(
+    "DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef",
+    {
+        "exportIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef",
+    {
+        "exportIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeExportConfigurationsResponseTypeDef = TypedDict(
     "DescribeExportConfigurationsResponseTypeDef",
     {
         "exportsInfo": List[ExportInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportTasksResponseTypeDef = TypedDict(
     "DescribeExportTasksResponseTypeDef",
     {
         "exportsInfo": List[ExportInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef = TypedDict(
     "DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef",
     {
         "exportIds": Sequence[str],
         "filters": Sequence[ExportFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeExportTasksRequestRequestTypeDef = TypedDict(
     "DescribeExportTasksRequestRequestTypeDef",
     {
@@ -798,31 +815,31 @@
 )
 
 DescribeImportTasksResponseTypeDef = TypedDict(
     "DescribeImportTasksResponseTypeDef",
     {
         "nextToken": str,
         "tasks": List[ImportTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartImportTaskResponseTypeDef = TypedDict(
     "StartImportTaskResponseTypeDef",
     {
         "task": ImportTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
     "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     {
         "filters": Sequence[TagFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeTagsRequestRequestTypeDef = TypedDict(
     "DescribeTagsRequestRequestTypeDef",
     {
@@ -854,25 +871,27 @@
     },
 )
 _OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef = TypedDict(
     "_OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef",
     {
         "filters": Sequence[FilterTypeDef],
         "orderBy": Sequence[OrderByElementTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListConfigurationsRequestListConfigurationsPaginateTypeDef(
     _RequiredListConfigurationsRequestListConfigurationsPaginateTypeDef,
     _OptionalListConfigurationsRequestListConfigurationsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListConfigurationsRequestRequestTypeDef = TypedDict(
     "_RequiredListConfigurationsRequestRequestTypeDef",
     {
         "configurationType": ConfigurationItemTypeType,
     },
 )
 _OptionalListConfigurationsRequestRequestTypeDef = TypedDict(
@@ -882,36 +901,38 @@
         "maxResults": int,
         "nextToken": str,
         "orderBy": Sequence[OrderByElementTypeDef],
     },
     total=False,
 )
 
+
 class ListConfigurationsRequestRequestTypeDef(
     _RequiredListConfigurationsRequestRequestTypeDef,
     _OptionalListConfigurationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListServerNeighborsResponseTypeDef = TypedDict(
     "ListServerNeighborsResponseTypeDef",
     {
         "neighbors": List[NeighborConnectionDetailTypeDef],
         "nextToken": str,
         "knownDependencyCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAgentsResponseTypeDef = TypedDict(
     "DescribeAgentsResponseTypeDef",
     {
         "agentsInfo": List[AgentInfoTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportPreferencesTypeDef = TypedDict(
     "ExportPreferencesTypeDef",
     {
         "ec2RecommendationsPreferences": Ec2RecommendationsExportPreferencesTypeDef,
```

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/PKG-INFO` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-discovery
-Version: 1.28.12
-Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-discovery.svg?color=blue)](https://pypi.org/project/mypy-boto3-discovery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-discovery)](https://pepy.tech/project/mypy-boto3-discovery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationDiscoveryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
+[boto3.ApplicationDiscoveryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/discovery.html#ApplicationDiscoveryService)
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
 [mypy-boto3-discovery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_discovery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -363,65 +363,65 @@
 ```python
 from mypy_boto3_discovery.type_defs import (
     AgentConfigurationStatusTypeDef,
     AgentNetworkInfoTypeDef,
     AssociateConfigurationItemsToApplicationRequestRequestTypeDef,
     BatchDeleteImportDataErrorTypeDef,
     BatchDeleteImportDataRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ConfigurationTagTypeDef,
     ContinuousExportDescriptionTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
     TagTypeDef,
     CustomerAgentInfoTypeDef,
     CustomerAgentlessCollectorInfoTypeDef,
     CustomerConnectorInfoTypeDef,
     CustomerMeCollectorInfoTypeDef,
     DeleteApplicationsRequestRequestTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     DescribeConfigurationsRequestRequestTypeDef,
-    DescribeConfigurationsResponseTypeDef,
-    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
     DescribeContinuousExportsRequestRequestTypeDef,
-    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsRequestRequestTypeDef,
     ExportInfoTypeDef,
     ExportFilterTypeDef,
     ImportTaskFilterTypeDef,
     ImportTaskTypeDef,
     TagFilterTypeDef,
     DisassociateConfigurationItemsFromApplicationRequestRequestTypeDef,
     ReservedInstanceOptionsTypeDef,
     UsageMetricBasisTypeDef,
-    ExportConfigurationsResponseTypeDef,
     OrderByElementTypeDef,
-    ListConfigurationsResponseTypeDef,
     ListServerNeighborsRequestRequestTypeDef,
     NeighborConnectionDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartContinuousExportResponseTypeDef,
     StartDataCollectionByAgentIdsRequestRequestTypeDef,
-    StartExportTaskResponseTypeDef,
     StartImportTaskRequestRequestTypeDef,
     StopContinuousExportRequestRequestTypeDef,
-    StopContinuousExportResponseTypeDef,
     StopDataCollectionByAgentIdsRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
-    StartDataCollectionByAgentIdsResponseTypeDef,
-    StopDataCollectionByAgentIdsResponseTypeDef,
     AgentInfoTypeDef,
     BatchDeleteImportDataResponseTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeConfigurationsResponseTypeDef,
+    ExportConfigurationsResponseTypeDef,
+    ListConfigurationsResponseTypeDef,
+    StartContinuousExportResponseTypeDef,
+    StartDataCollectionByAgentIdsResponseTypeDef,
+    StartExportTaskResponseTypeDef,
+    StopContinuousExportResponseTypeDef,
+    StopDataCollectionByAgentIdsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DescribeContinuousExportsResponseTypeDef,
     CreateTagsRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     GetDiscoverySummaryResponseTypeDef,
-    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
     DescribeAgentsRequestRequestTypeDef,
+    DescribeAgentsRequestDescribeAgentsPaginateTypeDef,
+    DescribeContinuousExportsRequestDescribeContinuousExportsPaginateTypeDef,
+    DescribeExportConfigurationsRequestDescribeExportConfigurationsPaginateTypeDef,
     DescribeExportConfigurationsResponseTypeDef,
     DescribeExportTasksResponseTypeDef,
     DescribeExportTasksRequestDescribeExportTasksPaginateTypeDef,
     DescribeExportTasksRequestRequestTypeDef,
     DescribeImportTasksRequestRequestTypeDef,
     DescribeImportTasksResponseTypeDef,
     StartImportTaskResponseTypeDef,
```

### Comparing `mypy-boto3-discovery-1.28.12/mypy_boto3_discovery.egg-info/SOURCES.txt` & `mypy-boto3-discovery-1.28.15/mypy_boto3_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-discovery-1.28.12/setup.py` & `mypy-boto3-discovery-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-discovery",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_discovery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationDiscoveryService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ApplicationDiscoveryService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

