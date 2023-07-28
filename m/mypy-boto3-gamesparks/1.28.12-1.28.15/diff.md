# Comparing `tmp/mypy-boto3-gamesparks-1.28.12.tar.gz` & `tmp/mypy-boto3-gamesparks-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-gamesparks-1.28.12.tar", last modified: Thu Jul 27 05:34:43 2023, max compression
+gzip compressed data, was "mypy-boto3-gamesparks-1.28.15.tar", last modified: Fri Jul 28 20:42:50 2023, max compression
```

## Comparing `mypy-boto3-gamesparks-1.28.12.tar` & `mypy-boto3-gamesparks-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:43.636503 mypy-boto3-gamesparks-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:41.000000 mypy-boto3-gamesparks-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-07-27 05:34:43.636503 mypy-boto3-gamesparks-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-07-27 05:22:41.000000 mypy-boto3-gamesparks-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:43.632503 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-27 05:22:41.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-27 05:22:41.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:22:41.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-07-27 05:22:42.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-07-27 05:22:42.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-27 05:22:42.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-27 05:22:42.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-07-27 05:22:42.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8283 2023-07-27 05:22:42.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:41.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29862 2023-07-27 05:22:43.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29819 2023-07-27 05:22:42.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:41.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:43.636503 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-07-27 05:34:43.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:34:43.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:43.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:34:43.000000 mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:43.636503 mypy-boto3-gamesparks-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:22:40.000000 mypy-boto3-gamesparks-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.329131 mypy-boto3-gamesparks-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-07-28 20:42:50.329131 mypy-boto3-gamesparks-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.317131 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24666 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24619 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8278 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29790 2023-07-28 20:26:28.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29747 2023-07-28 20:26:28.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.329131 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-07-28 20:42:50.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:42:50.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:50.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:50.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:50.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:42:50.000000 mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:50.329131 mypy-boto3-gamesparks-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:26:27.000000 mypy-boto3-gamesparks-1.28.15/setup.py
```

### Comparing `mypy-boto3-gamesparks-1.28.12/LICENSE` & `mypy-boto3-gamesparks-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.12/PKG-INFO` & `mypy-boto3-gamesparks-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamesparks
-Version: 1.28.12
-Summary: Type annotations for boto3.GameSparks 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GameSparks 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamesparks)](https://pepy.tech/project/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,24 +354,23 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
-    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -380,45 +379,39 @@
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     ImportGameConfigurationSourceTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
     CreateGameResultTypeDef,
+    DisconnectPlayerResultTypeDef,
+    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -428,14 +421,21 @@
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
     ImportGameConfigurationRequestRequestTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
```

### Comparing `mypy-boto3-gamesparks-1.28.12/README.md` & `mypy-boto3-gamesparks-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamesparks)](https://pepy.tech/project/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,24 +322,23 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
-    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -348,45 +347,39 @@
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     ImportGameConfigurationSourceTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
     CreateGameResultTypeDef,
+    DisconnectPlayerResultTypeDef,
+    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -396,14 +389,21 @@
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
     ImportGameConfigurationRequestRequestTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
```

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/__init__.py` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/__init__.pyi` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/__main__.py` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GameSparks 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.GameSparks 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks\nOther"
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

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/client.py` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/client.pyi` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/literals.py` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/literals.pyi` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/paginator.py` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,103 +70,103 @@
 class ListExtensionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, Namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, Namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExtensionVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionversionspaginator)
         """
 
 
 class ListExtensionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionspaginator)
         """
 
 
 class ListGamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgamespaginator)
         """
 
 
 class ListGeneratedCodeJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgeneratedcodejobspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, SnapshotId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, SnapshotId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGeneratedCodeJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgeneratedcodejobspaginator)
         """
 
 
 class ListSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listsnapshotspaginator)
         """
 
 
 class ListStageDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagedeploymentspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, StageName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, StageName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStageDeploymentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagedeploymentspaginator)
         """
 
 
 class ListStagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagespaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagespaginator)
         """
```

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/paginator.pyi` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -67,97 +67,97 @@
 class ListExtensionVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionversionspaginator)
     """
 
     def paginate(
-        self, *, Name: str, Namespace: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Name: str, Namespace: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExtensionVersionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensionVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionversionspaginator)
         """
 
 class ListExtensionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListExtensionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListExtensions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listextensionspaginator)
         """
 
 class ListGamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgamespaginator)
         """
 
 class ListGeneratedCodeJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgeneratedcodejobspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, SnapshotId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, SnapshotId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGeneratedCodeJobsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListGeneratedCodeJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listgeneratedcodejobspaginator)
         """
 
 class ListSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listsnapshotspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#listsnapshotspaginator)
         """
 
 class ListStageDeploymentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagedeploymentspaginator)
     """
 
     def paginate(
-        self, *, GameName: str, StageName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, StageName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStageDeploymentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStageDeployments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagedeploymentspaginator)
         """
 
 class ListStagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagespaginator)
     """
 
     def paginate(
-        self, *, GameName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, GameName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStagesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks.Paginator.ListStages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/paginators/#liststagespaginator)
         """
```

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/type_defs.py` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -28,29 +28,27 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ConnectionTypeDef",
     "CreateGameRequestRequestTypeDef",
     "GameDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateStageRequestRequestTypeDef",
     "StageDetailsTypeDef",
     "DeleteGameRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeploymentResultTypeDef",
     "DisconnectPlayerRequestRequestTypeDef",
-    "DisconnectPlayerResultTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
-    "ExportSnapshotResultTypeDef",
     "ExtensionDetailsTypeDef",
     "ExtensionVersionDetailsTypeDef",
     "SectionTypeDef",
     "GameSummaryTypeDef",
     "GeneratedCodeJobDetailsTypeDef",
     "GeneratorTypeDef",
     "GetExtensionRequestRequestTypeDef",
@@ -59,45 +57,39 @@
     "GetGameRequestRequestTypeDef",
     "GetGeneratedCodeJobRequestRequestTypeDef",
     "GetPlayerConnectionStatusRequestRequestTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetStageDeploymentRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
     "ImportGameConfigurationSourceTypeDef",
-    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListExtensionVersionsRequestRequestTypeDef",
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
     "ListExtensionsRequestRequestTypeDef",
-    "ListGamesRequestListGamesPaginateTypeDef",
     "ListGamesRequestRequestTypeDef",
-    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     "ListGeneratedCodeJobsRequestRequestTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "SnapshotSummaryTypeDef",
-    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
     "ListStageDeploymentsRequestRequestTypeDef",
-    "ListStagesRequestListStagesPaginateTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SectionModificationTypeDef",
-    "StartGeneratedCodeJobResultTypeDef",
     "StartStageDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGameRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
-    "GetPlayerConnectionStatusResultTypeDef",
     "CreateGameResultTypeDef",
+    "DisconnectPlayerResultTypeDef",
+    "ExportSnapshotResultTypeDef",
     "GetGameResultTypeDef",
+    "GetPlayerConnectionStatusResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "StartGeneratedCodeJobResultTypeDef",
     "UpdateGameResultTypeDef",
     "CreateStageResultTypeDef",
     "GetStageResultTypeDef",
     "UpdateStageResultTypeDef",
     "StageDeploymentDetailsTypeDef",
     "StageDeploymentSummaryTypeDef",
     "GetExtensionResultTypeDef",
@@ -107,14 +99,21 @@
     "GameConfigurationDetailsTypeDef",
     "SnapshotDetailsTypeDef",
     "ListGamesResultTypeDef",
     "GetGeneratedCodeJobResultTypeDef",
     "ListGeneratedCodeJobsResultTypeDef",
     "StartGeneratedCodeJobRequestRequestTypeDef",
     "ImportGameConfigurationRequestRequestTypeDef",
+    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    "ListGamesRequestListGamesPaginateTypeDef",
+    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    "ListStagesRequestListStagesPaginateTypeDef",
     "ListSnapshotsResultTypeDef",
     "ListStagesResultTypeDef",
     "UpdateGameConfigurationRequestRequestTypeDef",
     "GetStageDeploymentResultTypeDef",
     "StartStageDeploymentResultTypeDef",
     "ListStageDeploymentsResultTypeDef",
     "GetGameConfigurationResultTypeDef",
@@ -146,21 +145,19 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateGameRequestRequestTypeDef(
     _RequiredCreateGameRequestRequestTypeDef, _OptionalCreateGameRequestRequestTypeDef
 ):
     pass
 
-
 GameDetailsTypeDef = TypedDict(
     "GameDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "EnableTerminationProtection": bool,
@@ -168,35 +165,44 @@
         "Name": str,
         "State": GameStateType,
         "Tags": Dict[str, str],
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
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "Role": str,
         "StageName": str,
     },
@@ -207,21 +213,19 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
-
 StageDetailsTypeDef = TypedDict(
     "StageDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "GameKey": str,
@@ -264,39 +268,22 @@
     {
         "GameName": str,
         "PlayerId": str,
         "StageName": str,
     },
 )
 
-DisconnectPlayerResultTypeDef = TypedDict(
-    "DisconnectPlayerResultTypeDef",
-    {
-        "DisconnectFailures": List[str],
-        "DisconnectSuccesses": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
 
-ExportSnapshotResultTypeDef = TypedDict(
-    "ExportSnapshotResultTypeDef",
-    {
-        "S3Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionDetailsTypeDef = TypedDict(
     "ExtensionDetailsTypeDef",
     {
         "Description": str,
         "Name": str,
         "Namespace": str,
     },
@@ -384,22 +371,20 @@
     "_OptionalGetGameConfigurationRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
-
 class GetGameConfigurationRequestRequestTypeDef(
     _RequiredGetGameConfigurationRequestRequestTypeDef,
     _OptionalGetGameConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetGameRequestRequestTypeDef = TypedDict(
     "GetGameRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 
@@ -432,21 +417,19 @@
     "_OptionalGetSnapshotRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
-
 class GetSnapshotRequestRequestTypeDef(
     _RequiredGetSnapshotRequestRequestTypeDef, _OptionalGetSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -454,22 +437,20 @@
     "_OptionalGetStageDeploymentRequestRequestTypeDef",
     {
         "DeploymentId": str,
     },
     total=False,
 )
 
-
 class GetStageDeploymentRequestRequestTypeDef(
     _RequiredGetStageDeploymentRequestRequestTypeDef,
     _OptionalGetStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -477,37 +458,24 @@
 ImportGameConfigurationSourceTypeDef = TypedDict(
     "ImportGameConfigurationSourceTypeDef",
     {
         "File": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    {
-        "Name": str,
-        "Namespace": str,
-    },
-)
-_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
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
-class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
-    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListExtensionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensionVersionsRequestRequestTypeDef",
     {
         "Name": str,
         "Namespace": str,
     },
 )
@@ -516,79 +484,38 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListExtensionVersionsRequestRequestTypeDef(
     _RequiredListExtensionVersionsRequestRequestTypeDef,
     _OptionalListExtensionVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListExtensionsRequestRequestTypeDef = TypedDict(
     "ListExtensionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListGamesRequestListGamesPaginateTypeDef = TypedDict(
-    "ListGamesRequestListGamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGamesRequestRequestTypeDef = TypedDict(
     "ListGamesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "GameName": str,
-        "SnapshotId": str,
-    },
-)
-_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
-    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGeneratedCodeJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListGeneratedCodeJobsRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -597,44 +524,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListGeneratedCodeJobsRequestRequestTypeDef(
     _RequiredListGeneratedCodeJobsRequestRequestTypeDef,
     _OptionalListGeneratedCodeJobsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
-    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSnapshotsRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalListSnapshotsRequestRequestTypeDef = TypedDict(
@@ -642,55 +545,30 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListSnapshotsRequestRequestTypeDef(
     _RequiredListSnapshotsRequestRequestTypeDef, _OptionalListSnapshotsRequestRequestTypeDef
 ):
     pass
 
-
 SnapshotSummaryTypeDef = TypedDict(
     "SnapshotSummaryTypeDef",
     {
         "Created": datetime,
         "Description": str,
         "Id": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
-_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "GameName": str,
-        "StageName": str,
-    },
-)
-_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
-    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStageDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStageDeploymentsRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -699,44 +577,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStageDeploymentsRequestRequestTypeDef(
     _RequiredListStageDeploymentsRequestRequestTypeDef,
     _OptionalListStageDeploymentsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_RequiredListStagesRequestListStagesPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_OptionalListStagesRequestListStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStagesRequestListStagesPaginateTypeDef(
-    _RequiredListStagesRequestListStagesPaginateTypeDef,
-    _OptionalListStagesRequestListStagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListStagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStagesRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalListStagesRequestRequestTypeDef = TypedDict(
@@ -744,21 +598,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListStagesRequestRequestTypeDef(
     _RequiredListStagesRequestRequestTypeDef, _OptionalListStagesRequestRequestTypeDef
 ):
     pass
 
-
 StageSummaryTypeDef = TypedDict(
     "StageSummaryTypeDef",
     {
         "Description": str,
         "GameKey": str,
         "Name": str,
         "State": StageStateType,
@@ -770,43 +622,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredSectionModificationTypeDef = TypedDict(
     "_RequiredSectionModificationTypeDef",
     {
         "Operation": OperationType,
         "Path": str,
         "Section": str,
     },
@@ -815,29 +638,19 @@
     "_OptionalSectionModificationTypeDef",
     {
         "Value": Mapping[str, Any],
     },
     total=False,
 )
 
-
 class SectionModificationTypeDef(
     _RequiredSectionModificationTypeDef, _OptionalSectionModificationTypeDef
 ):
     pass
 
-
-StartGeneratedCodeJobResultTypeDef = TypedDict(
-    "StartGeneratedCodeJobResultTypeDef",
-    {
-        "GeneratedCodeJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStartStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
         "StageName": str,
     },
@@ -846,22 +659,20 @@
     "_OptionalStartStageDeploymentRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class StartStageDeploymentRequestRequestTypeDef(
     _RequiredStartStageDeploymentRequestRequestTypeDef,
     _OptionalStartStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -884,21 +695,19 @@
     "_OptionalUpdateGameRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateGameRequestRequestTypeDef(
     _RequiredUpdateGameRequestRequestTypeDef, _OptionalUpdateGameRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -906,21 +715,19 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateStageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -929,74 +736,105 @@
     {
         "Description": str,
         "Role": str,
     },
     total=False,
 )
 
-
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
+CreateGameResultTypeDef = TypedDict(
+    "CreateGameResultTypeDef",
+    {
+        "Game": GameDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-GetPlayerConnectionStatusResultTypeDef = TypedDict(
-    "GetPlayerConnectionStatusResultTypeDef",
+DisconnectPlayerResultTypeDef = TypedDict(
+    "DisconnectPlayerResultTypeDef",
     {
-        "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DisconnectFailures": List[str],
+        "DisconnectSuccesses": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateGameResultTypeDef = TypedDict(
-    "CreateGameResultTypeDef",
+ExportSnapshotResultTypeDef = TypedDict(
+    "ExportSnapshotResultTypeDef",
     {
-        "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "S3Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGameResultTypeDef = TypedDict(
     "GetGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPlayerConnectionStatusResultTypeDef = TypedDict(
+    "GetPlayerConnectionStatusResultTypeDef",
+    {
+        "Connections": List[ConnectionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartGeneratedCodeJobResultTypeDef = TypedDict(
+    "StartGeneratedCodeJobResultTypeDef",
+    {
+        "GeneratedCodeJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameResultTypeDef = TypedDict(
     "UpdateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStageResultTypeDef = TypedDict(
     "CreateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResultTypeDef = TypedDict(
     "GetStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStageResultTypeDef = TypedDict(
     "UpdateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StageDeploymentDetailsTypeDef = TypedDict(
     "StageDeploymentDetailsTypeDef",
     {
         "Created": datetime,
@@ -1023,41 +861,41 @@
     total=False,
 )
 
 GetExtensionResultTypeDef = TypedDict(
     "GetExtensionResultTypeDef",
     {
         "Extension": ExtensionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExtensionsResultTypeDef = TypedDict(
     "ListExtensionsResultTypeDef",
     {
         "Extensions": List[ExtensionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExtensionVersionResultTypeDef = TypedDict(
     "GetExtensionVersionResultTypeDef",
     {
         "ExtensionVersion": ExtensionVersionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExtensionVersionsResultTypeDef = TypedDict(
     "ListExtensionVersionsResultTypeDef",
     {
         "ExtensionVersions": List[ExtensionVersionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GameConfigurationDetailsTypeDef = TypedDict(
     "GameConfigurationDetailsTypeDef",
     {
         "Created": datetime,
@@ -1080,32 +918,32 @@
 )
 
 ListGamesResultTypeDef = TypedDict(
     "ListGamesResultTypeDef",
     {
         "Games": List[GameSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeneratedCodeJobResultTypeDef = TypedDict(
     "GetGeneratedCodeJobResultTypeDef",
     {
         "GeneratedCodeJob": GeneratedCodeJobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeneratedCodeJobsResultTypeDef = TypedDict(
     "ListGeneratedCodeJobsResultTypeDef",
     {
         "GeneratedCodeJobs": List[GeneratedCodeJobDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartGeneratedCodeJobRequestRequestTypeDef = TypedDict(
     "StartGeneratedCodeJobRequestRequestTypeDef",
     {
         "GameName": str,
@@ -1118,29 +956,148 @@
     "ImportGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
         "ImportSource": ImportGameConfigurationSourceTypeDef,
     },
 )
 
+_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "Name": str,
+        "Namespace": str,
+    },
+)
+_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
+    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+):
+    pass
+
+ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGamesRequestListGamesPaginateTypeDef = TypedDict(
+    "ListGamesRequestListGamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "GameName": str,
+        "SnapshotId": str,
+    },
+)
+_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
+    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
+    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "GameName": str,
+        "StageName": str,
+    },
+)
+_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
+    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+):
+    pass
+
+_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_RequiredListStagesRequestListStagesPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_OptionalListStagesRequestListStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStagesRequestListStagesPaginateTypeDef(
+    _RequiredListStagesRequestListStagesPaginateTypeDef,
+    _OptionalListStagesRequestListStagesPaginateTypeDef,
+):
+    pass
+
 ListSnapshotsResultTypeDef = TypedDict(
     "ListSnapshotsResultTypeDef",
     {
         "NextToken": str,
         "Snapshots": List[SnapshotSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStagesResultTypeDef = TypedDict(
     "ListStagesResultTypeDef",
     {
         "NextToken": str,
         "Stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
@@ -1148,75 +1105,75 @@
     },
 )
 
 GetStageDeploymentResultTypeDef = TypedDict(
     "GetStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartStageDeploymentResultTypeDef = TypedDict(
     "StartStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStageDeploymentsResultTypeDef = TypedDict(
     "ListStageDeploymentsResultTypeDef",
     {
         "NextToken": str,
         "StageDeployments": List[StageDeploymentSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGameConfigurationResultTypeDef = TypedDict(
     "GetGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportGameConfigurationResultTypeDef = TypedDict(
     "ImportGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameConfigurationResultTypeDef = TypedDict(
     "UpdateGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotResultTypeDef = TypedDict(
     "GetSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSnapshotResultTypeDef = TypedDict(
     "UpdateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks/type_defs.pyi` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,28 +28,28 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ConnectionTypeDef",
     "CreateGameRequestRequestTypeDef",
     "GameDetailsTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateStageRequestRequestTypeDef",
     "StageDetailsTypeDef",
     "DeleteGameRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeploymentResultTypeDef",
     "DisconnectPlayerRequestRequestTypeDef",
-    "DisconnectPlayerResultTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
-    "ExportSnapshotResultTypeDef",
     "ExtensionDetailsTypeDef",
     "ExtensionVersionDetailsTypeDef",
     "SectionTypeDef",
     "GameSummaryTypeDef",
     "GeneratedCodeJobDetailsTypeDef",
     "GeneratorTypeDef",
     "GetExtensionRequestRequestTypeDef",
@@ -58,45 +58,39 @@
     "GetGameRequestRequestTypeDef",
     "GetGeneratedCodeJobRequestRequestTypeDef",
     "GetPlayerConnectionStatusRequestRequestTypeDef",
     "GetSnapshotRequestRequestTypeDef",
     "GetStageDeploymentRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
     "ImportGameConfigurationSourceTypeDef",
-    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListExtensionVersionsRequestRequestTypeDef",
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
     "ListExtensionsRequestRequestTypeDef",
-    "ListGamesRequestListGamesPaginateTypeDef",
     "ListGamesRequestRequestTypeDef",
-    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
     "ListGeneratedCodeJobsRequestRequestTypeDef",
-    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "SnapshotSummaryTypeDef",
-    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
     "ListStageDeploymentsRequestRequestTypeDef",
-    "ListStagesRequestListStagesPaginateTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SectionModificationTypeDef",
-    "StartGeneratedCodeJobResultTypeDef",
     "StartStageDeploymentRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGameRequestRequestTypeDef",
     "UpdateSnapshotRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
-    "GetPlayerConnectionStatusResultTypeDef",
     "CreateGameResultTypeDef",
+    "DisconnectPlayerResultTypeDef",
+    "ExportSnapshotResultTypeDef",
     "GetGameResultTypeDef",
+    "GetPlayerConnectionStatusResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "StartGeneratedCodeJobResultTypeDef",
     "UpdateGameResultTypeDef",
     "CreateStageResultTypeDef",
     "GetStageResultTypeDef",
     "UpdateStageResultTypeDef",
     "StageDeploymentDetailsTypeDef",
     "StageDeploymentSummaryTypeDef",
     "GetExtensionResultTypeDef",
@@ -106,14 +100,21 @@
     "GameConfigurationDetailsTypeDef",
     "SnapshotDetailsTypeDef",
     "ListGamesResultTypeDef",
     "GetGeneratedCodeJobResultTypeDef",
     "ListGeneratedCodeJobsResultTypeDef",
     "StartGeneratedCodeJobRequestRequestTypeDef",
     "ImportGameConfigurationRequestRequestTypeDef",
+    "ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    "ListGamesRequestListGamesPaginateTypeDef",
+    "ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    "ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    "ListStagesRequestListStagesPaginateTypeDef",
     "ListSnapshotsResultTypeDef",
     "ListStagesResultTypeDef",
     "UpdateGameConfigurationRequestRequestTypeDef",
     "GetStageDeploymentResultTypeDef",
     "StartStageDeploymentResultTypeDef",
     "ListStageDeploymentsResultTypeDef",
     "GetGameConfigurationResultTypeDef",
@@ -145,19 +146,21 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateGameRequestRequestTypeDef(
     _RequiredCreateGameRequestRequestTypeDef, _OptionalCreateGameRequestRequestTypeDef
 ):
     pass
 
+
 GameDetailsTypeDef = TypedDict(
     "GameDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "EnableTerminationProtection": bool,
@@ -165,33 +168,46 @@
         "Name": str,
         "State": GameStateType,
         "Tags": Dict[str, str],
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
 _RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 _OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateSnapshotRequestRequestTypeDef(
     _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "Role": str,
         "StageName": str,
     },
@@ -202,19 +218,21 @@
         "ClientToken": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
+
 StageDetailsTypeDef = TypedDict(
     "StageDetailsTypeDef",
     {
         "Arn": str,
         "Created": datetime,
         "Description": str,
         "GameKey": str,
@@ -257,39 +275,22 @@
     {
         "GameName": str,
         "PlayerId": str,
         "StageName": str,
     },
 )
 
-DisconnectPlayerResultTypeDef = TypedDict(
-    "DisconnectPlayerResultTypeDef",
-    {
-        "DisconnectFailures": List[str],
-        "DisconnectSuccesses": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
 
-ExportSnapshotResultTypeDef = TypedDict(
-    "ExportSnapshotResultTypeDef",
-    {
-        "S3Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExtensionDetailsTypeDef = TypedDict(
     "ExtensionDetailsTypeDef",
     {
         "Description": str,
         "Name": str,
         "Namespace": str,
     },
@@ -377,20 +378,22 @@
     "_OptionalGetGameConfigurationRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
+
 class GetGameConfigurationRequestRequestTypeDef(
     _RequiredGetGameConfigurationRequestRequestTypeDef,
     _OptionalGetGameConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetGameRequestRequestTypeDef = TypedDict(
     "GetGameRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
 
@@ -423,19 +426,21 @@
     "_OptionalGetSnapshotRequestRequestTypeDef",
     {
         "Sections": Sequence[str],
     },
     total=False,
 )
 
+
 class GetSnapshotRequestRequestTypeDef(
     _RequiredGetSnapshotRequestRequestTypeDef, _OptionalGetSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredGetStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -443,20 +448,22 @@
     "_OptionalGetStageDeploymentRequestRequestTypeDef",
     {
         "DeploymentId": str,
     },
     total=False,
 )
 
+
 class GetStageDeploymentRequestRequestTypeDef(
     _RequiredGetStageDeploymentRequestRequestTypeDef,
     _OptionalGetStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -464,35 +471,24 @@
 ImportGameConfigurationSourceTypeDef = TypedDict(
     "ImportGameConfigurationSourceTypeDef",
     {
         "File": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
-    {
-        "Name": str,
-        "Namespace": str,
-    },
-)
-_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
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
 
-class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
-    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListExtensionVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListExtensionVersionsRequestRequestTypeDef",
     {
         "Name": str,
         "Namespace": str,
     },
 )
@@ -501,75 +497,40 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListExtensionVersionsRequestRequestTypeDef(
     _RequiredListExtensionVersionsRequestRequestTypeDef,
     _OptionalListExtensionVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
-    "ListExtensionsRequestListExtensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListExtensionsRequestRequestTypeDef = TypedDict(
     "ListExtensionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListGamesRequestListGamesPaginateTypeDef = TypedDict(
-    "ListGamesRequestListGamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGamesRequestRequestTypeDef = TypedDict(
     "ListGamesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "GameName": str,
-        "SnapshotId": str,
-    },
-)
-_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
-    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
-    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGeneratedCodeJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListGeneratedCodeJobsRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -578,39 +539,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListGeneratedCodeJobsRequestRequestTypeDef(
     _RequiredListGeneratedCodeJobsRequestRequestTypeDef,
     _OptionalListGeneratedCodeJobsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
-    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
-    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
-    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
-):
-    pass
 
 _RequiredListSnapshotsRequestRequestTypeDef = TypedDict(
     "_RequiredListSnapshotsRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
@@ -619,51 +562,32 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListSnapshotsRequestRequestTypeDef(
     _RequiredListSnapshotsRequestRequestTypeDef, _OptionalListSnapshotsRequestRequestTypeDef
 ):
     pass
 
+
 SnapshotSummaryTypeDef = TypedDict(
     "SnapshotSummaryTypeDef",
     {
         "Created": datetime,
         "Description": str,
         "Id": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
-_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "GameName": str,
-        "StageName": str,
-    },
-)
-_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
-    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
-):
-    pass
-
 _RequiredListStageDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredListStageDeploymentsRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -672,39 +596,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStageDeploymentsRequestRequestTypeDef(
     _RequiredListStageDeploymentsRequestRequestTypeDef,
     _OptionalListStageDeploymentsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_RequiredListStagesRequestListStagesPaginateTypeDef",
-    {
-        "GameName": str,
-    },
-)
-_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
-    "_OptionalListStagesRequestListStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStagesRequestListStagesPaginateTypeDef(
-    _RequiredListStagesRequestListStagesPaginateTypeDef,
-    _OptionalListStagesRequestListStagesPaginateTypeDef,
-):
-    pass
 
 _RequiredListStagesRequestRequestTypeDef = TypedDict(
     "_RequiredListStagesRequestRequestTypeDef",
     {
         "GameName": str,
     },
 )
@@ -713,19 +619,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListStagesRequestRequestTypeDef(
     _RequiredListStagesRequestRequestTypeDef, _OptionalListStagesRequestRequestTypeDef
 ):
     pass
 
+
 StageSummaryTypeDef = TypedDict(
     "StageSummaryTypeDef",
     {
         "Description": str,
         "GameKey": str,
         "Name": str,
         "State": StageStateType,
@@ -737,43 +645,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
 _RequiredSectionModificationTypeDef = TypedDict(
     "_RequiredSectionModificationTypeDef",
     {
         "Operation": OperationType,
         "Path": str,
         "Section": str,
     },
@@ -782,26 +661,20 @@
     "_OptionalSectionModificationTypeDef",
     {
         "Value": Mapping[str, Any],
     },
     total=False,
 )
 
+
 class SectionModificationTypeDef(
     _RequiredSectionModificationTypeDef, _OptionalSectionModificationTypeDef
 ):
     pass
 
-StartGeneratedCodeJobResultTypeDef = TypedDict(
-    "StartGeneratedCodeJobResultTypeDef",
-    {
-        "GeneratedCodeJobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredStartStageDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredStartStageDeploymentRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
         "StageName": str,
@@ -811,20 +684,22 @@
     "_OptionalStartStageDeploymentRequestRequestTypeDef",
     {
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class StartStageDeploymentRequestRequestTypeDef(
     _RequiredStartStageDeploymentRequestRequestTypeDef,
     _OptionalStartStageDeploymentRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -847,19 +722,21 @@
     "_OptionalUpdateGameRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateGameRequestRequestTypeDef(
     _RequiredUpdateGameRequestRequestTypeDef, _OptionalUpdateGameRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSnapshotRequestRequestTypeDef",
     {
         "GameName": str,
         "SnapshotId": str,
     },
 )
@@ -867,19 +744,21 @@
     "_OptionalUpdateSnapshotRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateSnapshotRequestRequestTypeDef(
     _RequiredUpdateSnapshotRequestRequestTypeDef, _OptionalUpdateSnapshotRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateStageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStageRequestRequestTypeDef",
     {
         "GameName": str,
         "StageName": str,
     },
 )
@@ -888,72 +767,107 @@
     {
         "Description": str,
         "Role": str,
     },
     total=False,
 )
 
+
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
-GetPlayerConnectionStatusResultTypeDef = TypedDict(
-    "GetPlayerConnectionStatusResultTypeDef",
-    {
-        "Connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateGameResultTypeDef = TypedDict(
     "CreateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisconnectPlayerResultTypeDef = TypedDict(
+    "DisconnectPlayerResultTypeDef",
+    {
+        "DisconnectFailures": List[str],
+        "DisconnectSuccesses": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportSnapshotResultTypeDef = TypedDict(
+    "ExportSnapshotResultTypeDef",
+    {
+        "S3Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGameResultTypeDef = TypedDict(
     "GetGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPlayerConnectionStatusResultTypeDef = TypedDict(
+    "GetPlayerConnectionStatusResultTypeDef",
+    {
+        "Connections": List[ConnectionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartGeneratedCodeJobResultTypeDef = TypedDict(
+    "StartGeneratedCodeJobResultTypeDef",
+    {
+        "GeneratedCodeJobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameResultTypeDef = TypedDict(
     "UpdateGameResultTypeDef",
     {
         "Game": GameDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStageResultTypeDef = TypedDict(
     "CreateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResultTypeDef = TypedDict(
     "GetStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStageResultTypeDef = TypedDict(
     "UpdateStageResultTypeDef",
     {
         "Stage": StageDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StageDeploymentDetailsTypeDef = TypedDict(
     "StageDeploymentDetailsTypeDef",
     {
         "Created": datetime,
@@ -980,41 +894,41 @@
     total=False,
 )
 
 GetExtensionResultTypeDef = TypedDict(
     "GetExtensionResultTypeDef",
     {
         "Extension": ExtensionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExtensionsResultTypeDef = TypedDict(
     "ListExtensionsResultTypeDef",
     {
         "Extensions": List[ExtensionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExtensionVersionResultTypeDef = TypedDict(
     "GetExtensionVersionResultTypeDef",
     {
         "ExtensionVersion": ExtensionVersionDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExtensionVersionsResultTypeDef = TypedDict(
     "ListExtensionVersionsResultTypeDef",
     {
         "ExtensionVersions": List[ExtensionVersionDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GameConfigurationDetailsTypeDef = TypedDict(
     "GameConfigurationDetailsTypeDef",
     {
         "Created": datetime,
@@ -1037,32 +951,32 @@
 )
 
 ListGamesResultTypeDef = TypedDict(
     "ListGamesResultTypeDef",
     {
         "Games": List[GameSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeneratedCodeJobResultTypeDef = TypedDict(
     "GetGeneratedCodeJobResultTypeDef",
     {
         "GeneratedCodeJob": GeneratedCodeJobDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeneratedCodeJobsResultTypeDef = TypedDict(
     "ListGeneratedCodeJobsResultTypeDef",
     {
         "GeneratedCodeJobs": List[GeneratedCodeJobDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartGeneratedCodeJobRequestRequestTypeDef = TypedDict(
     "StartGeneratedCodeJobRequestRequestTypeDef",
     {
         "GameName": str,
@@ -1075,29 +989,158 @@
     "ImportGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
         "ImportSource": ImportGameConfigurationSourceTypeDef,
     },
 )
 
+_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "Name": str,
+        "Namespace": str,
+    },
+)
+_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef(
+    _RequiredListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    _OptionalListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListExtensionsRequestListExtensionsPaginateTypeDef = TypedDict(
+    "ListExtensionsRequestListExtensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListGamesRequestListGamesPaginateTypeDef = TypedDict(
+    "ListGamesRequestListGamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "GameName": str,
+        "SnapshotId": str,
+    },
+)
+_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef = TypedDict(
+    "_OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef(
+    _RequiredListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    _OptionalListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef = TypedDict(
+    "_OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSnapshotsRequestListSnapshotsPaginateTypeDef(
+    _RequiredListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    _OptionalListSnapshotsRequestListSnapshotsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "GameName": str,
+        "StageName": str,
+    },
+)
+_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef(
+    _RequiredListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    _OptionalListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_RequiredListStagesRequestListStagesPaginateTypeDef",
+    {
+        "GameName": str,
+    },
+)
+_OptionalListStagesRequestListStagesPaginateTypeDef = TypedDict(
+    "_OptionalListStagesRequestListStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStagesRequestListStagesPaginateTypeDef(
+    _RequiredListStagesRequestListStagesPaginateTypeDef,
+    _OptionalListStagesRequestListStagesPaginateTypeDef,
+):
+    pass
+
+
 ListSnapshotsResultTypeDef = TypedDict(
     "ListSnapshotsResultTypeDef",
     {
         "NextToken": str,
         "Snapshots": List[SnapshotSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStagesResultTypeDef = TypedDict(
     "ListStagesResultTypeDef",
     {
         "NextToken": str,
         "Stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateGameConfigurationRequestRequestTypeDef",
     {
         "GameName": str,
@@ -1105,75 +1148,75 @@
     },
 )
 
 GetStageDeploymentResultTypeDef = TypedDict(
     "GetStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartStageDeploymentResultTypeDef = TypedDict(
     "StartStageDeploymentResultTypeDef",
     {
         "StageDeployment": StageDeploymentDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStageDeploymentsResultTypeDef = TypedDict(
     "ListStageDeploymentsResultTypeDef",
     {
         "NextToken": str,
         "StageDeployments": List[StageDeploymentSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGameConfigurationResultTypeDef = TypedDict(
     "GetGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportGameConfigurationResultTypeDef = TypedDict(
     "ImportGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGameConfigurationResultTypeDef = TypedDict(
     "UpdateGameConfigurationResultTypeDef",
     {
         "GameConfiguration": GameConfigurationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSnapshotResultTypeDef = TypedDict(
     "CreateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotResultTypeDef = TypedDict(
     "GetSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSnapshotResultTypeDef = TypedDict(
     "UpdateSnapshotResultTypeDef",
     {
         "Snapshot": SnapshotDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/PKG-INFO` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-gamesparks
-Version: 1.28.12
-Summary: Type annotations for boto3.GameSparks 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GameSparks 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-gamesparks.svg?color=blue)](https://pypi.org/project/mypy-boto3-gamesparks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-gamesparks)](https://pepy.tech/project/mypy-boto3-gamesparks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GameSparks 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
+[boto3.GameSparks 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/gamesparks.html#GameSparks)
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
 [mypy-boto3-gamesparks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_gamesparks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,24 +354,23 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_gamesparks.type_defs import (
     ConnectionTypeDef,
     CreateGameRequestRequestTypeDef,
     GameDetailsTypeDef,
+    ResponseMetadataTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateStageRequestRequestTypeDef,
     StageDetailsTypeDef,
     DeleteGameRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeploymentResultTypeDef,
     DisconnectPlayerRequestRequestTypeDef,
-    DisconnectPlayerResultTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    ExportSnapshotResultTypeDef,
     ExtensionDetailsTypeDef,
     ExtensionVersionDetailsTypeDef,
     SectionTypeDef,
     GameSummaryTypeDef,
     GeneratedCodeJobDetailsTypeDef,
     GeneratorTypeDef,
     GetExtensionRequestRequestTypeDef,
@@ -380,45 +379,39 @@
     GetGameRequestRequestTypeDef,
     GetGeneratedCodeJobRequestRequestTypeDef,
     GetPlayerConnectionStatusRequestRequestTypeDef,
     GetSnapshotRequestRequestTypeDef,
     GetStageDeploymentRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
     ImportGameConfigurationSourceTypeDef,
-    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListExtensionVersionsRequestRequestTypeDef,
-    ListExtensionsRequestListExtensionsPaginateTypeDef,
     ListExtensionsRequestRequestTypeDef,
-    ListGamesRequestListGamesPaginateTypeDef,
     ListGamesRequestRequestTypeDef,
-    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
     ListGeneratedCodeJobsRequestRequestTypeDef,
-    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     SnapshotSummaryTypeDef,
-    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
     ListStageDeploymentsRequestRequestTypeDef,
-    ListStagesRequestListStagesPaginateTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SectionModificationTypeDef,
-    StartGeneratedCodeJobResultTypeDef,
     StartStageDeploymentRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateGameRequestRequestTypeDef,
     UpdateSnapshotRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
-    GetPlayerConnectionStatusResultTypeDef,
     CreateGameResultTypeDef,
+    DisconnectPlayerResultTypeDef,
+    ExportSnapshotResultTypeDef,
     GetGameResultTypeDef,
+    GetPlayerConnectionStatusResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartGeneratedCodeJobResultTypeDef,
     UpdateGameResultTypeDef,
     CreateStageResultTypeDef,
     GetStageResultTypeDef,
     UpdateStageResultTypeDef,
     StageDeploymentDetailsTypeDef,
     StageDeploymentSummaryTypeDef,
     GetExtensionResultTypeDef,
@@ -428,14 +421,21 @@
     GameConfigurationDetailsTypeDef,
     SnapshotDetailsTypeDef,
     ListGamesResultTypeDef,
     GetGeneratedCodeJobResultTypeDef,
     ListGeneratedCodeJobsResultTypeDef,
     StartGeneratedCodeJobRequestRequestTypeDef,
     ImportGameConfigurationRequestRequestTypeDef,
+    ListExtensionVersionsRequestListExtensionVersionsPaginateTypeDef,
+    ListExtensionsRequestListExtensionsPaginateTypeDef,
+    ListGamesRequestListGamesPaginateTypeDef,
+    ListGeneratedCodeJobsRequestListGeneratedCodeJobsPaginateTypeDef,
+    ListSnapshotsRequestListSnapshotsPaginateTypeDef,
+    ListStageDeploymentsRequestListStageDeploymentsPaginateTypeDef,
+    ListStagesRequestListStagesPaginateTypeDef,
     ListSnapshotsResultTypeDef,
     ListStagesResultTypeDef,
     UpdateGameConfigurationRequestRequestTypeDef,
     GetStageDeploymentResultTypeDef,
     StartStageDeploymentResultTypeDef,
     ListStageDeploymentsResultTypeDef,
     GetGameConfigurationResultTypeDef,
```

### Comparing `mypy-boto3-gamesparks-1.28.12/mypy_boto3_gamesparks.egg-info/SOURCES.txt` & `mypy-boto3-gamesparks-1.28.15/mypy_boto3_gamesparks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-gamesparks-1.28.12/setup.py` & `mypy-boto3-gamesparks-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-gamesparks",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_gamesparks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GameSparks 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.GameSparks 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

