# Comparing `tmp/mypy-boto3-appfabric-1.28.12.tar.gz` & `tmp/mypy-boto3-appfabric-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appfabric-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
+gzip compressed data, was "mypy-boto3-appfabric-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-appfabric-1.28.12.tar` & `mypy-boto3-appfabric-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.260584 mypy-boto3-appfabric-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-07-27 05:34:16.252584 mypy-boto3-appfabric-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15095 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.248584 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    27162 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    27127 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:18.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.252584 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:16.000000 mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.260584 mypy-boto3-appfabric-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:17:17.000000 mypy-boto3-appfabric-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.196654 mypy-boto3-appfabric-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-28 20:42:16.184653 mypy-boto3-appfabric-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.180653 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21298 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21261 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8941 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8939 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-07-28 20:19:16.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25020 2023-07-28 20:19:16.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.184653 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16267 2023-07-28 20:42:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:16.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:15.000000 mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.196654 mypy-boto3-appfabric-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:19:15.000000 mypy-boto3-appfabric-1.28.15/setup.py
```

### Comparing `mypy-boto3-appfabric-1.28.12/LICENSE` & `mypy-boto3-appfabric-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.12/PKG-INFO` & `mypy-boto3-appfabric-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appfabric
-Version: 1.28.12
-Summary: Type annotations for boto3.AppFabric 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppFabric 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appfabric)](https://pepy.tech/project/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [mypy-boto3-appfabric docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,92 +342,83 @@
 
 `mypy_boto3_appfabric.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appfabric.type_defs import (
     ApiKeyCredentialTypeDef,
-    TenantOutputTypeDef,
+    TenantTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
-    AuditLogProcessingConfigurationOutputTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    TenantTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
-    FirehoseStreamOutputTypeDef,
-    S3BucketOutputTypeDef,
     FirehoseStreamTypeDef,
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
     IngestionSummaryTypeDef,
-    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppAuthorizationsRequestRequestTypeDef,
-    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
-    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
-    ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
-    ListAppBundlesResponseTypeDef,
-    CreateAppBundleResponseTypeDef,
-    GetAppBundleResponseTypeDef,
-    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     ConnectAppAuthorizationRequestRequestTypeDef,
+    CreateAppBundleResponseTypeDef,
+    GetAppBundleResponseTypeDef,
+    ListAppBundlesResponseTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
+    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+    ListIngestionsRequestListIngestionsPaginateTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
     CreateAppAuthorizationRequestRequestTypeDef,
     UpdateAppAuthorizationRequestRequestTypeDef,
-    AuditLogDestinationConfigurationOutputTypeDef,
     AuditLogDestinationConfigurationTypeDef,
     BatchGetUserAccessTasksResponseTypeDef,
     StartUserAccessTasksResponseTypeDef,
-    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
-    IngestionDestinationTypeDef,
     CreateIngestionDestinationRequestRequestTypeDef,
+    IngestionDestinationTypeDef,
     UpdateIngestionDestinationRequestRequestTypeDef,
     CreateIngestionDestinationResponseTypeDef,
     GetIngestionDestinationResponseTypeDef,
     UpdateIngestionDestinationResponseTypeDef,
 )
```

### Comparing `mypy-boto3-appfabric-1.28.12/README.md` & `mypy-boto3-appfabric-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appfabric)](https://pepy.tech/project/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [mypy-boto3-appfabric docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/).
 
 See how it helps to find and fix potential bugs:
 
@@ -310,92 +310,83 @@
 
 `mypy_boto3_appfabric.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appfabric.type_defs import (
     ApiKeyCredentialTypeDef,
-    TenantOutputTypeDef,
+    TenantTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
-    AuditLogProcessingConfigurationOutputTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    TenantTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
-    FirehoseStreamOutputTypeDef,
-    S3BucketOutputTypeDef,
     FirehoseStreamTypeDef,
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
     IngestionSummaryTypeDef,
-    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppAuthorizationsRequestRequestTypeDef,
-    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
-    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
-    ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
-    ListAppBundlesResponseTypeDef,
-    CreateAppBundleResponseTypeDef,
-    GetAppBundleResponseTypeDef,
-    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     ConnectAppAuthorizationRequestRequestTypeDef,
+    CreateAppBundleResponseTypeDef,
+    GetAppBundleResponseTypeDef,
+    ListAppBundlesResponseTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
+    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+    ListIngestionsRequestListIngestionsPaginateTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
     CreateAppAuthorizationRequestRequestTypeDef,
     UpdateAppAuthorizationRequestRequestTypeDef,
-    AuditLogDestinationConfigurationOutputTypeDef,
     AuditLogDestinationConfigurationTypeDef,
     BatchGetUserAccessTasksResponseTypeDef,
     StartUserAccessTasksResponseTypeDef,
-    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
-    IngestionDestinationTypeDef,
     CreateIngestionDestinationRequestRequestTypeDef,
+    IngestionDestinationTypeDef,
     UpdateIngestionDestinationRequestRequestTypeDef,
     CreateIngestionDestinationResponseTypeDef,
     GetIngestionDestinationResponseTypeDef,
     UpdateIngestionDestinationResponseTypeDef,
 )
```

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__init__.py` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__init__.pyi` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/__main__.py` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppFabric 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.AppFabric 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric\nOther"
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

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/client.py` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/client.pyi` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/literals.py` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/literals.pyi` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/paginator.py` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,80 +40,74 @@
 __all__ = (
     "ListAppAuthorizationsPaginator",
     "ListAppBundlesPaginator",
     "ListIngestionDestinationsPaginator",
     "ListIngestionsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAppAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappauthorizationspaginator)
     """
 
     def paginate(
-        self, *, appBundleIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appBundleIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappauthorizationspaginator)
         """
 
-
 class ListAppBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappbundlespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppBundlesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappbundlespaginator)
         """
 
-
 class ListIngestionDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestionDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestiondestinationspaginator)
     """
 
     def paginate(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIngestionDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestionDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestiondestinationspaginator)
         """
 
-
 class ListIngestionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestionspaginator)
     """
 
     def paginate(
-        self, *, appBundleIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appBundleIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIngestionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestionspaginator)
         """
```

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/paginator.pyi` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,74 +40,80 @@
 __all__ = (
     "ListAppAuthorizationsPaginator",
     "ListAppBundlesPaginator",
     "ListIngestionDestinationsPaginator",
     "ListIngestionsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAppAuthorizationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppAuthorizations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappauthorizationspaginator)
     """
 
     def paginate(
-        self, *, appBundleIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appBundleIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppAuthorizations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappauthorizationspaginator)
         """
 
+
 class ListAppBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappbundlespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppBundlesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListAppBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listappbundlespaginator)
         """
 
+
 class ListIngestionDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestionDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestiondestinationspaginator)
     """
 
     def paginate(
         self,
         *,
         appBundleIdentifier: str,
         ingestionIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIngestionDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestionDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestiondestinationspaginator)
         """
 
