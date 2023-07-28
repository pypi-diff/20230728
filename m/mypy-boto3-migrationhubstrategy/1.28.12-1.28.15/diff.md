# Comparing `tmp/mypy-boto3-migrationhubstrategy-1.28.12.tar.gz` & `tmp/mypy-boto3-migrationhubstrategy-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
+gzip compressed data, was "mypy-boto3-migrationhubstrategy-1.28.15.tar", last modified: Fri Jul 28 20:43:20 2023, max compression
```

## Comparing `mypy-boto3-migrationhubstrategy-1.28.12.tar` & `mypy-boto3-migrationhubstrategy-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.120430 mypy-boto3-migrationhubstrategy-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-27 05:35:04.120430 mypy-boto3-migrationhubstrategy-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17786 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.116430 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-27 05:26:43.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-27 05:26:43.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    35121 2023-07-27 05:26:45.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-07-27 05:26:45.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.120430 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19340 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 05:35:03.000000 mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.120430 mypy-boto3-migrationhubstrategy-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-27 05:26:42.000000 mypy-boto3-migrationhubstrategy-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.841550 mypy-boto3-migrationhubstrategy-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19266 2023-07-28 20:43:20.841550 mypy-boto3-migrationhubstrategy-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17712 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.825550 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20788 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20755 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15739 2023-07-28 20:32:06.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15737 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7248 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    34508 2023-07-28 20:32:09.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34497 2023-07-28 20:32:06.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:20.841550 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19266 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-28 20:43:20.000000 mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:20.841550 mypy-boto3-migrationhubstrategy-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-28 20:32:05.000000 mypy-boto3-migrationhubstrategy-1.28.15/setup.py
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/LICENSE` & `mypy-boto3-migrationhubstrategy-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,71 +399,69 @@
     ServerSummaryTypeDef,
     StrategySummaryTypeDef,
     AssessmentTargetOutputTypeDef,
     AssessmentTargetTypeDef,
     AssociatedApplicationTypeDef,
     AwsManagedResourcesOutputTypeDef,
     AwsManagedResourcesTypeDef,
-    BusinessGoalsOutputTypeDef,
     BusinessGoalsTypeDef,
     IPAddressBasedRemoteInfoTypeDef,
     PipelineInfoTypeDef,
     RemoteSourceCodeAnalysisServerInfoTypeDef,
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
     HeterogeneousOutputTypeDef,
     HomogeneousOutputTypeDef,
     NoDatabaseMigrationPreferenceOutputTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
-    GetImportFileTaskResponseTypeDef,
-    GetLatestAssessmentIdResponseTypeDef,
     GetRecommendationReportDetailsRequestRequestTypeDef,
     RecommendationReportDetailsTypeDef,
-    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetServerDetailsRequestRequestTypeDef,
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
-    ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
-    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
     NoManagementPreferenceOutputTypeDef,
     SelfManageResourcesOutputTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
-    PaginatorConfigTypeDef,
     TransformationToolTypeDef,
-    ResponseMetadataTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
-    StartAssessmentResponseTypeDef,
-    StartImportFileTaskResponseTypeDef,
-    StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
-    PrioritizeBusinessGoalsOutputTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
-    GetAssessmentResponseTypeDef,
     DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
+    GetAssessmentResponseTypeDef,
+    GetImportFileTaskResponseTypeDef,
+    GetLatestAssessmentIdResponseTypeDef,
+    StartAssessmentResponseTypeDef,
+    StartImportFileTaskResponseTypeDef,
+    StartRecommendationReportGenerationResponseTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
+    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    ListCollectorsRequestListCollectorsPaginateTypeDef,
+    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/README.md` & `mypy-boto3-migrationhubstrategy-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -367,71 +367,69 @@
     ServerSummaryTypeDef,
     StrategySummaryTypeDef,
     AssessmentTargetOutputTypeDef,
     AssessmentTargetTypeDef,
     AssociatedApplicationTypeDef,
     AwsManagedResourcesOutputTypeDef,
     AwsManagedResourcesTypeDef,
-    BusinessGoalsOutputTypeDef,
     BusinessGoalsTypeDef,
     IPAddressBasedRemoteInfoTypeDef,
     PipelineInfoTypeDef,
     RemoteSourceCodeAnalysisServerInfoTypeDef,
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
     HeterogeneousOutputTypeDef,
     HomogeneousOutputTypeDef,
     NoDatabaseMigrationPreferenceOutputTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
-    GetImportFileTaskResponseTypeDef,
-    GetLatestAssessmentIdResponseTypeDef,
     GetRecommendationReportDetailsRequestRequestTypeDef,
     RecommendationReportDetailsTypeDef,
-    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetServerDetailsRequestRequestTypeDef,
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
-    ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
-    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
     NoManagementPreferenceOutputTypeDef,
     SelfManageResourcesOutputTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
-    PaginatorConfigTypeDef,
     TransformationToolTypeDef,
-    ResponseMetadataTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
-    StartAssessmentResponseTypeDef,
-    StartImportFileTaskResponseTypeDef,
-    StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
-    PrioritizeBusinessGoalsOutputTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
-    GetAssessmentResponseTypeDef,
     DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
