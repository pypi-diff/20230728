# Comparing `tmp/mypy-boto3-athena-1.28.12.tar.gz` & `tmp/mypy-boto3-athena-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-athena-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
+gzip compressed data, was "mypy-boto3-athena-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
```

## Comparing `mypy-boto3-athena-1.28.12.tar` & `mypy-boto3-athena-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-athena-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21381 2023-07-27 05:34:20.584572 mypy-boto3-athena-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19898 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.580572 mypy-boto3-athena-1.28.12/mypy_boto3_athena/
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46117 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    67186 2023-07-27 05:17:43.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    67091 2023-07-27 05:17:42.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21381 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:20.000000 mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.584572 mypy-boto3-athena-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:17:41.000000 mypy-boto3-athena-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-athena-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-07-28 20:42:19.228695 mypy-boto3-athena-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19494 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.220695 mypy-boto3-athena-1.28.15/mypy_boto3_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46117 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46035 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10516 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-07-28 20:19:47.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63549 2023-07-28 20:19:49.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63458 2023-07-28 20:19:48.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:19.000000 mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.228695 mypy-boto3-athena-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:19:46.000000 mypy-boto3-athena-1.28.15/setup.py
```

### Comparing `mypy-boto3-athena-1.28.12/LICENSE` & `mypy-boto3-athena-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.12/PKG-INFO` & `mypy-boto3-athena-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.28.12
-Summary: Type annotations for boto3.Athena 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,20 +358,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
-    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
@@ -382,188 +382,178 @@
     CapacityAllocationTypeDef,
     CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
-    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
-    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
-    CustomerContentEncryptionConfigurationOutputTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
-    EngineVersionOutputTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
     GetCapacityAssignmentConfigurationInputRequestTypeDef,
     GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
-    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
     ListCapacityReservationsInputRequestTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
-    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
-    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     ListWorkGroupsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryExecutionContextOutputTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
-    ResponseMetadataTypeDef,
-    ResultReuseByAgeConfigurationOutputTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
-    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
+    CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
+    ListNamedQueriesOutputTypeDef,
+    ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
     PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
-    ResultConfigurationOutputTypeDef,
-    SessionConfigurationTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
+    SessionConfigurationTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
-    ResultReuseConfigurationOutputTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
-    WorkGroupConfigurationOutputTypeDef,
-    GetSessionResponseTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
+    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
     ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
-    WorkGroupTypeDef,
     CreateWorkGroupInputRequestTypeDef,
+    WorkGroupTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationOutputTypeDef:
+def get_structure() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.12/README.md` & `mypy-boto3-athena-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,20 +326,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
-    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
@@ -350,188 +350,178 @@
     CapacityAllocationTypeDef,
     CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
-    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
-    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
-    CustomerContentEncryptionConfigurationOutputTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
-    EngineVersionOutputTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
     GetCapacityAssignmentConfigurationInputRequestTypeDef,
     GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
-    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
     ListCapacityReservationsInputRequestTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
-    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
-    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     ListWorkGroupsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryExecutionContextOutputTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
-    ResponseMetadataTypeDef,
-    ResultReuseByAgeConfigurationOutputTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
-    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
+    CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
+    ListNamedQueriesOutputTypeDef,
+    ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
     PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
-    ResultConfigurationOutputTypeDef,
-    SessionConfigurationTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
+    SessionConfigurationTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
-    ResultReuseConfigurationOutputTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
-    WorkGroupConfigurationOutputTypeDef,
-    GetSessionResponseTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
+    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
     ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
-    WorkGroupTypeDef,
     CreateWorkGroupInputRequestTypeDef,
+    WorkGroupTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationOutputTypeDef:
+def get_structure() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/__init__.py` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/__init__.pyi` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/__main__.py` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Athena 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Athena 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
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

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/client.py` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/client.pyi` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/literals.py` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/literals.pyi` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/paginator.py` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,75 +70,75 @@
 class GetQueryResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#getqueryresultspaginator)
     """
 
     def paginate(
-        self, *, QueryExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetQueryResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#getqueryresultspaginator)
         """
 
 
 class ListDataCatalogsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatacatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCatalogsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatacatalogspaginator)
         """
 
 
 class ListDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatabasespaginator)
     """
 
     def paginate(
-        self, *, CatalogName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CatalogName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatabasespaginator)
         """
 
 
 class ListNamedQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listnamedqueriespaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNamedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listnamedqueriespaginator)
         """
 
 
 class ListQueryExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listqueryexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueryExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listqueryexecutionspaginator)
         """
 
 
@@ -150,28 +150,28 @@
 
     def paginate(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTableMetadataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtablemetadatapaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/paginator.pyi` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,71 +67,71 @@
 class GetQueryResultsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#getqueryresultspaginator)
     """
 
     def paginate(
-        self, *, QueryExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetQueryResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#getqueryresultspaginator)
         """
 
 class ListDataCatalogsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatacatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataCatalogsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatacatalogspaginator)
         """
 
 class ListDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatabasespaginator)
     """
 
     def paginate(
-        self, *, CatalogName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CatalogName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listdatabasespaginator)
         """
 
 class ListNamedQueriesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listnamedqueriespaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNamedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listnamedqueriespaginator)
         """
 
 class ListQueryExecutionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listqueryexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListQueryExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listqueryexecutionspaginator)
         """
 
 class ListTableMetadataPaginator(Paginator):
