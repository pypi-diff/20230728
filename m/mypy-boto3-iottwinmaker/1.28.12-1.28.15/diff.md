# Comparing `tmp/mypy-boto3-iottwinmaker-1.28.12.tar.gz` & `tmp/mypy-boto3-iottwinmaker-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iottwinmaker-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
+gzip compressed data, was "mypy-boto3-iottwinmaker-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
```

## Comparing `mypy-boto3-iottwinmaker-1.28.12.tar` & `mypy-boto3-iottwinmaker-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16697 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    47041 2023-07-27 05:24:18.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    46960 2023-07-27 05:24:18.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16697 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:51.000000 mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.288476 mypy-boto3-iottwinmaker-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:24:16.000000 mypy-boto3-iottwinmaker-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16564 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15057 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24767 2023-07-28 20:28:44.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24727 2023-07-28 20:28:43.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9644 2023-07-28 20:28:44.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-07-28 20:28:44.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    46171 2023-07-28 20:28:45.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46090 2023-07-28 20:28:44.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:42.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16564 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:02.000000 mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.505299 mypy-boto3-iottwinmaker-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:28:41.000000 mypy-boto3-iottwinmaker-1.28.15/setup.py
```

### Comparing `mypy-boto3-iottwinmaker-1.28.12/LICENSE` & `mypy-boto3-iottwinmaker-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.12/PKG-INFO` & `mypy-boto3-iottwinmaker-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTTwinMaker 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,41 +316,31 @@
 ### Typed dictionaries
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
+    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
-    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
-    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    LambdaFunctionOutputTypeDef,
     LambdaFunctionTypeDef,
-    RelationshipOutputTypeDef,
     RelationshipTypeDef,
-    RelationshipValueOutputTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
-    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
-    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
-    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
@@ -359,42 +349,48 @@
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
-    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueOutputTypeDef,
     PropertyValueTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComponentTypeResponseTypeDef,
-    UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
-    UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
+    CreateSceneResponseTypeDef,
+    CreateSyncJobResponseTypeDef,
+    CreateWorkspaceResponseTypeDef,
+    DeleteComponentTypeResponseTypeDef,
+    DeleteEntityResponseTypeDef,
+    DeleteSyncJobResponseTypeDef,
+    GetWorkspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateComponentTypeResponseTypeDef,
+    UpdateEntityResponseTypeDef,
+    UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
-    DataConnectorOutputTypeDef,
     DataConnectorTypeDef,
     DataTypeOutputTypeDef,
     DataTypeTypeDef,
     DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
@@ -413,43 +409,43 @@
     PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
     PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
-    FunctionResponseTypeDef,
     FunctionRequestTypeDef,
+    FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
     BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
-    GetComponentTypeResponseTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
+    GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> BundleInformationTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iottwinmaker-1.28.12/README.md` & `mypy-boto3-iottwinmaker-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -284,41 +284,31 @@
 ### Typed dictionaries
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
+    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
-    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
-    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    LambdaFunctionOutputTypeDef,
     LambdaFunctionTypeDef,
-    RelationshipOutputTypeDef,
     RelationshipTypeDef,
-    RelationshipValueOutputTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
-    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
-    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
-    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
@@ -327,42 +317,48 @@
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
-    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueOutputTypeDef,
     PropertyValueTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComponentTypeResponseTypeDef,
-    UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
-    UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
+    CreateSceneResponseTypeDef,
+    CreateSyncJobResponseTypeDef,
+    CreateWorkspaceResponseTypeDef,
+    DeleteComponentTypeResponseTypeDef,
+    DeleteEntityResponseTypeDef,
+    DeleteSyncJobResponseTypeDef,
+    GetWorkspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateComponentTypeResponseTypeDef,
+    UpdateEntityResponseTypeDef,
+    UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
-    DataConnectorOutputTypeDef,
     DataConnectorTypeDef,
     DataTypeOutputTypeDef,
     DataTypeTypeDef,
     DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
@@ -381,43 +377,43 @@
     PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
     PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
-    FunctionResponseTypeDef,
     FunctionRequestTypeDef,
+    FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
     BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
-    GetComponentTypeResponseTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
+    GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> BundleInformationTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/__main__.py` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTTwinMaker 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTTwinMaker 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker\nOther"
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

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/client.py` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/client.pyi` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/literals.py` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/literals.pyi` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/type_defs.py` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iottwinmaker service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iottwinmaker.type_defs import BundleInformationTypeDef
+    from mypy_boto3_iottwinmaker.type_defs import ResponseMetadataTypeDef
 
-    data: BundleInformationTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -42,41 +42,31 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "ResponseMetadataTypeDef",
     "BundleInformationTypeDef",
     "ColumnDescriptionTypeDef",
     "ComponentPropertyGroupRequestTypeDef",
     "ComponentPropertyGroupResponseTypeDef",
     "PropertyDefinitionRequestTypeDef",
     "PropertyGroupRequestTypeDef",
-    "CreateComponentTypeResponseTypeDef",
-    "CreateEntityResponseTypeDef",
     "CreateSceneRequestRequestTypeDef",
-    "CreateSceneResponseTypeDef",
     "CreateSyncJobRequestRequestTypeDef",
-    "CreateSyncJobResponseTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
-    "CreateWorkspaceResponseTypeDef",
-    "LambdaFunctionOutputTypeDef",
     "LambdaFunctionTypeDef",
-    "RelationshipOutputTypeDef",
     "RelationshipTypeDef",
-    "RelationshipValueOutputTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
-    "DeleteComponentTypeResponseTypeDef",
     "DeleteEntityRequestRequestTypeDef",
-    "DeleteEntityResponseTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
-    "DeleteSyncJobResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
     "EntityPropertyReferenceOutputTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
@@ -85,42 +75,48 @@
     "GetEntityRequestRequestTypeDef",
     "InterpolationParametersTypeDef",
     "PropertyFilterTypeDef",
     "GetSceneRequestRequestTypeDef",
     "SceneErrorTypeDef",
     "GetSyncJobRequestRequestTypeDef",
     "GetWorkspaceRequestRequestTypeDef",
-    "GetWorkspaceResponseTypeDef",
     "ListComponentTypesFilterTypeDef",
     "ListEntitiesFilterTypeDef",
     "ListScenesRequestRequestTypeDef",
     "SceneSummaryTypeDef",
     "ListSyncJobsRequestRequestTypeDef",
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
     "PropertyValueOutputTypeDef",
     "PropertyValueTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateComponentTypeResponseTypeDef",
-    "UpdateEntityResponseTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
-    "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
+    "CreateComponentTypeResponseTypeDef",
+    "CreateEntityResponseTypeDef",
+    "CreateSceneResponseTypeDef",
+    "CreateSyncJobResponseTypeDef",
+    "CreateWorkspaceResponseTypeDef",
+    "DeleteComponentTypeResponseTypeDef",
+    "DeleteEntityResponseTypeDef",
+    "DeleteSyncJobResponseTypeDef",
+    "GetWorkspaceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateComponentTypeResponseTypeDef",
+    "UpdateEntityResponseTypeDef",
+    "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
-    "DataConnectorOutputTypeDef",
     "DataConnectorTypeDef",
     "DataTypeOutputTypeDef",
     "DataTypeTypeDef",
     "DataValueOutputTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
@@ -139,41 +135,52 @@
     "PropertyValueEntryOutputTypeDef",
     "PropertyValueHistoryTypeDef",
     "PropertyValueEntryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
-    "FunctionResponseTypeDef",
     "FunctionRequestTypeDef",
+    "FunctionResponseTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
     "BatchPutPropertyErrorTypeDef",
     "GetPropertyValueHistoryResponseTypeDef",
     "BatchPutPropertyValuesRequestRequestTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
-    "GetComponentTypeResponseTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
+    "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
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
 _RequiredBundleInformationTypeDef = TypedDict(
     "_RequiredBundleInformationTypeDef",
     {
         "bundleNames": List[str],
     },
 )
 _OptionalBundleInformationTypeDef = TypedDict(
@@ -239,35 +246,14 @@
     {
         "groupType": Literal["TABULAR"],
         "propertyNames": Sequence[str],
     },
     total=False,
 )
 
-CreateComponentTypeResponseTypeDef = TypedDict(
-    "CreateComponentTypeResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEntityResponseTypeDef = TypedDict(
-    "CreateEntityResponseTypeDef",
-    {
-        "entityId": str,
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSceneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
     },
@@ -286,23 +272,14 @@
 
 class CreateSceneRequestRequestTypeDef(
     _RequiredCreateSceneRequestRequestTypeDef, _OptionalCreateSceneRequestRequestTypeDef
 ):
     pass
 
 
-CreateSceneResponseTypeDef = TypedDict(
-    "CreateSceneResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSyncJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
     },
@@ -318,24 +295,14 @@
 
 class CreateSyncJobRequestRequestTypeDef(
     _RequiredCreateSyncJobRequestRequestTypeDef, _OptionalCreateSyncJobRequestRequestTypeDef
 ):
     pass
 
 
-CreateSyncJobResponseTypeDef = TypedDict(
-    "CreateSyncJobResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": SyncJobStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
         "s3Location": str,
         "role": str,
     },
@@ -352,64 +319,30 @@
 
 class CreateWorkspaceRequestRequestTypeDef(
     _RequiredCreateWorkspaceRequestRequestTypeDef, _OptionalCreateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LambdaFunctionOutputTypeDef = TypedDict(
-    "LambdaFunctionOutputTypeDef",
-    {
-        "arn": str,
-    },
-)
-
 LambdaFunctionTypeDef = TypedDict(
     "LambdaFunctionTypeDef",
     {
         "arn": str,
     },
 )
 
-RelationshipOutputTypeDef = TypedDict(
-    "RelationshipOutputTypeDef",
-    {
-        "targetComponentTypeId": str,
-        "relationshipType": str,
-    },
-    total=False,
-)
-
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "targetComponentTypeId": str,
         "relationshipType": str,
     },
     total=False,
 )
 
-RelationshipValueOutputTypeDef = TypedDict(
-    "RelationshipValueOutputTypeDef",
-    {
-        "targetEntityId": str,
-        "targetComponentName": str,
-    },
-    total=False,
-)
-
 RelationshipValueTypeDef = TypedDict(
     "RelationshipValueTypeDef",
     {
         "targetEntityId": str,
         "targetComponentName": str,
     },
     total=False,
@@ -419,22 +352,14 @@
     "DeleteComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
 
-DeleteComponentTypeResponseTypeDef = TypedDict(
-    "DeleteComponentTypeResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityId": str,
     },
 )
@@ -449,22 +374,14 @@
 
 class DeleteEntityRequestRequestTypeDef(
     _RequiredDeleteEntityRequestRequestTypeDef, _OptionalDeleteEntityRequestRequestTypeDef
 ):
     pass
 
 
-DeleteEntityResponseTypeDef = TypedDict(
-    "DeleteEntityResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSceneRequestRequestTypeDef = TypedDict(
     "DeleteSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -473,22 +390,14 @@
     "DeleteSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
     },
 )
 