+    GetAssessmentResponseTypeDef,
+    GetImportFileTaskResponseTypeDef,
+    GetLatestAssessmentIdResponseTypeDef,
+    StartAssessmentResponseTypeDef,
+    StartImportFileTaskResponseTypeDef,
+    StartRecommendationReportGenerationResponseTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
+    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    ListCollectorsRequestListCollectorsPaginateTypeDef,
+    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__init__.py` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__init__.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/__main__.py` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations\nOther"
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

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/client.py` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/client.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/literals.py` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/literals.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/paginator.py` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 class GetServerDetailsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#getserverdetailspaginator)
     """
 
     def paginate(
-        self, *, serverId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serverId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetServerDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#getserverdetailspaginator)
         """
 
 
@@ -85,45 +85,45 @@
     def paginate(
         self,
         *,
         applicationComponentCriteria: ApplicationComponentCriteriaType = ...,
         filterValue: str = ...,
         groupIdFilter: Sequence[GroupTypeDef] = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListApplicationComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listapplicationcomponentspaginator)
         """
 
 
 class ListCollectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listcollectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCollectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listcollectorspaginator)
         """
 
 
 class ListImportFileTaskPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listimportfiletaskpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportFileTaskResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listimportfiletaskpaginator)
         """
 
 
@@ -136,13 +136,13 @@
     def paginate(
         self,
         *,
         filterValue: str = ...,
         groupIdFilter: Sequence[GroupTypeDef] = ...,
         serverCriteria: ServerCriteriaType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listserverspaginator)
         """
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/paginator.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 class GetServerDetailsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#getserverdetailspaginator)
     """
 
     def paginate(
-        self, *, serverId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serverId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetServerDetailsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.GetServerDetails.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#getserverdetailspaginator)
         """
 
 class ListApplicationComponentsPaginator(Paginator):
@@ -81,43 +81,43 @@
     def paginate(
         self,
         *,
         applicationComponentCriteria: ApplicationComponentCriteriaType = ...,
         filterValue: str = ...,
         groupIdFilter: Sequence[GroupTypeDef] = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationComponentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListApplicationComponents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listapplicationcomponentspaginator)
         """
 
 class ListCollectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listcollectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCollectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListCollectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listcollectorspaginator)
         """
 
 class ListImportFileTaskPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listimportfiletaskpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListImportFileTaskResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListImportFileTask.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listimportfiletaskpaginator)
         """
 
 class ListServersPaginator(Paginator):
@@ -129,13 +129,13 @@
     def paginate(
         self,
         *,
         filterValue: str = ...,
         groupIdFilter: Sequence[GroupTypeDef] = ...,
         serverCriteria: ServerCriteriaType = ...,
         sort: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations.Paginator.ListServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/paginators/#listserverspaginator)
         """
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/type_defs.py` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,71 +83,69 @@
     "ServerSummaryTypeDef",
     "StrategySummaryTypeDef",
     "AssessmentTargetOutputTypeDef",
     "AssessmentTargetTypeDef",
     "AssociatedApplicationTypeDef",
     "AwsManagedResourcesOutputTypeDef",
     "AwsManagedResourcesTypeDef",
-    "BusinessGoalsOutputTypeDef",
     "BusinessGoalsTypeDef",
     "IPAddressBasedRemoteInfoTypeDef",
     "PipelineInfoTypeDef",
     "RemoteSourceCodeAnalysisServerInfoTypeDef",
     "VcenterBasedRemoteInfoTypeDef",
     "VersionControlInfoTypeDef",
     "DataCollectionDetailsTypeDef",
     "HeterogeneousOutputTypeDef",
     "HomogeneousOutputTypeDef",
     "NoDatabaseMigrationPreferenceOutputTypeDef",
     "HeterogeneousTypeDef",
     "HomogeneousTypeDef",
     "NoDatabaseMigrationPreferenceTypeDef",
     "GetApplicationComponentDetailsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetImportFileTaskRequestRequestTypeDef",
-    "GetImportFileTaskResponseTypeDef",
-    "GetLatestAssessmentIdResponseTypeDef",
     "GetRecommendationReportDetailsRequestRequestTypeDef",
     "RecommendationReportDetailsTypeDef",
-    "GetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetServerDetailsRequestRequestTypeDef",
     "GetServerStrategiesRequestRequestTypeDef",
     "GroupTypeDef",
     "ImportFileTaskInformationTypeDef",
-    "ListCollectorsRequestListCollectorsPaginateTypeDef",
     "ListCollectorsRequestRequestTypeDef",
-    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListImportFileTaskRequestRequestTypeDef",
     "NoManagementPreferenceOutputTypeDef",
     "SelfManageResourcesOutputTypeDef",
     "NoManagementPreferenceTypeDef",
     "SelfManageResourcesTypeDef",
     "NetworkInfoTypeDef",
     "OSInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "TransformationToolTypeDef",
-    "ResponseMetadataTypeDef",
     "ServerErrorTypeDef",
     "SourceCodeTypeDef",
-    "StartAssessmentResponseTypeDef",
-    "StartImportFileTaskResponseTypeDef",
-    "StartRecommendationReportGenerationResponseTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
     "StartAssessmentRequestRequestTypeDef",
-    "PrioritizeBusinessGoalsOutputTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
-    "GetAssessmentResponseTypeDef",
     "DatabaseMigrationPreferenceOutputTypeDef",
     "DatabaseMigrationPreferenceTypeDef",
+    "GetAssessmentResponseTypeDef",
+    "GetImportFileTaskResponseTypeDef",
+    "GetLatestAssessmentIdResponseTypeDef",
+    "StartAssessmentResponseTypeDef",
+    "StartImportFileTaskResponseTypeDef",
+    "StartRecommendationReportGenerationResponseTypeDef",
     "GetRecommendationReportDetailsResponseTypeDef",