@@ -142,27 +142,27 @@
 
     def paginate(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTableMetadataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtablemetadatapaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/type_defs.py` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for athena service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_athena.type_defs import AclConfigurationOutputTypeDef
+    from mypy_boto3_athena.type_defs import AclConfigurationTypeDef
 
-    data: AclConfigurationOutputTypeDef = {...}
+    data: AclConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -37,20 +37,20 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AclConfigurationOutputTypeDef",
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
     "PreparedStatementTypeDef",
     "UnprocessedPreparedStatementNameTypeDef",
     "BatchGetQueryExecutionInputRequestTypeDef",
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
@@ -61,193 +61,176 @@
     "CapacityAllocationTypeDef",
     "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
-    "CreateNamedQueryOutputTypeDef",
     "CreateNotebookInputRequestTypeDef",
-    "CreateNotebookOutputTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    "CustomerContentEncryptionConfigurationOutputTypeDef",
     "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
-    "EngineVersionOutputTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
-    "GetCalculationExecutionCodeResponseTypeDef",
     "GetCalculationExecutionRequestRequestTypeDef",
     "GetCalculationExecutionStatusRequestRequestTypeDef",
     "GetCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetCapacityReservationInputRequestTypeDef",
     "GetDataCatalogInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetNamedQueryInputRequestTypeDef",
     "GetNotebookMetadataInputRequestTypeDef",
     "GetPreparedStatementInputRequestTypeDef",
     "GetQueryExecutionInputRequestTypeDef",
-    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetQueryResultsInputRequestTypeDef",
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
     "SessionStatisticsTypeDef",
     "SessionStatusTypeDef",
     "GetSessionStatusRequestRequestTypeDef",
     "GetTableMetadataInputRequestTypeDef",
     "GetWorkGroupInputRequestTypeDef",
     "ImportNotebookInputRequestTypeDef",
-    "ImportNotebookOutputTypeDef",
     "ListApplicationDPUSizesInputRequestTypeDef",
     "ListCalculationExecutionsRequestRequestTypeDef",
     "ListCapacityReservationsInputRequestTypeDef",
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
     "ListDataCatalogsInputRequestTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListEngineVersionsInputRequestTypeDef",
     "ListExecutorsRequestRequestTypeDef",
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
     "ListNamedQueriesInputRequestTypeDef",
-    "ListNamedQueriesOutputTypeDef",
     "ListNotebookSessionsRequestRequestTypeDef",
     "NotebookSessionSummaryTypeDef",
     "ListPreparedStatementsInputRequestTypeDef",
     "PreparedStatementSummaryTypeDef",
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
     "ListQueryExecutionsInputRequestTypeDef",
-    "ListQueryExecutionsOutputTypeDef",
     "ListSessionsRequestRequestTypeDef",
-    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTableMetadataInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "QueryExecutionContextOutputTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
-    "ResponseMetadataTypeDef",
-    "ResultReuseByAgeConfigurationOutputTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
-    "StartCalculationExecutionResponseTypeDef",
-    "StartQueryExecutionOutputTypeDef",
-    "StartSessionResponseTypeDef",
     "StopCalculationExecutionRequestRequestTypeDef",
-    "StopCalculationExecutionResponseTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
-    "TerminateSessionResponseTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCapacityReservationInputRequestTypeDef",
     "UpdateDataCatalogInputRequestTypeDef",
     "UpdateNamedQueryInputRequestTypeDef",
     "UpdateNotebookInputRequestTypeDef",
     "UpdateNotebookMetadataInputRequestTypeDef",
     "UpdatePreparedStatementInputRequestTypeDef",
-    "ListApplicationDPUSizesOutputTypeDef",
     "QueryExecutionStatusTypeDef",
+    "CreateNamedQueryOutputTypeDef",
+    "CreateNotebookOutputTypeDef",
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    "GetCalculationExecutionCodeResponseTypeDef",
     "GetNamedQueryOutputTypeDef",
+    "ImportNotebookOutputTypeDef",
+    "ListApplicationDPUSizesOutputTypeDef",
+    "ListNamedQueriesOutputTypeDef",
+    "ListQueryExecutionsOutputTypeDef",
+    "StartCalculationExecutionResponseTypeDef",
+    "StartQueryExecutionOutputTypeDef",
+    "StartSessionResponseTypeDef",
+    "StopCalculationExecutionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
     "BatchGetNamedQueryOutputTypeDef",
     "GetPreparedStatementOutputTypeDef",
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
     "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
-    "ResultConfigurationOutputTypeDef",
-    "SessionConfigurationTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
+    "SessionConfigurationTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataInputRequestTypeDef",
+    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "GetSessionStatusResponseTypeDef",
     "SessionSummaryTypeDef",
     "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
-    "ResultReuseConfigurationOutputTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
-    "WorkGroupConfigurationOutputTypeDef",
-    "GetSessionResponseTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
+    "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
     "ListSessionsResponseTypeDef",
     "GetQueryRuntimeStatisticsOutputTypeDef",
     "QueryExecutionTypeDef",
     "StartQueryExecutionInputRequestTypeDef",
     "GetQueryResultsOutputTypeDef",
-    "WorkGroupTypeDef",
     "CreateWorkGroupInputRequestTypeDef",
+    "WorkGroupTypeDef",
     "UpdateWorkGroupInputRequestTypeDef",
     "BatchGetQueryExecutionOutputTypeDef",
     "GetQueryExecutionOutputTypeDef",
     "GetWorkGroupOutputTypeDef",
 )
 
-AclConfigurationOutputTypeDef = TypedDict(
-    "AclConfigurationOutputTypeDef",
-    {
-        "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
-    },
-)
-
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
     },
 )
 
@@ -297,14 +280,25 @@
 )
 
 
 class NamedQueryTypeDef(_RequiredNamedQueryTypeDef, _OptionalNamedQueryTypeDef):
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
 UnprocessedNamedQueryIdTypeDef = TypedDict(
     "UnprocessedNamedQueryIdTypeDef",
     {
         "NamedQueryId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -520,22 +514,14 @@
 
 class CreateNamedQueryInputRequestTypeDef(
     _RequiredCreateNamedQueryInputRequestTypeDef, _OptionalCreateNamedQueryInputRequestTypeDef
 ):
     pass
 
 
-CreateNamedQueryOutputTypeDef = TypedDict(
-    "CreateNamedQueryOutputTypeDef",
-    {
-        "NamedQueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateNotebookInputRequestTypeDef = TypedDict(
     "_RequiredCreateNotebookInputRequestTypeDef",
     {
         "WorkGroup": str,
         "Name": str,
     },
 )
@@ -550,22 +536,14 @@
 
 class CreateNotebookInputRequestTypeDef(
     _RequiredCreateNotebookInputRequestTypeDef, _OptionalCreateNotebookInputRequestTypeDef
 ):
     pass
 
 
-CreateNotebookOutputTypeDef = TypedDict(
-    "CreateNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredCreatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -589,31 +567,14 @@
 CreatePresignedNotebookUrlRequestRequestTypeDef = TypedDict(
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    {
-        "NotebookUrl": str,
-        "AuthToken": str,
-        "AuthTokenExpirationTime": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CustomerContentEncryptionConfigurationOutputTypeDef = TypedDict(
-    "CustomerContentEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKey": str,
-    },
-)
-
 CustomerContentEncryptionConfigurationTypeDef = TypedDict(
     "CustomerContentEncryptionConfigurationTypeDef",
     {
         "KmsKey": str,
     },
 )
 
@@ -728,35 +689,14 @@
 
 class DeleteWorkGroupInputRequestTypeDef(
     _RequiredDeleteWorkGroupInputRequestTypeDef, _OptionalDeleteWorkGroupInputRequestTypeDef
 ):
     pass
 
 
-_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigurationOutputTypeDef",
-    {
-        "EncryptionOption": EncryptionOptionType,
-    },
-)
-_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKey": str,
-    },
-    total=False,
-)
-
-
-class EncryptionConfigurationOutputTypeDef(
-    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "EncryptionOption": EncryptionOptionType,
     },
 )
 _OptionalEncryptionConfigurationTypeDef = TypedDict(
@@ -818,23 +758,14 @@
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
 ):
     pass
 
 
-EngineVersionOutputTypeDef = TypedDict(
-    "EngineVersionOutputTypeDef",
-    {
-        "SelectedEngineVersion": str,
-        "EffectiveEngineVersion": str,
-    },
-    total=False,
-)
-
 EngineVersionTypeDef = TypedDict(
     "EngineVersionTypeDef",
     {
         "SelectedEngineVersion": str,
         "EffectiveEngineVersion": str,
     },
     total=False,
@@ -894,22 +825,14 @@
 GetCalculationExecutionCodeRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionCodeRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
-GetCalculationExecutionCodeResponseTypeDef = TypedDict(
-    "GetCalculationExecutionCodeResponseTypeDef",
-    {
-        "CodeBlock": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCalculationExecutionRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
@@ -974,36 +897,24 @@
 GetQueryExecutionInputRequestTypeDef = TypedDict(
     "GetQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
-_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    {
-        "QueryExecutionId": str,
-    },
-)
-_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
-    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetQueryResultsInputRequestTypeDef = TypedDict(
     "_RequiredGetQueryResultsInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 _OptionalGetQueryResultsInputRequestTypeDef = TypedDict(
@@ -1100,22 +1011,14 @@
 
 class ImportNotebookInputRequestTypeDef(
     _RequiredImportNotebookInputRequestTypeDef, _OptionalImportNotebookInputRequestTypeDef
 ):
     pass
 
 
-ImportNotebookOutputTypeDef = TypedDict(
-    "ImportNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListApplicationDPUSizesInputRequestTypeDef = TypedDict(
     "ListApplicationDPUSizesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1150,53 +1053,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataCatalogsInputRequestTypeDef = TypedDict(
     "ListDataCatalogsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "CatalogName": str,
-    },
-)
-_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatabasesInputListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatabasesInputRequestTypeDef = TypedDict(
     "_RequiredListDatabasesInputRequestTypeDef",
     {
         "CatalogName": str,
     },
 )
 _OptionalListDatabasesInputRequestTypeDef = TypedDict(
@@ -1243,42 +1116,24 @@
 
 class ListExecutorsRequestRequestTypeDef(
     _RequiredListExecutorsRequestRequestTypeDef, _OptionalListExecutorsRequestRequestTypeDef
 ):
     pass
 
 
-ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNamedQueriesInputRequestTypeDef = TypedDict(
     "ListNamedQueriesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
-ListNamedQueriesOutputTypeDef = TypedDict(
-    "ListNamedQueriesOutputTypeDef",
-    {
-        "NamedQueryIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListNotebookSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListNotebookSessionsRequestRequestTypeDef",
     {
         "NotebookId": str,
     },
 )
 _OptionalListNotebookSessionsRequestRequestTypeDef = TypedDict(
@@ -1335,42 +1190,24 @@
     {
         "StatementName": str,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueryExecutionsInputRequestTypeDef = TypedDict(
     "ListQueryExecutionsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
-ListQueryExecutionsOutputTypeDef = TypedDict(
-    "ListQueryExecutionsOutputTypeDef",
-    {
-        "QueryExecutionIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSessionsRequestRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 _OptionalListSessionsRequestRequestTypeDef = TypedDict(
@@ -1386,38 +1223,14 @@
 
 class ListSessionsRequestRequestTypeDef(
     _RequiredListSessionsRequestRequestTypeDef, _OptionalListSessionsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "CatalogName": str,
-        "DatabaseName": str,
-    },
-)
-_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "Expression": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTableMetadataInputListTableMetadataPaginateTypeDef(
-    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
-    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTableMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
     },
 )
@@ -1434,36 +1247,14 @@
 
 class ListTableMetadataInputRequestTypeDef(
     _RequiredListTableMetadataInputRequestTypeDef, _OptionalListTableMetadataInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1478,51 +1269,23 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 ListWorkGroupsInputRequestTypeDef = TypedDict(
     "ListWorkGroupsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
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
-QueryExecutionContextOutputTypeDef = TypedDict(
-    "QueryExecutionContextOutputTypeDef",
-    {
-        "Database": str,
-        "Catalog": str,
-    },
-    total=False,
-)
-
 QueryExecutionContextTypeDef = TypedDict(
     "QueryExecutionContextTypeDef",
     {
         "Database": str,
         "Catalog": str,
     },
     total=False,
@@ -1581,47 +1344,14 @@
         "ExecutionTime": int,
         "QueryStagePlan": "QueryStagePlanNodeTypeDef",
         "SubStages": List[Dict[str, Any]],
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
-_RequiredResultReuseByAgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredResultReuseByAgeConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalResultReuseByAgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalResultReuseByAgeConfigurationOutputTypeDef",
-    {
-        "MaxAgeInMinutes": int,
-    },
-    total=False,
-)
-
-
-class ResultReuseByAgeConfigurationOutputTypeDef(
-    _RequiredResultReuseByAgeConfigurationOutputTypeDef,
-    _OptionalResultReuseByAgeConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredResultReuseByAgeConfigurationTypeDef = TypedDict(
     "_RequiredResultReuseByAgeConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResultReuseByAgeConfigurationTypeDef = TypedDict(
@@ -1635,77 +1365,35 @@
 
 class ResultReuseByAgeConfigurationTypeDef(
     _RequiredResultReuseByAgeConfigurationTypeDef, _OptionalResultReuseByAgeConfigurationTypeDef
 ):
     pass
 
 
-StartCalculationExecutionResponseTypeDef = TypedDict(
-    "StartCalculationExecutionResponseTypeDef",
-    {
-        "CalculationExecutionId": str,
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartQueryExecutionOutputTypeDef = TypedDict(
-    "StartQueryExecutionOutputTypeDef",
-    {
-        "QueryExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "State": SessionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopCalculationExecutionRequestRequestTypeDef = TypedDict(
     "StopCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
-StopCalculationExecutionResponseTypeDef = TypedDict(
-    "StopCalculationExecutionResponseTypeDef",
-    {
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopQueryExecutionInputRequestTypeDef = TypedDict(
     "StopQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "State": SessionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1831,66 +1519,168 @@
 class UpdatePreparedStatementInputRequestTypeDef(
     _RequiredUpdatePreparedStatementInputRequestTypeDef,
     _OptionalUpdatePreparedStatementInputRequestTypeDef,
 ):
     pass
 
 
-ListApplicationDPUSizesOutputTypeDef = TypedDict(
-    "ListApplicationDPUSizesOutputTypeDef",
-    {
-        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 QueryExecutionStatusTypeDef = TypedDict(
     "QueryExecutionStatusTypeDef",
     {
         "State": QueryExecutionStateType,
         "StateChangeReason": str,
         "SubmissionDateTime": datetime,
         "CompletionDateTime": datetime,
         "AthenaError": AthenaErrorTypeDef,
     },
     total=False,
 )
 
+CreateNamedQueryOutputTypeDef = TypedDict(
+    "CreateNamedQueryOutputTypeDef",
+    {
+        "NamedQueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNotebookOutputTypeDef = TypedDict(
+    "CreateNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    {
+        "NotebookUrl": str,
+        "AuthToken": str,
+        "AuthTokenExpirationTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculationExecutionCodeResponseTypeDef = TypedDict(
+    "GetCalculationExecutionCodeResponseTypeDef",
+    {
+        "CodeBlock": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetNamedQueryOutputTypeDef = TypedDict(
     "GetNamedQueryOutputTypeDef",
     {
         "NamedQuery": NamedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportNotebookOutputTypeDef = TypedDict(
+    "ImportNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationDPUSizesOutputTypeDef = TypedDict(
+    "ListApplicationDPUSizesOutputTypeDef",
+    {
+        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNamedQueriesOutputTypeDef = TypedDict(
+    "ListNamedQueriesOutputTypeDef",
+    {
+        "NamedQueryIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueryExecutionsOutputTypeDef = TypedDict(
+    "ListQueryExecutionsOutputTypeDef",
+    {
+        "QueryExecutionIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCalculationExecutionResponseTypeDef = TypedDict(
+    "StartCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryExecutionOutputTypeDef = TypedDict(
+    "StartQueryExecutionOutputTypeDef",
+    {
+        "QueryExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopCalculationExecutionResponseTypeDef = TypedDict(
+    "StopCalculationExecutionResponseTypeDef",
+    {
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetNamedQueryOutputTypeDef = TypedDict(
     "BatchGetNamedQueryOutputTypeDef",
     {
         "NamedQueries": List[NamedQueryTypeDef],
         "UnprocessedNamedQueryIds": List[UnprocessedNamedQueryIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPreparedStatementOutputTypeDef = TypedDict(
     "GetPreparedStatementOutputTypeDef",
     {
         "PreparedStatement": PreparedStatementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetPreparedStatementOutputTypeDef = TypedDict(
     "BatchGetPreparedStatementOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementTypeDef],
         "UnprocessedPreparedStatementNames": List[UnprocessedPreparedStatementNameTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartCalculationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCalculationExecutionRequestRequestTypeDef",
     {
         "SessionId": str,
@@ -1931,24 +1721,24 @@
         "CalculationExecutionId": str,
         "SessionId": str,
         "Description": str,
         "WorkingDirectory": str,
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
         "Result": CalculationResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCalculationExecutionStatusResponseTypeDef = TypedDict(
     "GetCalculationExecutionStatusResponseTypeDef",
     {
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCapacityReservationTypeDef = TypedDict(
     "_RequiredCapacityReservationTypeDef",
     {
         "Name": str,
@@ -2066,86 +1856,73 @@
 
 class CreateDataCatalogInputRequestTypeDef(
     _RequiredCreateDataCatalogInputRequestTypeDef, _OptionalCreateDataCatalogInputRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListDataCatalogsOutputTypeDef = TypedDict(
     "ListDataCatalogsOutputTypeDef",
     {
         "DataCatalogsSummary": List[DataCatalogSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCatalogOutputTypeDef = TypedDict(
     "GetDataCatalogOutputTypeDef",
     {
         "DataCatalog": DataCatalogTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List[DatumTypeDef],
     },
     total=False,
 )
 
-ResultConfigurationOutputTypeDef = TypedDict(
-    "ResultConfigurationOutputTypeDef",
-    {
-        "OutputLocation": str,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "ExpectedBucketOwner": str,
-        "AclConfiguration": AclConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-SessionConfigurationTypeDef = TypedDict(
-    "SessionConfigurationTypeDef",
-    {
-        "ExecutionRole": str,
-        "WorkingDirectory": str,
-        "IdleTimeoutSeconds": int,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ResultConfigurationTypeDef = TypedDict(
     "ResultConfigurationTypeDef",
     {
         "OutputLocation": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "ExpectedBucketOwner": str,
         "AclConfiguration": AclConfigurationTypeDef,
@@ -2164,14 +1941,25 @@
         "RemoveExpectedBucketOwner": bool,
         "AclConfiguration": AclConfigurationTypeDef,
         "RemoveAclConfiguration": bool,
     },
     total=False,
 )
 
+SessionConfigurationTypeDef = TypedDict(
+    "SessionConfigurationTypeDef",
+    {
+        "ExecutionRole": str,
+        "WorkingDirectory": str,
+        "IdleTimeoutSeconds": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -2192,65 +1980,65 @@
 ):
     pass
 
 
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
-        "EngineVersions": List[EngineVersionOutputTypeDef],
+        "EngineVersions": List[EngineVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": str,
         "State": WorkGroupStateType,
         "Description": str,
         "CreationTime": datetime,
-        "EngineVersion": EngineVersionOutputTypeDef,
+        "EngineVersion": EngineVersionTypeDef,
     },
     total=False,
 )
 
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
         "SessionId": str,
         "NextToken": str,
         "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportNotebookOutputTypeDef = TypedDict(
     "ExportNotebookOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
         "Payload": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNotebookMetadataOutputTypeDef = TypedDict(
     "GetNotebookMetadataOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotebookMetadataOutputTypeDef = TypedDict(
     "ListNotebookMetadataOutputTypeDef",
     {
         "NextToken": str,
         "NotebookMetadataList": List[NotebookMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListNotebookMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListNotebookMetadataInputRequestTypeDef",
     {
         "WorkGroup": str,
@@ -2270,59 +2058,166 @@
 class ListNotebookMetadataInputRequestTypeDef(
     _RequiredListNotebookMetadataInputRequestTypeDef,
     _OptionalListNotebookMetadataInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "QueryExecutionId": str,
+    },
+)
+_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
+    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+):
+    pass
+
+
+ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "CatalogName": str,
+    },
+)
+_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatabasesInputListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
+):
+    pass
+
+
+ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "CatalogName": str,
+        "DatabaseName": str,
+    },
+)
+_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "Expression": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTableMetadataInputListTableMetadataPaginateTypeDef(
+    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
+    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 GetSessionStatusResponseTypeDef = TypedDict(
     "GetSessionStatusResponseTypeDef",
     {
         "SessionId": str,
         "Status": SessionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "SessionId": str,
         "Description": str,
-        "EngineVersion": EngineVersionOutputTypeDef,
+        "EngineVersion": EngineVersionTypeDef,
         "NotebookVersion": str,
         "Status": SessionStatusTypeDef,
     },
     total=False,
 )
 
 ListNotebookSessionsResponseTypeDef = TypedDict(
     "ListNotebookSessionsResponseTypeDef",
     {
         "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": int,
@@ -2343,125 +2238,82 @@
         "Timeline": QueryRuntimeStatisticsTimelineTypeDef,
         "Rows": QueryRuntimeStatisticsRowsTypeDef,
         "OutputStage": "QueryStageTypeDef",
     },
     total=False,
 )
 
-ResultReuseConfigurationOutputTypeDef = TypedDict(
-    "ResultReuseConfigurationOutputTypeDef",
-    {
-        "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ResultReuseConfigurationTypeDef = TypedDict(
     "ResultReuseConfigurationTypeDef",
     {
         "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationTypeDef,
     },
     total=False,
 )
 
 ListCalculationExecutionsResponseTypeDef = TypedDict(
     "ListCalculationExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "Calculations": List[CalculationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCapacityReservationOutputTypeDef = TypedDict(
     "GetCapacityReservationOutputTypeDef",
     {
         "CapacityReservation": CapacityReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCapacityReservationsOutputTypeDef = TypedDict(
     "ListCapacityReservationsOutputTypeDef",
     {
         "NextToken": str,
         "CapacityReservations": List[CapacityReservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCapacityAssignmentConfigurationOutputTypeDef = TypedDict(
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTableMetadataOutputTypeDef = TypedDict(
     "ListTableMetadataOutputTypeDef",
     {
         "TableMetadataList": List[TableMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "Rows": List[RowTypeDef],
         "ResultSetMetadata": ResultSetMetadataTypeDef,
     },
     total=False,
 )
 
-WorkGroupConfigurationOutputTypeDef = TypedDict(
-    "WorkGroupConfigurationOutputTypeDef",
-    {
-        "ResultConfiguration": ResultConfigurationOutputTypeDef,
-        "EnforceWorkGroupConfiguration": bool,
-        "PublishCloudWatchMetricsEnabled": bool,
-        "BytesScannedCutoffPerQuery": int,
-        "RequesterPaysEnabled": bool,
-        "EngineVersion": EngineVersionOutputTypeDef,
-        "AdditionalConfiguration": str,
-        "ExecutionRole": str,
-        "CustomerContentEncryptionConfiguration": (
-            CustomerContentEncryptionConfigurationOutputTypeDef
-        ),
-        "EnableMinimumEncryptionConfiguration": bool,
-    },
-    total=False,
-)
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "Description": str,
-        "WorkGroup": str,
-        "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationOutputTypeDef,
-        "NotebookVersion": str,
-        "SessionConfiguration": SessionConfigurationTypeDef,
-        "Status": SessionStatusTypeDef,
-        "Statistics": SessionStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkGroupConfigurationTypeDef = TypedDict(
     "WorkGroupConfigurationTypeDef",
     {
         "ResultConfiguration": ResultConfigurationTypeDef,
         "EnforceWorkGroupConfiguration": bool,
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
@@ -2490,53 +2342,69 @@
         "ExecutionRole": str,
         "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
         "EnableMinimumEncryptionConfiguration": bool,
     },
     total=False,
 )
 
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "Description": str,
+        "WorkGroup": str,
+        "EngineVersion": str,
+        "EngineConfiguration": EngineConfigurationOutputTypeDef,
+        "NotebookVersion": str,
+        "SessionConfiguration": SessionConfigurationTypeDef,
+        "Status": SessionStatusTypeDef,
+        "Statistics": SessionStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
         "NextToken": str,
         "Sessions": List[SessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryExecutionTypeDef = TypedDict(
     "QueryExecutionTypeDef",
     {
         "QueryExecutionId": str,
         "Query": str,
         "StatementType": StatementTypeType,
-        "ResultConfiguration": ResultConfigurationOutputTypeDef,
-        "ResultReuseConfiguration": ResultReuseConfigurationOutputTypeDef,
-        "QueryExecutionContext": QueryExecutionContextOutputTypeDef,
+        "ResultConfiguration": ResultConfigurationTypeDef,
+        "ResultReuseConfiguration": ResultReuseConfigurationTypeDef,
+        "QueryExecutionContext": QueryExecutionContextTypeDef,
         "Status": QueryExecutionStatusTypeDef,
         "Statistics": QueryExecutionStatisticsTypeDef,
         "WorkGroup": str,
-        "EngineVersion": EngineVersionOutputTypeDef,
+        "EngineVersion": EngineVersionTypeDef,
         "ExecutionParameters": List[str],
         "SubstatementType": str,
     },
     total=False,
 )
 
 _RequiredStartQueryExecutionInputRequestTypeDef = TypedDict(
@@ -2567,60 +2435,60 @@
 
 GetQueryResultsOutputTypeDef = TypedDict(
     "GetQueryResultsOutputTypeDef",
     {
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredWorkGroupTypeDef = TypedDict(
-    "_RequiredWorkGroupTypeDef",
+_RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalWorkGroupTypeDef = TypedDict(
-    "_OptionalWorkGroupTypeDef",
+_OptionalCreateWorkGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkGroupInputRequestTypeDef",
     {
-        "State": WorkGroupStateType,
-        "Configuration": WorkGroupConfigurationOutputTypeDef,
+        "Configuration": WorkGroupConfigurationTypeDef,
         "Description": str,
-        "CreationTime": datetime,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class WorkGroupTypeDef(_RequiredWorkGroupTypeDef, _OptionalWorkGroupTypeDef):
+class CreateWorkGroupInputRequestTypeDef(
+    _RequiredCreateWorkGroupInputRequestTypeDef, _OptionalCreateWorkGroupInputRequestTypeDef
+):
     pass
 
 
-_RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkGroupInputRequestTypeDef",
+_RequiredWorkGroupTypeDef = TypedDict(
+    "_RequiredWorkGroupTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalCreateWorkGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkGroupInputRequestTypeDef",
+_OptionalWorkGroupTypeDef = TypedDict(
+    "_OptionalWorkGroupTypeDef",
     {
+        "State": WorkGroupStateType,
         "Configuration": WorkGroupConfigurationTypeDef,
         "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "CreationTime": datetime,
     },
     total=False,
 )
 
 
-class CreateWorkGroupInputRequestTypeDef(
-    _RequiredCreateWorkGroupInputRequestTypeDef, _OptionalCreateWorkGroupInputRequestTypeDef
-):
+class WorkGroupTypeDef(_RequiredWorkGroupTypeDef, _OptionalWorkGroupTypeDef):
     pass
 
 
 _RequiredUpdateWorkGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkGroupInputRequestTypeDef",
     {
         "WorkGroup": str,
@@ -2644,26 +2512,26 @@
 
 
 BatchGetQueryExecutionOutputTypeDef = TypedDict(
     "BatchGetQueryExecutionOutputTypeDef",
     {
         "QueryExecutions": List[QueryExecutionTypeDef],
         "UnprocessedQueryExecutionIds": List[UnprocessedQueryExecutionIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryExecutionOutputTypeDef = TypedDict(
     "GetQueryExecutionOutputTypeDef",
     {
         "QueryExecution": QueryExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkGroupOutputTypeDef = TypedDict(
     "GetWorkGroupOutputTypeDef",
     {
         "WorkGroup": WorkGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena/type_defs.pyi` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for athena service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_athena.type_defs import AclConfigurationOutputTypeDef
+    from mypy_boto3_athena.type_defs import AclConfigurationTypeDef
 
-    data: AclConfigurationOutputTypeDef = {...}
+    data: AclConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -36,20 +36,20 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AclConfigurationOutputTypeDef",
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
     "PreparedStatementTypeDef",
     "UnprocessedPreparedStatementNameTypeDef",
     "BatchGetQueryExecutionInputRequestTypeDef",
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
@@ -60,193 +60,176 @@
     "CapacityAllocationTypeDef",
     "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
-    "CreateNamedQueryOutputTypeDef",
     "CreateNotebookInputRequestTypeDef",
-    "CreateNotebookOutputTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    "CustomerContentEncryptionConfigurationOutputTypeDef",
     "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "EncryptionConfigurationTypeDef",
     "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
-    "EngineVersionOutputTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
-    "GetCalculationExecutionCodeResponseTypeDef",
     "GetCalculationExecutionRequestRequestTypeDef",
     "GetCalculationExecutionStatusRequestRequestTypeDef",
     "GetCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetCapacityReservationInputRequestTypeDef",
     "GetDataCatalogInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetNamedQueryInputRequestTypeDef",
     "GetNotebookMetadataInputRequestTypeDef",
     "GetPreparedStatementInputRequestTypeDef",
     "GetQueryExecutionInputRequestTypeDef",
-    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetQueryResultsInputRequestTypeDef",
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
     "SessionStatisticsTypeDef",
     "SessionStatusTypeDef",
     "GetSessionStatusRequestRequestTypeDef",
     "GetTableMetadataInputRequestTypeDef",
     "GetWorkGroupInputRequestTypeDef",
     "ImportNotebookInputRequestTypeDef",
-    "ImportNotebookOutputTypeDef",
     "ListApplicationDPUSizesInputRequestTypeDef",
     "ListCalculationExecutionsRequestRequestTypeDef",
     "ListCapacityReservationsInputRequestTypeDef",
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
     "ListDataCatalogsInputRequestTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListEngineVersionsInputRequestTypeDef",
     "ListExecutorsRequestRequestTypeDef",
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
     "ListNamedQueriesInputRequestTypeDef",
-    "ListNamedQueriesOutputTypeDef",
     "ListNotebookSessionsRequestRequestTypeDef",
     "NotebookSessionSummaryTypeDef",
     "ListPreparedStatementsInputRequestTypeDef",
     "PreparedStatementSummaryTypeDef",
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
     "ListQueryExecutionsInputRequestTypeDef",
-    "ListQueryExecutionsOutputTypeDef",
     "ListSessionsRequestRequestTypeDef",
-    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTableMetadataInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "QueryExecutionContextOutputTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
-    "ResponseMetadataTypeDef",
-    "ResultReuseByAgeConfigurationOutputTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
-    "StartCalculationExecutionResponseTypeDef",
-    "StartQueryExecutionOutputTypeDef",
-    "StartSessionResponseTypeDef",
     "StopCalculationExecutionRequestRequestTypeDef",
-    "StopCalculationExecutionResponseTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
-    "TerminateSessionResponseTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCapacityReservationInputRequestTypeDef",
     "UpdateDataCatalogInputRequestTypeDef",
     "UpdateNamedQueryInputRequestTypeDef",
     "UpdateNotebookInputRequestTypeDef",
     "UpdateNotebookMetadataInputRequestTypeDef",
     "UpdatePreparedStatementInputRequestTypeDef",
-    "ListApplicationDPUSizesOutputTypeDef",
     "QueryExecutionStatusTypeDef",
+    "CreateNamedQueryOutputTypeDef",
+    "CreateNotebookOutputTypeDef",
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    "GetCalculationExecutionCodeResponseTypeDef",
     "GetNamedQueryOutputTypeDef",
+    "ImportNotebookOutputTypeDef",
+    "ListApplicationDPUSizesOutputTypeDef",
+    "ListNamedQueriesOutputTypeDef",
+    "ListQueryExecutionsOutputTypeDef",
+    "StartCalculationExecutionResponseTypeDef",
+    "StartQueryExecutionOutputTypeDef",
+    "StartSessionResponseTypeDef",
+    "StopCalculationExecutionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
     "BatchGetNamedQueryOutputTypeDef",
     "GetPreparedStatementOutputTypeDef",
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
     "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
-    "ResultConfigurationOutputTypeDef",
-    "SessionConfigurationTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
+    "SessionConfigurationTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataInputRequestTypeDef",
+    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "GetSessionStatusResponseTypeDef",
     "SessionSummaryTypeDef",
     "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
-    "ResultReuseConfigurationOutputTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
-    "WorkGroupConfigurationOutputTypeDef",
-    "GetSessionResponseTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
+    "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
     "ListSessionsResponseTypeDef",
     "GetQueryRuntimeStatisticsOutputTypeDef",
     "QueryExecutionTypeDef",
     "StartQueryExecutionInputRequestTypeDef",
     "GetQueryResultsOutputTypeDef",
-    "WorkGroupTypeDef",
     "CreateWorkGroupInputRequestTypeDef",
+    "WorkGroupTypeDef",
     "UpdateWorkGroupInputRequestTypeDef",
     "BatchGetQueryExecutionOutputTypeDef",
     "GetQueryExecutionOutputTypeDef",
     "GetWorkGroupOutputTypeDef",
 )
 
