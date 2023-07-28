# Comparing `tmp/mypy-boto3-iotthingsgraph-1.28.12.tar.gz` & `tmp/mypy-boto3-iotthingsgraph-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotthingsgraph-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
+gzip compressed data, was "mypy-boto3-iotthingsgraph-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
```

## Comparing `mypy-boto3-iotthingsgraph-1.28.12.tar` & `mypy-boto3-iotthingsgraph-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.068477 mypy-boto3-iotthingsgraph-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19007 2023-07-27 05:34:51.068477 mypy-boto3-iotthingsgraph-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17492 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.056477 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29198 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34361 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34314 2023-07-27 05:24:15.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.068477 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19007 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-27 05:34:50.000000 mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.068477 mypy-boto3-iotthingsgraph-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:24:14.000000 mypy-boto3-iotthingsgraph-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.449298 mypy-boto3-iotthingsgraph-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-07-28 20:43:02.449298 mypy-boto3-iotthingsgraph-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17394 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.441298 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29250 2023-07-28 20:28:40.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29198 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11270 2023-07-28 20:28:40.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-07-28 20:28:40.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13076 2023-07-28 20:28:40.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13064 2023-07-28 20:28:40.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33685 2023-07-28 20:28:41.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33638 2023-07-28 20:28:40.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.449298 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-07-28 20:43:02.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-28 20:43:02.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-28 20:43:02.000000 mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.449298 mypy-boto3-iotthingsgraph-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:28:39.000000 mypy-boto3-iotthingsgraph-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/LICENSE` & `mypy-boto3-iotthingsgraph-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/PKG-INFO` & `mypy-boto3-iotthingsgraph-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotthingsgraph
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTThingsGraph 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTThingsGraph 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -381,93 +381,90 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
+    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
-    DefinitionDocumentOutputTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
-    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
-    GetUploadStatusResponseTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MetricsConfigurationOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
+    EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
+    FlowTemplateDescriptionTypeDef,
     CreateFlowTemplateResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DescribeNamespaceResponseTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
+    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
-    UpdateSystemTemplateResponseTypeDef,
-    EntityDescriptionTypeDef,
-    FlowTemplateDescriptionTypeDef,
     SystemTemplateDescriptionTypeDef,
+    UpdateSystemTemplateResponseTypeDef,
+    SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SystemInstanceDescriptionTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/README.md` & `mypy-boto3-iotthingsgraph-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,93 +349,90 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
+    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
-    DefinitionDocumentOutputTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
-    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
-    GetUploadStatusResponseTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MetricsConfigurationOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
+    EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
+    FlowTemplateDescriptionTypeDef,
     CreateFlowTemplateResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DescribeNamespaceResponseTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
+    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
-    UpdateSystemTemplateResponseTypeDef,
-    EntityDescriptionTypeDef,
-    FlowTemplateDescriptionTypeDef,
     SystemTemplateDescriptionTypeDef,
+    UpdateSystemTemplateResponseTypeDef,
+    SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SystemInstanceDescriptionTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__init__.py` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__init__.pyi` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/__main__.py` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/__main__.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTThingsGraph 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTThingsGraph 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph\nOther"
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

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/client.py` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/client.pyi` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/literals.py` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/literals.pyi` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/paginator.py` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,60 +88,60 @@
 class GetFlowTemplateRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFlowTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
         """
 
 
 class GetSystemTemplateRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSystemTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
         """
 
 
 class ListFlowExecutionMessagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
     """
 
     def paginate(
-        self, *, flowExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, flowExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFlowExecutionMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listtagsforresourcepaginator)
         """
 
 
@@ -153,15 +153,15 @@
 
     def paginate(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         namespaceVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchentitiespaginator)
         """
 
 
@@ -174,15 +174,15 @@
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
         startTime: Union[datetime, str] = ...,
         endTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
 
 
@@ -192,15 +192,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchFlowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowtemplatespaginator)
         """
 
 
@@ -210,15 +210,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsysteminstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchSystemInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsysteminstancespaginator)
         """
 
 
@@ -228,15 +228,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchSystemTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
         """
 
 
@@ -247,13 +247,13 @@
     """
 
     def paginate(
         self,
         *,
         entityId: str,
         namespaceVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchthingspaginator)
         """
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/paginator.pyi` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -85,57 +85,57 @@
 class GetFlowTemplateRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetFlowTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetFlowTemplateRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getflowtemplaterevisionspaginator)
         """
 
 class GetSystemTemplateRevisionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
     """
 
     def paginate(
-        self, *, id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetSystemTemplateRevisionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.GetSystemTemplateRevisions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#getsystemtemplaterevisionspaginator)
         """
 
 class ListFlowExecutionMessagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
     """
 
     def paginate(
-        self, *, flowExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, flowExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFlowExecutionMessagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListFlowExecutionMessages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listflowexecutionmessagespaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#listtagsforresourcepaginator)
         """
 
 class SearchEntitiesPaginator(Paginator):
@@ -146,15 +146,15 @@
 
     def paginate(
         self,
         *,
         entityTypes: Sequence[EntityTypeType],
         filters: Sequence[EntityFilterTypeDef] = ...,
         namespaceVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchEntities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchentitiespaginator)
         """
 
 class SearchFlowExecutionsPaginator(Paginator):
@@ -166,15 +166,15 @@
     def paginate(
         self,
         *,
         systemInstanceId: str,
         flowExecutionId: str = ...,
         startTime: Union[datetime, str] = ...,
         endTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchFlowExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowexecutionspaginator)
         """
 
 class SearchFlowTemplatesPaginator(Paginator):
@@ -183,15 +183,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[FlowTemplateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchFlowTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchFlowTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchflowtemplatespaginator)
         """
 
 class SearchSystemInstancesPaginator(Paginator):
@@ -200,15 +200,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsysteminstancespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemInstanceFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchSystemInstancesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsysteminstancespaginator)
         """
 
 class SearchSystemTemplatesPaginator(Paginator):
@@ -217,15 +217,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[SystemTemplateFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchSystemTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchSystemTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchsystemtemplatespaginator)
         """
 
 class SearchThingsPaginator(Paginator):
@@ -235,13 +235,13 @@
     """
 
     def paginate(
         self,
         *,
         entityId: str,
         namespaceVersion: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[SearchThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph.Paginator.SearchThings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/paginators/#searchthingspaginator)
         """
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/type_defs.py` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -32,98 +32,94 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
     "SystemInstanceSummaryTypeDef",
     "SystemTemplateSummaryTypeDef",
-    "DefinitionDocumentOutputTypeDef",
     "DeleteFlowTemplateRequestRequestTypeDef",