+    "GetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    "ListCollectorsRequestListCollectorsPaginateTypeDef",
+    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     "ListApplicationComponentsRequestRequestTypeDef",
     "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "StartImportFileTaskRequestRequestTypeDef",
     "StartRecommendationReportGenerationRequestRequestTypeDef",
     "ListImportFileTaskResponseTypeDef",
@@ -325,25 +323,14 @@
 AwsManagedResourcesTypeDef = TypedDict(
     "AwsManagedResourcesTypeDef",
     {
         "targetDestination": Sequence[AwsManagedTargetDestinationType],
     },
 )
 
-BusinessGoalsOutputTypeDef = TypedDict(
-    "BusinessGoalsOutputTypeDef",
-    {
-        "licenseCostReduction": int,
-        "modernizeInfrastructureWithCloudNativeTechnologies": int,
-        "reduceOperationalOverheadWithManagedServices": int,
-        "speedOfMigration": int,
-    },
-    total=False,
-)
-
 BusinessGoalsTypeDef = TypedDict(
     "BusinessGoalsTypeDef",
     {
         "licenseCostReduction": int,
         "modernizeInfrastructureWithCloudNativeTechnologies": int,
         "reduceOperationalOverheadWithManagedServices": int,
         "speedOfMigration": int,
@@ -458,14 +445,25 @@
 GetApplicationComponentDetailsRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     {
         "applicationComponentId": str,
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
 GetApplicationComponentStrategiesRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     {
         "applicationComponentId": str,
     },
 )
 
@@ -479,40 +477,14 @@
 GetImportFileTaskRequestRequestTypeDef = TypedDict(
     "GetImportFileTaskRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetImportFileTaskResponseTypeDef = TypedDict(
-    "GetImportFileTaskResponseTypeDef",
-    {
-        "completionTime": datetime,
-        "id": str,
-        "importName": str,
-        "inputS3Bucket": str,
-        "inputS3Key": str,
-        "numberOfRecordsFailed": int,
-        "numberOfRecordsSuccess": int,
-        "startTime": datetime,
-        "status": ImportFileTaskStatusType,
-        "statusReportS3Bucket": str,
-        "statusReportS3Key": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLatestAssessmentIdResponseTypeDef = TypedDict(
-    "GetLatestAssessmentIdResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRecommendationReportDetailsRequestRequestTypeDef = TypedDict(
     "GetRecommendationReportDetailsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -525,36 +497,24 @@
         "startTime": datetime,
         "status": RecommendationReportStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
-    "_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
-    {
-        "serverId": str,
-    },
-)
-_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
-    "_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
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
-class GetServerDetailsRequestGetServerDetailsPaginateTypeDef(
-    _RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-    _OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetServerDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetServerDetailsRequestRequestTypeDef",
     {
         "serverId": str,
     },
 )
 _OptionalGetServerDetailsRequestRequestTypeDef = TypedDict(
@@ -603,39 +563,23 @@
         "status": ImportFileTaskStatusType,
         "statusReportS3Bucket": str,
         "statusReportS3Key": str,
     },
     total=False,
 )
 
-ListCollectorsRequestListCollectorsPaginateTypeDef = TypedDict(
-    "ListCollectorsRequestListCollectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCollectorsRequestRequestTypeDef = TypedDict(
     "ListCollectorsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = TypedDict(
-    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListImportFileTaskRequestRequestTypeDef = TypedDict(
     "ListImportFileTaskRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -684,45 +628,24 @@
     {
         "type": OSTypeType,
         "version": str,
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
 TransformationToolTypeDef = TypedDict(
     "TransformationToolTypeDef",
     {
         "description": str,
         "name": TransformationToolNameType,
         "tranformationToolInstallationLink": str,
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
 ServerErrorTypeDef = TypedDict(
     "ServerErrorTypeDef",
     {
         "serverErrorCategory": ServerErrorCategoryType,
     },
     total=False,
 )
@@ -734,38 +657,14 @@
         "projectName": str,
         "sourceVersion": str,
         "versionControl": VersionControlType,
     },
     total=False,
 )
 
-StartAssessmentResponseTypeDef = TypedDict(
-    "StartAssessmentResponseTypeDef",
-    {
-        "assessmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartImportFileTaskResponseTypeDef = TypedDict(
-    "StartImportFileTaskResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartRecommendationReportGenerationResponseTypeDef = TypedDict(
-    "StartRecommendationReportGenerationResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAssessmentRequestRequestTypeDef = TypedDict(
     "StopAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
     },
 )
 
@@ -815,22 +714,14 @@
         "assessmentTargets": Sequence[AssessmentTargetTypeDef],
         "s3bucketForAnalysisData": str,
         "s3bucketForReportData": str,
     },
     total=False,
 )
 
-PrioritizeBusinessGoalsOutputTypeDef = TypedDict(
-    "PrioritizeBusinessGoalsOutputTypeDef",
-    {
-        "businessGoals": BusinessGoalsOutputTypeDef,
-    },
-    total=False,
-)
-
 PrioritizeBusinessGoalsTypeDef = TypedDict(
     "PrioritizeBusinessGoalsTypeDef",
     {
         "businessGoals": BusinessGoalsTypeDef,
     },
     total=False,
 )
@@ -843,24 +734,14 @@
         "remoteSourceCodeAnalysisServerInfo": RemoteSourceCodeAnalysisServerInfoTypeDef,
         "vcenterBasedRemoteInfoList": List[VcenterBasedRemoteInfoTypeDef],
         "versionControlInfoList": List[VersionControlInfoTypeDef],
     },
     total=False,
 )
 
-GetAssessmentResponseTypeDef = TypedDict(
-    "GetAssessmentResponseTypeDef",
-    {
-        "assessmentTargets": List[AssessmentTargetOutputTypeDef],
-        "dataCollectionDetails": DataCollectionDetailsTypeDef,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DatabaseMigrationPreferenceOutputTypeDef = TypedDict(
     "DatabaseMigrationPreferenceOutputTypeDef",
     {
         "heterogeneous": HeterogeneousOutputTypeDef,
         "homogeneous": HomogeneousOutputTypeDef,
         "noPreference": NoDatabaseMigrationPreferenceOutputTypeDef,
     },
@@ -873,31 +754,129 @@
         "heterogeneous": HeterogeneousTypeDef,
         "homogeneous": HomogeneousTypeDef,
         "noPreference": NoDatabaseMigrationPreferenceTypeDef,
     },
     total=False,
 )
 
+GetAssessmentResponseTypeDef = TypedDict(
+    "GetAssessmentResponseTypeDef",
+    {
+        "assessmentTargets": List[AssessmentTargetOutputTypeDef],
+        "dataCollectionDetails": DataCollectionDetailsTypeDef,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImportFileTaskResponseTypeDef = TypedDict(
+    "GetImportFileTaskResponseTypeDef",
+    {
+        "completionTime": datetime,
+        "id": str,
+        "importName": str,
+        "inputS3Bucket": str,
+        "inputS3Key": str,
+        "numberOfRecordsFailed": int,
+        "numberOfRecordsSuccess": int,
+        "startTime": datetime,
+        "status": ImportFileTaskStatusType,
+        "statusReportS3Bucket": str,
+        "statusReportS3Key": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLatestAssessmentIdResponseTypeDef = TypedDict(
+    "GetLatestAssessmentIdResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAssessmentResponseTypeDef = TypedDict(
+    "StartAssessmentResponseTypeDef",
+    {
+        "assessmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartImportFileTaskResponseTypeDef = TypedDict(
+    "StartImportFileTaskResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRecommendationReportGenerationResponseTypeDef = TypedDict(
+    "StartRecommendationReportGenerationResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetRecommendationReportDetailsResponseTypeDef = TypedDict(
     "GetRecommendationReportDetailsResponseTypeDef",
     {
         "id": str,
         "recommendationReportDetails": RecommendationReportDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
+    "_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    {
+        "serverId": str,
+    },
+)
+_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
+    "_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetServerDetailsRequestGetServerDetailsPaginateTypeDef(
+    _RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    _OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+):
+    pass
+
+
+ListCollectorsRequestListCollectorsPaginateTypeDef = TypedDict(
+    "ListCollectorsRequestListCollectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = TypedDict(
+    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef = TypedDict(
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     {
         "applicationComponentCriteria": ApplicationComponentCriteriaType,
         "filterValue": str,
         "groupIdFilter": Sequence[GroupTypeDef],
         "sort": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListApplicationComponentsRequestRequestTypeDef = TypedDict(
     "ListApplicationComponentsRequestRequestTypeDef",
     {
@@ -914,15 +893,15 @@
 ListServersRequestListServersPaginateTypeDef = TypedDict(
     "ListServersRequestListServersPaginateTypeDef",
     {
         "filterValue": str,
         "groupIdFilter": Sequence[GroupTypeDef],
         "serverCriteria": ServerCriteriaType,
         "sort": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListServersRequestRequestTypeDef = TypedDict(
     "ListServersRequestRequestTypeDef",
     {
@@ -972,15 +951,15 @@
 )
 
 ListImportFileTaskResponseTypeDef = TypedDict(
     "ListImportFileTaskResponseTypeDef",
     {
         "nextToken": str,
         "taskInfos": List[ImportFileTaskInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ManagementPreferenceOutputTypeDef = TypedDict(
     "ManagementPreferenceOutputTypeDef",
     {
         "awsManagedResources": AwsManagedResourcesOutputTypeDef,
@@ -1081,15 +1060,15 @@
     total=False,
 )
 
 GetPortfolioSummaryResponseTypeDef = TypedDict(
     "GetPortfolioSummaryResponseTypeDef",
     {
         "assessmentSummary": AssessmentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CollectorTypeDef = TypedDict(
     "CollectorTypeDef",
     {
         "collectorHealth": CollectorHealthType,
@@ -1211,26 +1190,26 @@
 )
 
 ListCollectorsResponseTypeDef = TypedDict(
     "ListCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesOutputTypeDef,
         "databasePreferences": DatabasePreferencesOutputTypeDef,
-        "prioritizeBusinessGoals": PrioritizeBusinessGoalsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
         "applicationMode": ApplicationModeType,
@@ -1241,57 +1220,57 @@
     total=False,
 )
 
 GetApplicationComponentStrategiesResponseTypeDef = TypedDict(
     "GetApplicationComponentStrategiesResponseTypeDef",
     {
         "applicationComponentStrategies": List[ApplicationComponentStrategyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServerDetailsResponseTypeDef = TypedDict(
     "GetServerDetailsResponseTypeDef",
     {
         "associatedApplications": List[AssociatedApplicationTypeDef],
         "nextToken": str,
         "serverDetail": ServerDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServersResponseTypeDef = TypedDict(
     "ListServersResponseTypeDef",
     {
         "nextToken": str,
         "serverInfos": List[ServerDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServerStrategiesResponseTypeDef = TypedDict(
     "GetServerStrategiesResponseTypeDef",
     {
         "serverStrategies": List[ServerStrategyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationComponentDetailsResponseTypeDef = TypedDict(
     "GetApplicationComponentDetailsResponseTypeDef",
     {
         "applicationComponentDetail": ApplicationComponentDetailTypeDef,
         "associatedApplications": List[AssociatedApplicationTypeDef],
         "associatedServerIds": List[str],
         "moreApplicationResource": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationComponentsResponseTypeDef = TypedDict(
     "ListApplicationComponentsResponseTypeDef",
     {
         "applicationComponentInfos": List[ApplicationComponentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy/type_defs.pyi` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -82,71 +82,69 @@
     "ServerSummaryTypeDef",
     "StrategySummaryTypeDef",
     "AssessmentTargetOutputTypeDef",
     "AssessmentTargetTypeDef",
     "AssociatedApplicationTypeDef",
     "AwsManagedResourcesOutputTypeDef",
     "AwsManagedResourcesTypeDef",
-    "BusinessGoalsOutputTypeDef",
     "BusinessGoalsTypeDef",
     "IPAddressBasedRemoteInfoTypeDef",
     "PipelineInfoTypeDef",
     "RemoteSourceCodeAnalysisServerInfoTypeDef",
     "VcenterBasedRemoteInfoTypeDef",
     "VersionControlInfoTypeDef",
     "DataCollectionDetailsTypeDef",
     "HeterogeneousOutputTypeDef",
     "HomogeneousOutputTypeDef",
     "NoDatabaseMigrationPreferenceOutputTypeDef",
     "HeterogeneousTypeDef",
     "HomogeneousTypeDef",
     "NoDatabaseMigrationPreferenceTypeDef",
     "GetApplicationComponentDetailsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     "GetAssessmentRequestRequestTypeDef",
     "GetImportFileTaskRequestRequestTypeDef",
-    "GetImportFileTaskResponseTypeDef",
-    "GetLatestAssessmentIdResponseTypeDef",
     "GetRecommendationReportDetailsRequestRequestTypeDef",
     "RecommendationReportDetailsTypeDef",
-    "GetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetServerDetailsRequestRequestTypeDef",
     "GetServerStrategiesRequestRequestTypeDef",
     "GroupTypeDef",
     "ImportFileTaskInformationTypeDef",
-    "ListCollectorsRequestListCollectorsPaginateTypeDef",
     "ListCollectorsRequestRequestTypeDef",
-    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListImportFileTaskRequestRequestTypeDef",
     "NoManagementPreferenceOutputTypeDef",
     "SelfManageResourcesOutputTypeDef",
     "NoManagementPreferenceTypeDef",
     "SelfManageResourcesTypeDef",
     "NetworkInfoTypeDef",
     "OSInfoTypeDef",
-    "PaginatorConfigTypeDef",
     "TransformationToolTypeDef",
-    "ResponseMetadataTypeDef",
     "ServerErrorTypeDef",
     "SourceCodeTypeDef",
-    "StartAssessmentResponseTypeDef",
-    "StartImportFileTaskResponseTypeDef",
-    "StartRecommendationReportGenerationResponseTypeDef",
     "StopAssessmentRequestRequestTypeDef",
     "StrategyOptionTypeDef",
     "AntipatternReportResultTypeDef",
     "AssessmentSummaryTypeDef",
     "StartAssessmentRequestRequestTypeDef",
-    "PrioritizeBusinessGoalsOutputTypeDef",
     "PrioritizeBusinessGoalsTypeDef",
     "ConfigurationSummaryTypeDef",
-    "GetAssessmentResponseTypeDef",
     "DatabaseMigrationPreferenceOutputTypeDef",
     "DatabaseMigrationPreferenceTypeDef",
+    "GetAssessmentResponseTypeDef",
+    "GetImportFileTaskResponseTypeDef",
+    "GetLatestAssessmentIdResponseTypeDef",
+    "StartAssessmentResponseTypeDef",
+    "StartImportFileTaskResponseTypeDef",
+    "StartRecommendationReportGenerationResponseTypeDef",
     "GetRecommendationReportDetailsResponseTypeDef",
+    "GetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    "ListCollectorsRequestListCollectorsPaginateTypeDef",
+    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     "ListApplicationComponentsRequestRequestTypeDef",
     "ListServersRequestListServersPaginateTypeDef",
     "ListServersRequestRequestTypeDef",
     "StartImportFileTaskRequestRequestTypeDef",
     "StartRecommendationReportGenerationRequestRequestTypeDef",
     "ListImportFileTaskResponseTypeDef",
@@ -324,25 +322,14 @@
 AwsManagedResourcesTypeDef = TypedDict(
     "AwsManagedResourcesTypeDef",
     {
         "targetDestination": Sequence[AwsManagedTargetDestinationType],
     },
 )
 
-BusinessGoalsOutputTypeDef = TypedDict(
-    "BusinessGoalsOutputTypeDef",
-    {
-        "licenseCostReduction": int,
-        "modernizeInfrastructureWithCloudNativeTechnologies": int,
-        "reduceOperationalOverheadWithManagedServices": int,
-        "speedOfMigration": int,
-    },
-    total=False,
-)
-
 BusinessGoalsTypeDef = TypedDict(
     "BusinessGoalsTypeDef",
     {
         "licenseCostReduction": int,
         "modernizeInfrastructureWithCloudNativeTechnologies": int,
         "reduceOperationalOverheadWithManagedServices": int,
         "speedOfMigration": int,
@@ -457,14 +444,25 @@
 GetApplicationComponentDetailsRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentDetailsRequestRequestTypeDef",
     {
         "applicationComponentId": str,
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
 GetApplicationComponentStrategiesRequestRequestTypeDef = TypedDict(
     "GetApplicationComponentStrategiesRequestRequestTypeDef",
     {
         "applicationComponentId": str,
     },
 )
 
@@ -478,40 +476,14 @@
 GetImportFileTaskRequestRequestTypeDef = TypedDict(
     "GetImportFileTaskRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetImportFileTaskResponseTypeDef = TypedDict(
-    "GetImportFileTaskResponseTypeDef",
-    {
-        "completionTime": datetime,
-        "id": str,
-        "importName": str,
-        "inputS3Bucket": str,
-        "inputS3Key": str,
-        "numberOfRecordsFailed": int,
-        "numberOfRecordsSuccess": int,
-        "startTime": datetime,
-        "status": ImportFileTaskStatusType,
-        "statusReportS3Bucket": str,
-        "statusReportS3Key": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLatestAssessmentIdResponseTypeDef = TypedDict(
-    "GetLatestAssessmentIdResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRecommendationReportDetailsRequestRequestTypeDef = TypedDict(
     "GetRecommendationReportDetailsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -524,34 +496,24 @@
         "startTime": datetime,
         "status": RecommendationReportStatusType,
         "statusMessage": str,
     },
     total=False,
 )
 
-_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
-    "_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
-    {
-        "serverId": str,
-    },
-)
-_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
-    "_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
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
 
-class GetServerDetailsRequestGetServerDetailsPaginateTypeDef(
-    _RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-    _OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetServerDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetServerDetailsRequestRequestTypeDef",
     {
         "serverId": str,
     },
 )
 _OptionalGetServerDetailsRequestRequestTypeDef = TypedDict(
@@ -598,39 +560,23 @@
         "status": ImportFileTaskStatusType,
         "statusReportS3Bucket": str,
         "statusReportS3Key": str,
     },
     total=False,
 )
 
-ListCollectorsRequestListCollectorsPaginateTypeDef = TypedDict(
-    "ListCollectorsRequestListCollectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCollectorsRequestRequestTypeDef = TypedDict(
     "ListCollectorsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = TypedDict(
-    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListImportFileTaskRequestRequestTypeDef = TypedDict(
     "ListImportFileTaskRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -679,45 +625,24 @@
     {
         "type": OSTypeType,
         "version": str,
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
 TransformationToolTypeDef = TypedDict(
     "TransformationToolTypeDef",
     {
         "description": str,
         "name": TransformationToolNameType,
         "tranformationToolInstallationLink": str,
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
 ServerErrorTypeDef = TypedDict(
     "ServerErrorTypeDef",
     {
         "serverErrorCategory": ServerErrorCategoryType,
     },
     total=False,
 )
@@ -729,38 +654,14 @@
         "projectName": str,
         "sourceVersion": str,
         "versionControl": VersionControlType,
     },
     total=False,
 )
 
-StartAssessmentResponseTypeDef = TypedDict(
-    "StartAssessmentResponseTypeDef",
-    {
-        "assessmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartImportFileTaskResponseTypeDef = TypedDict(
-    "StartImportFileTaskResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartRecommendationReportGenerationResponseTypeDef = TypedDict(
-    "StartRecommendationReportGenerationResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopAssessmentRequestRequestTypeDef = TypedDict(
     "StopAssessmentRequestRequestTypeDef",
     {
         "assessmentId": str,
     },
 )
 
@@ -810,22 +711,14 @@
         "assessmentTargets": Sequence[AssessmentTargetTypeDef],
         "s3bucketForAnalysisData": str,
         "s3bucketForReportData": str,
     },
     total=False,
 )
 
-PrioritizeBusinessGoalsOutputTypeDef = TypedDict(
-    "PrioritizeBusinessGoalsOutputTypeDef",
-    {
-        "businessGoals": BusinessGoalsOutputTypeDef,
-    },
-    total=False,
-)
-
 PrioritizeBusinessGoalsTypeDef = TypedDict(
     "PrioritizeBusinessGoalsTypeDef",
     {
         "businessGoals": BusinessGoalsTypeDef,
     },
     total=False,
 )
@@ -838,24 +731,14 @@
         "remoteSourceCodeAnalysisServerInfo": RemoteSourceCodeAnalysisServerInfoTypeDef,
         "vcenterBasedRemoteInfoList": List[VcenterBasedRemoteInfoTypeDef],
         "versionControlInfoList": List[VersionControlInfoTypeDef],
     },
     total=False,
 )
 
-GetAssessmentResponseTypeDef = TypedDict(
-    "GetAssessmentResponseTypeDef",
-    {
-        "assessmentTargets": List[AssessmentTargetOutputTypeDef],
-        "dataCollectionDetails": DataCollectionDetailsTypeDef,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DatabaseMigrationPreferenceOutputTypeDef = TypedDict(
     "DatabaseMigrationPreferenceOutputTypeDef",
     {
         "heterogeneous": HeterogeneousOutputTypeDef,
         "homogeneous": HomogeneousOutputTypeDef,
         "noPreference": NoDatabaseMigrationPreferenceOutputTypeDef,
     },
@@ -868,31 +751,127 @@
         "heterogeneous": HeterogeneousTypeDef,
         "homogeneous": HomogeneousTypeDef,
         "noPreference": NoDatabaseMigrationPreferenceTypeDef,
     },
     total=False,
 )
 
+GetAssessmentResponseTypeDef = TypedDict(
+    "GetAssessmentResponseTypeDef",
+    {
+        "assessmentTargets": List[AssessmentTargetOutputTypeDef],
+        "dataCollectionDetails": DataCollectionDetailsTypeDef,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetImportFileTaskResponseTypeDef = TypedDict(
+    "GetImportFileTaskResponseTypeDef",
+    {
+        "completionTime": datetime,
+        "id": str,
+        "importName": str,
+        "inputS3Bucket": str,
+        "inputS3Key": str,
+        "numberOfRecordsFailed": int,
+        "numberOfRecordsSuccess": int,
+        "startTime": datetime,
+        "status": ImportFileTaskStatusType,
+        "statusReportS3Bucket": str,
+        "statusReportS3Key": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLatestAssessmentIdResponseTypeDef = TypedDict(
+    "GetLatestAssessmentIdResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAssessmentResponseTypeDef = TypedDict(
+    "StartAssessmentResponseTypeDef",
+    {
+        "assessmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartImportFileTaskResponseTypeDef = TypedDict(
+    "StartImportFileTaskResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartRecommendationReportGenerationResponseTypeDef = TypedDict(
+    "StartRecommendationReportGenerationResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetRecommendationReportDetailsResponseTypeDef = TypedDict(
     "GetRecommendationReportDetailsResponseTypeDef",
     {
         "id": str,
         "recommendationReportDetails": RecommendationReportDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
+    "_RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    {
+        "serverId": str,
+    },
+)
+_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef = TypedDict(
+    "_OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetServerDetailsRequestGetServerDetailsPaginateTypeDef(
+    _RequiredGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    _OptionalGetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+):
+    pass
+
+ListCollectorsRequestListCollectorsPaginateTypeDef = TypedDict(
+    "ListCollectorsRequestListCollectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListImportFileTaskRequestListImportFileTaskPaginateTypeDef = TypedDict(
+    "ListImportFileTaskRequestListImportFileTaskPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef = TypedDict(
     "ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef",
     {
         "applicationComponentCriteria": ApplicationComponentCriteriaType,
         "filterValue": str,
         "groupIdFilter": Sequence[GroupTypeDef],
         "sort": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListApplicationComponentsRequestRequestTypeDef = TypedDict(
     "ListApplicationComponentsRequestRequestTypeDef",
     {
@@ -909,15 +888,15 @@
 ListServersRequestListServersPaginateTypeDef = TypedDict(
     "ListServersRequestListServersPaginateTypeDef",
     {
         "filterValue": str,
         "groupIdFilter": Sequence[GroupTypeDef],
         "serverCriteria": ServerCriteriaType,
         "sort": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListServersRequestRequestTypeDef = TypedDict(
     "ListServersRequestRequestTypeDef",
     {
@@ -965,15 +944,15 @@
 )
 
 ListImportFileTaskResponseTypeDef = TypedDict(
     "ListImportFileTaskResponseTypeDef",
     {
         "nextToken": str,
         "taskInfos": List[ImportFileTaskInformationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ManagementPreferenceOutputTypeDef = TypedDict(
     "ManagementPreferenceOutputTypeDef",
     {
         "awsManagedResources": AwsManagedResourcesOutputTypeDef,
@@ -1070,15 +1049,15 @@
     total=False,
 )
 
 GetPortfolioSummaryResponseTypeDef = TypedDict(
     "GetPortfolioSummaryResponseTypeDef",
     {
         "assessmentSummary": AssessmentSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CollectorTypeDef = TypedDict(
     "CollectorTypeDef",
     {
         "collectorHealth": CollectorHealthType,
@@ -1200,26 +1179,26 @@
 )
 
 ListCollectorsResponseTypeDef = TypedDict(
     "ListCollectorsResponseTypeDef",
     {
         "Collectors": List[CollectorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPortfolioPreferencesResponseTypeDef = TypedDict(
     "GetPortfolioPreferencesResponseTypeDef",
     {
         "applicationMode": ApplicationModeType,
         "applicationPreferences": ApplicationPreferencesOutputTypeDef,
         "databasePreferences": DatabasePreferencesOutputTypeDef,
-        "prioritizeBusinessGoals": PrioritizeBusinessGoalsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "prioritizeBusinessGoals": PrioritizeBusinessGoalsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPortfolioPreferencesRequestRequestTypeDef = TypedDict(
     "PutPortfolioPreferencesRequestRequestTypeDef",
     {
         "applicationMode": ApplicationModeType,
@@ -1230,57 +1209,57 @@
     total=False,
 )
 
 GetApplicationComponentStrategiesResponseTypeDef = TypedDict(
     "GetApplicationComponentStrategiesResponseTypeDef",
     {
         "applicationComponentStrategies": List[ApplicationComponentStrategyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServerDetailsResponseTypeDef = TypedDict(
     "GetServerDetailsResponseTypeDef",
     {
         "associatedApplications": List[AssociatedApplicationTypeDef],
         "nextToken": str,
         "serverDetail": ServerDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServersResponseTypeDef = TypedDict(
     "ListServersResponseTypeDef",
     {
         "nextToken": str,
         "serverInfos": List[ServerDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServerStrategiesResponseTypeDef = TypedDict(
     "GetServerStrategiesResponseTypeDef",
     {
         "serverStrategies": List[ServerStrategyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationComponentDetailsResponseTypeDef = TypedDict(
     "GetApplicationComponentDetailsResponseTypeDef",
     {
         "applicationComponentDetail": ApplicationComponentDetailTypeDef,
         "associatedApplications": List[AssociatedApplicationTypeDef],
         "associatedServerIds": List[str],
         "moreApplicationResource": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationComponentsResponseTypeDef = TypedDict(
     "ListApplicationComponentsResponseTypeDef",
     {
         "applicationComponentInfos": List[ApplicationComponentDetailTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migrationhubstrategy
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migrationhubstrategy.svg?color=blue)](https://pypi.org/project/mypy-boto3-migrationhubstrategy)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migrationhubstrategy)](https://pepy.tech/project/mypy-boto3-migrationhubstrategy)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubStrategyRecommendations 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
+[boto3.MigrationHubStrategyRecommendations 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhubstrategy.html#MigrationHubStrategyRecommendations)
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
 [mypy-boto3-migrationhubstrategy docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migrationhubstrategy/).
 
 See how it helps to find and fix potential bugs:
 
@@ -399,71 +399,69 @@
     ServerSummaryTypeDef,
     StrategySummaryTypeDef,
     AssessmentTargetOutputTypeDef,
     AssessmentTargetTypeDef,
     AssociatedApplicationTypeDef,
     AwsManagedResourcesOutputTypeDef,
     AwsManagedResourcesTypeDef,
-    BusinessGoalsOutputTypeDef,
     BusinessGoalsTypeDef,
     IPAddressBasedRemoteInfoTypeDef,
     PipelineInfoTypeDef,
     RemoteSourceCodeAnalysisServerInfoTypeDef,
     VcenterBasedRemoteInfoTypeDef,
     VersionControlInfoTypeDef,
     DataCollectionDetailsTypeDef,
     HeterogeneousOutputTypeDef,
     HomogeneousOutputTypeDef,
     NoDatabaseMigrationPreferenceOutputTypeDef,
     HeterogeneousTypeDef,
     HomogeneousTypeDef,
     NoDatabaseMigrationPreferenceTypeDef,
     GetApplicationComponentDetailsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetApplicationComponentStrategiesRequestRequestTypeDef,
     GetAssessmentRequestRequestTypeDef,
     GetImportFileTaskRequestRequestTypeDef,
-    GetImportFileTaskResponseTypeDef,
-    GetLatestAssessmentIdResponseTypeDef,
     GetRecommendationReportDetailsRequestRequestTypeDef,
     RecommendationReportDetailsTypeDef,
-    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetServerDetailsRequestRequestTypeDef,
     GetServerStrategiesRequestRequestTypeDef,
     GroupTypeDef,
     ImportFileTaskInformationTypeDef,
-    ListCollectorsRequestListCollectorsPaginateTypeDef,
     ListCollectorsRequestRequestTypeDef,
-    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListImportFileTaskRequestRequestTypeDef,
     NoManagementPreferenceOutputTypeDef,
     SelfManageResourcesOutputTypeDef,
     NoManagementPreferenceTypeDef,
     SelfManageResourcesTypeDef,
     NetworkInfoTypeDef,
     OSInfoTypeDef,
-    PaginatorConfigTypeDef,
     TransformationToolTypeDef,
-    ResponseMetadataTypeDef,
     ServerErrorTypeDef,
     SourceCodeTypeDef,
-    StartAssessmentResponseTypeDef,
-    StartImportFileTaskResponseTypeDef,
-    StartRecommendationReportGenerationResponseTypeDef,
     StopAssessmentRequestRequestTypeDef,
     StrategyOptionTypeDef,
     AntipatternReportResultTypeDef,
     AssessmentSummaryTypeDef,
     StartAssessmentRequestRequestTypeDef,
-    PrioritizeBusinessGoalsOutputTypeDef,
     PrioritizeBusinessGoalsTypeDef,
     ConfigurationSummaryTypeDef,
-    GetAssessmentResponseTypeDef,
     DatabaseMigrationPreferenceOutputTypeDef,
     DatabaseMigrationPreferenceTypeDef,
+    GetAssessmentResponseTypeDef,
+    GetImportFileTaskResponseTypeDef,
+    GetLatestAssessmentIdResponseTypeDef,
+    StartAssessmentResponseTypeDef,
+    StartImportFileTaskResponseTypeDef,
+    StartRecommendationReportGenerationResponseTypeDef,
     GetRecommendationReportDetailsResponseTypeDef,
+    GetServerDetailsRequestGetServerDetailsPaginateTypeDef,
+    ListCollectorsRequestListCollectorsPaginateTypeDef,
+    ListImportFileTaskRequestListImportFileTaskPaginateTypeDef,
     ListApplicationComponentsRequestListApplicationComponentsPaginateTypeDef,
     ListApplicationComponentsRequestRequestTypeDef,
     ListServersRequestListServersPaginateTypeDef,
     ListServersRequestRequestTypeDef,
     StartImportFileTaskRequestRequestTypeDef,
     StartRecommendationReportGenerationRequestRequestTypeDef,
     ListImportFileTaskResponseTypeDef,
```

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt` & `mypy-boto3-migrationhubstrategy-1.28.15/mypy_boto3_migrationhubstrategy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migrationhubstrategy-1.28.12/setup.py` & `mypy-boto3-migrationhubstrategy-1.28.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migrationhubstrategy",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_migrationhubstrategy"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.12 service generated"
-        " with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MigrationHubStrategyRecommendations 1.28.15 service generated"
+        " with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