-AclConfigurationOutputTypeDef = TypedDict(
-    "AclConfigurationOutputTypeDef",
-    {
-        "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
-    },
-)
-
 AclConfigurationTypeDef = TypedDict(
     "AclConfigurationTypeDef",
     {
         "S3AclOption": Literal["BUCKET_OWNER_FULL_CONTROL"],
     },
 )
 
@@ -294,14 +277,25 @@
     },
     total=False,
 )
 
 class NamedQueryTypeDef(_RequiredNamedQueryTypeDef, _OptionalNamedQueryTypeDef):
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
 UnprocessedNamedQueryIdTypeDef = TypedDict(
     "UnprocessedNamedQueryIdTypeDef",
     {
         "NamedQueryId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -509,22 +503,14 @@
 )
 
 class CreateNamedQueryInputRequestTypeDef(
     _RequiredCreateNamedQueryInputRequestTypeDef, _OptionalCreateNamedQueryInputRequestTypeDef
 ):
     pass
 
-CreateNamedQueryOutputTypeDef = TypedDict(
-    "CreateNamedQueryOutputTypeDef",
-    {
-        "NamedQueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateNotebookInputRequestTypeDef = TypedDict(
     "_RequiredCreateNotebookInputRequestTypeDef",
     {
         "WorkGroup": str,
         "Name": str,
     },
 )
@@ -537,22 +523,14 @@
 )
 
 class CreateNotebookInputRequestTypeDef(
     _RequiredCreateNotebookInputRequestTypeDef, _OptionalCreateNotebookInputRequestTypeDef
 ):
     pass
 
-CreateNotebookOutputTypeDef = TypedDict(
-    "CreateNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredCreatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -574,31 +552,14 @@
 CreatePresignedNotebookUrlRequestRequestTypeDef = TypedDict(
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    {
-        "NotebookUrl": str,
-        "AuthToken": str,
-        "AuthTokenExpirationTime": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CustomerContentEncryptionConfigurationOutputTypeDef = TypedDict(
-    "CustomerContentEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKey": str,
-    },
-)
-
 CustomerContentEncryptionConfigurationTypeDef = TypedDict(
     "CustomerContentEncryptionConfigurationTypeDef",
     {
         "KmsKey": str,
     },
 )
 
@@ -707,33 +668,14 @@
 )
 
 class DeleteWorkGroupInputRequestTypeDef(
     _RequiredDeleteWorkGroupInputRequestTypeDef, _OptionalDeleteWorkGroupInputRequestTypeDef
 ):
     pass
 
-_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigurationOutputTypeDef",
-    {
-        "EncryptionOption": EncryptionOptionType,
-    },
-)
-_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigurationOutputTypeDef",
-    {
-        "KmsKey": str,
-    },
-    total=False,
-)
-
-class EncryptionConfigurationOutputTypeDef(
-    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredEncryptionConfigurationTypeDef = TypedDict(
     "_RequiredEncryptionConfigurationTypeDef",
     {
         "EncryptionOption": EncryptionOptionType,
     },
 )
 _OptionalEncryptionConfigurationTypeDef = TypedDict(
@@ -789,23 +731,14 @@
 )
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
 ):
     pass
 