-DeleteSyncJobResponseTypeDef = TypedDict(
-    "DeleteSyncJobResponseTypeDef",
-    {
-        "state": SyncJobStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
@@ -693,28 +602,14 @@
 GetWorkspaceRequestRequestTypeDef = TypedDict(
     "GetWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
-GetWorkspaceResponseTypeDef = TypedDict(
-    "GetWorkspaceResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "description": str,
-        "s3Location": str,
-        "role": str,
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListComponentTypesFilterTypeDef = TypedDict(
     "ListComponentTypesFilterTypeDef",
     {
         "extendsFrom": str,
         "namespace": str,
         "isAbstract": bool,
     },
@@ -828,23 +723,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -950,25 +836,14 @@
 )
 
 
 class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -977,34 +852,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateComponentTypeResponseTypeDef = TypedDict(
-    "UpdateComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "componentTypeId": str,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateEntityResponseTypeDef = TypedDict(
-    "UpdateEntityResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePricingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePricingPlanRequestRequestTypeDef",
     {
         "pricingMode": PricingModeType,
     },
 )
 _OptionalUpdatePricingPlanRequestRequestTypeDef = TypedDict(
@@ -1043,22 +898,14 @@
 
 class UpdateSceneRequestRequestTypeDef(
     _RequiredUpdateSceneRequestRequestTypeDef, _OptionalUpdateSceneRequestRequestTypeDef
 ):
     pass
 
 
-UpdateSceneResponseTypeDef = TypedDict(
-    "UpdateSceneResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalUpdateWorkspaceRequestRequestTypeDef = TypedDict(
@@ -1073,19 +920,143 @@
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
 
+CreateComponentTypeResponseTypeDef = TypedDict(
+    "CreateComponentTypeResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEntityResponseTypeDef = TypedDict(
+    "CreateEntityResponseTypeDef",
+    {
+        "entityId": str,
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSceneResponseTypeDef = TypedDict(
+    "CreateSceneResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSyncJobResponseTypeDef = TypedDict(
+    "CreateSyncJobResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": SyncJobStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteComponentTypeResponseTypeDef = TypedDict(
+    "DeleteComponentTypeResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEntityResponseTypeDef = TypedDict(
+    "DeleteEntityResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSyncJobResponseTypeDef = TypedDict(
+    "DeleteSyncJobResponseTypeDef",
+    {
+        "state": SyncJobStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkspaceResponseTypeDef = TypedDict(
+    "GetWorkspaceResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "description": str,
+        "s3Location": str,
+        "role": str,
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComponentTypeResponseTypeDef = TypedDict(
+    "UpdateComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "componentTypeId": str,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEntityResponseTypeDef = TypedDict(
+    "UpdateEntityResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSceneResponseTypeDef = TypedDict(
+    "UpdateSceneResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPricingPlanTypeDef = TypedDict(
     "_RequiredPricingPlanTypeDef",
     {
         "effectiveDateTime": datetime,
@@ -1114,23 +1085,14 @@
         "definition": PropertyDefinitionRequestTypeDef,
         "value": "DataValueTypeDef",
         "updateType": PropertyUpdateTypeType,
     },
     total=False,
 )
 
-DataConnectorOutputTypeDef = TypedDict(
-    "DataConnectorOutputTypeDef",
-    {
-        "lambda": LambdaFunctionOutputTypeDef,
-        "isNative": bool,
-    },
-    total=False,
-)
-
 DataConnectorTypeDef = TypedDict(
     "DataConnectorTypeDef",
     {
         "lambda": LambdaFunctionTypeDef,
         "isNative": bool,
     },
     total=False,
@@ -1144,15 +1106,15 @@
 )
 _OptionalDataTypeOutputTypeDef = TypedDict(
     "_OptionalDataTypeOutputTypeDef",
     {
         "nestedType": Dict[str, Any],
         "allowedValues": List["DataValueOutputTypeDef"],
         "unitOfMeasure": str,
-        "relationship": RelationshipOutputTypeDef,
+        "relationship": RelationshipTypeDef,
     },
     total=False,
 )
 
 
 class DataTypeOutputTypeDef(_RequiredDataTypeOutputTypeDef, _OptionalDataTypeOutputTypeDef):
     pass
@@ -1186,15 +1148,15 @@
         "booleanValue": bool,
         "doubleValue": float,
         "integerValue": int,
         "longValue": int,
         "stringValue": str,
         "listValue": List[Dict[str, Any]],
         "mapValue": Dict[str, Dict[str, Any]],
-        "relationshipValue": RelationshipValueOutputTypeDef,
+        "relationshipValue": RelationshipValueTypeDef,
         "expression": str,
     },
     total=False,
 )
 
 DataValueTypeDef = TypedDict(
     "DataValueTypeDef",
@@ -1262,15 +1224,15 @@
 
 ExecuteQueryResponseTypeDef = TypedDict(
     "ExecuteQueryResponseTypeDef",
     {
         "columnDescriptions": List[ColumnDescriptionTypeDef],
         "rows": List[RowTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
@@ -1323,15 +1285,15 @@
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "description": str,
         "capabilities": List[str],
         "sceneMetadata": Dict[str, str],
         "generatedSceneMetadata": Dict[str, str],
         "error": SceneErrorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListComponentTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentTypesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1379,15 +1341,15 @@
 
 
 ListScenesResponseTypeDef = TypedDict(
     "ListScenesResponseTypeDef",
     {
         "sceneSummaries": List[SceneSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSyncResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListSyncResourcesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1412,15 +1374,15 @@
 
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "workspaceSummaries": List[WorkspaceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TabularConditionsTypeDef = TypedDict(
     "TabularConditionsTypeDef",
     {
         "orderBy": Sequence[OrderByTypeDef],
@@ -1493,24 +1455,24 @@
 
 
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePricingPlanResponseTypeDef = TypedDict(
     "UpdatePricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentRequestTypeDef = TypedDict(
     "ComponentRequestTypeDef",
     {
         "description": str,
@@ -1529,42 +1491,42 @@
         "componentTypeId": str,
         "propertyUpdates": Mapping[str, PropertyRequestTypeDef],
         "propertyGroupUpdates": Mapping[str, ComponentPropertyGroupRequestTypeDef],
     },
     total=False,
 )
 
-FunctionResponseTypeDef = TypedDict(
-    "FunctionResponseTypeDef",
+FunctionRequestTypeDef = TypedDict(
+    "FunctionRequestTypeDef",
     {
-        "requiredProperties": List[str],
+        "requiredProperties": Sequence[str],
         "scope": ScopeType,
-        "implementedBy": DataConnectorOutputTypeDef,
-        "isInherited": bool,
+        "implementedBy": DataConnectorTypeDef,
     },
     total=False,
 )
 
-FunctionRequestTypeDef = TypedDict(
-    "FunctionRequestTypeDef",
+FunctionResponseTypeDef = TypedDict(
+    "FunctionResponseTypeDef",
     {
-        "requiredProperties": Sequence[str],
+        "requiredProperties": List[str],
         "scope": ScopeType,
         "implementedBy": DataConnectorTypeDef,
+        "isInherited": bool,
     },
     total=False,
 )
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
         "tabularPropertyValues": List[List[Dict[str, "DataValueOutputTypeDef"]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
         "arn": str,
@@ -1622,15 +1584,15 @@
         "arn": str,
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
         "status": SyncJobStatusTypeDef,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SyncJobSummaryTypeDef = TypedDict(
     "SyncJobSummaryTypeDef",
     {
         "arn": str,
@@ -1708,15 +1670,15 @@
 )
 
 GetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetPropertyValueHistoryResponseTypeDef",
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
     "BatchPutPropertyValuesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1771,37 +1733,14 @@
 
 class UpdateEntityRequestRequestTypeDef(
     _RequiredUpdateEntityRequestRequestTypeDef, _OptionalUpdateEntityRequestRequestTypeDef
 ):
     pass
 
 
-GetComponentTypeResponseTypeDef = TypedDict(
-    "GetComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "isSingleton": bool,
-        "componentTypeId": str,
-        "description": str,
-        "propertyDefinitions": Dict[str, PropertyDefinitionResponseTypeDef],
-        "extendsFrom": List[str],
-        "functions": Dict[str, FunctionResponseTypeDef],
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "arn": str,
-        "isAbstract": bool,
-        "isSchemaInitialized": bool,
-        "status": StatusTypeDef,
-        "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
-        "syncSource": str,
-        "componentTypeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateComponentTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
@@ -1853,49 +1792,72 @@
 class UpdateComponentTypeRequestRequestTypeDef(
     _RequiredUpdateComponentTypeRequestRequestTypeDef,
     _OptionalUpdateComponentTypeRequestRequestTypeDef,
 ):
     pass
 
 
+GetComponentTypeResponseTypeDef = TypedDict(
+    "GetComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "isSingleton": bool,
+        "componentTypeId": str,
+        "description": str,
+        "propertyDefinitions": Dict[str, PropertyDefinitionResponseTypeDef],
+        "extendsFrom": List[str],
+        "functions": Dict[str, FunctionResponseTypeDef],
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "arn": str,
+        "isAbstract": bool,
+        "isSchemaInitialized": bool,
+        "status": StatusTypeDef,
+        "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
+        "syncSource": str,
+        "componentTypeName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListComponentTypesResponseTypeDef = TypedDict(
     "ListComponentTypesResponseTypeDef",
     {
         "workspaceId": str,
         "componentTypeSummaries": List[ComponentTypeSummaryTypeDef],
         "nextToken": str,
         "maxResults": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "entitySummaries": List[EntitySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSyncJobsResponseTypeDef = TypedDict(
     "ListSyncJobsResponseTypeDef",
     {
         "syncJobSummaries": List[SyncJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSyncResourcesResponseTypeDef = TypedDict(
     "ListSyncResourcesResponseTypeDef",
     {
         "syncResources": List[SyncResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEntityResponseTypeDef = TypedDict(
     "GetEntityResponseTypeDef",
     {
         "entityId": str,
@@ -1906,25 +1868,25 @@
         "description": str,
         "components": Dict[str, ComponentResponseTypeDef],
         "parentEntityId": str,
         "hasChildEntities": bool,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutPropertyErrorEntryTypeDef",
     {
         "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker/type_defs.pyi` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iottwinmaker service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iottwinmaker.type_defs import BundleInformationTypeDef
+    from mypy_boto3_iottwinmaker.type_defs import ResponseMetadataTypeDef
 
-    data: BundleInformationTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -41,41 +41,31 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "ResponseMetadataTypeDef",
     "BundleInformationTypeDef",
     "ColumnDescriptionTypeDef",
     "ComponentPropertyGroupRequestTypeDef",
     "ComponentPropertyGroupResponseTypeDef",
     "PropertyDefinitionRequestTypeDef",
     "PropertyGroupRequestTypeDef",
-    "CreateComponentTypeResponseTypeDef",
-    "CreateEntityResponseTypeDef",
     "CreateSceneRequestRequestTypeDef",
-    "CreateSceneResponseTypeDef",
     "CreateSyncJobRequestRequestTypeDef",
-    "CreateSyncJobResponseTypeDef",
     "CreateWorkspaceRequestRequestTypeDef",
-    "CreateWorkspaceResponseTypeDef",
-    "LambdaFunctionOutputTypeDef",
     "LambdaFunctionTypeDef",
-    "RelationshipOutputTypeDef",
     "RelationshipTypeDef",
-    "RelationshipValueOutputTypeDef",
     "RelationshipValueTypeDef",
     "DeleteComponentTypeRequestRequestTypeDef",
-    "DeleteComponentTypeResponseTypeDef",
     "DeleteEntityRequestRequestTypeDef",
-    "DeleteEntityResponseTypeDef",
     "DeleteSceneRequestRequestTypeDef",
     "DeleteSyncJobRequestRequestTypeDef",
-    "DeleteSyncJobResponseTypeDef",
     "DeleteWorkspaceRequestRequestTypeDef",
     "EntityPropertyReferenceOutputTypeDef",
     "EntityPropertyReferenceTypeDef",
     "ErrorDetailsTypeDef",
     "ExecuteQueryRequestRequestTypeDef",
     "RowTypeDef",
     "GetComponentTypeRequestRequestTypeDef",
@@ -84,42 +74,48 @@
     "GetEntityRequestRequestTypeDef",
     "InterpolationParametersTypeDef",
     "PropertyFilterTypeDef",
     "GetSceneRequestRequestTypeDef",
     "SceneErrorTypeDef",
     "GetSyncJobRequestRequestTypeDef",
     "GetWorkspaceRequestRequestTypeDef",
-    "GetWorkspaceResponseTypeDef",
     "ListComponentTypesFilterTypeDef",
     "ListEntitiesFilterTypeDef",
     "ListScenesRequestRequestTypeDef",
     "SceneSummaryTypeDef",
     "ListSyncJobsRequestRequestTypeDef",
     "SyncResourceFilterTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListWorkspacesRequestRequestTypeDef",
     "WorkspaceSummaryTypeDef",
     "OrderByTypeDef",
     "ParentEntityUpdateRequestTypeDef",
     "PropertyValueOutputTypeDef",
     "PropertyValueTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateComponentTypeResponseTypeDef",
-    "UpdateEntityResponseTypeDef",
     "UpdatePricingPlanRequestRequestTypeDef",
     "UpdateSceneRequestRequestTypeDef",
-    "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceRequestRequestTypeDef",
+    "CreateComponentTypeResponseTypeDef",
+    "CreateEntityResponseTypeDef",
+    "CreateSceneResponseTypeDef",
+    "CreateSyncJobResponseTypeDef",
+    "CreateWorkspaceResponseTypeDef",
+    "DeleteComponentTypeResponseTypeDef",
+    "DeleteEntityResponseTypeDef",
+    "DeleteSyncJobResponseTypeDef",
+    "GetWorkspaceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateComponentTypeResponseTypeDef",
+    "UpdateEntityResponseTypeDef",
+    "UpdateSceneResponseTypeDef",
     "UpdateWorkspaceResponseTypeDef",
     "PricingPlanTypeDef",
     "PropertyRequestTypeDef",
-    "DataConnectorOutputTypeDef",
     "DataConnectorTypeDef",
     "DataTypeOutputTypeDef",
     "DataTypeTypeDef",
     "DataValueOutputTypeDef",
     "DataValueTypeDef",
     "PropertyLatestValueTypeDef",
     "StatusTypeDef",
@@ -138,41 +134,52 @@
     "PropertyValueEntryOutputTypeDef",
     "PropertyValueHistoryTypeDef",
     "PropertyValueEntryTypeDef",
     "GetPricingPlanResponseTypeDef",
     "UpdatePricingPlanResponseTypeDef",
     "ComponentRequestTypeDef",
     "ComponentUpdateRequestTypeDef",
-    "FunctionResponseTypeDef",
     "FunctionRequestTypeDef",
+    "FunctionResponseTypeDef",
     "GetPropertyValueResponseTypeDef",
     "ComponentTypeSummaryTypeDef",
     "EntitySummaryTypeDef",
     "GetSyncJobResponseTypeDef",
     "SyncJobSummaryTypeDef",
     "SyncResourceSummaryTypeDef",
     "ComponentResponseTypeDef",
     "GetPropertyValueRequestRequestTypeDef",
     "BatchPutPropertyErrorTypeDef",
     "GetPropertyValueHistoryResponseTypeDef",
     "BatchPutPropertyValuesRequestRequestTypeDef",
     "CreateEntityRequestRequestTypeDef",
     "UpdateEntityRequestRequestTypeDef",
-    "GetComponentTypeResponseTypeDef",
     "CreateComponentTypeRequestRequestTypeDef",
     "UpdateComponentTypeRequestRequestTypeDef",
+    "GetComponentTypeResponseTypeDef",
     "ListComponentTypesResponseTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListSyncJobsResponseTypeDef",
     "ListSyncResourcesResponseTypeDef",
     "GetEntityResponseTypeDef",
     "BatchPutPropertyErrorEntryTypeDef",
     "BatchPutPropertyValuesResponseTypeDef",
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
 _RequiredBundleInformationTypeDef = TypedDict(
     "_RequiredBundleInformationTypeDef",
     {
         "bundleNames": List[str],
     },
 )
 _OptionalBundleInformationTypeDef = TypedDict(
@@ -236,35 +243,14 @@
     {
         "groupType": Literal["TABULAR"],
         "propertyNames": Sequence[str],
     },
     total=False,
 )
 
-CreateComponentTypeResponseTypeDef = TypedDict(
-    "CreateComponentTypeResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateEntityResponseTypeDef = TypedDict(
-    "CreateEntityResponseTypeDef",
-    {
-        "entityId": str,
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSceneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
         "contentLocation": str,
     },
@@ -281,23 +267,14 @@
 )
 
 class CreateSceneRequestRequestTypeDef(
     _RequiredCreateSceneRequestRequestTypeDef, _OptionalCreateSceneRequestRequestTypeDef
 ):
     pass
 
-CreateSceneResponseTypeDef = TypedDict(
-    "CreateSceneResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSyncJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
     },
@@ -311,24 +288,14 @@
 )
 
 class CreateSyncJobRequestRequestTypeDef(
     _RequiredCreateSyncJobRequestRequestTypeDef, _OptionalCreateSyncJobRequestRequestTypeDef
 ):
     pass
 
-CreateSyncJobResponseTypeDef = TypedDict(
-    "CreateSyncJobResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "state": SyncJobStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
         "s3Location": str,
         "role": str,
     },
@@ -343,64 +310,30 @@
 )
 
 class CreateWorkspaceRequestRequestTypeDef(
     _RequiredCreateWorkspaceRequestRequestTypeDef, _OptionalCreateWorkspaceRequestRequestTypeDef
 ):
     pass
 
-CreateWorkspaceResponseTypeDef = TypedDict(
-    "CreateWorkspaceResponseTypeDef",
-    {
-        "arn": str,
-        "creationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-LambdaFunctionOutputTypeDef = TypedDict(
-    "LambdaFunctionOutputTypeDef",
-    {
-        "arn": str,
-    },
-)
-
 LambdaFunctionTypeDef = TypedDict(
     "LambdaFunctionTypeDef",
     {
         "arn": str,
     },
 )
 
-RelationshipOutputTypeDef = TypedDict(
-    "RelationshipOutputTypeDef",
-    {
-        "targetComponentTypeId": str,
-        "relationshipType": str,
-    },
-    total=False,
-)
-
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "targetComponentTypeId": str,
         "relationshipType": str,
     },
     total=False,
 )
 
-RelationshipValueOutputTypeDef = TypedDict(
-    "RelationshipValueOutputTypeDef",
-    {
-        "targetEntityId": str,
-        "targetComponentName": str,
-    },
-    total=False,
-)
-
 RelationshipValueTypeDef = TypedDict(
     "RelationshipValueTypeDef",
     {
         "targetEntityId": str,
         "targetComponentName": str,
     },
     total=False,
@@ -410,22 +343,14 @@
     "DeleteComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
 
-DeleteComponentTypeResponseTypeDef = TypedDict(
-    "DeleteComponentTypeResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteEntityRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteEntityRequestRequestTypeDef",
     {
         "workspaceId": str,
         "entityId": str,
     },
 )
@@ -438,22 +363,14 @@
 )
 
 class DeleteEntityRequestRequestTypeDef(
     _RequiredDeleteEntityRequestRequestTypeDef, _OptionalDeleteEntityRequestRequestTypeDef
 ):
     pass
 
-DeleteEntityResponseTypeDef = TypedDict(
-    "DeleteEntityResponseTypeDef",
-    {
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSceneRequestRequestTypeDef = TypedDict(
     "DeleteSceneRequestRequestTypeDef",
     {
         "workspaceId": str,
         "sceneId": str,
     },
 )
@@ -462,22 +379,14 @@
     "DeleteSyncJobRequestRequestTypeDef",
     {
         "workspaceId": str,
         "syncSource": str,
     },
 )
 
-DeleteSyncJobResponseTypeDef = TypedDict(
-    "DeleteSyncJobResponseTypeDef",
-    {
-        "state": SyncJobStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteWorkspaceRequestRequestTypeDef = TypedDict(
     "DeleteWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
@@ -672,28 +581,14 @@
 GetWorkspaceRequestRequestTypeDef = TypedDict(
     "GetWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 
-GetWorkspaceResponseTypeDef = TypedDict(
-    "GetWorkspaceResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "description": str,
-        "s3Location": str,
-        "role": str,
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListComponentTypesFilterTypeDef = TypedDict(
     "ListComponentTypesFilterTypeDef",
     {
         "extendsFrom": str,
         "namespace": str,
         "isAbstract": bool,
     },
@@ -799,23 +694,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListWorkspacesRequestRequestTypeDef = TypedDict(
     "ListWorkspacesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -911,25 +797,14 @@
     },
     total=False,
 )
 
 class PropertyValueTypeDef(_RequiredPropertyValueTypeDef, _OptionalPropertyValueTypeDef):
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tags": Mapping[str, str],
     },
 )
@@ -938,34 +813,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceARN": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateComponentTypeResponseTypeDef = TypedDict(
-    "UpdateComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "arn": str,
-        "componentTypeId": str,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateEntityResponseTypeDef = TypedDict(
-    "UpdateEntityResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "state": StateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePricingPlanRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePricingPlanRequestRequestTypeDef",
     {
         "pricingMode": PricingModeType,
     },
 )
 _OptionalUpdatePricingPlanRequestRequestTypeDef = TypedDict(
@@ -1000,22 +855,14 @@
 )
 
 class UpdateSceneRequestRequestTypeDef(
     _RequiredUpdateSceneRequestRequestTypeDef, _OptionalUpdateSceneRequestRequestTypeDef
 ):
     pass
 
-UpdateSceneResponseTypeDef = TypedDict(
-    "UpdateSceneResponseTypeDef",
-    {
-        "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateWorkspaceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateWorkspaceRequestRequestTypeDef",
     {
         "workspaceId": str,
     },
 )
 _OptionalUpdateWorkspaceRequestRequestTypeDef = TypedDict(
@@ -1028,19 +875,143 @@
 )
 
 class UpdateWorkspaceRequestRequestTypeDef(
     _RequiredUpdateWorkspaceRequestRequestTypeDef, _OptionalUpdateWorkspaceRequestRequestTypeDef
 ):
     pass
 
+CreateComponentTypeResponseTypeDef = TypedDict(
+    "CreateComponentTypeResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEntityResponseTypeDef = TypedDict(
+    "CreateEntityResponseTypeDef",
+    {
+        "entityId": str,
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSceneResponseTypeDef = TypedDict(
+    "CreateSceneResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSyncJobResponseTypeDef = TypedDict(
+    "CreateSyncJobResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "state": SyncJobStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWorkspaceResponseTypeDef = TypedDict(
+    "CreateWorkspaceResponseTypeDef",
+    {
+        "arn": str,
+        "creationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteComponentTypeResponseTypeDef = TypedDict(
+    "DeleteComponentTypeResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEntityResponseTypeDef = TypedDict(
+    "DeleteEntityResponseTypeDef",
+    {
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSyncJobResponseTypeDef = TypedDict(
+    "DeleteSyncJobResponseTypeDef",
+    {
+        "state": SyncJobStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkspaceResponseTypeDef = TypedDict(
+    "GetWorkspaceResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "description": str,
+        "s3Location": str,
+        "role": str,
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateComponentTypeResponseTypeDef = TypedDict(
+    "UpdateComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "arn": str,
+        "componentTypeId": str,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEntityResponseTypeDef = TypedDict(
+    "UpdateEntityResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "state": StateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSceneResponseTypeDef = TypedDict(
+    "UpdateSceneResponseTypeDef",
+    {
+        "updateDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateWorkspaceResponseTypeDef = TypedDict(
     "UpdateWorkspaceResponseTypeDef",
     {
         "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPricingPlanTypeDef = TypedDict(
     "_RequiredPricingPlanTypeDef",
     {
         "effectiveDateTime": datetime,
@@ -1067,23 +1038,14 @@
         "definition": PropertyDefinitionRequestTypeDef,
         "value": "DataValueTypeDef",
         "updateType": PropertyUpdateTypeType,
     },
     total=False,
 )
 
-DataConnectorOutputTypeDef = TypedDict(
-    "DataConnectorOutputTypeDef",
-    {
-        "lambda": LambdaFunctionOutputTypeDef,
-        "isNative": bool,
-    },
-    total=False,
-)
-
 DataConnectorTypeDef = TypedDict(
     "DataConnectorTypeDef",
     {
         "lambda": LambdaFunctionTypeDef,
         "isNative": bool,
     },
     total=False,
@@ -1097,15 +1059,15 @@
 )
 _OptionalDataTypeOutputTypeDef = TypedDict(
     "_OptionalDataTypeOutputTypeDef",
     {
         "nestedType": Dict[str, Any],
         "allowedValues": List["DataValueOutputTypeDef"],
         "unitOfMeasure": str,
-        "relationship": RelationshipOutputTypeDef,
+        "relationship": RelationshipTypeDef,
     },
     total=False,
 )
 
 class DataTypeOutputTypeDef(_RequiredDataTypeOutputTypeDef, _OptionalDataTypeOutputTypeDef):
     pass
 
@@ -1135,15 +1097,15 @@
         "booleanValue": bool,
         "doubleValue": float,
         "integerValue": int,
         "longValue": int,
         "stringValue": str,
         "listValue": List[Dict[str, Any]],
         "mapValue": Dict[str, Dict[str, Any]],
-        "relationshipValue": RelationshipValueOutputTypeDef,
+        "relationshipValue": RelationshipValueTypeDef,
         "expression": str,
     },
     total=False,
 )
 
 DataValueTypeDef = TypedDict(
     "DataValueTypeDef",
@@ -1209,15 +1171,15 @@
 
 ExecuteQueryResponseTypeDef = TypedDict(
     "ExecuteQueryResponseTypeDef",
     {
         "columnDescriptions": List[ColumnDescriptionTypeDef],
         "rows": List[RowTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PropertyResponseTypeDef = TypedDict(
     "PropertyResponseTypeDef",
     {
         "definition": PropertyDefinitionResponseTypeDef,
@@ -1268,15 +1230,15 @@
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "description": str,
         "capabilities": List[str],
         "sceneMetadata": Dict[str, str],
         "generatedSceneMetadata": Dict[str, str],
         "error": SceneErrorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListComponentTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListComponentTypesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1320,15 +1282,15 @@
     pass
 
 ListScenesResponseTypeDef = TypedDict(
     "ListScenesResponseTypeDef",
     {
         "sceneSummaries": List[SceneSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListSyncResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListSyncResourcesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1351,15 +1313,15 @@
     pass
 
 ListWorkspacesResponseTypeDef = TypedDict(
     "ListWorkspacesResponseTypeDef",
     {
         "workspaceSummaries": List[WorkspaceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TabularConditionsTypeDef = TypedDict(
     "TabularConditionsTypeDef",
     {
         "orderBy": Sequence[OrderByTypeDef],
@@ -1426,24 +1388,24 @@
     pass
 
 GetPricingPlanResponseTypeDef = TypedDict(
     "GetPricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePricingPlanResponseTypeDef = TypedDict(
     "UpdatePricingPlanResponseTypeDef",
     {
         "currentPricingPlan": PricingPlanTypeDef,
         "pendingPricingPlan": PricingPlanTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComponentRequestTypeDef = TypedDict(
     "ComponentRequestTypeDef",
     {
         "description": str,
@@ -1462,42 +1424,42 @@
         "componentTypeId": str,
         "propertyUpdates": Mapping[str, PropertyRequestTypeDef],
         "propertyGroupUpdates": Mapping[str, ComponentPropertyGroupRequestTypeDef],
     },
     total=False,
 )
 
-FunctionResponseTypeDef = TypedDict(
-    "FunctionResponseTypeDef",
+FunctionRequestTypeDef = TypedDict(
+    "FunctionRequestTypeDef",
     {
-        "requiredProperties": List[str],
+        "requiredProperties": Sequence[str],
         "scope": ScopeType,
-        "implementedBy": DataConnectorOutputTypeDef,
-        "isInherited": bool,
+        "implementedBy": DataConnectorTypeDef,
     },
     total=False,
 )
 
-FunctionRequestTypeDef = TypedDict(
-    "FunctionRequestTypeDef",
+FunctionResponseTypeDef = TypedDict(
+    "FunctionResponseTypeDef",
     {
-        "requiredProperties": Sequence[str],
+        "requiredProperties": List[str],
         "scope": ScopeType,
         "implementedBy": DataConnectorTypeDef,
+        "isInherited": bool,
     },
     total=False,
 )
 
 GetPropertyValueResponseTypeDef = TypedDict(
     "GetPropertyValueResponseTypeDef",
     {
         "propertyValues": Dict[str, PropertyLatestValueTypeDef],
         "nextToken": str,
         "tabularPropertyValues": List[List[Dict[str, "DataValueOutputTypeDef"]]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredComponentTypeSummaryTypeDef = TypedDict(
     "_RequiredComponentTypeSummaryTypeDef",
     {
         "arn": str,
@@ -1551,15 +1513,15 @@
         "arn": str,
         "workspaceId": str,
         "syncSource": str,
         "syncRole": str,
         "status": SyncJobStatusTypeDef,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SyncJobSummaryTypeDef = TypedDict(
     "SyncJobSummaryTypeDef",
     {
         "arn": str,
@@ -1635,15 +1597,15 @@
 )
 
 GetPropertyValueHistoryResponseTypeDef = TypedDict(
     "GetPropertyValueHistoryResponseTypeDef",
     {
         "propertyValues": List[PropertyValueHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutPropertyValuesRequestRequestTypeDef = TypedDict(
     "BatchPutPropertyValuesRequestRequestTypeDef",
     {
         "workspaceId": str,
@@ -1694,37 +1656,14 @@
 )
 
 class UpdateEntityRequestRequestTypeDef(
     _RequiredUpdateEntityRequestRequestTypeDef, _OptionalUpdateEntityRequestRequestTypeDef
 ):
     pass
 
-GetComponentTypeResponseTypeDef = TypedDict(
-    "GetComponentTypeResponseTypeDef",
-    {
-        "workspaceId": str,
-        "isSingleton": bool,
-        "componentTypeId": str,
-        "description": str,
-        "propertyDefinitions": Dict[str, PropertyDefinitionResponseTypeDef],
-        "extendsFrom": List[str],
-        "functions": Dict[str, FunctionResponseTypeDef],
-        "creationDateTime": datetime,
-        "updateDateTime": datetime,
-        "arn": str,
-        "isAbstract": bool,
-        "isSchemaInitialized": bool,
-        "status": StatusTypeDef,
-        "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
-        "syncSource": str,
-        "componentTypeName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateComponentTypeRequestRequestTypeDef = TypedDict(
     "_RequiredCreateComponentTypeRequestRequestTypeDef",
     {
         "workspaceId": str,
         "componentTypeId": str,
     },
 )
@@ -1772,49 +1711,72 @@
 
 class UpdateComponentTypeRequestRequestTypeDef(
     _RequiredUpdateComponentTypeRequestRequestTypeDef,
     _OptionalUpdateComponentTypeRequestRequestTypeDef,
 ):
     pass
 
+GetComponentTypeResponseTypeDef = TypedDict(
+    "GetComponentTypeResponseTypeDef",
+    {
+        "workspaceId": str,
+        "isSingleton": bool,
+        "componentTypeId": str,
+        "description": str,
+        "propertyDefinitions": Dict[str, PropertyDefinitionResponseTypeDef],
+        "extendsFrom": List[str],
+        "functions": Dict[str, FunctionResponseTypeDef],
+        "creationDateTime": datetime,
+        "updateDateTime": datetime,
+        "arn": str,
+        "isAbstract": bool,
+        "isSchemaInitialized": bool,
+        "status": StatusTypeDef,
+        "propertyGroups": Dict[str, PropertyGroupResponseTypeDef],
+        "syncSource": str,
+        "componentTypeName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListComponentTypesResponseTypeDef = TypedDict(
     "ListComponentTypesResponseTypeDef",
     {
         "workspaceId": str,
         "componentTypeSummaries": List[ComponentTypeSummaryTypeDef],
         "nextToken": str,
         "maxResults": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "entitySummaries": List[EntitySummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSyncJobsResponseTypeDef = TypedDict(
     "ListSyncJobsResponseTypeDef",
     {
         "syncJobSummaries": List[SyncJobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSyncResourcesResponseTypeDef = TypedDict(
     "ListSyncResourcesResponseTypeDef",
     {
         "syncResources": List[SyncResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEntityResponseTypeDef = TypedDict(
     "GetEntityResponseTypeDef",
     {
         "entityId": str,
@@ -1825,25 +1787,25 @@
         "description": str,
         "components": Dict[str, ComponentResponseTypeDef],
         "parentEntityId": str,
         "hasChildEntities": bool,
         "creationDateTime": datetime,
         "updateDateTime": datetime,
         "syncSource": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutPropertyErrorEntryTypeDef = TypedDict(
     "BatchPutPropertyErrorEntryTypeDef",
     {
         "errors": List[BatchPutPropertyErrorTypeDef],
     },
 )
 
 BatchPutPropertyValuesResponseTypeDef = TypedDict(
     "BatchPutPropertyValuesResponseTypeDef",
     {
         "errorEntries": List[BatchPutPropertyErrorEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/PKG-INFO` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iottwinmaker
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTTwinMaker 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iottwinmaker.svg?color=blue)](https://pypi.org/project/mypy-boto3-iottwinmaker)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iottwinmaker)](https://pepy.tech/project/mypy-boto3-iottwinmaker)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTTwinMaker 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
+[boto3.IoTTwinMaker 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iottwinmaker.html#IoTTwinMaker)
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
 [mypy-boto3-iottwinmaker docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iottwinmaker/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,41 +316,31 @@
 ### Typed dictionaries
 
 `mypy_boto3_iottwinmaker.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iottwinmaker.type_defs import (
+    ResponseMetadataTypeDef,
     BundleInformationTypeDef,
     ColumnDescriptionTypeDef,
     ComponentPropertyGroupRequestTypeDef,
     ComponentPropertyGroupResponseTypeDef,
     PropertyDefinitionRequestTypeDef,
     PropertyGroupRequestTypeDef,
-    CreateComponentTypeResponseTypeDef,
-    CreateEntityResponseTypeDef,
     CreateSceneRequestRequestTypeDef,
-    CreateSceneResponseTypeDef,
     CreateSyncJobRequestRequestTypeDef,
-    CreateSyncJobResponseTypeDef,
     CreateWorkspaceRequestRequestTypeDef,
-    CreateWorkspaceResponseTypeDef,
-    LambdaFunctionOutputTypeDef,
     LambdaFunctionTypeDef,
-    RelationshipOutputTypeDef,
     RelationshipTypeDef,
-    RelationshipValueOutputTypeDef,
     RelationshipValueTypeDef,
     DeleteComponentTypeRequestRequestTypeDef,
-    DeleteComponentTypeResponseTypeDef,
     DeleteEntityRequestRequestTypeDef,
-    DeleteEntityResponseTypeDef,
     DeleteSceneRequestRequestTypeDef,
     DeleteSyncJobRequestRequestTypeDef,
-    DeleteSyncJobResponseTypeDef,
     DeleteWorkspaceRequestRequestTypeDef,
     EntityPropertyReferenceOutputTypeDef,
     EntityPropertyReferenceTypeDef,
     ErrorDetailsTypeDef,
     ExecuteQueryRequestRequestTypeDef,
     RowTypeDef,
     GetComponentTypeRequestRequestTypeDef,
@@ -359,42 +349,48 @@
     GetEntityRequestRequestTypeDef,
     InterpolationParametersTypeDef,
     PropertyFilterTypeDef,
     GetSceneRequestRequestTypeDef,
     SceneErrorTypeDef,
     GetSyncJobRequestRequestTypeDef,
     GetWorkspaceRequestRequestTypeDef,
-    GetWorkspaceResponseTypeDef,
     ListComponentTypesFilterTypeDef,
     ListEntitiesFilterTypeDef,
     ListScenesRequestRequestTypeDef,
     SceneSummaryTypeDef,
     ListSyncJobsRequestRequestTypeDef,
     SyncResourceFilterTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListWorkspacesRequestRequestTypeDef,
     WorkspaceSummaryTypeDef,
     OrderByTypeDef,
     ParentEntityUpdateRequestTypeDef,
     PropertyValueOutputTypeDef,
     PropertyValueTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateComponentTypeResponseTypeDef,
-    UpdateEntityResponseTypeDef,
     UpdatePricingPlanRequestRequestTypeDef,
     UpdateSceneRequestRequestTypeDef,
-    UpdateSceneResponseTypeDef,
     UpdateWorkspaceRequestRequestTypeDef,
+    CreateComponentTypeResponseTypeDef,
+    CreateEntityResponseTypeDef,
+    CreateSceneResponseTypeDef,
+    CreateSyncJobResponseTypeDef,
+    CreateWorkspaceResponseTypeDef,
+    DeleteComponentTypeResponseTypeDef,
+    DeleteEntityResponseTypeDef,
+    DeleteSyncJobResponseTypeDef,
+    GetWorkspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateComponentTypeResponseTypeDef,
+    UpdateEntityResponseTypeDef,
+    UpdateSceneResponseTypeDef,
     UpdateWorkspaceResponseTypeDef,
     PricingPlanTypeDef,
     PropertyRequestTypeDef,
-    DataConnectorOutputTypeDef,
     DataConnectorTypeDef,
     DataTypeOutputTypeDef,
     DataTypeTypeDef,
     DataValueOutputTypeDef,
     DataValueTypeDef,
     PropertyLatestValueTypeDef,
     StatusTypeDef,
@@ -413,43 +409,43 @@
     PropertyValueEntryOutputTypeDef,
     PropertyValueHistoryTypeDef,
     PropertyValueEntryTypeDef,
     GetPricingPlanResponseTypeDef,
     UpdatePricingPlanResponseTypeDef,
     ComponentRequestTypeDef,
     ComponentUpdateRequestTypeDef,
-    FunctionResponseTypeDef,
     FunctionRequestTypeDef,
+    FunctionResponseTypeDef,
     GetPropertyValueResponseTypeDef,
     ComponentTypeSummaryTypeDef,
     EntitySummaryTypeDef,
     GetSyncJobResponseTypeDef,
     SyncJobSummaryTypeDef,
     SyncResourceSummaryTypeDef,
     ComponentResponseTypeDef,
     GetPropertyValueRequestRequestTypeDef,
     BatchPutPropertyErrorTypeDef,
     GetPropertyValueHistoryResponseTypeDef,
     BatchPutPropertyValuesRequestRequestTypeDef,
     CreateEntityRequestRequestTypeDef,
     UpdateEntityRequestRequestTypeDef,
-    GetComponentTypeResponseTypeDef,
     CreateComponentTypeRequestRequestTypeDef,
     UpdateComponentTypeRequestRequestTypeDef,
+    GetComponentTypeResponseTypeDef,
     ListComponentTypesResponseTypeDef,
     ListEntitiesResponseTypeDef,
     ListSyncJobsResponseTypeDef,
     ListSyncResourcesResponseTypeDef,
     GetEntityResponseTypeDef,
     BatchPutPropertyErrorEntryTypeDef,
     BatchPutPropertyValuesResponseTypeDef,
 )
 
 
-def get_structure() -> BundleInformationTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iottwinmaker-1.28.12/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt` & `mypy-boto3-iottwinmaker-1.28.15/mypy_boto3_iottwinmaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iottwinmaker-1.28.12/setup.py` & `mypy-boto3-iottwinmaker-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iottwinmaker",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iottwinmaker"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTTwinMaker 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTTwinMaker 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