-    "DeleteNamespaceResponseTypeDef",
     "DeleteSystemInstanceRequestRequestTypeDef",
     "DeleteSystemTemplateRequestRequestTypeDef",
     "DependencyRevisionTypeDef",
     "DeploySystemInstanceRequestRequestTypeDef",
     "DeprecateFlowTemplateRequestRequestTypeDef",
     "DeprecateSystemTemplateRequestRequestTypeDef",
     "DescribeNamespaceRequestRequestTypeDef",
-    "DescribeNamespaceResponseTypeDef",
     "DissociateEntityFromThingRequestRequestTypeDef",
     "EntityFilterTypeDef",
     "FlowExecutionMessageTypeDef",
     "FlowExecutionSummaryTypeDef",
     "FlowTemplateFilterTypeDef",
     "GetEntitiesRequestRequestTypeDef",
     "GetFlowTemplateRequestRequestTypeDef",
-    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetFlowTemplateRevisionsRequestRequestTypeDef",
-    "GetNamespaceDeletionStatusResponseTypeDef",
     "GetSystemInstanceRequestRequestTypeDef",
     "GetSystemTemplateRequestRequestTypeDef",
-    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
-    "GetUploadStatusResponseTypeDef",
-    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "MetricsConfigurationOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchFlowExecutionsRequestRequestTypeDef",
-    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
-    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadEntityDefinitionsResponseTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
     "CreateSystemTemplateRequestRequestTypeDef",
+    "EntityDescriptionTypeDef",
     "UpdateFlowTemplateRequestRequestTypeDef",
     "UpdateSystemTemplateRequestRequestTypeDef",
     "UploadEntityDefinitionsRequestRequestTypeDef",
+    "FlowTemplateDescriptionTypeDef",
     "CreateFlowTemplateResponseTypeDef",
+    "DeleteNamespaceResponseTypeDef",
+    "DescribeNamespaceResponseTypeDef",
     "GetFlowTemplateRevisionsResponseTypeDef",
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    "GetUploadStatusResponseTypeDef",
     "SearchFlowTemplatesResponseTypeDef",
     "UpdateFlowTemplateResponseTypeDef",
+    "UploadEntityDefinitionsResponseTypeDef",
     "CreateSystemInstanceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSystemInstanceResponseTypeDef",
     "DeploySystemInstanceResponseTypeDef",
     "SearchSystemInstancesResponseTypeDef",
     "UndeploySystemInstanceResponseTypeDef",
     "CreateSystemTemplateResponseTypeDef",
     "GetSystemTemplateRevisionsResponseTypeDef",
     "SearchSystemTemplatesResponseTypeDef",
-    "UpdateSystemTemplateResponseTypeDef",
-    "EntityDescriptionTypeDef",
-    "FlowTemplateDescriptionTypeDef",
     "SystemTemplateDescriptionTypeDef",
+    "UpdateSystemTemplateResponseTypeDef",
+    "SystemInstanceDescriptionTypeDef",
     "SearchEntitiesRequestRequestTypeDef",
-    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "ListFlowExecutionMessagesResponseTypeDef",
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
+    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
+    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SystemInstanceDescriptionTypeDef",
+    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -143,22 +139,20 @@
     "_OptionalAssociateEntityToThingRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class AssociateEntityToThingRequestRequestTypeDef(
     _RequiredAssociateEntityToThingRequestRequestTypeDef,
     _OptionalAssociateEntityToThingRequestRequestTypeDef,
 ):
     pass
 
-
 DefinitionDocumentTypeDef = TypedDict(
     "DefinitionDocumentTypeDef",
     {
         "language": Literal["GRAPHQL"],
         "text": str,
     },
 )
@@ -170,14 +164,25 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
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
 MetricsConfigurationTypeDef = TypedDict(
     "MetricsConfigurationTypeDef",
     {
         "cloudMetricEnabled": bool,
         "metricRuleRoleArn": str,
     },
     total=False,
@@ -214,38 +219,21 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
     },
     total=False,
 )
 
-DefinitionDocumentOutputTypeDef = TypedDict(
-    "DefinitionDocumentOutputTypeDef",
-    {
-        "language": Literal["GRAPHQL"],
-        "text": str,
-    },
-)
-
 DeleteFlowTemplateRequestRequestTypeDef = TypedDict(
     "DeleteFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSystemInstanceRequestRequestTypeDef = TypedDict(
     "DeleteSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
     total=False,
 )
@@ -292,26 +280,14 @@
     "DescribeNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
     total=False,
 )
 
-DescribeNamespaceResponseTypeDef = TypedDict(
-    "DescribeNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "trackingNamespaceName": str,
-        "trackingNamespaceVersion": int,
-        "namespaceVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DissociateEntityFromThingRequestRequestTypeDef = TypedDict(
     "DissociateEntityFromThingRequestRequestTypeDef",
     {
         "thingName": str,
         "entityType": EntityTypeType,
     },
 )
@@ -367,64 +343,48 @@
     "_OptionalGetEntitiesRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class GetEntitiesRequestRequestTypeDef(
     _RequiredGetEntitiesRequestRequestTypeDef, _OptionalGetEntitiesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetFlowTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