+
 class ListIngestionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestionspaginator)
     """
 
     def paginate(
-        self, *, appBundleIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, appBundleIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIngestionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric.Paginator.ListIngestions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/paginators/#listingestionspaginator)
         """
```

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/type_defs.py` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,107 +34,98 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApiKeyCredentialTypeDef",
-    "TenantOutputTypeDef",
+    "TenantTypeDef",
     "AppBundleSummaryTypeDef",
     "AppBundleTypeDef",
-    "AuditLogProcessingConfigurationOutputTypeDef",
     "AuditLogProcessingConfigurationTypeDef",
     "AuthRequestTypeDef",
     "BatchGetUserAccessTasksRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "TenantTypeDef",
     "IngestionTypeDef",
     "Oauth2CredentialTypeDef",
     "DeleteAppAuthorizationRequestRequestTypeDef",
     "DeleteAppBundleRequestRequestTypeDef",
     "DeleteIngestionDestinationRequestRequestTypeDef",
     "DeleteIngestionRequestRequestTypeDef",
-    "FirehoseStreamOutputTypeDef",
-    "S3BucketOutputTypeDef",
     "FirehoseStreamTypeDef",
     "S3BucketTypeDef",
     "GetAppAuthorizationRequestRequestTypeDef",
     "GetAppBundleRequestRequestTypeDef",
     "GetIngestionDestinationRequestRequestTypeDef",
     "GetIngestionRequestRequestTypeDef",
     "IngestionDestinationSummaryTypeDef",
     "IngestionSummaryTypeDef",
-    "ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAppAuthorizationsRequestRequestTypeDef",
-    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
     "ListAppBundlesRequestRequestTypeDef",
-    "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
     "ListIngestionDestinationsRequestRequestTypeDef",
-    "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "ListIngestionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartIngestionRequestRequestTypeDef",
     "StartUserAccessTasksRequestRequestTypeDef",
     "StopIngestionRequestRequestTypeDef",
     "TaskErrorTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppAuthorizationSummaryTypeDef",
     "AppAuthorizationTypeDef",
-    "ListAppBundlesResponseTypeDef",
-    "CreateAppBundleResponseTypeDef",
-    "GetAppBundleResponseTypeDef",
-    "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
     "ConnectAppAuthorizationRequestRequestTypeDef",
+    "CreateAppBundleResponseTypeDef",
+    "GetAppBundleResponseTypeDef",
+    "ListAppBundlesResponseTypeDef",
     "CreateAppBundleRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIngestionResponseTypeDef",
     "GetIngestionResponseTypeDef",
     "CredentialTypeDef",
-    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "ListIngestionDestinationsResponseTypeDef",
     "ListIngestionsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
+    "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
+    "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "UserAccessResultItemTypeDef",
     "UserAccessTaskItemTypeDef",
     "ConnectAppAuthorizationResponseTypeDef",
     "ListAppAuthorizationsResponseTypeDef",
     "CreateAppAuthorizationResponseTypeDef",
     "GetAppAuthorizationResponseTypeDef",
     "UpdateAppAuthorizationResponseTypeDef",
     "CreateAppAuthorizationRequestRequestTypeDef",
     "UpdateAppAuthorizationRequestRequestTypeDef",
-    "AuditLogDestinationConfigurationOutputTypeDef",
     "AuditLogDestinationConfigurationTypeDef",
     "BatchGetUserAccessTasksResponseTypeDef",
     "StartUserAccessTasksResponseTypeDef",
-    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
-    "IngestionDestinationTypeDef",
     "CreateIngestionDestinationRequestRequestTypeDef",
+    "IngestionDestinationTypeDef",
     "UpdateIngestionDestinationRequestRequestTypeDef",
     "CreateIngestionDestinationResponseTypeDef",
     "GetIngestionDestinationResponseTypeDef",
     "UpdateIngestionDestinationResponseTypeDef",
 )
 
 ApiKeyCredentialTypeDef = TypedDict(
     "ApiKeyCredentialTypeDef",
     {
         "apiKey": str,
     },
 )
 
-TenantOutputTypeDef = TypedDict(
-    "TenantOutputTypeDef",
+TenantTypeDef = TypedDict(
+    "TenantTypeDef",
     {
         "tenantIdentifier": str,
         "tenantDisplayName": str,
     },
 )
 
 AppBundleSummaryTypeDef = TypedDict(
@@ -159,22 +150,14 @@
 )
 
 
 class AppBundleTypeDef(_RequiredAppBundleTypeDef, _OptionalAppBundleTypeDef):
     pass
 
 
-AuditLogProcessingConfigurationOutputTypeDef = TypedDict(
-    "AuditLogProcessingConfigurationOutputTypeDef",
-    {
-        "schema": SchemaType,
-        "format": FormatType,
-    },
-)
-
 AuditLogProcessingConfigurationTypeDef = TypedDict(
     "AuditLogProcessingConfigurationTypeDef",
     {
         "schema": SchemaType,
         "format": FormatType,
     },
 )
@@ -191,27 +174,30 @@
     "BatchGetUserAccessTasksRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "taskIdList": Sequence[str],
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "key": str,
-        "value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-TenantTypeDef = TypedDict(
-    "TenantTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "tenantIdentifier": str,
-        "tenantDisplayName": str,
+        "key": str,
+        "value": str,
     },
 )
 
 IngestionTypeDef = TypedDict(
     "IngestionTypeDef",
     {
         "arn": str,
@@ -261,40 +247,14 @@
     "DeleteIngestionRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
     },
 )
 