-EngineVersionOutputTypeDef = TypedDict(
-    "EngineVersionOutputTypeDef",
-    {
-        "SelectedEngineVersion": str,
-        "EffectiveEngineVersion": str,
-    },
-    total=False,
-)
-
 EngineVersionTypeDef = TypedDict(
     "EngineVersionTypeDef",
     {
         "SelectedEngineVersion": str,
         "EffectiveEngineVersion": str,
     },
     total=False,
@@ -863,22 +796,14 @@
 GetCalculationExecutionCodeRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionCodeRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
-GetCalculationExecutionCodeResponseTypeDef = TypedDict(
-    "GetCalculationExecutionCodeResponseTypeDef",
-    {
-        "CodeBlock": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCalculationExecutionRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
@@ -943,34 +868,24 @@
 GetQueryExecutionInputRequestTypeDef = TypedDict(
     "GetQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
-_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    {
-        "QueryExecutionId": str,
-    },
-)
-_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
-    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetQueryResultsInputRequestTypeDef = TypedDict(
     "_RequiredGetQueryResultsInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 _OptionalGetQueryResultsInputRequestTypeDef = TypedDict(
@@ -1063,22 +978,14 @@
 )
 
 class ImportNotebookInputRequestTypeDef(
     _RequiredImportNotebookInputRequestTypeDef, _OptionalImportNotebookInputRequestTypeDef
 ):
     pass
 
-ImportNotebookOutputTypeDef = TypedDict(
-    "ImportNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListApplicationDPUSizesInputRequestTypeDef = TypedDict(
     "ListApplicationDPUSizesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1111,51 +1018,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataCatalogsInputRequestTypeDef = TypedDict(
     "ListDataCatalogsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "CatalogName": str,
-    },
-)
-_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatabasesInputListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatabasesInputRequestTypeDef = TypedDict(
     "_RequiredListDatabasesInputRequestTypeDef",
     {
         "CatalogName": str,
     },
 )
 _OptionalListDatabasesInputRequestTypeDef = TypedDict(
@@ -1198,42 +1077,24 @@
 )
 
 class ListExecutorsRequestRequestTypeDef(
     _RequiredListExecutorsRequestRequestTypeDef, _OptionalListExecutorsRequestRequestTypeDef
 ):
     pass
 
-ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNamedQueriesInputRequestTypeDef = TypedDict(
     "ListNamedQueriesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
-ListNamedQueriesOutputTypeDef = TypedDict(
-    "ListNamedQueriesOutputTypeDef",
-    {
-        "NamedQueryIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListNotebookSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListNotebookSessionsRequestRequestTypeDef",
     {
         "NotebookId": str,
     },
 )
 _OptionalListNotebookSessionsRequestRequestTypeDef = TypedDict(
@@ -1286,42 +1147,24 @@
     {
         "StatementName": str,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueryExecutionsInputRequestTypeDef = TypedDict(
     "ListQueryExecutionsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
-ListQueryExecutionsOutputTypeDef = TypedDict(
-    "ListQueryExecutionsOutputTypeDef",
-    {
-        "QueryExecutionIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSessionsRequestRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 _OptionalListSessionsRequestRequestTypeDef = TypedDict(
@@ -1335,36 +1178,14 @@
 )
 
 class ListSessionsRequestRequestTypeDef(
     _RequiredListSessionsRequestRequestTypeDef, _OptionalListSessionsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "CatalogName": str,
-        "DatabaseName": str,
-    },
-)
-_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "Expression": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTableMetadataInputListTableMetadataPaginateTypeDef(
-    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
-    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
-):
-    pass
-
 _RequiredListTableMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
     },
 )
@@ -1379,34 +1200,14 @@
 )
 
 class ListTableMetadataInputRequestTypeDef(
     _RequiredListTableMetadataInputRequestTypeDef, _OptionalListTableMetadataInputRequestTypeDef
 ):
     pass
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1419,51 +1220,23 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 ListWorkGroupsInputRequestTypeDef = TypedDict(
     "ListWorkGroupsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
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
-QueryExecutionContextOutputTypeDef = TypedDict(
-    "QueryExecutionContextOutputTypeDef",
-    {
-        "Database": str,
-        "Catalog": str,
-    },
-    total=False,
-)
-
 QueryExecutionContextTypeDef = TypedDict(
     "QueryExecutionContextTypeDef",
     {
         "Database": str,
         "Catalog": str,
     },
     total=False,
@@ -1522,45 +1295,14 @@
         "ExecutionTime": int,
         "QueryStagePlan": "QueryStagePlanNodeTypeDef",
         "SubStages": List[Dict[str, Any]],
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
-_RequiredResultReuseByAgeConfigurationOutputTypeDef = TypedDict(
-    "_RequiredResultReuseByAgeConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-_OptionalResultReuseByAgeConfigurationOutputTypeDef = TypedDict(
-    "_OptionalResultReuseByAgeConfigurationOutputTypeDef",
-    {
-        "MaxAgeInMinutes": int,
-    },
-    total=False,
-)
-
-class ResultReuseByAgeConfigurationOutputTypeDef(
-    _RequiredResultReuseByAgeConfigurationOutputTypeDef,
-    _OptionalResultReuseByAgeConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredResultReuseByAgeConfigurationTypeDef = TypedDict(
     "_RequiredResultReuseByAgeConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResultReuseByAgeConfigurationTypeDef = TypedDict(
@@ -1572,77 +1314,35 @@
 )
 
 class ResultReuseByAgeConfigurationTypeDef(
     _RequiredResultReuseByAgeConfigurationTypeDef, _OptionalResultReuseByAgeConfigurationTypeDef
 ):
     pass
 
-StartCalculationExecutionResponseTypeDef = TypedDict(
-    "StartCalculationExecutionResponseTypeDef",
-    {
-        "CalculationExecutionId": str,
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartQueryExecutionOutputTypeDef = TypedDict(
-    "StartQueryExecutionOutputTypeDef",
-    {
-        "QueryExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "State": SessionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopCalculationExecutionRequestRequestTypeDef = TypedDict(
     "StopCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
-StopCalculationExecutionResponseTypeDef = TypedDict(
-    "StopCalculationExecutionResponseTypeDef",
-    {
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopQueryExecutionInputRequestTypeDef = TypedDict(
     "StopQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "State": SessionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1758,66 +1458,168 @@
 
 class UpdatePreparedStatementInputRequestTypeDef(
     _RequiredUpdatePreparedStatementInputRequestTypeDef,
     _OptionalUpdatePreparedStatementInputRequestTypeDef,
 ):
     pass
 
-ListApplicationDPUSizesOutputTypeDef = TypedDict(
-    "ListApplicationDPUSizesOutputTypeDef",
-    {
-        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 QueryExecutionStatusTypeDef = TypedDict(
     "QueryExecutionStatusTypeDef",
     {
         "State": QueryExecutionStateType,
         "StateChangeReason": str,
         "SubmissionDateTime": datetime,
         "CompletionDateTime": datetime,
         "AthenaError": AthenaErrorTypeDef,
     },
     total=False,
 )
 
+CreateNamedQueryOutputTypeDef = TypedDict(
+    "CreateNamedQueryOutputTypeDef",
+    {
+        "NamedQueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNotebookOutputTypeDef = TypedDict(
+    "CreateNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    {
+        "NotebookUrl": str,
+        "AuthToken": str,
+        "AuthTokenExpirationTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculationExecutionCodeResponseTypeDef = TypedDict(
+    "GetCalculationExecutionCodeResponseTypeDef",
+    {
+        "CodeBlock": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetNamedQueryOutputTypeDef = TypedDict(
     "GetNamedQueryOutputTypeDef",
     {
         "NamedQuery": NamedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportNotebookOutputTypeDef = TypedDict(
+    "ImportNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationDPUSizesOutputTypeDef = TypedDict(
+    "ListApplicationDPUSizesOutputTypeDef",
+    {
+        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNamedQueriesOutputTypeDef = TypedDict(
+    "ListNamedQueriesOutputTypeDef",
+    {
+        "NamedQueryIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueryExecutionsOutputTypeDef = TypedDict(
+    "ListQueryExecutionsOutputTypeDef",
+    {
+        "QueryExecutionIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCalculationExecutionResponseTypeDef = TypedDict(
+    "StartCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryExecutionOutputTypeDef = TypedDict(
+    "StartQueryExecutionOutputTypeDef",
+    {
+        "QueryExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopCalculationExecutionResponseTypeDef = TypedDict(
+    "StopCalculationExecutionResponseTypeDef",
+    {
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetNamedQueryOutputTypeDef = TypedDict(
     "BatchGetNamedQueryOutputTypeDef",
     {
         "NamedQueries": List[NamedQueryTypeDef],
         "UnprocessedNamedQueryIds": List[UnprocessedNamedQueryIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPreparedStatementOutputTypeDef = TypedDict(
     "GetPreparedStatementOutputTypeDef",
     {
         "PreparedStatement": PreparedStatementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetPreparedStatementOutputTypeDef = TypedDict(
     "BatchGetPreparedStatementOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementTypeDef],
         "UnprocessedPreparedStatementNames": List[UnprocessedPreparedStatementNameTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartCalculationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCalculationExecutionRequestRequestTypeDef",
     {
         "SessionId": str,
@@ -1856,24 +1658,24 @@
         "CalculationExecutionId": str,
         "SessionId": str,
         "Description": str,
         "WorkingDirectory": str,
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
         "Result": CalculationResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCalculationExecutionStatusResponseTypeDef = TypedDict(
     "GetCalculationExecutionStatusResponseTypeDef",
     {
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCapacityReservationTypeDef = TypedDict(
     "_RequiredCapacityReservationTypeDef",
     {
         "Name": str,
@@ -1983,86 +1785,73 @@
 )
 
 class CreateDataCatalogInputRequestTypeDef(
     _RequiredCreateDataCatalogInputRequestTypeDef, _OptionalCreateDataCatalogInputRequestTypeDef
 ):
     pass
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 ListDataCatalogsOutputTypeDef = TypedDict(
     "ListDataCatalogsOutputTypeDef",
     {
         "DataCatalogsSummary": List[DataCatalogSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCatalogOutputTypeDef = TypedDict(
     "GetDataCatalogOutputTypeDef",
     {
         "DataCatalog": DataCatalogTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List[DatumTypeDef],
     },
     total=False,
 )
 
-ResultConfigurationOutputTypeDef = TypedDict(
-    "ResultConfigurationOutputTypeDef",
-    {
-        "OutputLocation": str,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-        "ExpectedBucketOwner": str,
-        "AclConfiguration": AclConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-SessionConfigurationTypeDef = TypedDict(
-    "SessionConfigurationTypeDef",
-    {
-        "ExecutionRole": str,
-        "WorkingDirectory": str,
-        "IdleTimeoutSeconds": int,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ResultConfigurationTypeDef = TypedDict(
     "ResultConfigurationTypeDef",
     {
         "OutputLocation": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
         "ExpectedBucketOwner": str,
         "AclConfiguration": AclConfigurationTypeDef,
@@ -2081,14 +1870,25 @@
         "RemoveExpectedBucketOwner": bool,
         "AclConfiguration": AclConfigurationTypeDef,
         "RemoveAclConfiguration": bool,
     },
     total=False,
 )
 
+SessionConfigurationTypeDef = TypedDict(
+    "SessionConfigurationTypeDef",
+    {
+        "ExecutionRole": str,
+        "WorkingDirectory": str,
+        "IdleTimeoutSeconds": int,
+        "EncryptionConfiguration": EncryptionConfigurationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -2107,65 +1907,65 @@
     _RequiredStartSessionRequestRequestTypeDef, _OptionalStartSessionRequestRequestTypeDef
 ):
     pass
 
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
-        "EngineVersions": List[EngineVersionOutputTypeDef],
+        "EngineVersions": List[EngineVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": str,
         "State": WorkGroupStateType,
         "Description": str,
         "CreationTime": datetime,
-        "EngineVersion": EngineVersionOutputTypeDef,
+        "EngineVersion": EngineVersionTypeDef,
     },
     total=False,
 )
 
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
         "SessionId": str,
         "NextToken": str,
         "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportNotebookOutputTypeDef = TypedDict(
     "ExportNotebookOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
         "Payload": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNotebookMetadataOutputTypeDef = TypedDict(
     "GetNotebookMetadataOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotebookMetadataOutputTypeDef = TypedDict(
     "ListNotebookMetadataOutputTypeDef",
     {
         "NextToken": str,
         "NotebookMetadataList": List[NotebookMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListNotebookMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListNotebookMetadataInputRequestTypeDef",
     {
         "WorkGroup": str,
@@ -2183,59 +1983,158 @@
 
 class ListNotebookMetadataInputRequestTypeDef(
     _RequiredListNotebookMetadataInputRequestTypeDef,
     _OptionalListNotebookMetadataInputRequestTypeDef,
 ):
     pass
 
+_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "QueryExecutionId": str,
+    },
+)
+_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
+    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+):
+    pass
+
+ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "CatalogName": str,
+    },
+)
+_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatabasesInputListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
+):
+    pass
+
+ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "CatalogName": str,
+        "DatabaseName": str,
+    },
+)
+_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "Expression": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTableMetadataInputListTableMetadataPaginateTypeDef(
+    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
+    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 GetSessionStatusResponseTypeDef = TypedDict(
     "GetSessionStatusResponseTypeDef",
     {
         "SessionId": str,
         "Status": SessionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "SessionId": str,
         "Description": str,
-        "EngineVersion": EngineVersionOutputTypeDef,
+        "EngineVersion": EngineVersionTypeDef,
         "NotebookVersion": str,
         "Status": SessionStatusTypeDef,
     },
     total=False,
 )
 
 ListNotebookSessionsResponseTypeDef = TypedDict(
     "ListNotebookSessionsResponseTypeDef",
     {
         "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": int,
@@ -2256,125 +2155,82 @@
         "Timeline": QueryRuntimeStatisticsTimelineTypeDef,
         "Rows": QueryRuntimeStatisticsRowsTypeDef,
         "OutputStage": "QueryStageTypeDef",
     },
     total=False,
 )
 
-ResultReuseConfigurationOutputTypeDef = TypedDict(
-    "ResultReuseConfigurationOutputTypeDef",
-    {
-        "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ResultReuseConfigurationTypeDef = TypedDict(
     "ResultReuseConfigurationTypeDef",
     {
         "ResultReuseByAgeConfiguration": ResultReuseByAgeConfigurationTypeDef,
     },
     total=False,
 )
 
 ListCalculationExecutionsResponseTypeDef = TypedDict(
     "ListCalculationExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "Calculations": List[CalculationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCapacityReservationOutputTypeDef = TypedDict(
     "GetCapacityReservationOutputTypeDef",
     {
         "CapacityReservation": CapacityReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCapacityReservationsOutputTypeDef = TypedDict(
     "ListCapacityReservationsOutputTypeDef",
     {
         "NextToken": str,
         "CapacityReservations": List[CapacityReservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCapacityAssignmentConfigurationOutputTypeDef = TypedDict(
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTableMetadataOutputTypeDef = TypedDict(
     "ListTableMetadataOutputTypeDef",
     {
         "TableMetadataList": List[TableMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "Rows": List[RowTypeDef],
         "ResultSetMetadata": ResultSetMetadataTypeDef,
     },
     total=False,
 )
 
-WorkGroupConfigurationOutputTypeDef = TypedDict(
-    "WorkGroupConfigurationOutputTypeDef",
-    {
-        "ResultConfiguration": ResultConfigurationOutputTypeDef,
-        "EnforceWorkGroupConfiguration": bool,
-        "PublishCloudWatchMetricsEnabled": bool,
-        "BytesScannedCutoffPerQuery": int,
-        "RequesterPaysEnabled": bool,
-        "EngineVersion": EngineVersionOutputTypeDef,
-        "AdditionalConfiguration": str,
-        "ExecutionRole": str,
-        "CustomerContentEncryptionConfiguration": (
-            CustomerContentEncryptionConfigurationOutputTypeDef
-        ),
-        "EnableMinimumEncryptionConfiguration": bool,
-    },
-    total=False,
-)
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "Description": str,
-        "WorkGroup": str,
-        "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationOutputTypeDef,
-        "NotebookVersion": str,
-        "SessionConfiguration": SessionConfigurationTypeDef,
-        "Status": SessionStatusTypeDef,
-        "Statistics": SessionStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WorkGroupConfigurationTypeDef = TypedDict(
     "WorkGroupConfigurationTypeDef",
     {
         "ResultConfiguration": ResultConfigurationTypeDef,
         "EnforceWorkGroupConfiguration": bool,
         "PublishCloudWatchMetricsEnabled": bool,
         "BytesScannedCutoffPerQuery": int,
@@ -2403,53 +2259,69 @@
         "ExecutionRole": str,
         "CustomerContentEncryptionConfiguration": CustomerContentEncryptionConfigurationTypeDef,
         "EnableMinimumEncryptionConfiguration": bool,
     },
     total=False,
 )
 
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "Description": str,
+        "WorkGroup": str,
+        "EngineVersion": str,
+        "EngineConfiguration": EngineConfigurationOutputTypeDef,
+        "NotebookVersion": str,
+        "SessionConfiguration": SessionConfigurationTypeDef,
+        "Status": SessionStatusTypeDef,
+        "Statistics": SessionStatisticsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
         "NextToken": str,
         "Sessions": List[SessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryExecutionTypeDef = TypedDict(
     "QueryExecutionTypeDef",
     {
         "QueryExecutionId": str,
         "Query": str,
         "StatementType": StatementTypeType,
-        "ResultConfiguration": ResultConfigurationOutputTypeDef,
-        "ResultReuseConfiguration": ResultReuseConfigurationOutputTypeDef,
-        "QueryExecutionContext": QueryExecutionContextOutputTypeDef,
+        "ResultConfiguration": ResultConfigurationTypeDef,
+        "ResultReuseConfiguration": ResultReuseConfigurationTypeDef,
+        "QueryExecutionContext": QueryExecutionContextTypeDef,
         "Status": QueryExecutionStatusTypeDef,
         "Statistics": QueryExecutionStatisticsTypeDef,
         "WorkGroup": str,
-        "EngineVersion": EngineVersionOutputTypeDef,
+        "EngineVersion": EngineVersionTypeDef,
         "ExecutionParameters": List[str],
         "SubstatementType": str,
     },
     total=False,
 )
 
 _RequiredStartQueryExecutionInputRequestTypeDef = TypedDict(
@@ -2478,57 +2350,57 @@
 
 GetQueryResultsOutputTypeDef = TypedDict(
     "GetQueryResultsOutputTypeDef",
     {
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredWorkGroupTypeDef = TypedDict(
-    "_RequiredWorkGroupTypeDef",
+_RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalWorkGroupTypeDef = TypedDict(
-    "_OptionalWorkGroupTypeDef",
+_OptionalCreateWorkGroupInputRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkGroupInputRequestTypeDef",
     {
-        "State": WorkGroupStateType,
-        "Configuration": WorkGroupConfigurationOutputTypeDef,
+        "Configuration": WorkGroupConfigurationTypeDef,
         "Description": str,
-        "CreationTime": datetime,
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-class WorkGroupTypeDef(_RequiredWorkGroupTypeDef, _OptionalWorkGroupTypeDef):
+class CreateWorkGroupInputRequestTypeDef(
+    _RequiredCreateWorkGroupInputRequestTypeDef, _OptionalCreateWorkGroupInputRequestTypeDef
+):
     pass
 
-_RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkGroupInputRequestTypeDef",
+_RequiredWorkGroupTypeDef = TypedDict(
+    "_RequiredWorkGroupTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalCreateWorkGroupInputRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkGroupInputRequestTypeDef",
+_OptionalWorkGroupTypeDef = TypedDict(
+    "_OptionalWorkGroupTypeDef",
     {
+        "State": WorkGroupStateType,
         "Configuration": WorkGroupConfigurationTypeDef,
         "Description": str,
-        "Tags": Sequence[TagTypeDef],
+        "CreationTime": datetime,
     },
     total=False,
 )
 
-class CreateWorkGroupInputRequestTypeDef(
-    _RequiredCreateWorkGroupInputRequestTypeDef, _OptionalCreateWorkGroupInputRequestTypeDef
-):
+class WorkGroupTypeDef(_RequiredWorkGroupTypeDef, _OptionalWorkGroupTypeDef):
     pass
 
 _RequiredUpdateWorkGroupInputRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkGroupInputRequestTypeDef",
     {
         "WorkGroup": str,
     },
@@ -2549,26 +2421,26 @@
     pass
 
 BatchGetQueryExecutionOutputTypeDef = TypedDict(
     "BatchGetQueryExecutionOutputTypeDef",
     {
         "QueryExecutions": List[QueryExecutionTypeDef],
         "UnprocessedQueryExecutionIds": List[UnprocessedQueryExecutionIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryExecutionOutputTypeDef = TypedDict(
     "GetQueryExecutionOutputTypeDef",
     {
         "QueryExecution": QueryExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkGroupOutputTypeDef = TypedDict(
     "GetWorkGroupOutputTypeDef",
     {
         "WorkGroup": WorkGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/PKG-INFO` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.28.12
-Summary: Type annotations for boto3.Athena 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,20 +358,20 @@
 ### Typed dictionaries
 
 `mypy_boto3_athena.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_athena.type_defs import (
-    AclConfigurationOutputTypeDef,
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
@@ -382,188 +382,178 @@
     CapacityAllocationTypeDef,
     CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
-    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
-    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
-    CustomerContentEncryptionConfigurationOutputTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     EncryptionConfigurationTypeDef,
     EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
-    EngineVersionOutputTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
     GetCapacityAssignmentConfigurationInputRequestTypeDef,
     GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
-    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
     ListCapacityReservationsInputRequestTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
-    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
-    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
     ListWorkGroupsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    QueryExecutionContextOutputTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
-    ResponseMetadataTypeDef,
-    ResultReuseByAgeConfigurationOutputTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
-    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
+    CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
+    ListNamedQueriesOutputTypeDef,
+    ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
     PutCapacityAssignmentConfigurationInputRequestTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
-    ResultConfigurationOutputTypeDef,
-    SessionConfigurationTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
+    SessionConfigurationTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
-    ResultReuseConfigurationOutputTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
-    WorkGroupConfigurationOutputTypeDef,
-    GetSessionResponseTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
+    GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
     ListSessionsResponseTypeDef,
     GetQueryRuntimeStatisticsOutputTypeDef,
     QueryExecutionTypeDef,
     StartQueryExecutionInputRequestTypeDef,
     GetQueryResultsOutputTypeDef,
-    WorkGroupTypeDef,
     CreateWorkGroupInputRequestTypeDef,
+    WorkGroupTypeDef,
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationOutputTypeDef:
+def get_structure() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-athena-1.28.12/mypy_boto3_athena.egg-info/SOURCES.txt` & `mypy-boto3-athena-1.28.15/mypy_boto3_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-athena-1.28.12/setup.py` & `mypy-boto3-athena-1.28.15/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-athena",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Athena 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Athena 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