-
 class GetFlowTemplateRequestRequestTypeDef(
     _RequiredGetFlowTemplateRequestRequestTypeDef, _OptionalGetFlowTemplateRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
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
-class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
-    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -432,34 +392,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetFlowTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
-GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
-    "GetNamespaceDeletionStatusResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "status": NamespaceDeletionStatusType,
-        "errorCode": Literal["VALIDATION_FAILED"],
-        "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSystemInstanceRequestRequestTypeDef = TypedDict(
     "GetSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
@@ -473,43 +419,19 @@
     "_OptionalGetSystemTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
-
 class GetSystemTemplateRequestRequestTypeDef(
     _RequiredGetSystemTemplateRequestRequestTypeDef, _OptionalGetSystemTemplateRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
-    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -517,65 +439,27 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetSystemTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
-
 GetUploadStatusRequestRequestTypeDef = TypedDict(
     "GetUploadStatusRequestRequestTypeDef",
     {
         "uploadId": str,
     },
 )
 
-GetUploadStatusResponseTypeDef = TypedDict(
-    "GetUploadStatusResponseTypeDef",
-    {
-        "uploadId": str,
-        "uploadStatus": UploadStatusType,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "namespaceVersion": int,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-    },
-)
-_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
-    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListFlowExecutionMessagesRequestRequestTypeDef",
     {
         "flowExecutionId": str,
     },
 )
 _OptionalListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
@@ -583,44 +467,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListFlowExecutionMessagesRequestRequestTypeDef(
     _RequiredListFlowExecutionMessagesRequestRequestTypeDef,
     _OptionalListFlowExecutionMessagesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -628,60 +488,20 @@
     {
         "maxResults": int,
         "nextToken": str,
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
-        "key": str,
-        "value": str,
-    },
-)
-
-MetricsConfigurationOutputTypeDef = TypedDict(
-    "MetricsConfigurationOutputTypeDef",
-    {
-        "cloudMetricEnabled": bool,
-        "metricRuleRoleArn": str,
-    },
-    total=False,
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
 _RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
     {
         "systemInstanceId": str,
     },
 )
 _OptionalSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
@@ -692,47 +512,20 @@
         "endTime": Union[datetime, str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class SearchFlowExecutionsRequestRequestTypeDef(
     _RequiredSearchFlowExecutionsRequestRequestTypeDef,
     _OptionalSearchFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
-    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-):
-    pass
-
-
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
     total=False,
@@ -758,44 +551,19 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class SearchThingsRequestRequestTypeDef(
     _RequiredSearchThingsRequestRequestTypeDef, _OptionalSearchThingsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "entityId": str,
-    },
-)
-_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "namespaceVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchThingsRequestSearchThingsPaginateTypeDef(
-    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
-    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
-):
-    pass
-
-
 ThingTypeDef = TypedDict(
     "ThingTypeDef",
     {
         "thingArn": str,
         "thingName": str,
     },
     total=False,
@@ -813,65 +581,65 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UploadEntityDefinitionsResponseTypeDef = TypedDict(
-    "UploadEntityDefinitionsResponseTypeDef",
-    {
-        "uploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class CreateFlowTemplateRequestRequestTypeDef(
     _RequiredCreateFlowTemplateRequestRequestTypeDef,
     _OptionalCreateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class CreateSystemTemplateRequestRequestTypeDef(
     _RequiredCreateSystemTemplateRequestRequestTypeDef,
     _OptionalCreateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
+EntityDescriptionTypeDef = TypedDict(
+    "EntityDescriptionTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "type": EntityTypeType,
+        "createdAt": datetime,
+        "definition": DefinitionDocumentTypeDef,
+    },
+    total=False,
+)
 
 _RequiredUpdateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
@@ -880,22 +648,20 @@
     "_OptionalUpdateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class UpdateFlowTemplateRequestRequestTypeDef(
     _RequiredUpdateFlowTemplateRequestRequestTypeDef,
     _OptionalUpdateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSystemTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
 )
@@ -903,63 +669,126 @@
     "_OptionalUpdateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
-
 class UpdateSystemTemplateRequestRequestTypeDef(
     _RequiredUpdateSystemTemplateRequestRequestTypeDef,
     _OptionalUpdateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 UploadEntityDefinitionsRequestRequestTypeDef = TypedDict(
     "UploadEntityDefinitionsRequestRequestTypeDef",
     {
         "document": DefinitionDocumentTypeDef,
         "syncWithPublicNamespace": bool,
         "deprecateExistingEntities": bool,
     },
     total=False,
 )
 
+FlowTemplateDescriptionTypeDef = TypedDict(
+    "FlowTemplateDescriptionTypeDef",
+    {
+        "summary": FlowTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "validatedNamespaceVersion": int,
+    },
+    total=False,
+)
+
 CreateFlowTemplateResponseTypeDef = TypedDict(
     "CreateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNamespaceResponseTypeDef = TypedDict(
+    "DescribeNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "trackingNamespaceName": str,
+        "trackingNamespaceVersion": int,
+        "namespaceVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFlowTemplateRevisionsResponseTypeDef = TypedDict(
     "GetFlowTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "status": NamespaceDeletionStatusType,
+        "errorCode": Literal["VALIDATION_FAILED"],
+        "errorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUploadStatusResponseTypeDef = TypedDict(
+    "GetUploadStatusResponseTypeDef",
+    {
+        "uploadId": str,
+        "uploadStatus": UploadStatusType,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "namespaceVersion": int,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFlowTemplatesResponseTypeDef = TypedDict(
     "SearchFlowTemplatesResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowTemplateResponseTypeDef = TypedDict(
     "UpdateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadEntityDefinitionsResponseTypeDef = TypedDict(
+    "UploadEntityDefinitionsResponseTypeDef",
+    {
+        "uploadId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSystemInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemInstanceRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
@@ -974,126 +803,125 @@
         "s3BucketName": str,
         "metricsConfiguration": MetricsConfigurationTypeDef,
         "flowActionsRoleArn": str,
     },
     total=False,
 )
 
-
 class CreateSystemInstanceRequestRequestTypeDef(
     _RequiredCreateSystemInstanceRequestRequestTypeDef,
     _OptionalCreateSystemInstanceRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
 CreateSystemInstanceResponseTypeDef = TypedDict(
     "CreateSystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploySystemInstanceResponseTypeDef = TypedDict(
     "DeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
         "greengrassDeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSystemInstancesResponseTypeDef = TypedDict(
     "SearchSystemInstancesResponseTypeDef",
     {
         "summaries": List[SystemInstanceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UndeploySystemInstanceResponseTypeDef = TypedDict(
     "UndeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSystemTemplateResponseTypeDef = TypedDict(
     "CreateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemTemplateRevisionsResponseTypeDef = TypedDict(
     "GetSystemTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSystemTemplatesResponseTypeDef = TypedDict(
     "SearchSystemTemplatesResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSystemTemplateResponseTypeDef = TypedDict(
-    "UpdateSystemTemplateResponseTypeDef",
+SystemTemplateDescriptionTypeDef = TypedDict(
+    "SystemTemplateDescriptionTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EntityDescriptionTypeDef = TypedDict(
-    "EntityDescriptionTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "type": EntityTypeType,
-        "createdAt": datetime,
-        "definition": DefinitionDocumentOutputTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "validatedNamespaceVersion": int,
     },
     total=False,
 )
 
-FlowTemplateDescriptionTypeDef = TypedDict(
-    "FlowTemplateDescriptionTypeDef",
+UpdateSystemTemplateResponseTypeDef = TypedDict(
+    "UpdateSystemTemplateResponseTypeDef",
     {
-        "summary": FlowTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentOutputTypeDef,
-        "validatedNamespaceVersion": int,
+        "summary": SystemTemplateSummaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-SystemTemplateDescriptionTypeDef = TypedDict(
-    "SystemTemplateDescriptionTypeDef",
+SystemInstanceDescriptionTypeDef = TypedDict(
+    "SystemInstanceDescriptionTypeDef",
     {
-        "summary": SystemTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentOutputTypeDef,
+        "summary": SystemInstanceSummaryTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "s3BucketName": str,
+        "metricsConfiguration": MetricsConfigurationTypeDef,
         "validatedNamespaceVersion": int,
+        "validatedDependencyRevisions": List[DependencyRevisionTypeDef],
+        "flowActionsRoleArn": str,
     },
     total=False,
 )
 
 _RequiredSearchEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestRequestTypeDef",
     {
@@ -1107,120 +935,217 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
-
 class SearchEntitiesRequestRequestTypeDef(
     _RequiredSearchEntitiesRequestRequestTypeDef, _OptionalSearchEntitiesRequestRequestTypeDef
 ):
     pass
 
+ListFlowExecutionMessagesResponseTypeDef = TypedDict(
+    "ListFlowExecutionMessagesResponseTypeDef",
+    {
+        "messages": List[FlowExecutionMessageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchFlowExecutionsResponseTypeDef = TypedDict(
+    "SearchFlowExecutionsResponseTypeDef",
+    {
+        "summaries": List[FlowExecutionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestRequestTypeDef",
+    {
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
+    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
+    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+    },
+)
+_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
+    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
 
 _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "entityTypes": Sequence[EntityTypeType],
     },
 )
 _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "filters": Sequence[EntityFilterTypeDef],
         "namespaceVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
-
-ListFlowExecutionMessagesResponseTypeDef = TypedDict(
-    "ListFlowExecutionMessagesResponseTypeDef",
-    {
-        "messages": List[FlowExecutionMessageTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SearchFlowExecutionsResponseTypeDef = TypedDict(
-    "SearchFlowExecutionsResponseTypeDef",
+_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
-        "summaries": List[FlowExecutionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "systemInstanceId": str,
     },
 )
-
-SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestRequestTypeDef",
+_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "flowExecutionId": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
+    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+):
+    pass
+
 SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     {
         "filters": Sequence[FlowTemplateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entityId": str,
     },
 )
-
-SystemInstanceDescriptionTypeDef = TypedDict(
-    "SystemInstanceDescriptionTypeDef",
+_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
     {
-        "summary": SystemInstanceSummaryTypeDef,
-        "definition": DefinitionDocumentOutputTypeDef,
-        "s3BucketName": str,
-        "metricsConfiguration": MetricsConfigurationOutputTypeDef,
-        "validatedNamespaceVersion": int,
-        "validatedDependencyRevisions": List[DependencyRevisionTypeDef],
-        "flowActionsRoleArn": str,
+        "namespaceVersion": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class SearchThingsRequestSearchThingsPaginateTypeDef(
+    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
+    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
+):
+    pass
+
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef = TypedDict(
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 SearchSystemTemplatesRequestRequestTypeDef = TypedDict(
     "SearchSystemTemplatesRequestRequestTypeDef",
     {
@@ -1231,61 +1156,61 @@
     total=False,
 )
 
 SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef = TypedDict(
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     {
         "filters": Sequence[SystemTemplateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 SearchThingsResponseTypeDef = TypedDict(
     "SearchThingsResponseTypeDef",
     {
         "things": List[ThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEntitiesResponseTypeDef = TypedDict(
     "GetEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchEntitiesResponseTypeDef = TypedDict(
     "SearchEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFlowTemplateResponseTypeDef = TypedDict(
     "GetFlowTemplateResponseTypeDef",
     {
         "description": FlowTemplateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemTemplateResponseTypeDef = TypedDict(
     "GetSystemTemplateResponseTypeDef",
     {
         "description": SystemTemplateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemInstanceResponseTypeDef = TypedDict(
     "GetSystemInstanceResponseTypeDef",
     {
         "description": SystemInstanceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph/type_defs.pyi` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,97 +32,95 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateEntityToThingRequestRequestTypeDef",
     "DefinitionDocumentTypeDef",
     "FlowTemplateSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricsConfigurationTypeDef",
     "TagTypeDef",
     "SystemInstanceSummaryTypeDef",
     "SystemTemplateSummaryTypeDef",
-    "DefinitionDocumentOutputTypeDef",
     "DeleteFlowTemplateRequestRequestTypeDef",
-    "DeleteNamespaceResponseTypeDef",
     "DeleteSystemInstanceRequestRequestTypeDef",
     "DeleteSystemTemplateRequestRequestTypeDef",
     "DependencyRevisionTypeDef",
     "DeploySystemInstanceRequestRequestTypeDef",
     "DeprecateFlowTemplateRequestRequestTypeDef",
     "DeprecateSystemTemplateRequestRequestTypeDef",
     "DescribeNamespaceRequestRequestTypeDef",
-    "DescribeNamespaceResponseTypeDef",
     "DissociateEntityFromThingRequestRequestTypeDef",
     "EntityFilterTypeDef",
     "FlowExecutionMessageTypeDef",
     "FlowExecutionSummaryTypeDef",
     "FlowTemplateFilterTypeDef",
     "GetEntitiesRequestRequestTypeDef",
     "GetFlowTemplateRequestRequestTypeDef",
-    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetFlowTemplateRevisionsRequestRequestTypeDef",
-    "GetNamespaceDeletionStatusResponseTypeDef",
     "GetSystemInstanceRequestRequestTypeDef",
     "GetSystemTemplateRequestRequestTypeDef",
-    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
     "GetSystemTemplateRevisionsRequestRequestTypeDef",
     "GetUploadStatusRequestRequestTypeDef",
-    "GetUploadStatusResponseTypeDef",
-    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
     "ListFlowExecutionMessagesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "MetricsConfigurationOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchFlowExecutionsRequestRequestTypeDef",
-    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SystemInstanceFilterTypeDef",
     "SystemTemplateFilterTypeDef",
     "SearchThingsRequestRequestTypeDef",
-    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "ThingTypeDef",
     "UndeploySystemInstanceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UploadEntityDefinitionsResponseTypeDef",
     "CreateFlowTemplateRequestRequestTypeDef",
     "CreateSystemTemplateRequestRequestTypeDef",
+    "EntityDescriptionTypeDef",
     "UpdateFlowTemplateRequestRequestTypeDef",
     "UpdateSystemTemplateRequestRequestTypeDef",
     "UploadEntityDefinitionsRequestRequestTypeDef",
+    "FlowTemplateDescriptionTypeDef",
     "CreateFlowTemplateResponseTypeDef",
+    "DeleteNamespaceResponseTypeDef",
+    "DescribeNamespaceResponseTypeDef",
     "GetFlowTemplateRevisionsResponseTypeDef",
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    "GetUploadStatusResponseTypeDef",
     "SearchFlowTemplatesResponseTypeDef",
     "UpdateFlowTemplateResponseTypeDef",
+    "UploadEntityDefinitionsResponseTypeDef",
     "CreateSystemInstanceRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSystemInstanceResponseTypeDef",
     "DeploySystemInstanceResponseTypeDef",
     "SearchSystemInstancesResponseTypeDef",
     "UndeploySystemInstanceResponseTypeDef",
     "CreateSystemTemplateResponseTypeDef",
     "GetSystemTemplateRevisionsResponseTypeDef",
     "SearchSystemTemplatesResponseTypeDef",
-    "UpdateSystemTemplateResponseTypeDef",
-    "EntityDescriptionTypeDef",
-    "FlowTemplateDescriptionTypeDef",
     "SystemTemplateDescriptionTypeDef",
+    "UpdateSystemTemplateResponseTypeDef",
+    "SystemInstanceDescriptionTypeDef",
     "SearchEntitiesRequestRequestTypeDef",
-    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     "ListFlowExecutionMessagesResponseTypeDef",
     "SearchFlowExecutionsResponseTypeDef",
     "SearchFlowTemplatesRequestRequestTypeDef",
+    "GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    "GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    "ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "SearchEntitiesRequestSearchEntitiesPaginateTypeDef",
+    "SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "SystemInstanceDescriptionTypeDef",
+    "SearchThingsRequestSearchThingsPaginateTypeDef",
     "SearchSystemInstancesRequestRequestTypeDef",
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     "SearchSystemTemplatesRequestRequestTypeDef",
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     "SearchThingsResponseTypeDef",
     "GetEntitiesResponseTypeDef",
     "SearchEntitiesResponseTypeDef",
@@ -142,20 +140,22 @@
     "_OptionalAssociateEntityToThingRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class AssociateEntityToThingRequestRequestTypeDef(
     _RequiredAssociateEntityToThingRequestRequestTypeDef,
     _OptionalAssociateEntityToThingRequestRequestTypeDef,
 ):
     pass
 
+
 DefinitionDocumentTypeDef = TypedDict(
     "DefinitionDocumentTypeDef",
     {
         "language": Literal["GRAPHQL"],
         "text": str,
     },
 )
@@ -167,14 +167,25 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
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
 MetricsConfigurationTypeDef = TypedDict(
     "MetricsConfigurationTypeDef",
     {
         "cloudMetricEnabled": bool,
         "metricRuleRoleArn": str,
     },
     total=False,
@@ -211,38 +222,21 @@
         "arn": str,
         "revisionNumber": int,
         "createdAt": datetime,
     },
     total=False,
 )
 
-DefinitionDocumentOutputTypeDef = TypedDict(
-    "DefinitionDocumentOutputTypeDef",
-    {
-        "language": Literal["GRAPHQL"],
-        "text": str,
-    },
-)
-
 DeleteFlowTemplateRequestRequestTypeDef = TypedDict(
     "DeleteFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-DeleteNamespaceResponseTypeDef = TypedDict(
-    "DeleteNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSystemInstanceRequestRequestTypeDef = TypedDict(
     "DeleteSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
     total=False,
 )
@@ -289,26 +283,14 @@
     "DescribeNamespaceRequestRequestTypeDef",
     {
         "namespaceName": str,
     },
     total=False,
 )
 
-DescribeNamespaceResponseTypeDef = TypedDict(
-    "DescribeNamespaceResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "trackingNamespaceName": str,
-        "trackingNamespaceVersion": int,
-        "namespaceVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DissociateEntityFromThingRequestRequestTypeDef = TypedDict(
     "DissociateEntityFromThingRequestRequestTypeDef",
     {
         "thingName": str,
         "entityType": EntityTypeType,
     },
 )
@@ -364,58 +346,52 @@
     "_OptionalGetEntitiesRequestRequestTypeDef",
     {
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class GetEntitiesRequestRequestTypeDef(
     _RequiredGetEntitiesRequestRequestTypeDef, _OptionalGetEntitiesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalGetFlowTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
+
 class GetFlowTemplateRequestRequestTypeDef(
     _RequiredGetFlowTemplateRequestRequestTypeDef, _OptionalGetFlowTemplateRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+
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
 
-class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
-    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFlowTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef = TypedDict(
@@ -423,31 +399,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetFlowTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetFlowTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetFlowTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
-GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
-    "GetNamespaceDeletionStatusResponseTypeDef",
-    {
-        "namespaceArn": str,
-        "namespaceName": str,
-        "status": NamespaceDeletionStatusType,
-        "errorCode": Literal["VALIDATION_FAILED"],
-        "errorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetSystemInstanceRequestRequestTypeDef = TypedDict(
     "GetSystemInstanceRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -462,38 +428,20 @@
     "_OptionalGetSystemTemplateRequestRequestTypeDef",
     {
         "revisionNumber": int,
     },
     total=False,
 )
 
+
 class GetSystemTemplateRequestRequestTypeDef(
     _RequiredGetSystemTemplateRequestRequestTypeDef, _OptionalGetSystemTemplateRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
-    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
-    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSystemTemplateRevisionsRequestRequestTypeDef",
     {
         "id": str,
     },
 )
@@ -502,61 +450,29 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetSystemTemplateRevisionsRequestRequestTypeDef(
     _RequiredGetSystemTemplateRevisionsRequestRequestTypeDef,
     _OptionalGetSystemTemplateRevisionsRequestRequestTypeDef,
 ):
     pass
 
+
 GetUploadStatusRequestRequestTypeDef = TypedDict(
     "GetUploadStatusRequestRequestTypeDef",
     {
         "uploadId": str,
     },
 )
 
-GetUploadStatusResponseTypeDef = TypedDict(
-    "GetUploadStatusResponseTypeDef",
-    {
-        "uploadId": str,
-        "uploadStatus": UploadStatusType,
-        "namespaceArn": str,
-        "namespaceName": str,
-        "namespaceVersion": int,
-        "failureReason": List[str],
-        "createdDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-    },
-)
-_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
-    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
-    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
-):
-    pass
-
 _RequiredListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
     "_RequiredListFlowExecutionMessagesRequestRequestTypeDef",
     {
         "flowExecutionId": str,
     },
 )
 _OptionalListFlowExecutionMessagesRequestRequestTypeDef = TypedDict(
@@ -564,39 +480,21 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListFlowExecutionMessagesRequestRequestTypeDef(
     _RequiredListFlowExecutionMessagesRequestRequestTypeDef,
     _OptionalListFlowExecutionMessagesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
 
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
@@ -605,57 +503,21 @@
     {
         "maxResults": int,
         "nextToken": str,
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
-        "key": str,
-        "value": str,
-    },
-)
-
-MetricsConfigurationOutputTypeDef = TypedDict(
-    "MetricsConfigurationOutputTypeDef",
-    {
-        "cloudMetricEnabled": bool,
-        "metricRuleRoleArn": str,
-    },
-    total=False,
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
 
 _RequiredSearchFlowExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchFlowExecutionsRequestRequestTypeDef",
     {
         "systemInstanceId": str,
     },
 )
@@ -667,42 +529,21 @@
         "endTime": Union[datetime, str],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class SearchFlowExecutionsRequestRequestTypeDef(
     _RequiredSearchFlowExecutionsRequestRequestTypeDef,
     _OptionalSearchFlowExecutionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "systemInstanceId": str,
-    },
-)
-_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
-    {
-        "flowExecutionId": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
-    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
-):
-    pass
 
 SystemInstanceFilterTypeDef = TypedDict(
     "SystemInstanceFilterTypeDef",
     {
         "name": SystemInstanceFilterNameType,
         "value": Sequence[str],
     },
@@ -729,39 +570,20 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class SearchThingsRequestRequestTypeDef(
     _RequiredSearchThingsRequestRequestTypeDef, _OptionalSearchThingsRequestRequestTypeDef
 ):
     pass
 
-_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "entityId": str,
-    },
-)
-_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
-    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
-    {
-        "namespaceVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchThingsRequestSearchThingsPaginateTypeDef(
-    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
-    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
-):
-    pass
 
 ThingTypeDef = TypedDict(
     "ThingTypeDef",
     {
         "thingArn": str,
         "thingName": str,
     },
@@ -780,62 +602,70 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UploadEntityDefinitionsResponseTypeDef = TypedDict(
-    "UploadEntityDefinitionsResponseTypeDef",
-    {
-        "uploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFlowTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class CreateFlowTemplateRequestRequestTypeDef(
     _RequiredCreateFlowTemplateRequestRequestTypeDef,
     _OptionalCreateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemTemplateRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
     },
 )
 _OptionalCreateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class CreateSystemTemplateRequestRequestTypeDef(
     _RequiredCreateSystemTemplateRequestRequestTypeDef,
     _OptionalCreateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
+
+EntityDescriptionTypeDef = TypedDict(
+    "EntityDescriptionTypeDef",
+    {
+        "id": str,
+        "arn": str,
+        "type": EntityTypeType,
+        "createdAt": datetime,
+        "definition": DefinitionDocumentTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateFlowTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFlowTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
 )
@@ -843,20 +673,22 @@
     "_OptionalUpdateFlowTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class UpdateFlowTemplateRequestRequestTypeDef(
     _RequiredUpdateFlowTemplateRequestRequestTypeDef,
     _OptionalUpdateFlowTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateSystemTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSystemTemplateRequestRequestTypeDef",
     {
         "id": str,
         "definition": DefinitionDocumentTypeDef,
     },
 )
@@ -864,61 +696,128 @@
     "_OptionalUpdateSystemTemplateRequestRequestTypeDef",
     {
         "compatibleNamespaceVersion": int,
     },
     total=False,
 )
 
+
 class UpdateSystemTemplateRequestRequestTypeDef(
     _RequiredUpdateSystemTemplateRequestRequestTypeDef,
     _OptionalUpdateSystemTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 UploadEntityDefinitionsRequestRequestTypeDef = TypedDict(
     "UploadEntityDefinitionsRequestRequestTypeDef",
     {
         "document": DefinitionDocumentTypeDef,
         "syncWithPublicNamespace": bool,
         "deprecateExistingEntities": bool,
     },
     total=False,
 )
 
+FlowTemplateDescriptionTypeDef = TypedDict(
+    "FlowTemplateDescriptionTypeDef",
+    {
+        "summary": FlowTemplateSummaryTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "validatedNamespaceVersion": int,
+    },
+    total=False,
+)
+
 CreateFlowTemplateResponseTypeDef = TypedDict(
     "CreateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteNamespaceResponseTypeDef = TypedDict(
+    "DeleteNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNamespaceResponseTypeDef = TypedDict(
+    "DescribeNamespaceResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "trackingNamespaceName": str,
+        "trackingNamespaceVersion": int,
+        "namespaceVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFlowTemplateRevisionsResponseTypeDef = TypedDict(
     "GetFlowTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNamespaceDeletionStatusResponseTypeDef = TypedDict(
+    "GetNamespaceDeletionStatusResponseTypeDef",
+    {
+        "namespaceArn": str,
+        "namespaceName": str,
+        "status": NamespaceDeletionStatusType,
+        "errorCode": Literal["VALIDATION_FAILED"],
+        "errorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUploadStatusResponseTypeDef = TypedDict(
+    "GetUploadStatusResponseTypeDef",
+    {
+        "uploadId": str,
+        "uploadStatus": UploadStatusType,
+        "namespaceArn": str,
+        "namespaceName": str,
+        "namespaceVersion": int,
+        "failureReason": List[str],
+        "createdDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchFlowTemplatesResponseTypeDef = TypedDict(
     "SearchFlowTemplatesResponseTypeDef",
     {
         "summaries": List[FlowTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFlowTemplateResponseTypeDef = TypedDict(
     "UpdateFlowTemplateResponseTypeDef",
     {
         "summary": FlowTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UploadEntityDefinitionsResponseTypeDef = TypedDict(
+    "UploadEntityDefinitionsResponseTypeDef",
+    {
+        "uploadId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateSystemInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSystemInstanceRequestRequestTypeDef",
     {
         "definition": DefinitionDocumentTypeDef,
@@ -933,124 +832,127 @@
         "s3BucketName": str,
         "metricsConfiguration": MetricsConfigurationTypeDef,
         "flowActionsRoleArn": str,
     },
     total=False,
 )
 
+
 class CreateSystemInstanceRequestRequestTypeDef(
     _RequiredCreateSystemInstanceRequestRequestTypeDef,
     _OptionalCreateSystemInstanceRequestRequestTypeDef,
 ):
     pass
 
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
 CreateSystemInstanceResponseTypeDef = TypedDict(
     "CreateSystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeploySystemInstanceResponseTypeDef = TypedDict(
     "DeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
         "greengrassDeploymentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSystemInstancesResponseTypeDef = TypedDict(
     "SearchSystemInstancesResponseTypeDef",
     {
         "summaries": List[SystemInstanceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UndeploySystemInstanceResponseTypeDef = TypedDict(
     "UndeploySystemInstanceResponseTypeDef",
     {
         "summary": SystemInstanceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSystemTemplateResponseTypeDef = TypedDict(
     "CreateSystemTemplateResponseTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemTemplateRevisionsResponseTypeDef = TypedDict(
     "GetSystemTemplateRevisionsResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSystemTemplatesResponseTypeDef = TypedDict(
     "SearchSystemTemplatesResponseTypeDef",
     {
         "summaries": List[SystemTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateSystemTemplateResponseTypeDef = TypedDict(
-    "UpdateSystemTemplateResponseTypeDef",
+SystemTemplateDescriptionTypeDef = TypedDict(
+    "SystemTemplateDescriptionTypeDef",
     {
         "summary": SystemTemplateSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EntityDescriptionTypeDef = TypedDict(
-    "EntityDescriptionTypeDef",
-    {
-        "id": str,
-        "arn": str,
-        "type": EntityTypeType,
-        "createdAt": datetime,
-        "definition": DefinitionDocumentOutputTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "validatedNamespaceVersion": int,
     },
     total=False,
 )
 
-FlowTemplateDescriptionTypeDef = TypedDict(
-    "FlowTemplateDescriptionTypeDef",
+UpdateSystemTemplateResponseTypeDef = TypedDict(
+    "UpdateSystemTemplateResponseTypeDef",
     {
-        "summary": FlowTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentOutputTypeDef,
-        "validatedNamespaceVersion": int,
+        "summary": SystemTemplateSummaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-SystemTemplateDescriptionTypeDef = TypedDict(
-    "SystemTemplateDescriptionTypeDef",
+SystemInstanceDescriptionTypeDef = TypedDict(
+    "SystemInstanceDescriptionTypeDef",
     {
-        "summary": SystemTemplateSummaryTypeDef,
-        "definition": DefinitionDocumentOutputTypeDef,
+        "summary": SystemInstanceSummaryTypeDef,
+        "definition": DefinitionDocumentTypeDef,
+        "s3BucketName": str,
+        "metricsConfiguration": MetricsConfigurationTypeDef,
         "validatedNamespaceVersion": int,
+        "validatedDependencyRevisions": List[DependencyRevisionTypeDef],
+        "flowActionsRoleArn": str,
     },
     total=False,
 )
 
 _RequiredSearchEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestRequestTypeDef",
     {
@@ -1064,116 +966,233 @@
         "nextToken": str,
         "maxResults": int,
         "namespaceVersion": int,
     },
     total=False,
 )
 
+
 class SearchEntitiesRequestRequestTypeDef(
     _RequiredSearchEntitiesRequestRequestTypeDef, _OptionalSearchEntitiesRequestRequestTypeDef
 ):
     pass
 
+
+ListFlowExecutionMessagesResponseTypeDef = TypedDict(
+    "ListFlowExecutionMessagesResponseTypeDef",
+    {
+        "messages": List[FlowExecutionMessageTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchFlowExecutionsResponseTypeDef = TypedDict(
+    "SearchFlowExecutionsResponseTypeDef",
+    {
+        "summaries": List[FlowExecutionSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
+    "SearchFlowTemplatesRequestRequestTypeDef",
+    {
+        "filters": Sequence[FlowTemplateFilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef(
+    _RequiredGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    _OptionalGetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef = TypedDict(
+    "_OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef(
+    _RequiredGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    _OptionalGetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "flowExecutionId": str,
+    },
+)
+_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef = TypedDict(
+    "_OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef(
+    _RequiredListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    _OptionalListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "entityTypes": Sequence[EntityTypeType],
     },
 )
 _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef",
     {
         "filters": Sequence[EntityFilterTypeDef],
         "namespaceVersion": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class SearchEntitiesRequestSearchEntitiesPaginateTypeDef(
     _RequiredSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     _OptionalSearchEntitiesRequestSearchEntitiesPaginateTypeDef,
 ):
     pass
 
-ListFlowExecutionMessagesResponseTypeDef = TypedDict(
-    "ListFlowExecutionMessagesResponseTypeDef",
-    {
-        "messages": List[FlowExecutionMessageTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-SearchFlowExecutionsResponseTypeDef = TypedDict(
-    "SearchFlowExecutionsResponseTypeDef",
+_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
-        "summaries": List[FlowExecutionSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "systemInstanceId": str,
     },
 )
-
-SearchFlowTemplatesRequestRequestTypeDef = TypedDict(
-    "SearchFlowTemplatesRequestRequestTypeDef",
+_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef",
     {
-        "filters": Sequence[FlowTemplateFilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "flowExecutionId": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef(
+    _RequiredSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+    _OptionalSearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
+):
+    pass
+
+
 SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef = TypedDict(
     "SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef",
     {
         "filters": Sequence[FlowTemplateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_RequiredSearchThingsRequestSearchThingsPaginateTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "entityId": str,
     },
 )
-
-SystemInstanceDescriptionTypeDef = TypedDict(
-    "SystemInstanceDescriptionTypeDef",
+_OptionalSearchThingsRequestSearchThingsPaginateTypeDef = TypedDict(
+    "_OptionalSearchThingsRequestSearchThingsPaginateTypeDef",
     {
-        "summary": SystemInstanceSummaryTypeDef,
-        "definition": DefinitionDocumentOutputTypeDef,
-        "s3BucketName": str,
-        "metricsConfiguration": MetricsConfigurationOutputTypeDef,
-        "validatedNamespaceVersion": int,
-        "validatedDependencyRevisions": List[DependencyRevisionTypeDef],
-        "flowActionsRoleArn": str,
+        "namespaceVersion": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
+class SearchThingsRequestSearchThingsPaginateTypeDef(
+    _RequiredSearchThingsRequestSearchThingsPaginateTypeDef,
+    _OptionalSearchThingsRequestSearchThingsPaginateTypeDef,
+):
+    pass
+
+
 SearchSystemInstancesRequestRequestTypeDef = TypedDict(
     "SearchSystemInstancesRequestRequestTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
 SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef = TypedDict(
     "SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef",
     {
         "filters": Sequence[SystemInstanceFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 SearchSystemTemplatesRequestRequestTypeDef = TypedDict(
     "SearchSystemTemplatesRequestRequestTypeDef",
     {
@@ -1184,61 +1203,61 @@
     total=False,
 )
 
 SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef = TypedDict(
     "SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef",
     {
         "filters": Sequence[SystemTemplateFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 SearchThingsResponseTypeDef = TypedDict(
     "SearchThingsResponseTypeDef",
     {
         "things": List[ThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEntitiesResponseTypeDef = TypedDict(
     "GetEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchEntitiesResponseTypeDef = TypedDict(
     "SearchEntitiesResponseTypeDef",
     {
         "descriptions": List[EntityDescriptionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFlowTemplateResponseTypeDef = TypedDict(
     "GetFlowTemplateResponseTypeDef",
     {
         "description": FlowTemplateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemTemplateResponseTypeDef = TypedDict(
     "GetSystemTemplateResponseTypeDef",
     {
         "description": SystemTemplateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSystemInstanceResponseTypeDef = TypedDict(
     "GetSystemInstanceResponseTypeDef",
     {
         "description": SystemInstanceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotthingsgraph
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTThingsGraph 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTThingsGraph 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotthingsgraph.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotthingsgraph)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotthingsgraph)](https://pepy.tech/project/mypy-boto3-iotthingsgraph)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTThingsGraph 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
+[boto3.IoTThingsGraph 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotthingsgraph.html#IoTThingsGraph)
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
 [mypy-boto3-iotthingsgraph docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotthingsgraph/).
 
 See how it helps to find and fix potential bugs:
 
@@ -381,93 +381,90 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotthingsgraph.type_defs import (
     AssociateEntityToThingRequestRequestTypeDef,
     DefinitionDocumentTypeDef,
     FlowTemplateSummaryTypeDef,
+    ResponseMetadataTypeDef,
     MetricsConfigurationTypeDef,
     TagTypeDef,
     SystemInstanceSummaryTypeDef,
     SystemTemplateSummaryTypeDef,
-    DefinitionDocumentOutputTypeDef,
     DeleteFlowTemplateRequestRequestTypeDef,
-    DeleteNamespaceResponseTypeDef,
     DeleteSystemInstanceRequestRequestTypeDef,
     DeleteSystemTemplateRequestRequestTypeDef,
     DependencyRevisionTypeDef,
     DeploySystemInstanceRequestRequestTypeDef,
     DeprecateFlowTemplateRequestRequestTypeDef,
     DeprecateSystemTemplateRequestRequestTypeDef,
     DescribeNamespaceRequestRequestTypeDef,
-    DescribeNamespaceResponseTypeDef,
     DissociateEntityFromThingRequestRequestTypeDef,
     EntityFilterTypeDef,
     FlowExecutionMessageTypeDef,
     FlowExecutionSummaryTypeDef,
     FlowTemplateFilterTypeDef,
     GetEntitiesRequestRequestTypeDef,
     GetFlowTemplateRequestRequestTypeDef,
-    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetFlowTemplateRevisionsRequestRequestTypeDef,
-    GetNamespaceDeletionStatusResponseTypeDef,
     GetSystemInstanceRequestRequestTypeDef,
     GetSystemTemplateRequestRequestTypeDef,
-    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
     GetSystemTemplateRevisionsRequestRequestTypeDef,
     GetUploadStatusRequestRequestTypeDef,
-    GetUploadStatusResponseTypeDef,
-    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
     ListFlowExecutionMessagesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    MetricsConfigurationOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SearchFlowExecutionsRequestRequestTypeDef,
-    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SystemInstanceFilterTypeDef,
     SystemTemplateFilterTypeDef,
     SearchThingsRequestRequestTypeDef,
-    SearchThingsRequestSearchThingsPaginateTypeDef,
     ThingTypeDef,
     UndeploySystemInstanceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UploadEntityDefinitionsResponseTypeDef,
     CreateFlowTemplateRequestRequestTypeDef,
     CreateSystemTemplateRequestRequestTypeDef,
+    EntityDescriptionTypeDef,
     UpdateFlowTemplateRequestRequestTypeDef,
     UpdateSystemTemplateRequestRequestTypeDef,
     UploadEntityDefinitionsRequestRequestTypeDef,
+    FlowTemplateDescriptionTypeDef,
     CreateFlowTemplateResponseTypeDef,
+    DeleteNamespaceResponseTypeDef,
+    DescribeNamespaceResponseTypeDef,
     GetFlowTemplateRevisionsResponseTypeDef,
+    GetNamespaceDeletionStatusResponseTypeDef,
+    GetUploadStatusResponseTypeDef,
     SearchFlowTemplatesResponseTypeDef,
     UpdateFlowTemplateResponseTypeDef,
+    UploadEntityDefinitionsResponseTypeDef,
     CreateSystemInstanceRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSystemInstanceResponseTypeDef,
     DeploySystemInstanceResponseTypeDef,
     SearchSystemInstancesResponseTypeDef,
     UndeploySystemInstanceResponseTypeDef,
     CreateSystemTemplateResponseTypeDef,
     GetSystemTemplateRevisionsResponseTypeDef,
     SearchSystemTemplatesResponseTypeDef,
-    UpdateSystemTemplateResponseTypeDef,
-    EntityDescriptionTypeDef,
-    FlowTemplateDescriptionTypeDef,
     SystemTemplateDescriptionTypeDef,
+    UpdateSystemTemplateResponseTypeDef,
+    SystemInstanceDescriptionTypeDef,
     SearchEntitiesRequestRequestTypeDef,
-    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
     ListFlowExecutionMessagesResponseTypeDef,
     SearchFlowExecutionsResponseTypeDef,
     SearchFlowTemplatesRequestRequestTypeDef,
+    GetFlowTemplateRevisionsRequestGetFlowTemplateRevisionsPaginateTypeDef,
+    GetSystemTemplateRevisionsRequestGetSystemTemplateRevisionsPaginateTypeDef,
+    ListFlowExecutionMessagesRequestListFlowExecutionMessagesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SearchEntitiesRequestSearchEntitiesPaginateTypeDef,
+    SearchFlowExecutionsRequestSearchFlowExecutionsPaginateTypeDef,
     SearchFlowTemplatesRequestSearchFlowTemplatesPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SystemInstanceDescriptionTypeDef,
+    SearchThingsRequestSearchThingsPaginateTypeDef,
     SearchSystemInstancesRequestRequestTypeDef,
     SearchSystemInstancesRequestSearchSystemInstancesPaginateTypeDef,
     SearchSystemTemplatesRequestRequestTypeDef,
     SearchSystemTemplatesRequestSearchSystemTemplatesPaginateTypeDef,
     SearchThingsResponseTypeDef,
     GetEntitiesResponseTypeDef,
     SearchEntitiesResponseTypeDef,
```

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt` & `mypy-boto3-iotthingsgraph-1.28.15/mypy_boto3_iotthingsgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotthingsgraph-1.28.12/setup.py` & `mypy-boto3-iotthingsgraph-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotthingsgraph",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotthingsgraph"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTThingsGraph 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IoTThingsGraph 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