-FirehoseStreamOutputTypeDef = TypedDict(
-    "FirehoseStreamOutputTypeDef",
-    {
-        "streamName": str,
-    },
-)
-
-_RequiredS3BucketOutputTypeDef = TypedDict(
-    "_RequiredS3BucketOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-_OptionalS3BucketOutputTypeDef = TypedDict(
-    "_OptionalS3BucketOutputTypeDef",
-    {
-        "prefix": str,
-    },
-    total=False,
-)
-
-
-class S3BucketOutputTypeDef(_RequiredS3BucketOutputTypeDef, _OptionalS3BucketOutputTypeDef):
-    pass
-
-
 FirehoseStreamTypeDef = TypedDict(
     "FirehoseStreamTypeDef",
     {
         "streamName": str,
     },
 )
 
@@ -362,36 +322,24 @@
         "arn": str,
         "app": str,
         "tenantId": str,
         "state": IngestionStateType,
     },
 )
 
-_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-    },
-)
-_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
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
-class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(
-    _RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-    _OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAppAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppAuthorizationsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
     },
 )
 _OptionalListAppAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -407,54 +355,23 @@
 class ListAppAuthorizationsRequestRequestTypeDef(
     _RequiredListAppAuthorizationsRequestRequestTypeDef,
     _OptionalListAppAuthorizationsRequestRequestTypeDef,
 ):
     pass
 
 
-ListAppBundlesRequestListAppBundlesPaginateTypeDef = TypedDict(
-    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAppBundlesRequestRequestTypeDef = TypedDict(
     "ListAppBundlesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-        "ingestionIdentifier": str,
-    },
-)
-_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(
-    _RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-    _OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIngestionDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListIngestionDestinationsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
     },
 )
@@ -471,36 +388,14 @@
 class ListIngestionDestinationsRequestRequestTypeDef(
     _RequiredListIngestionDestinationsRequestRequestTypeDef,
     _OptionalListIngestionDestinationsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
-    "_RequiredListIngestionsRequestListIngestionsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-    },
-)
-_OptionalListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
-    "_OptionalListIngestionsRequestListIngestionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIngestionsRequestListIngestionsPaginateTypeDef(
-    _RequiredListIngestionsRequestListIngestionsPaginateTypeDef,
-    _OptionalListIngestionsRequestListIngestionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIngestionsRequestRequestTypeDef = TypedDict(
     "_RequiredListIngestionsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
     },
 )
 _OptionalListIngestionsRequestRequestTypeDef = TypedDict(
@@ -522,43 +417,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
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
 StartIngestionRequestRequestTypeDef = TypedDict(
     "StartIngestionRequestRequestTypeDef",
     {
         "ingestionIdentifier": str,
         "appBundleIdentifier": str,
     },
 )
@@ -598,27 +464,27 @@
 
 AppAuthorizationSummaryTypeDef = TypedDict(
     "AppAuthorizationSummaryTypeDef",
     {
         "appAuthorizationArn": str,
         "appBundleArn": str,
         "app": str,
-        "tenant": TenantOutputTypeDef,
+        "tenant": TenantTypeDef,
         "status": AppAuthorizationStatusType,
         "updatedAt": datetime,
     },
 )
 
 _RequiredAppAuthorizationTypeDef = TypedDict(
     "_RequiredAppAuthorizationTypeDef",
     {
         "appAuthorizationArn": str,
         "appBundleArn": str,
         "app": str,
-        "tenant": TenantOutputTypeDef,
+        "tenant": TenantTypeDef,
         "authType": AuthTypeType,
         "status": AppAuthorizationStatusType,
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 _OptionalAppAuthorizationTypeDef = TypedDict(
@@ -631,47 +497,14 @@
 )
 
 
 class AppAuthorizationTypeDef(_RequiredAppAuthorizationTypeDef, _OptionalAppAuthorizationTypeDef):
     pass
 
 
-ListAppBundlesResponseTypeDef = TypedDict(
-    "ListAppBundlesResponseTypeDef",
-    {
-        "appBundleSummaryList": List[AppBundleSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAppBundleResponseTypeDef = TypedDict(
-    "CreateAppBundleResponseTypeDef",
-    {
-        "appBundle": AppBundleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAppBundleResponseTypeDef = TypedDict(
-    "GetAppBundleResponseTypeDef",
-    {
-        "appBundle": AppBundleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProcessingConfigurationOutputTypeDef = TypedDict(
-    "ProcessingConfigurationOutputTypeDef",
-    {
-        "auditLog": AuditLogProcessingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "auditLog": AuditLogProcessingConfigurationTypeDef,
     },
     total=False,
 )
@@ -695,14 +528,39 @@
 class ConnectAppAuthorizationRequestRequestTypeDef(
     _RequiredConnectAppAuthorizationRequestRequestTypeDef,
     _OptionalConnectAppAuthorizationRequestRequestTypeDef,
 ):
     pass
 
 
+CreateAppBundleResponseTypeDef = TypedDict(
+    "CreateAppBundleResponseTypeDef",
+    {
+        "appBundle": AppBundleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppBundleResponseTypeDef = TypedDict(
+    "GetAppBundleResponseTypeDef",
+    {
+        "appBundle": AppBundleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppBundlesResponseTypeDef = TypedDict(
+    "ListAppBundlesResponseTypeDef",
+    {
+        "appBundleSummaryList": List[AppBundleSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateAppBundleRequestRequestTypeDef = TypedDict(
     "CreateAppBundleRequestRequestTypeDef",
     {
         "clientToken": str,
         "customerManagedKeyIdentifier": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -730,91 +588,157 @@
 
 class CreateIngestionRequestRequestTypeDef(
     _RequiredCreateIngestionRequestRequestTypeDef, _OptionalCreateIngestionRequestRequestTypeDef
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
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
 
 CreateIngestionResponseTypeDef = TypedDict(
     "CreateIngestionResponseTypeDef",
     {
         "ingestion": IngestionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIngestionResponseTypeDef = TypedDict(
     "GetIngestionResponseTypeDef",
     {
         "ingestion": IngestionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CredentialTypeDef = TypedDict(
     "CredentialTypeDef",
     {
         "oauth2Credential": Oauth2CredentialTypeDef,
         "apiKeyCredential": ApiKeyCredentialTypeDef,
     },
     total=False,
 )
 
-DestinationOutputTypeDef = TypedDict(
-    "DestinationOutputTypeDef",
-    {
-        "s3Bucket": S3BucketOutputTypeDef,
-        "firehoseStream": FirehoseStreamOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Bucket": S3BucketTypeDef,
         "firehoseStream": FirehoseStreamTypeDef,
     },
     total=False,
 )
 
 ListIngestionDestinationsResponseTypeDef = TypedDict(
     "ListIngestionDestinationsResponseTypeDef",
     {
         "ingestionDestinations": List[IngestionDestinationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIngestionsResponseTypeDef = TypedDict(
     "ListIngestionsResponseTypeDef",
     {
         "ingestions": List[IngestionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+    },
+)
+_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(
+    _RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    _OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+):
+    pass
+
+
+ListAppBundlesRequestListAppBundlesPaginateTypeDef = TypedDict(
+    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+        "ingestionIdentifier": str,
+    },
+)
+_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(
+    _RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+    _OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
+    "_RequiredListIngestionsRequestListIngestionsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+    },
+)
+_OptionalListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
+    "_OptionalListIngestionsRequestListIngestionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIngestionsRequestListIngestionsPaginateTypeDef(
+    _RequiredListIngestionsRequestListIngestionsPaginateTypeDef,
+    _OptionalListIngestionsRequestListIngestionsPaginateTypeDef,
+):
+    pass
+
+
 UserAccessResultItemTypeDef = TypedDict(
     "UserAccessResultItemTypeDef",
     {
         "app": str,
         "tenantId": str,
         "tenantDisplayName": str,
         "taskId": str,
@@ -853,48 +777,48 @@
     pass
 
 
 ConnectAppAuthorizationResponseTypeDef = TypedDict(
     "ConnectAppAuthorizationResponseTypeDef",
     {
         "appAuthorizationSummary": AppAuthorizationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppAuthorizationsResponseTypeDef = TypedDict(
     "ListAppAuthorizationsResponseTypeDef",
     {
         "appAuthorizationSummaryList": List[AppAuthorizationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppAuthorizationResponseTypeDef = TypedDict(
     "CreateAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppAuthorizationResponseTypeDef = TypedDict(
     "GetAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppAuthorizationResponseTypeDef = TypedDict(
     "UpdateAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAppAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppAuthorizationRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
@@ -941,109 +865,94 @@
 class UpdateAppAuthorizationRequestRequestTypeDef(
     _RequiredUpdateAppAuthorizationRequestRequestTypeDef,
     _OptionalUpdateAppAuthorizationRequestRequestTypeDef,
 ):
     pass
 
 
-AuditLogDestinationConfigurationOutputTypeDef = TypedDict(
-    "AuditLogDestinationConfigurationOutputTypeDef",
-    {
-        "destination": DestinationOutputTypeDef,
-    },
-)
-
 AuditLogDestinationConfigurationTypeDef = TypedDict(
     "AuditLogDestinationConfigurationTypeDef",
     {
         "destination": DestinationTypeDef,
     },
 )
 
 BatchGetUserAccessTasksResponseTypeDef = TypedDict(
     "BatchGetUserAccessTasksResponseTypeDef",
     {
         "userAccessResultsList": List[UserAccessResultItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartUserAccessTasksResponseTypeDef = TypedDict(
     "StartUserAccessTasksResponseTypeDef",
     {
         "userAccessTasksList": List[UserAccessTaskItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DestinationConfigurationOutputTypeDef = TypedDict(
-    "DestinationConfigurationOutputTypeDef",
-    {
-        "auditLog": AuditLogDestinationConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "auditLog": AuditLogDestinationConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredIngestionDestinationTypeDef = TypedDict(
-    "_RequiredIngestionDestinationTypeDef",
+_RequiredCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIngestionDestinationRequestRequestTypeDef",
     {
-        "arn": str,
-        "ingestionArn": str,
-        "processingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "appBundleIdentifier": str,
+        "ingestionIdentifier": str,
+        "processingConfiguration": ProcessingConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
     },
 )
-_OptionalIngestionDestinationTypeDef = TypedDict(
-    "_OptionalIngestionDestinationTypeDef",
+_OptionalCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIngestionDestinationRequestRequestTypeDef",
     {
-        "status": IngestionDestinationStatusType,
-        "statusReason": str,
-        "createdAt": datetime,
-        "updatedAt": datetime,
+        "clientToken": str,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
-class IngestionDestinationTypeDef(
-    _RequiredIngestionDestinationTypeDef, _OptionalIngestionDestinationTypeDef
+class CreateIngestionDestinationRequestRequestTypeDef(
+    _RequiredCreateIngestionDestinationRequestRequestTypeDef,
+    _OptionalCreateIngestionDestinationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIngestionDestinationRequestRequestTypeDef",
+_RequiredIngestionDestinationTypeDef = TypedDict(
+    "_RequiredIngestionDestinationTypeDef",
     {
-        "appBundleIdentifier": str,
-        "ingestionIdentifier": str,
+        "arn": str,
+        "ingestionArn": str,
         "processingConfiguration": ProcessingConfigurationTypeDef,
         "destinationConfiguration": DestinationConfigurationTypeDef,
     },
 )
-_OptionalCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIngestionDestinationRequestRequestTypeDef",
+_OptionalIngestionDestinationTypeDef = TypedDict(
+    "_OptionalIngestionDestinationTypeDef",
     {
-        "clientToken": str,
-        "tags": Sequence[TagTypeDef],
+        "status": IngestionDestinationStatusType,
+        "statusReason": str,
+        "createdAt": datetime,
+        "updatedAt": datetime,
     },
     total=False,
 )
 
 
-class CreateIngestionDestinationRequestRequestTypeDef(
-    _RequiredCreateIngestionDestinationRequestRequestTypeDef,
-    _OptionalCreateIngestionDestinationRequestRequestTypeDef,
+class IngestionDestinationTypeDef(
+    _RequiredIngestionDestinationTypeDef, _OptionalIngestionDestinationTypeDef
 ):
     pass
 
 
 UpdateIngestionDestinationRequestRequestTypeDef = TypedDict(
     "UpdateIngestionDestinationRequestRequestTypeDef",
     {
@@ -1054,26 +963,26 @@
     },
 )
 
 CreateIngestionDestinationResponseTypeDef = TypedDict(
     "CreateIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIngestionDestinationResponseTypeDef = TypedDict(
     "GetIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIngestionDestinationResponseTypeDef = TypedDict(
     "UpdateIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric/type_defs.pyi` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -33,107 +33,98 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiKeyCredentialTypeDef",
-    "TenantOutputTypeDef",
+    "TenantTypeDef",
     "AppBundleSummaryTypeDef",
     "AppBundleTypeDef",
-    "AuditLogProcessingConfigurationOutputTypeDef",
     "AuditLogProcessingConfigurationTypeDef",
     "AuthRequestTypeDef",
     "BatchGetUserAccessTasksRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
-    "TenantTypeDef",
     "IngestionTypeDef",
     "Oauth2CredentialTypeDef",
     "DeleteAppAuthorizationRequestRequestTypeDef",
     "DeleteAppBundleRequestRequestTypeDef",
     "DeleteIngestionDestinationRequestRequestTypeDef",
     "DeleteIngestionRequestRequestTypeDef",
-    "FirehoseStreamOutputTypeDef",
-    "S3BucketOutputTypeDef",
     "FirehoseStreamTypeDef",
     "S3BucketTypeDef",
     "GetAppAuthorizationRequestRequestTypeDef",
     "GetAppBundleRequestRequestTypeDef",
     "GetIngestionDestinationRequestRequestTypeDef",
     "GetIngestionRequestRequestTypeDef",
     "IngestionDestinationSummaryTypeDef",
     "IngestionSummaryTypeDef",
-    "ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAppAuthorizationsRequestRequestTypeDef",
-    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
     "ListAppBundlesRequestRequestTypeDef",
-    "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
     "ListIngestionDestinationsRequestRequestTypeDef",
-    "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "ListIngestionsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartIngestionRequestRequestTypeDef",
     "StartUserAccessTasksRequestRequestTypeDef",
     "StopIngestionRequestRequestTypeDef",
     "TaskErrorTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AppAuthorizationSummaryTypeDef",
     "AppAuthorizationTypeDef",
-    "ListAppBundlesResponseTypeDef",
-    "CreateAppBundleResponseTypeDef",
-    "GetAppBundleResponseTypeDef",
-    "ProcessingConfigurationOutputTypeDef",
     "ProcessingConfigurationTypeDef",
     "ConnectAppAuthorizationRequestRequestTypeDef",
+    "CreateAppBundleResponseTypeDef",
+    "GetAppBundleResponseTypeDef",
+    "ListAppBundlesResponseTypeDef",
     "CreateAppBundleRequestRequestTypeDef",
     "CreateIngestionRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateIngestionResponseTypeDef",
     "GetIngestionResponseTypeDef",
     "CredentialTypeDef",
-    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "ListIngestionDestinationsResponseTypeDef",
     "ListIngestionsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
+    "ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
+    "ListIngestionsRequestListIngestionsPaginateTypeDef",
     "UserAccessResultItemTypeDef",
     "UserAccessTaskItemTypeDef",
     "ConnectAppAuthorizationResponseTypeDef",
     "ListAppAuthorizationsResponseTypeDef",
     "CreateAppAuthorizationResponseTypeDef",
     "GetAppAuthorizationResponseTypeDef",
     "UpdateAppAuthorizationResponseTypeDef",
     "CreateAppAuthorizationRequestRequestTypeDef",
     "UpdateAppAuthorizationRequestRequestTypeDef",
-    "AuditLogDestinationConfigurationOutputTypeDef",
     "AuditLogDestinationConfigurationTypeDef",
     "BatchGetUserAccessTasksResponseTypeDef",
     "StartUserAccessTasksResponseTypeDef",
-    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
-    "IngestionDestinationTypeDef",
     "CreateIngestionDestinationRequestRequestTypeDef",
+    "IngestionDestinationTypeDef",
     "UpdateIngestionDestinationRequestRequestTypeDef",
     "CreateIngestionDestinationResponseTypeDef",
     "GetIngestionDestinationResponseTypeDef",
     "UpdateIngestionDestinationResponseTypeDef",
 )
 
 ApiKeyCredentialTypeDef = TypedDict(
     "ApiKeyCredentialTypeDef",
     {
         "apiKey": str,
     },
 )
 
-TenantOutputTypeDef = TypedDict(
-    "TenantOutputTypeDef",
+TenantTypeDef = TypedDict(
+    "TenantTypeDef",
     {
         "tenantIdentifier": str,
         "tenantDisplayName": str,
     },
 )
 
 AppBundleSummaryTypeDef = TypedDict(
@@ -156,22 +147,14 @@
     },
     total=False,
 )
 
 class AppBundleTypeDef(_RequiredAppBundleTypeDef, _OptionalAppBundleTypeDef):
     pass
 
-AuditLogProcessingConfigurationOutputTypeDef = TypedDict(
-    "AuditLogProcessingConfigurationOutputTypeDef",
-    {
-        "schema": SchemaType,
-        "format": FormatType,
-    },
-)
-
 AuditLogProcessingConfigurationTypeDef = TypedDict(
     "AuditLogProcessingConfigurationTypeDef",
     {
         "schema": SchemaType,
         "format": FormatType,
     },
 )
@@ -188,27 +171,30 @@
     "BatchGetUserAccessTasksRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "taskIdList": Sequence[str],
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "key": str,
-        "value": str,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-TenantTypeDef = TypedDict(
-    "TenantTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "tenantIdentifier": str,
-        "tenantDisplayName": str,
+        "key": str,
+        "value": str,
     },
 )
 
 IngestionTypeDef = TypedDict(
     "IngestionTypeDef",
     {
         "arn": str,
@@ -258,38 +244,14 @@
     "DeleteIngestionRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
     },
 )
 
-FirehoseStreamOutputTypeDef = TypedDict(
-    "FirehoseStreamOutputTypeDef",
-    {
-        "streamName": str,
-    },
-)
-
-_RequiredS3BucketOutputTypeDef = TypedDict(
-    "_RequiredS3BucketOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-_OptionalS3BucketOutputTypeDef = TypedDict(
-    "_OptionalS3BucketOutputTypeDef",
-    {
-        "prefix": str,
-    },
-    total=False,
-)
-
-class S3BucketOutputTypeDef(_RequiredS3BucketOutputTypeDef, _OptionalS3BucketOutputTypeDef):
-    pass
-
 FirehoseStreamTypeDef = TypedDict(
     "FirehoseStreamTypeDef",
     {
         "streamName": str,
     },
 )
 
@@ -355,34 +317,24 @@
         "arn": str,
         "app": str,
         "tenantId": str,
         "state": IngestionStateType,
     },
 )
 
-_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-    },
-)
-_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
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
 
-class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(
-    _RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-    _OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAppAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppAuthorizationsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
     },
 )
 _OptionalListAppAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -396,52 +348,23 @@
 
 class ListAppAuthorizationsRequestRequestTypeDef(
     _RequiredListAppAuthorizationsRequestRequestTypeDef,
     _OptionalListAppAuthorizationsRequestRequestTypeDef,
 ):
     pass
 
-ListAppBundlesRequestListAppBundlesPaginateTypeDef = TypedDict(
-    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAppBundlesRequestRequestTypeDef = TypedDict(
     "ListAppBundlesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
-    "_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-        "ingestionIdentifier": str,
-    },
-)
-_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
-    "_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(
-    _RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-    _OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListIngestionDestinationsRequestRequestTypeDef = TypedDict(
     "_RequiredListIngestionDestinationsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
     },
 )
@@ -456,34 +379,14 @@
 
 class ListIngestionDestinationsRequestRequestTypeDef(
     _RequiredListIngestionDestinationsRequestRequestTypeDef,
     _OptionalListIngestionDestinationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
-    "_RequiredListIngestionsRequestListIngestionsPaginateTypeDef",
-    {
-        "appBundleIdentifier": str,
-    },
-)
-_OptionalListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
-    "_OptionalListIngestionsRequestListIngestionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIngestionsRequestListIngestionsPaginateTypeDef(
-    _RequiredListIngestionsRequestListIngestionsPaginateTypeDef,
-    _OptionalListIngestionsRequestListIngestionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListIngestionsRequestRequestTypeDef = TypedDict(
     "_RequiredListIngestionsRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
     },
 )
 _OptionalListIngestionsRequestRequestTypeDef = TypedDict(
@@ -503,43 +406,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
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
 StartIngestionRequestRequestTypeDef = TypedDict(
     "StartIngestionRequestRequestTypeDef",
     {
         "ingestionIdentifier": str,
         "appBundleIdentifier": str,
     },
 )
@@ -579,27 +453,27 @@
 
 AppAuthorizationSummaryTypeDef = TypedDict(
     "AppAuthorizationSummaryTypeDef",
     {
         "appAuthorizationArn": str,
         "appBundleArn": str,
         "app": str,
-        "tenant": TenantOutputTypeDef,
+        "tenant": TenantTypeDef,
         "status": AppAuthorizationStatusType,
         "updatedAt": datetime,
     },
 )
 
 _RequiredAppAuthorizationTypeDef = TypedDict(
     "_RequiredAppAuthorizationTypeDef",
     {
         "appAuthorizationArn": str,
         "appBundleArn": str,
         "app": str,
-        "tenant": TenantOutputTypeDef,
+        "tenant": TenantTypeDef,
         "authType": AuthTypeType,
         "status": AppAuthorizationStatusType,
         "createdAt": datetime,
         "updatedAt": datetime,
     },
 )
 _OptionalAppAuthorizationTypeDef = TypedDict(
@@ -610,47 +484,14 @@
     },
     total=False,
 )
 
 class AppAuthorizationTypeDef(_RequiredAppAuthorizationTypeDef, _OptionalAppAuthorizationTypeDef):
     pass
 
-ListAppBundlesResponseTypeDef = TypedDict(
-    "ListAppBundlesResponseTypeDef",
-    {
-        "appBundleSummaryList": List[AppBundleSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAppBundleResponseTypeDef = TypedDict(
-    "CreateAppBundleResponseTypeDef",
-    {
-        "appBundle": AppBundleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAppBundleResponseTypeDef = TypedDict(
-    "GetAppBundleResponseTypeDef",
-    {
-        "appBundle": AppBundleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ProcessingConfigurationOutputTypeDef = TypedDict(
-    "ProcessingConfigurationOutputTypeDef",
-    {
-        "auditLog": AuditLogProcessingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 ProcessingConfigurationTypeDef = TypedDict(
     "ProcessingConfigurationTypeDef",
     {
         "auditLog": AuditLogProcessingConfigurationTypeDef,
     },
     total=False,
 )
@@ -672,14 +513,39 @@
 
 class ConnectAppAuthorizationRequestRequestTypeDef(
     _RequiredConnectAppAuthorizationRequestRequestTypeDef,
     _OptionalConnectAppAuthorizationRequestRequestTypeDef,
 ):
     pass
 
+CreateAppBundleResponseTypeDef = TypedDict(
+    "CreateAppBundleResponseTypeDef",
+    {
+        "appBundle": AppBundleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAppBundleResponseTypeDef = TypedDict(
+    "GetAppBundleResponseTypeDef",
+    {
+        "appBundle": AppBundleTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAppBundlesResponseTypeDef = TypedDict(
+    "ListAppBundlesResponseTypeDef",
+    {
+        "appBundleSummaryList": List[AppBundleSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateAppBundleRequestRequestTypeDef = TypedDict(
     "CreateAppBundleRequestRequestTypeDef",
     {
         "clientToken": str,
         "customerManagedKeyIdentifier": str,
         "tags": Sequence[TagTypeDef],
     },
@@ -705,91 +571,151 @@
 )
 
 class CreateIngestionRequestRequestTypeDef(
     _RequiredCreateIngestionRequestRequestTypeDef, _OptionalCreateIngestionRequestRequestTypeDef
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
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
 
 CreateIngestionResponseTypeDef = TypedDict(
     "CreateIngestionResponseTypeDef",
     {
         "ingestion": IngestionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIngestionResponseTypeDef = TypedDict(
     "GetIngestionResponseTypeDef",
     {
         "ingestion": IngestionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CredentialTypeDef = TypedDict(
     "CredentialTypeDef",
     {
         "oauth2Credential": Oauth2CredentialTypeDef,
         "apiKeyCredential": ApiKeyCredentialTypeDef,
     },
     total=False,
 )
 
-DestinationOutputTypeDef = TypedDict(
-    "DestinationOutputTypeDef",
-    {
-        "s3Bucket": S3BucketOutputTypeDef,
-        "firehoseStream": FirehoseStreamOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Bucket": S3BucketTypeDef,
         "firehoseStream": FirehoseStreamTypeDef,
     },
     total=False,
 )
 
 ListIngestionDestinationsResponseTypeDef = TypedDict(
     "ListIngestionDestinationsResponseTypeDef",
     {
         "ingestionDestinations": List[IngestionDestinationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIngestionsResponseTypeDef = TypedDict(
     "ListIngestionsResponseTypeDef",
     {
         "ingestions": List[IngestionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+    },
+)
+_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef(
+    _RequiredListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    _OptionalListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+):
+    pass
+
+ListAppBundlesRequestListAppBundlesPaginateTypeDef = TypedDict(
+    "ListAppBundlesRequestListAppBundlesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
+    "_RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+        "ingestionIdentifier": str,
+    },
+)
+_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef = TypedDict(
+    "_OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef(
+    _RequiredListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+    _OptionalListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+):
+    pass
+
+_RequiredListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
+    "_RequiredListIngestionsRequestListIngestionsPaginateTypeDef",
+    {
+        "appBundleIdentifier": str,
+    },
+)
+_OptionalListIngestionsRequestListIngestionsPaginateTypeDef = TypedDict(
+    "_OptionalListIngestionsRequestListIngestionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIngestionsRequestListIngestionsPaginateTypeDef(
+    _RequiredListIngestionsRequestListIngestionsPaginateTypeDef,
+    _OptionalListIngestionsRequestListIngestionsPaginateTypeDef,
+):
+    pass
+
 UserAccessResultItemTypeDef = TypedDict(
     "UserAccessResultItemTypeDef",
     {
         "app": str,
         "tenantId": str,
         "tenantDisplayName": str,
         "taskId": str,
@@ -826,48 +752,48 @@
 ):
     pass
 
 ConnectAppAuthorizationResponseTypeDef = TypedDict(
     "ConnectAppAuthorizationResponseTypeDef",
     {
         "appAuthorizationSummary": AppAuthorizationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppAuthorizationsResponseTypeDef = TypedDict(
     "ListAppAuthorizationsResponseTypeDef",
     {
         "appAuthorizationSummaryList": List[AppAuthorizationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateAppAuthorizationResponseTypeDef = TypedDict(
     "CreateAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAppAuthorizationResponseTypeDef = TypedDict(
     "GetAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAppAuthorizationResponseTypeDef = TypedDict(
     "UpdateAppAuthorizationResponseTypeDef",
     {
         "appAuthorization": AppAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateAppAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppAuthorizationRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
@@ -910,67 +836,76 @@
 
 class UpdateAppAuthorizationRequestRequestTypeDef(
     _RequiredUpdateAppAuthorizationRequestRequestTypeDef,
     _OptionalUpdateAppAuthorizationRequestRequestTypeDef,
 ):
     pass
 
-AuditLogDestinationConfigurationOutputTypeDef = TypedDict(
-    "AuditLogDestinationConfigurationOutputTypeDef",
-    {
-        "destination": DestinationOutputTypeDef,
-    },
-)
-
 AuditLogDestinationConfigurationTypeDef = TypedDict(
     "AuditLogDestinationConfigurationTypeDef",
     {
         "destination": DestinationTypeDef,
     },
 )
 
 BatchGetUserAccessTasksResponseTypeDef = TypedDict(
     "BatchGetUserAccessTasksResponseTypeDef",
     {
         "userAccessResultsList": List[UserAccessResultItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartUserAccessTasksResponseTypeDef = TypedDict(
     "StartUserAccessTasksResponseTypeDef",
     {
         "userAccessTasksList": List[UserAccessTaskItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DestinationConfigurationOutputTypeDef = TypedDict(
-    "DestinationConfigurationOutputTypeDef",
+DestinationConfigurationTypeDef = TypedDict(
+    "DestinationConfigurationTypeDef",
     {
-        "auditLog": AuditLogDestinationConfigurationOutputTypeDef,
+        "auditLog": AuditLogDestinationConfigurationTypeDef,
     },
     total=False,
 )
 
-DestinationConfigurationTypeDef = TypedDict(
-    "DestinationConfigurationTypeDef",
+_RequiredCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIngestionDestinationRequestRequestTypeDef",
     {
-        "auditLog": AuditLogDestinationConfigurationTypeDef,
+        "appBundleIdentifier": str,
+        "ingestionIdentifier": str,
+        "processingConfiguration": ProcessingConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
+    },
+)
+_OptionalCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIngestionDestinationRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+class CreateIngestionDestinationRequestRequestTypeDef(
+    _RequiredCreateIngestionDestinationRequestRequestTypeDef,
+    _OptionalCreateIngestionDestinationRequestRequestTypeDef,
+):
+    pass
+
 _RequiredIngestionDestinationTypeDef = TypedDict(
     "_RequiredIngestionDestinationTypeDef",
     {
         "arn": str,
         "ingestionArn": str,
-        "processingConfiguration": ProcessingConfigurationOutputTypeDef,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "processingConfiguration": ProcessingConfigurationTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
     },
 )
 _OptionalIngestionDestinationTypeDef = TypedDict(
     "_OptionalIngestionDestinationTypeDef",
     {
         "status": IngestionDestinationStatusType,
         "statusReason": str,
@@ -981,64 +916,40 @@
 )
 
 class IngestionDestinationTypeDef(
     _RequiredIngestionDestinationTypeDef, _OptionalIngestionDestinationTypeDef
 ):
     pass
 
-_RequiredCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIngestionDestinationRequestRequestTypeDef",
-    {
-        "appBundleIdentifier": str,
-        "ingestionIdentifier": str,
-        "processingConfiguration": ProcessingConfigurationTypeDef,
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateIngestionDestinationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIngestionDestinationRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateIngestionDestinationRequestRequestTypeDef(
-    _RequiredCreateIngestionDestinationRequestRequestTypeDef,
-    _OptionalCreateIngestionDestinationRequestRequestTypeDef,
-):
-    pass
-
 UpdateIngestionDestinationRequestRequestTypeDef = TypedDict(
     "UpdateIngestionDestinationRequestRequestTypeDef",
     {
         "appBundleIdentifier": str,
         "ingestionIdentifier": str,
         "ingestionDestinationIdentifier": str,
         "destinationConfiguration": DestinationConfigurationTypeDef,
     },
 )
 
 CreateIngestionDestinationResponseTypeDef = TypedDict(
     "CreateIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIngestionDestinationResponseTypeDef = TypedDict(
     "GetIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIngestionDestinationResponseTypeDef = TypedDict(
     "UpdateIngestionDestinationResponseTypeDef",
     {
         "ingestionDestination": IngestionDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/PKG-INFO` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appfabric
-Version: 1.28.12
-Summary: Type annotations for boto3.AppFabric 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppFabric 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appfabric.svg?color=blue)](https://pypi.org/project/mypy-boto3-appfabric)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appfabric)](https://pepy.tech/project/mypy-boto3-appfabric)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppFabric 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
+[boto3.AppFabric 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appfabric.html#AppFabric)
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
 [mypy-boto3-appfabric docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appfabric/).
 
 See how it helps to find and fix potential bugs:
 
@@ -342,92 +342,83 @@
 
 `mypy_boto3_appfabric.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appfabric.type_defs import (
     ApiKeyCredentialTypeDef,
-    TenantOutputTypeDef,
+    TenantTypeDef,
     AppBundleSummaryTypeDef,
     AppBundleTypeDef,
-    AuditLogProcessingConfigurationOutputTypeDef,
     AuditLogProcessingConfigurationTypeDef,
     AuthRequestTypeDef,
     BatchGetUserAccessTasksRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
-    TenantTypeDef,
     IngestionTypeDef,
     Oauth2CredentialTypeDef,
     DeleteAppAuthorizationRequestRequestTypeDef,
     DeleteAppBundleRequestRequestTypeDef,
     DeleteIngestionDestinationRequestRequestTypeDef,
     DeleteIngestionRequestRequestTypeDef,
-    FirehoseStreamOutputTypeDef,
-    S3BucketOutputTypeDef,
     FirehoseStreamTypeDef,
     S3BucketTypeDef,
     GetAppAuthorizationRequestRequestTypeDef,
     GetAppBundleRequestRequestTypeDef,
     GetIngestionDestinationRequestRequestTypeDef,
     GetIngestionRequestRequestTypeDef,
     IngestionDestinationSummaryTypeDef,
     IngestionSummaryTypeDef,
-    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAppAuthorizationsRequestRequestTypeDef,
-    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
     ListAppBundlesRequestRequestTypeDef,
-    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
     ListIngestionDestinationsRequestRequestTypeDef,
-    ListIngestionsRequestListIngestionsPaginateTypeDef,
     ListIngestionsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartIngestionRequestRequestTypeDef,
     StartUserAccessTasksRequestRequestTypeDef,
     StopIngestionRequestRequestTypeDef,
     TaskErrorTypeDef,
     UntagResourceRequestRequestTypeDef,
     AppAuthorizationSummaryTypeDef,
     AppAuthorizationTypeDef,
-    ListAppBundlesResponseTypeDef,
-    CreateAppBundleResponseTypeDef,
-    GetAppBundleResponseTypeDef,
-    ProcessingConfigurationOutputTypeDef,
     ProcessingConfigurationTypeDef,
     ConnectAppAuthorizationRequestRequestTypeDef,
+    CreateAppBundleResponseTypeDef,
+    GetAppBundleResponseTypeDef,
+    ListAppBundlesResponseTypeDef,
     CreateAppBundleRequestRequestTypeDef,
     CreateIngestionRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateIngestionResponseTypeDef,
     GetIngestionResponseTypeDef,
     CredentialTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListIngestionDestinationsResponseTypeDef,
     ListIngestionsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAppAuthorizationsRequestListAppAuthorizationsPaginateTypeDef,
+    ListAppBundlesRequestListAppBundlesPaginateTypeDef,
+    ListIngestionDestinationsRequestListIngestionDestinationsPaginateTypeDef,
+    ListIngestionsRequestListIngestionsPaginateTypeDef,
     UserAccessResultItemTypeDef,
     UserAccessTaskItemTypeDef,
     ConnectAppAuthorizationResponseTypeDef,
     ListAppAuthorizationsResponseTypeDef,
     CreateAppAuthorizationResponseTypeDef,
     GetAppAuthorizationResponseTypeDef,
     UpdateAppAuthorizationResponseTypeDef,
     CreateAppAuthorizationRequestRequestTypeDef,
     UpdateAppAuthorizationRequestRequestTypeDef,
-    AuditLogDestinationConfigurationOutputTypeDef,
     AuditLogDestinationConfigurationTypeDef,
     BatchGetUserAccessTasksResponseTypeDef,
     StartUserAccessTasksResponseTypeDef,
-    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
-    IngestionDestinationTypeDef,
     CreateIngestionDestinationRequestRequestTypeDef,
+    IngestionDestinationTypeDef,
     UpdateIngestionDestinationRequestRequestTypeDef,
     CreateIngestionDestinationResponseTypeDef,
     GetIngestionDestinationResponseTypeDef,
     UpdateIngestionDestinationResponseTypeDef,
 )
```

### Comparing `mypy-boto3-appfabric-1.28.12/mypy_boto3_appfabric.egg-info/SOURCES.txt` & `mypy-boto3-appfabric-1.28.15/mypy_boto3_appfabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appfabric-1.28.12/setup.py` & `mypy-boto3-appfabric-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appfabric",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_appfabric"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppFabric 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AppFabric 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

