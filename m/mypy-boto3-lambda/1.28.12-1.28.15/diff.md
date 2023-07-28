# Comparing `tmp/mypy-boto3-lambda-1.28.12.tar.gz` & `tmp/mypy-boto3-lambda-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lambda-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
+gzip compressed data, was "mypy-boto3-lambda-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
```

## Comparing `mypy-boto3-lambda-1.28.12.tar` & `mypy-boto3-lambda-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25529 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24046 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59888 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    59798 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13717 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    82923 2023-07-27 05:24:58.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    82816 2023-07-27 05:24:56.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25529 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:55.000000 mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.556461 mypy-boto3-lambda-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:24:55.000000 mypy-boto3-lambda-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.513381 mypy-boto3-lambda-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25001 2023-07-28 20:43:08.501381 mypy-boto3-lambda-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23518 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.501381 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59706 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59616 2023-07-28 20:29:34.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14373 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13695 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    79959 2023-07-28 20:29:38.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79852 2023-07-28 20:29:37.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6159 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-07-28 20:29:36.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.501381 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25001 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:08.000000 mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.513381 mypy-boto3-lambda-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:29:33.000000 mypy-boto3-lambda-1.28.15/setup.py
```

### Comparing `mypy-boto3-lambda-1.28.12/LICENSE` & `mypy-boto3-lambda-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.12/PKG-INFO` & `mypy-boto3-lambda-1.28.15/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lambda
-Version: 1.28.12
-Summary: Type annotations for boto3.Lambda 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -461,26 +461,22 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
-    AddLayerVersionPermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddPermissionRequestRequestTypeDef,
-    AddPermissionResponseTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
-    AmazonManagedKafkaEventSourceConfigOutputTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
-    CodeSigningPoliciesOutputTypeDef,
     CodeSigningPoliciesTypeDef,
-    ConcurrencyResponseMetadataTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
@@ -490,138 +486,118 @@
     EphemeralStorageTypeDef,
     FileSystemConfigTypeDef,
     FunctionCodeTypeDef,
     ImageConfigTypeDef,
     SnapStartTypeDef,
     TracingConfigTypeDef,
     VpcConfigTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCodeSigningConfigRequestRequestTypeDef,
     DeleteEventSourceMappingRequestRequestTypeDef,
     DeleteFunctionCodeSigningConfigRequestRequestTypeDef,
     DeleteFunctionConcurrencyRequestRequestTypeDef,
     DeleteFunctionEventInvokeConfigRequestRequestTypeDef,
     DeleteFunctionRequestRequestTypeDef,
     DeleteFunctionUrlConfigRequestRequestTypeDef,
     DeleteLayerVersionRequestRequestTypeDef,
     DeleteProvisionedConcurrencyConfigRequestRequestTypeDef,
-    OnFailureOutputTypeDef,
-    OnSuccessOutputTypeDef,
     OnFailureTypeDef,
     OnSuccessTypeDef,
-    DocumentDBEventSourceConfigOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentErrorTypeDef,
-    EphemeralStorageOutputTypeDef,
-    ScalingConfigOutputTypeDef,
     SelfManagedEventSourceOutputTypeDef,
-    SelfManagedKafkaEventSourceConfigOutputTypeDef,
-    SourceAccessConfigurationOutputTypeDef,
-    FileSystemConfigOutputTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     FunctionCodeLocationTypeDef,
     LayerTypeDef,
     SnapStartResponseTypeDef,
     TracingConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     GetAliasRequestRequestTypeDef,
     GetCodeSigningConfigRequestRequestTypeDef,
     GetEventSourceMappingRequestRequestTypeDef,
     GetFunctionCodeSigningConfigRequestRequestTypeDef,
-    GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyRequestRequestTypeDef,
-    GetFunctionConcurrencyResponseTypeDef,
     WaiterConfigTypeDef,
     GetFunctionConfigurationRequestRequestTypeDef,
     GetFunctionEventInvokeConfigRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionUrlConfigRequestRequestTypeDef,
     GetLayerVersionByArnRequestRequestTypeDef,
     GetLayerVersionPolicyRequestRequestTypeDef,
-    GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
-    GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
-    GetRuntimeManagementConfigResponseTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
     InvocationRequestRequestTypeDef,
-    InvocationResponseTypeDef,
     InvokeAsyncRequestRequestTypeDef,
-    InvokeAsyncResponseTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
     InvokeWithResponseStreamRequestRequestTypeDef,
     LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
-    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
-    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
-    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
-    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
     ListFunctionsByCodeSigningConfigRequestRequestTypeDef,
-    ListFunctionsByCodeSigningConfigResponseTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayerVersionsRequestRequestTypeDef,
-    ListLayersRequestListLayersPaginateTypeDef,
     ListLayersRequestRequestTypeDef,
-    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestRequestTypeDef,
     ProvisionedConcurrencyConfigListItemTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
-    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListVersionsByFunctionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishVersionRequestRequestTypeDef,
     PutFunctionCodeSigningConfigRequestRequestTypeDef,
-    PutFunctionCodeSigningConfigResponseTypeDef,
     PutFunctionConcurrencyRequestRequestTypeDef,
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
-    PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
-    PutRuntimeManagementConfigResponseTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFunctionCodeRequestRequestTypeDef,
+    AddLayerVersionPermissionResponseTypeDef,
+    AddPermissionResponseTypeDef,
+    ConcurrencyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
-    AliasConfigurationResponseMetadataTypeDef,
+    GetFunctionCodeSigningConfigResponseTypeDef,
+    GetFunctionConcurrencyResponseTypeDef,
+    GetLayerVersionPolicyResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProvisionedConcurrencyConfigResponseTypeDef,
+    GetRuntimeManagementConfigResponseTypeDef,
+    InvocationResponseTypeDef,
+    InvokeAsyncResponseTypeDef,
+    ListFunctionsByCodeSigningConfigResponseTypeDef,
+    ListTagsResponseTypeDef,
+    PutFunctionCodeSigningConfigResponseTypeDef,
+    PutProvisionedConcurrencyConfigResponseTypeDef,
+    PutRuntimeManagementConfigResponseTypeDef,
+    AliasConfigurationResponseTypeDef,
     AliasConfigurationTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     FunctionUrlConfigTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
     CreateFunctionUrlConfigRequestRequestTypeDef,
     UpdateFunctionUrlConfigRequestRequestTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionConfigurationRequestRequestTypeDef,
-    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     EnvironmentResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     GetFunctionConfigurationRequestFunctionActiveWaitTypeDef,
     GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef,
     GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef,
@@ -631,33 +607,44 @@
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
     PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
+    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
+    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
+    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+    ListLayersRequestListLayersPaginateTypeDef,
+    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     ListFunctionUrlConfigsResponseTypeDef,
-    FunctionEventInvokeConfigResponseMetadataTypeDef,
+    FunctionEventInvokeConfigResponseTypeDef,
     FunctionEventInvokeConfigTypeDef,
     PutFunctionEventInvokeConfigRequestRequestTypeDef,
     UpdateFunctionEventInvokeConfigRequestRequestTypeDef,
-    EventSourceMappingConfigurationResponseMetadataTypeDef,
+    EventSourceMappingConfigurationResponseTypeDef,
     EventSourceMappingConfigurationTypeDef,
     CreateEventSourceMappingRequestRequestTypeDef,
     UpdateEventSourceMappingRequestRequestTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     ListLayersResponseTypeDef,
-    FunctionConfigurationResponseMetadataTypeDef,
+    FunctionConfigurationResponseTypeDef,
     FunctionConfigurationTypeDef,
     ListFunctionEventInvokeConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
     GetFunctionResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lambda-1.28.12/README.md` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-lambda
+Version: 1.28.15
+Summary: Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 lambda type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-lambda"></a>
 
 # mypy-boto3-lambda
 
 [![PyPI - mypy-boto3-lambda](https://img.shields.io/pypi/v/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -429,26 +461,22 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
-    AddLayerVersionPermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddPermissionRequestRequestTypeDef,
-    AddPermissionResponseTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
-    AmazonManagedKafkaEventSourceConfigOutputTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
-    CodeSigningPoliciesOutputTypeDef,
     CodeSigningPoliciesTypeDef,
-    ConcurrencyResponseMetadataTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
@@ -458,138 +486,118 @@
     EphemeralStorageTypeDef,
     FileSystemConfigTypeDef,
     FunctionCodeTypeDef,
     ImageConfigTypeDef,
     SnapStartTypeDef,
     TracingConfigTypeDef,
     VpcConfigTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCodeSigningConfigRequestRequestTypeDef,
     DeleteEventSourceMappingRequestRequestTypeDef,
     DeleteFunctionCodeSigningConfigRequestRequestTypeDef,
     DeleteFunctionConcurrencyRequestRequestTypeDef,
     DeleteFunctionEventInvokeConfigRequestRequestTypeDef,
     DeleteFunctionRequestRequestTypeDef,
     DeleteFunctionUrlConfigRequestRequestTypeDef,
     DeleteLayerVersionRequestRequestTypeDef,
     DeleteProvisionedConcurrencyConfigRequestRequestTypeDef,
-    OnFailureOutputTypeDef,
-    OnSuccessOutputTypeDef,
     OnFailureTypeDef,
     OnSuccessTypeDef,
-    DocumentDBEventSourceConfigOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentErrorTypeDef,
-    EphemeralStorageOutputTypeDef,
-    ScalingConfigOutputTypeDef,
     SelfManagedEventSourceOutputTypeDef,
-    SelfManagedKafkaEventSourceConfigOutputTypeDef,
-    SourceAccessConfigurationOutputTypeDef,
-    FileSystemConfigOutputTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     FunctionCodeLocationTypeDef,
     LayerTypeDef,
     SnapStartResponseTypeDef,
     TracingConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     GetAliasRequestRequestTypeDef,
     GetCodeSigningConfigRequestRequestTypeDef,
     GetEventSourceMappingRequestRequestTypeDef,
     GetFunctionCodeSigningConfigRequestRequestTypeDef,
-    GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyRequestRequestTypeDef,
-    GetFunctionConcurrencyResponseTypeDef,
     WaiterConfigTypeDef,
     GetFunctionConfigurationRequestRequestTypeDef,
     GetFunctionEventInvokeConfigRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionUrlConfigRequestRequestTypeDef,
     GetLayerVersionByArnRequestRequestTypeDef,
     GetLayerVersionPolicyRequestRequestTypeDef,
-    GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
-    GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
-    GetRuntimeManagementConfigResponseTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
     InvocationRequestRequestTypeDef,
-    InvocationResponseTypeDef,
     InvokeAsyncRequestRequestTypeDef,
-    InvokeAsyncResponseTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
     InvokeWithResponseStreamRequestRequestTypeDef,
     LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
-    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
-    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
-    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
-    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
     ListFunctionsByCodeSigningConfigRequestRequestTypeDef,
-    ListFunctionsByCodeSigningConfigResponseTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayerVersionsRequestRequestTypeDef,
-    ListLayersRequestListLayersPaginateTypeDef,
     ListLayersRequestRequestTypeDef,
-    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestRequestTypeDef,
     ProvisionedConcurrencyConfigListItemTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
-    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListVersionsByFunctionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishVersionRequestRequestTypeDef,
     PutFunctionCodeSigningConfigRequestRequestTypeDef,
-    PutFunctionCodeSigningConfigResponseTypeDef,
     PutFunctionConcurrencyRequestRequestTypeDef,
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
-    PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
-    PutRuntimeManagementConfigResponseTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFunctionCodeRequestRequestTypeDef,
+    AddLayerVersionPermissionResponseTypeDef,
+    AddPermissionResponseTypeDef,
+    ConcurrencyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
-    AliasConfigurationResponseMetadataTypeDef,
+    GetFunctionCodeSigningConfigResponseTypeDef,
+    GetFunctionConcurrencyResponseTypeDef,
+    GetLayerVersionPolicyResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProvisionedConcurrencyConfigResponseTypeDef,
+    GetRuntimeManagementConfigResponseTypeDef,
+    InvocationResponseTypeDef,
+    InvokeAsyncResponseTypeDef,
+    ListFunctionsByCodeSigningConfigResponseTypeDef,
+    ListTagsResponseTypeDef,
+    PutFunctionCodeSigningConfigResponseTypeDef,
+    PutProvisionedConcurrencyConfigResponseTypeDef,
+    PutRuntimeManagementConfigResponseTypeDef,
+    AliasConfigurationResponseTypeDef,
     AliasConfigurationTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     FunctionUrlConfigTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
     CreateFunctionUrlConfigRequestRequestTypeDef,
     UpdateFunctionUrlConfigRequestRequestTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionConfigurationRequestRequestTypeDef,
-    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     EnvironmentResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     GetFunctionConfigurationRequestFunctionActiveWaitTypeDef,
     GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef,
     GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef,
@@ -599,33 +607,44 @@
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
     PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
+    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
+    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
+    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+    ListLayersRequestListLayersPaginateTypeDef,
+    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     ListFunctionUrlConfigsResponseTypeDef,
-    FunctionEventInvokeConfigResponseMetadataTypeDef,
+    FunctionEventInvokeConfigResponseTypeDef,
     FunctionEventInvokeConfigTypeDef,
     PutFunctionEventInvokeConfigRequestRequestTypeDef,
     UpdateFunctionEventInvokeConfigRequestRequestTypeDef,
-    EventSourceMappingConfigurationResponseMetadataTypeDef,
+    EventSourceMappingConfigurationResponseTypeDef,
     EventSourceMappingConfigurationTypeDef,
     CreateEventSourceMappingRequestRequestTypeDef,
     UpdateEventSourceMappingRequestRequestTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     ListLayersResponseTypeDef,
-    FunctionConfigurationResponseMetadataTypeDef,
+    FunctionConfigurationResponseTypeDef,
     FunctionConfigurationTypeDef,
     ListFunctionEventInvokeConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
     GetFunctionResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__init__.py` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__init__.pyi` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/__main__.py` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lambda 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Lambda 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda\nOther"
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

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/client.py` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,35 +44,35 @@
     ListLayerVersionsPaginator,
     ListProvisionedConcurrencyConfigsPaginator,
     ListVersionsByFunctionPaginator,
 )
 from .type_defs import (
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
-    AliasConfigurationResponseMetadataTypeDef,
+    AliasConfigurationResponseTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesTypeDef,
-    ConcurrencyResponseMetadataTypeDef,
+    ConcurrencyResponseTypeDef,
     CorsTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
-    EventSourceMappingConfigurationResponseMetadataTypeDef,
+    EventSourceMappingConfigurationResponseTypeDef,
     FileSystemConfigTypeDef,
     FilterCriteriaTypeDef,
     FunctionCodeTypeDef,
-    FunctionConfigurationResponseMetadataTypeDef,
-    FunctionEventInvokeConfigResponseMetadataTypeDef,
+    FunctionConfigurationResponseTypeDef,
+    FunctionEventInvokeConfigResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     GetLayerVersionPolicyResponseTypeDef,
@@ -258,15 +258,15 @@
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
         RoutingConfig: AliasRoutingConfigurationTypeDef = ...
-    ) -> AliasConfigurationResponseMetadataTypeDef:
+    ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_ for a Lambda function version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_alias)
         """
@@ -307,15 +307,15 @@
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
-    ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
+    ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Creates a mapping between an event source and an Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_event_source_mapping)
         """
 
@@ -341,15 +341,15 @@
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
         ImageConfig: ImageConfigTypeDef = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_function)
         """
 
@@ -385,15 +385,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.delete_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#delete_code_signing_config)
         """
 
     def delete_event_source_mapping(
         self, *, UUID: str
-    ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
+    ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Deletes an [event source
         mapping](https://docs.aws.amazon.com/lambda/latest/dg/intro-invocation-
         modes.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.delete_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#delete_event_source_mapping)
@@ -489,17 +489,15 @@
         [limits](https://docs.aws.amazon.com/lambda/latest/dg/limits.html)_ and usage in
         an Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_account_settings)
         """
 
-    def get_alias(
-        self, *, FunctionName: str, Name: str
-    ) -> AliasConfigurationResponseMetadataTypeDef:
+    def get_alias(self, *, FunctionName: str, Name: str) -> AliasConfigurationResponseTypeDef:
         """
         Returns details about a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_alias)
@@ -513,15 +511,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_code_signing_config)
         """
 
     def get_event_source_mapping(
         self, *, UUID: str
-    ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
+    ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Returns details about an event source mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_event_source_mapping)
         """
 
@@ -554,25 +552,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_function_concurrency)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_function_concurrency)
         """
 
     def get_function_configuration(
         self, *, FunctionName: str, Qualifier: str = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Returns the version-specific settings of a Lambda function or version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_function_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_function_configuration)
         """
 
     def get_function_event_invoke_config(
         self, *, FunctionName: str, Qualifier: str = ...
-    ) -> FunctionEventInvokeConfigResponseMetadataTypeDef:
+    ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Retrieves the configuration for asynchronous invocation for a function, version,
         or alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_function_event_invoke_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_function_event_invoke_config)
         """
@@ -871,15 +869,15 @@
     def publish_version(
         self,
         *,
         FunctionName: str,
         CodeSha256: str = ...,
         Description: str = ...,
         RevisionId: str = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a [version](https://docs.aws.amazon.com/lambda/latest/dg/versioning-
         aliases.html)_ from the current code and configuration of a function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.publish_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#publish_version)
         """
@@ -892,15 +890,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.put_function_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#put_function_code_signing_config)
         """
 
     def put_function_concurrency(
         self, *, FunctionName: str, ReservedConcurrentExecutions: int
-    ) -> ConcurrencyResponseMetadataTypeDef:
+    ) -> ConcurrencyResponseTypeDef:
         """
         Sets the maximum number of simultaneous executions for a function, and reserves
         capacity for that concurrency level.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.put_function_concurrency)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#put_function_concurrency)
         """
@@ -909,15 +907,15 @@
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         MaximumRetryAttempts: int = ...,
         MaximumEventAgeInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...
-    ) -> FunctionEventInvokeConfigResponseMetadataTypeDef:
+    ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Configures options for [asynchronous
         invocation](https://docs.aws.amazon.com/lambda/latest/dg/invocation-async.html)_
         on a function, version, or alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.put_function_event_invoke_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#put_function_event_invoke_config)
@@ -997,15 +995,15 @@
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
         RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
         RevisionId: str = ...
-    ) -> AliasConfigurationResponseMetadataTypeDef:
+    ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_alias)
@@ -1041,15 +1039,15 @@
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         TumblingWindowInSeconds: int = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
-    ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
+    ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Updates an event source mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_event_source_mapping)
         """
 
@@ -1062,15 +1060,15 @@
         S3Key: str = ...,
         S3ObjectVersion: str = ...,
         ImageUri: str = ...,
         Publish: bool = ...,
         DryRun: bool = ...,
         RevisionId: str = ...,
         Architectures: Sequence[ArchitectureType] = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Updates a Lambda function's code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_code)
         """
 
@@ -1091,15 +1089,15 @@
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
         ImageConfig: ImageConfigTypeDef = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_configuration)
         """
 
@@ -1107,15 +1105,15 @@
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         MaximumRetryAttempts: int = ...,
         MaximumEventAgeInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...
-    ) -> FunctionEventInvokeConfigResponseMetadataTypeDef:
+    ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Updates the configuration for asynchronous invocation for a function, version,
         or alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_event_invoke_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_event_invoke_config)
         """
```

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/client.pyi` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,35 +44,35 @@
     ListLayerVersionsPaginator,
     ListProvisionedConcurrencyConfigsPaginator,
     ListVersionsByFunctionPaginator,
 )
 from .type_defs import (
     AddLayerVersionPermissionResponseTypeDef,
     AddPermissionResponseTypeDef,
-    AliasConfigurationResponseMetadataTypeDef,
+    AliasConfigurationResponseTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
     CodeSigningPoliciesTypeDef,
-    ConcurrencyResponseMetadataTypeDef,
+    ConcurrencyResponseTypeDef,
     CorsTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     DeadLetterConfigTypeDef,
     DestinationConfigTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     EmptyResponseMetadataTypeDef,
     EnvironmentTypeDef,
     EphemeralStorageTypeDef,
-    EventSourceMappingConfigurationResponseMetadataTypeDef,
+    EventSourceMappingConfigurationResponseTypeDef,
     FileSystemConfigTypeDef,
     FilterCriteriaTypeDef,
     FunctionCodeTypeDef,
-    FunctionConfigurationResponseMetadataTypeDef,
-    FunctionEventInvokeConfigResponseMetadataTypeDef,
+    FunctionConfigurationResponseTypeDef,
+    FunctionEventInvokeConfigResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyResponseTypeDef,
     GetFunctionResponseTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     GetLayerVersionPolicyResponseTypeDef,
@@ -249,15 +249,15 @@
         self,
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str,
         Description: str = ...,
         RoutingConfig: AliasRoutingConfigurationTypeDef = ...
-    ) -> AliasConfigurationResponseMetadataTypeDef:
+    ) -> AliasConfigurationResponseTypeDef:
         """
         Creates an [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_ for a Lambda function version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_alias)
         """
@@ -296,15 +296,15 @@
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         SelfManagedEventSource: SelfManagedEventSourceTypeDef = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         AmazonManagedKafkaEventSourceConfig: AmazonManagedKafkaEventSourceConfigTypeDef = ...,
         SelfManagedKafkaEventSourceConfig: SelfManagedKafkaEventSourceConfigTypeDef = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
-    ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
+    ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Creates a mapping between an event source and an Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_event_source_mapping)
         """
     def create_function(
@@ -329,15 +329,15 @@
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
         ImageConfig: ImageConfigTypeDef = ...,
         CodeSigningConfigArn: str = ...,
         Architectures: Sequence[ArchitectureType] = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.create_function)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#create_function)
         """
     def create_function_url_config(
@@ -369,15 +369,15 @@
         Deletes the code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.delete_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#delete_code_signing_config)
         """
     def delete_event_source_mapping(
         self, *, UUID: str
-    ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
+    ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Deletes an [event source
         mapping](https://docs.aws.amazon.com/lambda/latest/dg/intro-invocation-
         modes.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.delete_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#delete_event_source_mapping)
@@ -463,17 +463,15 @@
         Retrieves details about your account's
         [limits](https://docs.aws.amazon.com/lambda/latest/dg/limits.html)_ and usage in
         an Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_account_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_account_settings)
         """
-    def get_alias(
-        self, *, FunctionName: str, Name: str
-    ) -> AliasConfigurationResponseMetadataTypeDef:
+    def get_alias(self, *, FunctionName: str, Name: str) -> AliasConfigurationResponseTypeDef:
         """
         Returns details about a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_alias)
@@ -485,15 +483,15 @@
         Returns information about the specified code signing configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_code_signing_config)
         """
     def get_event_source_mapping(
         self, *, UUID: str
-    ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
+    ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Returns details about an event source mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_event_source_mapping)
         """
     def get_function(
@@ -522,24 +520,24 @@
         Returns details about the reserved concurrency configuration for a function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_function_concurrency)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_function_concurrency)
         """
     def get_function_configuration(
         self, *, FunctionName: str, Qualifier: str = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Returns the version-specific settings of a Lambda function or version.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_function_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_function_configuration)
         """
     def get_function_event_invoke_config(
         self, *, FunctionName: str, Qualifier: str = ...
-    ) -> FunctionEventInvokeConfigResponseMetadataTypeDef:
+    ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Retrieves the configuration for asynchronous invocation for a function, version,
         or alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.get_function_event_invoke_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#get_function_event_invoke_config)
         """
@@ -814,15 +812,15 @@
     def publish_version(
         self,
         *,
         FunctionName: str,
         CodeSha256: str = ...,
         Description: str = ...,
         RevisionId: str = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Creates a [version](https://docs.aws.amazon.com/lambda/latest/dg/versioning-
         aliases.html)_ from the current code and configuration of a function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.publish_version)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#publish_version)
         """
@@ -833,15 +831,15 @@
         Update the code signing configuration for the function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.put_function_code_signing_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#put_function_code_signing_config)
         """
     def put_function_concurrency(
         self, *, FunctionName: str, ReservedConcurrentExecutions: int
-    ) -> ConcurrencyResponseMetadataTypeDef:
+    ) -> ConcurrencyResponseTypeDef:
         """
         Sets the maximum number of simultaneous executions for a function, and reserves
         capacity for that concurrency level.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.put_function_concurrency)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#put_function_concurrency)
         """
@@ -849,15 +847,15 @@
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         MaximumRetryAttempts: int = ...,
         MaximumEventAgeInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...
-    ) -> FunctionEventInvokeConfigResponseMetadataTypeDef:
+    ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Configures options for [asynchronous
         invocation](https://docs.aws.amazon.com/lambda/latest/dg/invocation-async.html)_
         on a function, version, or alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.put_function_event_invoke_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#put_function_event_invoke_config)
@@ -930,15 +928,15 @@
         *,
         FunctionName: str,
         Name: str,
         FunctionVersion: str = ...,
         Description: str = ...,
         RoutingConfig: AliasRoutingConfigurationTypeDef = ...,
         RevisionId: str = ...
-    ) -> AliasConfigurationResponseMetadataTypeDef:
+    ) -> AliasConfigurationResponseTypeDef:
         """
         Updates the configuration of a Lambda function
         [alias](https://docs.aws.amazon.com/lambda/latest/dg/configuration-
         aliases.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_alias)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_alias)
@@ -972,15 +970,15 @@
         MaximumRetryAttempts: int = ...,
         ParallelizationFactor: int = ...,
         SourceAccessConfigurations: Sequence[SourceAccessConfigurationTypeDef] = ...,
         TumblingWindowInSeconds: int = ...,
         FunctionResponseTypes: Sequence[Literal["ReportBatchItemFailures"]] = ...,
         ScalingConfig: ScalingConfigTypeDef = ...,
         DocumentDBEventSourceConfig: DocumentDBEventSourceConfigTypeDef = ...
-    ) -> EventSourceMappingConfigurationResponseMetadataTypeDef:
+    ) -> EventSourceMappingConfigurationResponseTypeDef:
         """
         Updates an event source mapping.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_event_source_mapping)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_event_source_mapping)
         """
     def update_function_code(
@@ -992,15 +990,15 @@
         S3Key: str = ...,
         S3ObjectVersion: str = ...,
         ImageUri: str = ...,
         Publish: bool = ...,
         DryRun: bool = ...,
         RevisionId: str = ...,
         Architectures: Sequence[ArchitectureType] = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Updates a Lambda function's code.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_code)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_code)
         """
     def update_function_configuration(
@@ -1020,30 +1018,30 @@
         TracingConfig: TracingConfigTypeDef = ...,
         RevisionId: str = ...,
         Layers: Sequence[str] = ...,
         FileSystemConfigs: Sequence[FileSystemConfigTypeDef] = ...,
         ImageConfig: ImageConfigTypeDef = ...,
         EphemeralStorage: EphemeralStorageTypeDef = ...,
         SnapStart: SnapStartTypeDef = ...
-    ) -> FunctionConfigurationResponseMetadataTypeDef:
+    ) -> FunctionConfigurationResponseTypeDef:
         """
         Modify the version-specific settings of a Lambda function.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_configuration)
         """
     def update_function_event_invoke_config(
         self,
         *,
         FunctionName: str,
         Qualifier: str = ...,
         MaximumRetryAttempts: int = ...,
         MaximumEventAgeInSeconds: int = ...,
         DestinationConfig: DestinationConfigTypeDef = ...
-    ) -> FunctionEventInvokeConfigResponseMetadataTypeDef:
+    ) -> FunctionEventInvokeConfigResponseTypeDef:
         """
         Updates the configuration for asynchronous invocation for a function, version,
         or alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Client.update_function_event_invoke_config)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/client/#update_function_event_invoke_config)
         """
```

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/literals.py` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/literals.pyi` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/paginator.py` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,30 +98,30 @@
     """
 
     def paginate(
         self,
         *,
         FunctionName: str,
         FunctionVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listaliasespaginator)
         """
 
 
 class ListCodeSigningConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListCodeSigningConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listcodesigningconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCodeSigningConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListCodeSigningConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listcodesigningconfigspaginator)
         """
 
 
@@ -132,45 +132,45 @@
     """
 
     def paginate(
         self,
         *,
         EventSourceArn: str = ...,
         FunctionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventSourceMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListEventSourceMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listeventsourcemappingspaginator)
         """
 
 
 class ListFunctionEventInvokeConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionEventInvokeConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctioneventinvokeconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionEventInvokeConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionEventInvokeConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctioneventinvokeconfigspaginator)
         """
 
 
 class ListFunctionUrlConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionUrlConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionurlconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionUrlConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionUrlConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionurlconfigspaginator)
         """
 
 
@@ -181,30 +181,30 @@
     """
 
     def paginate(
         self,
         *,
         MasterRegion: str = ...,
         FunctionVersion: Literal["ALL"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionspaginator)
         """
 
 
 class ListFunctionsByCodeSigningConfigPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionsbycodesigningconfigpaginator)
     """
 
     def paginate(
-        self, *, CodeSigningConfigArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CodeSigningConfigArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionsByCodeSigningConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionsbycodesigningconfigpaginator)
         """
 
 
@@ -216,15 +216,15 @@
 
     def paginate(
         self,
         *,
         LayerName: str,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLayerVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayerVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerversionspaginator)
         """
 
 
@@ -235,43 +235,43 @@
     """
 
     def paginate(
         self,
         *,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLayersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerspaginator)
         """
 
 
 class ListProvisionedConcurrencyConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listprovisionedconcurrencyconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisionedConcurrencyConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listprovisionedconcurrencyconfigspaginator)
         """
 
 
 class ListVersionsByFunctionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListVersionsByFunction)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listversionsbyfunctionpaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVersionsByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListVersionsByFunction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listversionsbyfunctionpaginator)
         """
```

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/paginator.pyi` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -94,29 +94,29 @@
     """
 
     def paginate(
         self,
         *,
         FunctionName: str,
         FunctionVersion: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listaliasespaginator)
         """
 
 class ListCodeSigningConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListCodeSigningConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listcodesigningconfigspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCodeSigningConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListCodeSigningConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listcodesigningconfigspaginator)
         """
 
 class ListEventSourceMappingsPaginator(Paginator):
@@ -126,43 +126,43 @@
     """
 
     def paginate(
         self,
         *,
         EventSourceArn: str = ...,
         FunctionName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEventSourceMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListEventSourceMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listeventsourcemappingspaginator)
         """
 
 class ListFunctionEventInvokeConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionEventInvokeConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctioneventinvokeconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionEventInvokeConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionEventInvokeConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctioneventinvokeconfigspaginator)
         """
 
 class ListFunctionUrlConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionUrlConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionurlconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionUrlConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionUrlConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionurlconfigspaginator)
         """
 
 class ListFunctionsPaginator(Paginator):
@@ -172,29 +172,29 @@
     """
 
     def paginate(
         self,
         *,
         MasterRegion: str = ...,
         FunctionVersion: Literal["ALL"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionspaginator)
         """
 
 class ListFunctionsByCodeSigningConfigPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionsbycodesigningconfigpaginator)
     """
 
     def paginate(
-        self, *, CodeSigningConfigArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CodeSigningConfigArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFunctionsByCodeSigningConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListFunctionsByCodeSigningConfig.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listfunctionsbycodesigningconfigpaginator)
         """
 
 class ListLayerVersionsPaginator(Paginator):
@@ -205,15 +205,15 @@
 
     def paginate(
         self,
         *,
         LayerName: str,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLayerVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayerVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerversionspaginator)
         """
 
 class ListLayersPaginator(Paginator):
@@ -223,41 +223,41 @@
     """
 
     def paginate(
         self,
         *,
         CompatibleRuntime: RuntimeType = ...,
         CompatibleArchitecture: ArchitectureType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListLayersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListLayers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listlayerspaginator)
         """
 
 class ListProvisionedConcurrencyConfigsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listprovisionedconcurrencyconfigspaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisionedConcurrencyConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListProvisionedConcurrencyConfigs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listprovisionedconcurrencyconfigspaginator)
         """
 
 class ListVersionsByFunctionPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListVersionsByFunction)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listversionsbyfunctionpaginator)
     """
 
     def paginate(
-        self, *, FunctionName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FunctionName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVersionsByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda.Paginator.ListVersionsByFunction.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/paginators/#listversionsbyfunctionpaginator)
         """
```

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/type_defs.py` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,26 +52,22 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountLimitTypeDef",
     "AccountUsageTypeDef",
     "AddLayerVersionPermissionRequestRequestTypeDef",
-    "AddLayerVersionPermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AddPermissionRequestRequestTypeDef",
-    "AddPermissionResponseTypeDef",
     "AliasRoutingConfigurationOutputTypeDef",
     "AliasRoutingConfigurationTypeDef",
     "AllowedPublishersOutputTypeDef",
     "AllowedPublishersTypeDef",
-    "AmazonManagedKafkaEventSourceConfigOutputTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
-    "CodeSigningPoliciesOutputTypeDef",
     "CodeSigningPoliciesTypeDef",
-    "ConcurrencyResponseMetadataTypeDef",
     "ConcurrencyTypeDef",
     "CorsOutputTypeDef",
     "CorsTypeDef",
     "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
@@ -81,138 +77,118 @@
     "EphemeralStorageTypeDef",
     "FileSystemConfigTypeDef",
     "FunctionCodeTypeDef",
     "ImageConfigTypeDef",
     "SnapStartTypeDef",
     "TracingConfigTypeDef",
     "VpcConfigTypeDef",
-    "DeadLetterConfigOutputTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCodeSigningConfigRequestRequestTypeDef",
     "DeleteEventSourceMappingRequestRequestTypeDef",
     "DeleteFunctionCodeSigningConfigRequestRequestTypeDef",
     "DeleteFunctionConcurrencyRequestRequestTypeDef",
     "DeleteFunctionEventInvokeConfigRequestRequestTypeDef",
     "DeleteFunctionRequestRequestTypeDef",
     "DeleteFunctionUrlConfigRequestRequestTypeDef",
     "DeleteLayerVersionRequestRequestTypeDef",
     "DeleteProvisionedConcurrencyConfigRequestRequestTypeDef",
-    "OnFailureOutputTypeDef",
-    "OnSuccessOutputTypeDef",
     "OnFailureTypeDef",
     "OnSuccessTypeDef",
-    "DocumentDBEventSourceConfigOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnvironmentErrorTypeDef",
-    "EphemeralStorageOutputTypeDef",
-    "ScalingConfigOutputTypeDef",
     "SelfManagedEventSourceOutputTypeDef",
-    "SelfManagedKafkaEventSourceConfigOutputTypeDef",
-    "SourceAccessConfigurationOutputTypeDef",
-    "FileSystemConfigOutputTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "FunctionCodeLocationTypeDef",
     "LayerTypeDef",
     "SnapStartResponseTypeDef",
     "TracingConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
     "GetAliasRequestRequestTypeDef",
     "GetCodeSigningConfigRequestRequestTypeDef",
     "GetEventSourceMappingRequestRequestTypeDef",
     "GetFunctionCodeSigningConfigRequestRequestTypeDef",
-    "GetFunctionCodeSigningConfigResponseTypeDef",
     "GetFunctionConcurrencyRequestRequestTypeDef",
-    "GetFunctionConcurrencyResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetFunctionConfigurationRequestRequestTypeDef",
     "GetFunctionEventInvokeConfigRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetFunctionUrlConfigRequestRequestTypeDef",
     "GetLayerVersionByArnRequestRequestTypeDef",
     "GetLayerVersionPolicyRequestRequestTypeDef",
-    "GetLayerVersionPolicyResponseTypeDef",
     "GetLayerVersionRequestRequestTypeDef",
     "LayerVersionContentOutputTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
-    "GetProvisionedConcurrencyConfigResponseTypeDef",
     "GetRuntimeManagementConfigRequestRequestTypeDef",
-    "GetRuntimeManagementConfigResponseTypeDef",
     "ImageConfigErrorTypeDef",
     "ImageConfigOutputTypeDef",
     "InvocationRequestRequestTypeDef",
-    "InvocationResponseTypeDef",
     "InvokeAsyncRequestRequestTypeDef",
-    "InvokeAsyncResponseTypeDef",
     "InvokeResponseStreamUpdateTypeDef",
     "InvokeWithResponseStreamCompleteEventTypeDef",
     "InvokeWithResponseStreamRequestRequestTypeDef",
     "LayerVersionContentInputTypeDef",
     "LayerVersionsListItemTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
-    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
     "ListCodeSigningConfigsRequestRequestTypeDef",
-    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
     "ListEventSourceMappingsRequestRequestTypeDef",
-    "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
     "ListFunctionEventInvokeConfigsRequestRequestTypeDef",
-    "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
     "ListFunctionUrlConfigsRequestRequestTypeDef",
-    "ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
     "ListFunctionsByCodeSigningConfigRequestRequestTypeDef",
-    "ListFunctionsByCodeSigningConfigResponseTypeDef",
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListFunctionsRequestRequestTypeDef",
-    "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
     "ListLayerVersionsRequestRequestTypeDef",
-    "ListLayersRequestListLayersPaginateTypeDef",
     "ListLayersRequestRequestTypeDef",
-    "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsRequestRequestTypeDef",
     "ProvisionedConcurrencyConfigListItemTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
-    "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListVersionsByFunctionRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishVersionRequestRequestTypeDef",
     "PutFunctionCodeSigningConfigRequestRequestTypeDef",
-    "PutFunctionCodeSigningConfigResponseTypeDef",
     "PutFunctionConcurrencyRequestRequestTypeDef",
     "PutProvisionedConcurrencyConfigRequestRequestTypeDef",
-    "PutProvisionedConcurrencyConfigResponseTypeDef",
     "PutRuntimeManagementConfigRequestRequestTypeDef",
-    "PutRuntimeManagementConfigResponseTypeDef",
     "RemoveLayerVersionPermissionRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RuntimeVersionErrorTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFunctionCodeRequestRequestTypeDef",
+    "AddLayerVersionPermissionResponseTypeDef",
+    "AddPermissionResponseTypeDef",
+    "ConcurrencyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetAccountSettingsResponseTypeDef",
-    "AliasConfigurationResponseMetadataTypeDef",
+    "GetFunctionCodeSigningConfigResponseTypeDef",
+    "GetFunctionConcurrencyResponseTypeDef",
+    "GetLayerVersionPolicyResponseTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetProvisionedConcurrencyConfigResponseTypeDef",
+    "GetRuntimeManagementConfigResponseTypeDef",
+    "InvocationResponseTypeDef",
+    "InvokeAsyncResponseTypeDef",
+    "ListFunctionsByCodeSigningConfigResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "PutFunctionCodeSigningConfigResponseTypeDef",
+    "PutProvisionedConcurrencyConfigResponseTypeDef",
+    "PutRuntimeManagementConfigResponseTypeDef",
+    "AliasConfigurationResponseTypeDef",
     "AliasConfigurationTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "CodeSigningConfigTypeDef",
     "CreateCodeSigningConfigRequestRequestTypeDef",
     "UpdateCodeSigningConfigRequestRequestTypeDef",
     "CreateFunctionUrlConfigResponseTypeDef",
     "FunctionUrlConfigTypeDef",
     "GetFunctionUrlConfigResponseTypeDef",
     "UpdateFunctionUrlConfigResponseTypeDef",
     "CreateFunctionUrlConfigRequestRequestTypeDef",
     "UpdateFunctionUrlConfigRequestRequestTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionConfigurationRequestRequestTypeDef",
-    "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "EnvironmentResponseTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "GetFunctionConfigurationRequestFunctionActiveWaitTypeDef",
     "GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef",
     "GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef",
@@ -222,33 +198,44 @@
     "GetLayerVersionResponseTypeDef",
     "PublishLayerVersionResponseTypeDef",
     "ImageConfigResponseTypeDef",
     "InvokeWithResponseStreamResponseEventTypeDef",
     "PublishLayerVersionRequestRequestTypeDef",
     "LayersListItemTypeDef",
     "ListLayerVersionsResponseTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
+    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
+    "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    "ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
+    "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    "ListLayersRequestListLayersPaginateTypeDef",
+    "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     "RuntimeVersionConfigTypeDef",
     "ListAliasesResponseTypeDef",
     "CreateCodeSigningConfigResponseTypeDef",
     "GetCodeSigningConfigResponseTypeDef",
     "ListCodeSigningConfigsResponseTypeDef",
     "UpdateCodeSigningConfigResponseTypeDef",
     "ListFunctionUrlConfigsResponseTypeDef",
-    "FunctionEventInvokeConfigResponseMetadataTypeDef",
+    "FunctionEventInvokeConfigResponseTypeDef",
     "FunctionEventInvokeConfigTypeDef",
     "PutFunctionEventInvokeConfigRequestRequestTypeDef",
     "UpdateFunctionEventInvokeConfigRequestRequestTypeDef",
-    "EventSourceMappingConfigurationResponseMetadataTypeDef",
+    "EventSourceMappingConfigurationResponseTypeDef",
     "EventSourceMappingConfigurationTypeDef",
     "CreateEventSourceMappingRequestRequestTypeDef",
     "UpdateEventSourceMappingRequestRequestTypeDef",
     "InvokeWithResponseStreamResponseTypeDef",
     "ListLayersResponseTypeDef",
-    "FunctionConfigurationResponseMetadataTypeDef",
+    "FunctionConfigurationResponseTypeDef",
     "FunctionConfigurationTypeDef",
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     "ListEventSourceMappingsResponseTypeDef",
     "GetFunctionResponseTypeDef",
     "ListFunctionsResponseTypeDef",
     "ListVersionsByFunctionResponseTypeDef",
 )
@@ -297,20 +284,22 @@
 class AddLayerVersionPermissionRequestRequestTypeDef(
     _RequiredAddLayerVersionPermissionRequestRequestTypeDef,
     _OptionalAddLayerVersionPermissionRequestRequestTypeDef,
 ):
     pass
 
 
-AddLayerVersionPermissionResponseTypeDef = TypedDict(
-    "AddLayerVersionPermissionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Statement": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAddPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAddPermissionRequestRequestTypeDef",
     {
         "FunctionName": str,
@@ -336,22 +325,14 @@
 
 class AddPermissionRequestRequestTypeDef(
     _RequiredAddPermissionRequestRequestTypeDef, _OptionalAddPermissionRequestRequestTypeDef
 ):
     pass
 
 
-AddPermissionResponseTypeDef = TypedDict(
-    "AddPermissionResponseTypeDef",
-    {
-        "Statement": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AliasRoutingConfigurationOutputTypeDef = TypedDict(
     "AliasRoutingConfigurationOutputTypeDef",
     {
         "AdditionalVersionWeights": Dict[str, float],
     },
     total=False,
 )
@@ -374,54 +355,30 @@
 AllowedPublishersTypeDef = TypedDict(
     "AllowedPublishersTypeDef",
     {
         "SigningProfileVersionArns": Sequence[str],
     },
 )
 
-AmazonManagedKafkaEventSourceConfigOutputTypeDef = TypedDict(
-    "AmazonManagedKafkaEventSourceConfigOutputTypeDef",
-    {
-        "ConsumerGroupId": str,
-    },
-    total=False,
-)
-
 AmazonManagedKafkaEventSourceConfigTypeDef = TypedDict(
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     {
         "ConsumerGroupId": str,
     },
     total=False,
 )
 
-CodeSigningPoliciesOutputTypeDef = TypedDict(
-    "CodeSigningPoliciesOutputTypeDef",
-    {
-        "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
-    },
-    total=False,
-)
-
 CodeSigningPoliciesTypeDef = TypedDict(
     "CodeSigningPoliciesTypeDef",
     {
         "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
     },
     total=False,
 )
 
-ConcurrencyResponseMetadataTypeDef = TypedDict(
-    "ConcurrencyResponseMetadataTypeDef",
-    {
-        "ReservedConcurrentExecutions": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConcurrencyTypeDef = TypedDict(
     "ConcurrencyTypeDef",
     {
         "ReservedConcurrentExecutions": int,
     },
     total=False,
 )
@@ -569,22 +526,14 @@
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-DeadLetterConfigOutputTypeDef = TypedDict(
-    "DeadLetterConfigOutputTypeDef",
-    {
-        "TargetArn": str,
-    },
-    total=False,
-)
-
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
     },
 )
@@ -694,30 +643,14 @@
     "DeleteProvisionedConcurrencyConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Qualifier": str,
     },
 )
 
-OnFailureOutputTypeDef = TypedDict(
-    "OnFailureOutputTypeDef",
-    {
-        "Destination": str,
-    },
-    total=False,
-)
-
-OnSuccessOutputTypeDef = TypedDict(
-    "OnSuccessOutputTypeDef",
-    {
-        "Destination": str,
-    },
-    total=False,
-)
-
 OnFailureTypeDef = TypedDict(
     "OnFailureTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
@@ -726,96 +659,31 @@
     "OnSuccessTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
-DocumentDBEventSourceConfigOutputTypeDef = TypedDict(
-    "DocumentDBEventSourceConfigOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "CollectionName": str,
-        "FullDocument": FullDocumentType,
-    },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentErrorTypeDef = TypedDict(
     "EnvironmentErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-EphemeralStorageOutputTypeDef = TypedDict(
-    "EphemeralStorageOutputTypeDef",
-    {
-        "Size": int,
-    },
-)
-
-ScalingConfigOutputTypeDef = TypedDict(
-    "ScalingConfigOutputTypeDef",
-    {
-        "MaximumConcurrency": int,
-    },
-    total=False,
-)
-
 SelfManagedEventSourceOutputTypeDef = TypedDict(
     "SelfManagedEventSourceOutputTypeDef",
     {
         "Endpoints": Dict[Literal["KAFKA_BOOTSTRAP_SERVERS"], List[str]],
     },
     total=False,
 )
 
-SelfManagedKafkaEventSourceConfigOutputTypeDef = TypedDict(
-    "SelfManagedKafkaEventSourceConfigOutputTypeDef",
-    {
-        "ConsumerGroupId": str,
-    },
-    total=False,
-)
-
-SourceAccessConfigurationOutputTypeDef = TypedDict(
-    "SourceAccessConfigurationOutputTypeDef",
-    {
-        "Type": SourceAccessTypeType,
-        "URI": str,
-    },
-    total=False,
-)
-
-FileSystemConfigOutputTypeDef = TypedDict(
-    "FileSystemConfigOutputTypeDef",
-    {
-        "Arn": str,
-        "LocalMountPath": str,
-    },
-)
-
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "Pattern": str,
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Pattern": str,
     },
     total=False,
 )
@@ -894,38 +762,21 @@
 GetFunctionCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "GetFunctionCodeSigningConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 
-GetFunctionCodeSigningConfigResponseTypeDef = TypedDict(
-    "GetFunctionCodeSigningConfigResponseTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-        "FunctionName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFunctionConcurrencyRequestRequestTypeDef = TypedDict(
     "GetFunctionConcurrencyRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 
-GetFunctionConcurrencyResponseTypeDef = TypedDict(
-    "GetFunctionConcurrencyResponseTypeDef",
-    {
-        "ReservedConcurrentExecutions": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1029,23 +880,14 @@
     "GetLayerVersionPolicyRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
     },
 )
 
-GetLayerVersionPolicyResponseTypeDef = TypedDict(
-    "GetLayerVersionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLayerVersionRequestRequestTypeDef = TypedDict(
     "GetLayerVersionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
     },
 )
@@ -1079,44 +921,22 @@
 
 class GetPolicyRequestRequestTypeDef(
     _RequiredGetPolicyRequestRequestTypeDef, _OptionalGetPolicyRequestRequestTypeDef
 ):
     pass
 
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProvisionedConcurrencyConfigRequestRequestTypeDef = TypedDict(
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Qualifier": str,
     },
 )
 
-GetProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
-    "GetProvisionedConcurrencyConfigResponseTypeDef",
-    {
-        "RequestedProvisionedConcurrentExecutions": int,
-        "AvailableProvisionedConcurrentExecutions": int,
-        "AllocatedProvisionedConcurrentExecutions": int,
-        "Status": ProvisionedConcurrencyStatusEnumType,
-        "StatusReason": str,
-        "LastModified": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
     "_RequiredGetRuntimeManagementConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalGetRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
@@ -1131,24 +951,14 @@
 class GetRuntimeManagementConfigRequestRequestTypeDef(
     _RequiredGetRuntimeManagementConfigRequestRequestTypeDef,
     _OptionalGetRuntimeManagementConfigRequestRequestTypeDef,
 ):
     pass
 
 
-GetRuntimeManagementConfigResponseTypeDef = TypedDict(
-    "GetRuntimeManagementConfigResponseTypeDef",
-    {
-        "UpdateRuntimeOn": UpdateRuntimeOnType,
-        "RuntimeVersionArn": str,
-        "FunctionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageConfigErrorTypeDef = TypedDict(
     "ImageConfigErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -1185,42 +995,22 @@
 
 class InvocationRequestRequestTypeDef(
     _RequiredInvocationRequestRequestTypeDef, _OptionalInvocationRequestRequestTypeDef
 ):
     pass
 
 
-InvocationResponseTypeDef = TypedDict(
-    "InvocationResponseTypeDef",
-    {
-        "StatusCode": int,
-        "FunctionError": str,
-        "LogResult": str,
-        "Payload": StreamingBody,
-        "ExecutedVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InvokeAsyncRequestRequestTypeDef = TypedDict(
     "InvokeAsyncRequestRequestTypeDef",
     {
         "FunctionName": str,
         "InvokeArgs": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-InvokeAsyncResponseTypeDef = TypedDict(
-    "InvokeAsyncResponseTypeDef",
-    {
-        "Status": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InvokeResponseStreamUpdateTypeDef = TypedDict(
     "InvokeResponseStreamUpdateTypeDef",
     {
         "Payload": bytes,
     },
     total=False,
 )
@@ -1282,37 +1072,24 @@
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
     },
     total=False,
 )
 
-_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "FunctionVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListAliasesRequestListAliasesPaginateTypeDef(
-    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
-    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListAliasesRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListAliasesRequestRequestTypeDef = TypedDict(
@@ -1328,74 +1105,34 @@
 
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
 
-ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef = TypedDict(
-    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCodeSigningConfigsRequestRequestTypeDef = TypedDict(
     "ListCodeSigningConfigsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef = TypedDict(
-    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
-    {
-        "EventSourceArn": str,
-        "FunctionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEventSourceMappingsRequestRequestTypeDef = TypedDict(
     "ListEventSourceMappingsRequestRequestTypeDef",
     {
         "EventSourceArn": str,
         "FunctionName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(
-    _RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-    _OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListFunctionEventInvokeConfigsRequestRequestTypeDef = TypedDict(
@@ -1411,36 +1148,14 @@
 class ListFunctionEventInvokeConfigsRequestRequestTypeDef(
     _RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef,
     _OptionalListFunctionEventInvokeConfigsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(
-    _RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-    _OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFunctionUrlConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionUrlConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListFunctionUrlConfigsRequestRequestTypeDef = TypedDict(
@@ -1456,36 +1171,14 @@
 class ListFunctionUrlConfigsRequestRequestTypeDef(
     _RequiredListFunctionUrlConfigsRequestRequestTypeDef,
     _OptionalListFunctionUrlConfigsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-    },
-)
-_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(
-    _RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-    _OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef",
     {
         "CodeSigningConfigArn": str,
     },
 )
 _OptionalListFunctionsByCodeSigningConfigRequestRequestTypeDef = TypedDict(
@@ -1501,68 +1194,25 @@
 class ListFunctionsByCodeSigningConfigRequestRequestTypeDef(
     _RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef,
     _OptionalListFunctionsByCodeSigningConfigRequestRequestTypeDef,
 ):
     pass
 
 
-ListFunctionsByCodeSigningConfigResponseTypeDef = TypedDict(
-    "ListFunctionsByCodeSigningConfigResponseTypeDef",
-    {
-        "NextMarker": str,
-        "FunctionArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "MasterRegion": str,
-        "FunctionVersion": Literal["ALL"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFunctionsRequestRequestTypeDef = TypedDict(
     "ListFunctionsRequestRequestTypeDef",
     {
         "MasterRegion": str,
         "FunctionVersion": Literal["ALL"],
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    {
-        "LayerName": str,
-    },
-)
-_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    {
-        "CompatibleRuntime": RuntimeType,
-        "CompatibleArchitecture": ArchitectureType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(
-    _RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-    _OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListLayerVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLayerVersionsRequestRequestTypeDef",
     {
         "LayerName": str,
     },
 )
 _OptionalListLayerVersionsRequestRequestTypeDef = TypedDict(
@@ -1579,57 +1229,25 @@
 
 class ListLayerVersionsRequestRequestTypeDef(
     _RequiredListLayerVersionsRequestRequestTypeDef, _OptionalListLayerVersionsRequestRequestTypeDef
 ):
     pass
 
 
-ListLayersRequestListLayersPaginateTypeDef = TypedDict(
-    "ListLayersRequestListLayersPaginateTypeDef",
-    {
-        "CompatibleRuntime": RuntimeType,
-        "CompatibleArchitecture": ArchitectureType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLayersRequestRequestTypeDef = TypedDict(
     "ListLayersRequestRequestTypeDef",
     {
         "CompatibleRuntime": RuntimeType,
         "Marker": str,
         "MaxItems": int,
         "CompatibleArchitecture": ArchitectureType,
     },
     total=False,
 )
 
-_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(
-    _RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-    _OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProvisionedConcurrencyConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListProvisionedConcurrencyConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListProvisionedConcurrencyConfigsRequestRequestTypeDef = TypedDict(
@@ -1666,44 +1284,14 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
-    "_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
-    "_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(
-    _RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
-    _OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVersionsByFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredListVersionsByFunctionRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListVersionsByFunctionRequestRequestTypeDef = TypedDict(
@@ -1719,24 +1307,14 @@
 class ListVersionsByFunctionRequestRequestTypeDef(
     _RequiredListVersionsByFunctionRequestRequestTypeDef,
     _OptionalListVersionsByFunctionRequestRequestTypeDef,
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
 _RequiredPublishVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishVersionRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalPublishVersionRequestRequestTypeDef = TypedDict(
@@ -1760,23 +1338,14 @@
     "PutFunctionCodeSigningConfigRequestRequestTypeDef",
     {
         "CodeSigningConfigArn": str,
         "FunctionName": str,
     },
 )
 
-PutFunctionCodeSigningConfigResponseTypeDef = TypedDict(
-    "PutFunctionCodeSigningConfigResponseTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-        "FunctionName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutFunctionConcurrencyRequestRequestTypeDef = TypedDict(
     "PutFunctionConcurrencyRequestRequestTypeDef",
     {
         "FunctionName": str,
         "ReservedConcurrentExecutions": int,
     },
 )
@@ -1786,27 +1355,14 @@
     {
         "FunctionName": str,
         "Qualifier": str,
         "ProvisionedConcurrentExecutions": int,
     },
 )
 
-PutProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
-    "PutProvisionedConcurrencyConfigResponseTypeDef",
-    {
-        "RequestedProvisionedConcurrentExecutions": int,
-        "AvailableProvisionedConcurrentExecutions": int,
-        "AllocatedProvisionedConcurrentExecutions": int,
-        "Status": ProvisionedConcurrencyStatusEnumType,
-        "StatusReason": str,
-        "LastModified": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuntimeManagementConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "UpdateRuntimeOn": UpdateRuntimeOnType,
     },
 )
@@ -1823,24 +1379,14 @@
 class PutRuntimeManagementConfigRequestRequestTypeDef(
     _RequiredPutRuntimeManagementConfigRequestRequestTypeDef,
     _OptionalPutRuntimeManagementConfigRequestRequestTypeDef,
 ):
     pass
 
 
-PutRuntimeManagementConfigResponseTypeDef = TypedDict(
-    "PutRuntimeManagementConfigResponseTypeDef",
-    {
-        "UpdateRuntimeOn": UpdateRuntimeOnType,
-        "FunctionArn": str,
-        "RuntimeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRemoveLayerVersionPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLayerVersionPermissionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
         "StatementId": str,
     },
@@ -1880,25 +1426,14 @@
 
 class RemovePermissionRequestRequestTypeDef(
     _RequiredRemovePermissionRequestRequestTypeDef, _OptionalRemovePermissionRequestRequestTypeDef
 ):
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
 RuntimeVersionErrorTypeDef = TypedDict(
     "RuntimeVersionErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -1946,33 +1481,192 @@
 class UpdateFunctionCodeRequestRequestTypeDef(
     _RequiredUpdateFunctionCodeRequestRequestTypeDef,
     _OptionalUpdateFunctionCodeRequestRequestTypeDef,
 ):
     pass
 
 
+AddLayerVersionPermissionResponseTypeDef = TypedDict(
+    "AddLayerVersionPermissionResponseTypeDef",
+    {
+        "Statement": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddPermissionResponseTypeDef = TypedDict(
+    "AddPermissionResponseTypeDef",
+    {
+        "Statement": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConcurrencyResponseTypeDef = TypedDict(
+    "ConcurrencyResponseTypeDef",
+    {
+        "ReservedConcurrentExecutions": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
         "AccountLimit": AccountLimitTypeDef,
         "AccountUsage": AccountUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionCodeSigningConfigResponseTypeDef = TypedDict(
+    "GetFunctionCodeSigningConfigResponseTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+        "FunctionName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionConcurrencyResponseTypeDef = TypedDict(
+    "GetFunctionConcurrencyResponseTypeDef",
+    {
+        "ReservedConcurrentExecutions": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLayerVersionPolicyResponseTypeDef = TypedDict(
+    "GetLayerVersionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
+    "GetProvisionedConcurrencyConfigResponseTypeDef",
+    {
+        "RequestedProvisionedConcurrentExecutions": int,
+        "AvailableProvisionedConcurrentExecutions": int,
+        "AllocatedProvisionedConcurrentExecutions": int,
+        "Status": ProvisionedConcurrencyStatusEnumType,
+        "StatusReason": str,
+        "LastModified": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRuntimeManagementConfigResponseTypeDef = TypedDict(
+    "GetRuntimeManagementConfigResponseTypeDef",
+    {
+        "UpdateRuntimeOn": UpdateRuntimeOnType,
+        "RuntimeVersionArn": str,
+        "FunctionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvocationResponseTypeDef = TypedDict(
+    "InvocationResponseTypeDef",
+    {
+        "StatusCode": int,
+        "FunctionError": str,
+        "LogResult": str,
+        "Payload": StreamingBody,
+        "ExecutedVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeAsyncResponseTypeDef = TypedDict(
+    "InvokeAsyncResponseTypeDef",
+    {
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFunctionsByCodeSigningConfigResponseTypeDef = TypedDict(
+    "ListFunctionsByCodeSigningConfigResponseTypeDef",
+    {
+        "NextMarker": str,
+        "FunctionArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutFunctionCodeSigningConfigResponseTypeDef = TypedDict(
+    "PutFunctionCodeSigningConfigResponseTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+        "FunctionName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
+    "PutProvisionedConcurrencyConfigResponseTypeDef",
+    {
+        "RequestedProvisionedConcurrentExecutions": int,
+        "AvailableProvisionedConcurrentExecutions": int,
+        "AllocatedProvisionedConcurrentExecutions": int,
+        "Status": ProvisionedConcurrencyStatusEnumType,
+        "StatusReason": str,
+        "LastModified": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRuntimeManagementConfigResponseTypeDef = TypedDict(
+    "PutRuntimeManagementConfigResponseTypeDef",
+    {
+        "UpdateRuntimeOn": UpdateRuntimeOnType,
+        "FunctionArn": str,
+        "RuntimeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AliasConfigurationResponseMetadataTypeDef = TypedDict(
-    "AliasConfigurationResponseMetadataTypeDef",
+AliasConfigurationResponseTypeDef = TypedDict(
+    "AliasConfigurationResponseTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
         "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
         "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AliasConfigurationTypeDef = TypedDict(
     "AliasConfigurationTypeDef",
     {
         "AliasArn": str,
@@ -2036,15 +1730,15 @@
 
 _RequiredCodeSigningConfigTypeDef = TypedDict(
     "_RequiredCodeSigningConfigTypeDef",
     {
         "CodeSigningConfigId": str,
         "CodeSigningConfigArn": str,
         "AllowedPublishers": AllowedPublishersOutputTypeDef,
-        "CodeSigningPolicies": CodeSigningPoliciesOutputTypeDef,
+        "CodeSigningPolicies": CodeSigningPoliciesTypeDef,
         "LastModified": str,
     },
 )
 _OptionalCodeSigningConfigTypeDef = TypedDict(
     "_OptionalCodeSigningConfigTypeDef",
     {
         "Description": str,
@@ -2111,15 +1805,15 @@
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFunctionUrlConfigTypeDef = TypedDict(
     "_RequiredFunctionUrlConfigTypeDef",
     {
         "FunctionUrl": str,
@@ -2151,29 +1845,29 @@
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFunctionUrlConfigResponseTypeDef = TypedDict(
     "UpdateFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
@@ -2299,23 +1993,14 @@
 class UpdateFunctionConfigurationRequestRequestTypeDef(
     _RequiredUpdateFunctionConfigurationRequestRequestTypeDef,
     _OptionalUpdateFunctionConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
-DestinationConfigOutputTypeDef = TypedDict(
-    "DestinationConfigOutputTypeDef",
-    {
-        "OnSuccess": OnSuccessOutputTypeDef,
-        "OnFailure": OnFailureOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationConfigTypeDef = TypedDict(
     "DestinationConfigTypeDef",
     {
         "OnSuccess": OnSuccessTypeDef,
         "OnFailure": OnFailureTypeDef,
     },
     total=False,
@@ -2329,15 +2014,15 @@
     },
     total=False,
 )
 
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
-        "Filters": List[FilterOutputTypeDef],
+        "Filters": List[FilterTypeDef],
     },
     total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
@@ -2492,15 +2177,15 @@
         "LayerVersionArn": str,
         "Description": str,
         "CreatedDate": str,
         "Version": int,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishLayerVersionResponseTypeDef = TypedDict(
     "PublishLayerVersionResponseTypeDef",
     {
         "Content": LayerVersionContentOutputTypeDef,
@@ -2508,15 +2193,15 @@
         "LayerVersionArn": str,
         "Description": str,
         "CreatedDate": str,
         "Version": int,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageConfigResponseTypeDef = TypedDict(
     "ImageConfigResponseTypeDef",
     {
         "ImageConfig": ImageConfigOutputTypeDef,
@@ -2571,24 +2256,219 @@
 )
 
 ListLayerVersionsResponseTypeDef = TypedDict(
     "ListLayerVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "LayerVersions": List[LayerVersionsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "FunctionVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAliasesRequestListAliasesPaginateTypeDef(
+    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
+    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
+):
+    pass
+
+
+ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef = TypedDict(
+    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef = TypedDict(
+    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
+    {
+        "EventSourceArn": str,
+        "FunctionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(
+    _RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+    _OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(
+    _RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+    _OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+    },
+)
+_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(
+    _RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+    _OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+):
+    pass
+
+
+ListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "MasterRegion": str,
+        "FunctionVersion": Literal["ALL"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    {
+        "LayerName": str,
+    },
+)
+_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    {
+        "CompatibleRuntime": RuntimeType,
+        "CompatibleArchitecture": ArchitectureType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(
+    _RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+    _OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListLayersRequestListLayersPaginateTypeDef = TypedDict(
+    "ListLayersRequestListLayersPaginateTypeDef",
+    {
+        "CompatibleRuntime": RuntimeType,
+        "CompatibleArchitecture": ArchitectureType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(
+    _RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+    _OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
+    "_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
+    "_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(
+    _RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
+    _OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
+):
+    pass
+
+
 ListProvisionedConcurrencyConfigsResponseTypeDef = TypedDict(
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     {
         "ProvisionedConcurrencyConfigs": List[ProvisionedConcurrencyConfigListItemTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuntimeVersionConfigTypeDef = TypedDict(
     "RuntimeVersionConfigTypeDef",
     {
         "RuntimeVersionArn": str,
@@ -2598,80 +2478,80 @@
 )
 
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "NextMarker": str,
         "Aliases": List[AliasConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCodeSigningConfigResponseTypeDef = TypedDict(
     "CreateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCodeSigningConfigResponseTypeDef = TypedDict(
     "GetCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCodeSigningConfigsResponseTypeDef = TypedDict(
     "ListCodeSigningConfigsResponseTypeDef",
     {
         "NextMarker": str,
         "CodeSigningConfigs": List[CodeSigningConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCodeSigningConfigResponseTypeDef = TypedDict(
     "UpdateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionUrlConfigsResponseTypeDef = TypedDict(
     "ListFunctionUrlConfigsResponseTypeDef",
     {
         "FunctionUrlConfigs": List[FunctionUrlConfigTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FunctionEventInvokeConfigResponseMetadataTypeDef = TypedDict(
-    "FunctionEventInvokeConfigResponseMetadataTypeDef",
+FunctionEventInvokeConfigResponseTypeDef = TypedDict(
+    "FunctionEventInvokeConfigResponseTypeDef",
     {
         "LastModified": datetime,
         "FunctionArn": str,
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
-        "DestinationConfig": DestinationConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DestinationConfig": DestinationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FunctionEventInvokeConfigTypeDef = TypedDict(
     "FunctionEventInvokeConfigTypeDef",
     {
         "LastModified": datetime,
         "FunctionArn": str,
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
-        "DestinationConfig": DestinationConfigOutputTypeDef,
+        "DestinationConfig": DestinationConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredPutFunctionEventInvokeConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutFunctionEventInvokeConfigRequestRequestTypeDef",
     {
@@ -2718,45 +2598,45 @@
 class UpdateFunctionEventInvokeConfigRequestRequestTypeDef(
     _RequiredUpdateFunctionEventInvokeConfigRequestRequestTypeDef,
     _OptionalUpdateFunctionEventInvokeConfigRequestRequestTypeDef,
 ):
     pass
 
 
-EventSourceMappingConfigurationResponseMetadataTypeDef = TypedDict(
-    "EventSourceMappingConfigurationResponseMetadataTypeDef",
+EventSourceMappingConfigurationResponseTypeDef = TypedDict(
+    "EventSourceMappingConfigurationResponseTypeDef",
     {
         "UUID": str,
         "StartingPosition": EventSourcePositionType,
         "StartingPositionTimestamp": datetime,
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
         "ParallelizationFactor": int,
         "EventSourceArn": str,
         "FilterCriteria": FilterCriteriaOutputTypeDef,
         "FunctionArn": str,
         "LastModified": datetime,
         "LastProcessingResult": str,
         "State": str,
         "StateTransitionReason": str,
-        "DestinationConfig": DestinationConfigOutputTypeDef,
+        "DestinationConfig": DestinationConfigTypeDef,
         "Topics": List[str],
         "Queues": List[str],
-        "SourceAccessConfigurations": List[SourceAccessConfigurationOutputTypeDef],
+        "SourceAccessConfigurations": List[SourceAccessConfigurationTypeDef],
         "SelfManagedEventSource": SelfManagedEventSourceOutputTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
-        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigOutputTypeDef,
-        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigOutputTypeDef,
-        "ScalingConfig": ScalingConfigOutputTypeDef,
-        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
+        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
+        "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSourceMappingConfigurationTypeDef = TypedDict(
     "EventSourceMappingConfigurationTypeDef",
     {
         "UUID": str,
@@ -2768,28 +2648,28 @@
         "EventSourceArn": str,
         "FilterCriteria": FilterCriteriaOutputTypeDef,
         "FunctionArn": str,
         "LastModified": datetime,
         "LastProcessingResult": str,
         "State": str,
         "StateTransitionReason": str,
-        "DestinationConfig": DestinationConfigOutputTypeDef,
+        "DestinationConfig": DestinationConfigTypeDef,
         "Topics": List[str],
         "Queues": List[str],
-        "SourceAccessConfigurations": List[SourceAccessConfigurationOutputTypeDef],
+        "SourceAccessConfigurations": List[SourceAccessConfigurationTypeDef],
         "SelfManagedEventSource": SelfManagedEventSourceOutputTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
-        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigOutputTypeDef,
-        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigOutputTypeDef,
-        "ScalingConfig": ScalingConfigOutputTypeDef,
-        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigOutputTypeDef,
+        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
+        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
+        "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventSourceMappingRequestRequestTypeDef",
     {
@@ -2872,66 +2752,66 @@
 InvokeWithResponseStreamResponseTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseTypeDef",
     {
         "StatusCode": int,
         "ExecutedVersion": str,
         "EventStream": "EventStream[InvokeWithResponseStreamResponseEventTypeDef]",
         "ResponseStreamContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLayersResponseTypeDef = TypedDict(
     "ListLayersResponseTypeDef",
     {
         "NextMarker": str,
         "Layers": List[LayersListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FunctionConfigurationResponseMetadataTypeDef = TypedDict(
-    "FunctionConfigurationResponseMetadataTypeDef",
+FunctionConfigurationResponseTypeDef = TypedDict(
+    "FunctionConfigurationResponseTypeDef",
     {
         "FunctionName": str,
         "FunctionArn": str,
         "Runtime": RuntimeType,
         "Role": str,
         "Handler": str,
         "CodeSize": int,
         "Description": str,
         "Timeout": int,
         "MemorySize": int,
         "LastModified": str,
         "CodeSha256": str,
         "Version": str,
         "VpcConfig": VpcConfigResponseTypeDef,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
         "Environment": EnvironmentResponseTypeDef,
         "KMSKeyArn": str,
         "TracingConfig": TracingConfigResponseTypeDef,
         "MasterArn": str,
         "RevisionId": str,
         "Layers": List[LayerTypeDef],
         "State": StateType,
         "StateReason": str,
         "StateReasonCode": StateReasonCodeType,
         "LastUpdateStatus": LastUpdateStatusType,
         "LastUpdateStatusReason": str,
         "LastUpdateStatusReasonCode": LastUpdateStatusReasonCodeType,
-        "FileSystemConfigs": List[FileSystemConfigOutputTypeDef],
+        "FileSystemConfigs": List[FileSystemConfigTypeDef],
         "PackageType": PackageTypeType,
         "ImageConfigResponse": ImageConfigResponseTypeDef,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
         "Architectures": List[ArchitectureType],
-        "EphemeralStorage": EphemeralStorageOutputTypeDef,
+        "EphemeralStorage": EphemeralStorageTypeDef,
         "SnapStart": SnapStartResponseTypeDef,
         "RuntimeVersionConfig": RuntimeVersionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "FunctionName": str,
@@ -2943,79 +2823,79 @@
         "Description": str,
         "Timeout": int,
         "MemorySize": int,
         "LastModified": str,
         "CodeSha256": str,
         "Version": str,
         "VpcConfig": VpcConfigResponseTypeDef,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
         "Environment": EnvironmentResponseTypeDef,
         "KMSKeyArn": str,
         "TracingConfig": TracingConfigResponseTypeDef,
         "MasterArn": str,
         "RevisionId": str,
         "Layers": List[LayerTypeDef],
         "State": StateType,
         "StateReason": str,
         "StateReasonCode": StateReasonCodeType,
         "LastUpdateStatus": LastUpdateStatusType,
         "LastUpdateStatusReason": str,
         "LastUpdateStatusReasonCode": LastUpdateStatusReasonCodeType,
-        "FileSystemConfigs": List[FileSystemConfigOutputTypeDef],
+        "FileSystemConfigs": List[FileSystemConfigTypeDef],
         "PackageType": PackageTypeType,
         "ImageConfigResponse": ImageConfigResponseTypeDef,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
         "Architectures": List[ArchitectureType],
-        "EphemeralStorage": EphemeralStorageOutputTypeDef,
+        "EphemeralStorage": EphemeralStorageTypeDef,
         "SnapStart": SnapStartResponseTypeDef,
         "RuntimeVersionConfig": RuntimeVersionConfigTypeDef,
     },
     total=False,
 )
 
 ListFunctionEventInvokeConfigsResponseTypeDef = TypedDict(
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     {
         "FunctionEventInvokeConfigs": List[FunctionEventInvokeConfigTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventSourceMappingsResponseTypeDef = TypedDict(
     "ListEventSourceMappingsResponseTypeDef",
     {
         "NextMarker": str,
         "EventSourceMappings": List[EventSourceMappingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFunctionResponseTypeDef = TypedDict(
     "GetFunctionResponseTypeDef",
     {
         "Configuration": FunctionConfigurationTypeDef,
         "Code": FunctionCodeLocationTypeDef,
         "Tags": Dict[str, str],
         "Concurrency": ConcurrencyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionsResponseTypeDef = TypedDict(
     "ListFunctionsResponseTypeDef",
     {
         "NextMarker": str,
         "Functions": List[FunctionConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVersionsByFunctionResponseTypeDef = TypedDict(
     "ListVersionsByFunctionResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[FunctionConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/type_defs.pyi` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -51,26 +51,22 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountLimitTypeDef",
     "AccountUsageTypeDef",
     "AddLayerVersionPermissionRequestRequestTypeDef",
-    "AddLayerVersionPermissionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AddPermissionRequestRequestTypeDef",
-    "AddPermissionResponseTypeDef",
     "AliasRoutingConfigurationOutputTypeDef",
     "AliasRoutingConfigurationTypeDef",
     "AllowedPublishersOutputTypeDef",
     "AllowedPublishersTypeDef",
-    "AmazonManagedKafkaEventSourceConfigOutputTypeDef",
     "AmazonManagedKafkaEventSourceConfigTypeDef",
-    "CodeSigningPoliciesOutputTypeDef",
     "CodeSigningPoliciesTypeDef",
-    "ConcurrencyResponseMetadataTypeDef",
     "ConcurrencyTypeDef",
     "CorsOutputTypeDef",
     "CorsTypeDef",
     "DocumentDBEventSourceConfigTypeDef",
     "ScalingConfigTypeDef",
     "SelfManagedEventSourceTypeDef",
     "SelfManagedKafkaEventSourceConfigTypeDef",
@@ -80,138 +76,118 @@
     "EphemeralStorageTypeDef",
     "FileSystemConfigTypeDef",
     "FunctionCodeTypeDef",
     "ImageConfigTypeDef",
     "SnapStartTypeDef",
     "TracingConfigTypeDef",
     "VpcConfigTypeDef",
-    "DeadLetterConfigOutputTypeDef",
     "DeleteAliasRequestRequestTypeDef",
     "DeleteCodeSigningConfigRequestRequestTypeDef",
     "DeleteEventSourceMappingRequestRequestTypeDef",
     "DeleteFunctionCodeSigningConfigRequestRequestTypeDef",
     "DeleteFunctionConcurrencyRequestRequestTypeDef",
     "DeleteFunctionEventInvokeConfigRequestRequestTypeDef",
     "DeleteFunctionRequestRequestTypeDef",
     "DeleteFunctionUrlConfigRequestRequestTypeDef",
     "DeleteLayerVersionRequestRequestTypeDef",
     "DeleteProvisionedConcurrencyConfigRequestRequestTypeDef",
-    "OnFailureOutputTypeDef",
-    "OnSuccessOutputTypeDef",
     "OnFailureTypeDef",
     "OnSuccessTypeDef",
-    "DocumentDBEventSourceConfigOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnvironmentErrorTypeDef",
-    "EphemeralStorageOutputTypeDef",
-    "ScalingConfigOutputTypeDef",
     "SelfManagedEventSourceOutputTypeDef",
-    "SelfManagedKafkaEventSourceConfigOutputTypeDef",
-    "SourceAccessConfigurationOutputTypeDef",
-    "FileSystemConfigOutputTypeDef",
-    "FilterOutputTypeDef",
     "FilterTypeDef",
     "FunctionCodeLocationTypeDef",
     "LayerTypeDef",
     "SnapStartResponseTypeDef",
     "TracingConfigResponseTypeDef",
     "VpcConfigResponseTypeDef",
     "GetAliasRequestRequestTypeDef",
     "GetCodeSigningConfigRequestRequestTypeDef",
     "GetEventSourceMappingRequestRequestTypeDef",
     "GetFunctionCodeSigningConfigRequestRequestTypeDef",
-    "GetFunctionCodeSigningConfigResponseTypeDef",
     "GetFunctionConcurrencyRequestRequestTypeDef",
-    "GetFunctionConcurrencyResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetFunctionConfigurationRequestRequestTypeDef",
     "GetFunctionEventInvokeConfigRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetFunctionUrlConfigRequestRequestTypeDef",
     "GetLayerVersionByArnRequestRequestTypeDef",
     "GetLayerVersionPolicyRequestRequestTypeDef",
-    "GetLayerVersionPolicyResponseTypeDef",
     "GetLayerVersionRequestRequestTypeDef",
     "LayerVersionContentOutputTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
-    "GetProvisionedConcurrencyConfigResponseTypeDef",
     "GetRuntimeManagementConfigRequestRequestTypeDef",
-    "GetRuntimeManagementConfigResponseTypeDef",
     "ImageConfigErrorTypeDef",
     "ImageConfigOutputTypeDef",
     "InvocationRequestRequestTypeDef",
-    "InvocationResponseTypeDef",
     "InvokeAsyncRequestRequestTypeDef",
-    "InvokeAsyncResponseTypeDef",
     "InvokeResponseStreamUpdateTypeDef",
     "InvokeWithResponseStreamCompleteEventTypeDef",
     "InvokeWithResponseStreamRequestRequestTypeDef",
     "LayerVersionContentInputTypeDef",
     "LayerVersionsListItemTypeDef",
-    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAliasesRequestRequestTypeDef",
-    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
     "ListCodeSigningConfigsRequestRequestTypeDef",
-    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
     "ListEventSourceMappingsRequestRequestTypeDef",
-    "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
     "ListFunctionEventInvokeConfigsRequestRequestTypeDef",
-    "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
     "ListFunctionUrlConfigsRequestRequestTypeDef",
-    "ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
     "ListFunctionsByCodeSigningConfigRequestRequestTypeDef",
-    "ListFunctionsByCodeSigningConfigResponseTypeDef",
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListFunctionsRequestRequestTypeDef",
-    "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
     "ListLayerVersionsRequestRequestTypeDef",
-    "ListLayersRequestListLayersPaginateTypeDef",
     "ListLayersRequestRequestTypeDef",
-    "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsRequestRequestTypeDef",
     "ProvisionedConcurrencyConfigListItemTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
-    "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListVersionsByFunctionRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PublishVersionRequestRequestTypeDef",
     "PutFunctionCodeSigningConfigRequestRequestTypeDef",
-    "PutFunctionCodeSigningConfigResponseTypeDef",
     "PutFunctionConcurrencyRequestRequestTypeDef",
     "PutProvisionedConcurrencyConfigRequestRequestTypeDef",
-    "PutProvisionedConcurrencyConfigResponseTypeDef",
     "PutRuntimeManagementConfigRequestRequestTypeDef",
-    "PutRuntimeManagementConfigResponseTypeDef",
     "RemoveLayerVersionPermissionRequestRequestTypeDef",
     "RemovePermissionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RuntimeVersionErrorTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFunctionCodeRequestRequestTypeDef",
+    "AddLayerVersionPermissionResponseTypeDef",
+    "AddPermissionResponseTypeDef",
+    "ConcurrencyResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetAccountSettingsResponseTypeDef",
-    "AliasConfigurationResponseMetadataTypeDef",
+    "GetFunctionCodeSigningConfigResponseTypeDef",
+    "GetFunctionConcurrencyResponseTypeDef",
+    "GetLayerVersionPolicyResponseTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetProvisionedConcurrencyConfigResponseTypeDef",
+    "GetRuntimeManagementConfigResponseTypeDef",
+    "InvocationResponseTypeDef",
+    "InvokeAsyncResponseTypeDef",
+    "ListFunctionsByCodeSigningConfigResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "PutFunctionCodeSigningConfigResponseTypeDef",
+    "PutProvisionedConcurrencyConfigResponseTypeDef",
+    "PutRuntimeManagementConfigResponseTypeDef",
+    "AliasConfigurationResponseTypeDef",
     "AliasConfigurationTypeDef",
     "CreateAliasRequestRequestTypeDef",
     "UpdateAliasRequestRequestTypeDef",
     "CodeSigningConfigTypeDef",
     "CreateCodeSigningConfigRequestRequestTypeDef",
     "UpdateCodeSigningConfigRequestRequestTypeDef",
     "CreateFunctionUrlConfigResponseTypeDef",
     "FunctionUrlConfigTypeDef",
     "GetFunctionUrlConfigResponseTypeDef",
     "UpdateFunctionUrlConfigResponseTypeDef",
     "CreateFunctionUrlConfigRequestRequestTypeDef",
     "UpdateFunctionUrlConfigRequestRequestTypeDef",
     "CreateFunctionRequestRequestTypeDef",
     "UpdateFunctionConfigurationRequestRequestTypeDef",
-    "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "EnvironmentResponseTypeDef",
     "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "GetFunctionConfigurationRequestFunctionActiveWaitTypeDef",
     "GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef",
     "GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef",
@@ -221,33 +197,44 @@
     "GetLayerVersionResponseTypeDef",
     "PublishLayerVersionResponseTypeDef",
     "ImageConfigResponseTypeDef",
     "InvokeWithResponseStreamResponseEventTypeDef",
     "PublishLayerVersionRequestRequestTypeDef",
     "LayersListItemTypeDef",
     "ListLayerVersionsResponseTypeDef",
+    "ListAliasesRequestListAliasesPaginateTypeDef",
+    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
+    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
+    "ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    "ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    "ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
+    "ListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    "ListLayersRequestListLayersPaginateTypeDef",
+    "ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    "ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     "RuntimeVersionConfigTypeDef",
     "ListAliasesResponseTypeDef",
     "CreateCodeSigningConfigResponseTypeDef",
     "GetCodeSigningConfigResponseTypeDef",
     "ListCodeSigningConfigsResponseTypeDef",
     "UpdateCodeSigningConfigResponseTypeDef",
     "ListFunctionUrlConfigsResponseTypeDef",
-    "FunctionEventInvokeConfigResponseMetadataTypeDef",
+    "FunctionEventInvokeConfigResponseTypeDef",
     "FunctionEventInvokeConfigTypeDef",
     "PutFunctionEventInvokeConfigRequestRequestTypeDef",
     "UpdateFunctionEventInvokeConfigRequestRequestTypeDef",
-    "EventSourceMappingConfigurationResponseMetadataTypeDef",
+    "EventSourceMappingConfigurationResponseTypeDef",
     "EventSourceMappingConfigurationTypeDef",
     "CreateEventSourceMappingRequestRequestTypeDef",
     "UpdateEventSourceMappingRequestRequestTypeDef",
     "InvokeWithResponseStreamResponseTypeDef",
     "ListLayersResponseTypeDef",
-    "FunctionConfigurationResponseMetadataTypeDef",
+    "FunctionConfigurationResponseTypeDef",
     "FunctionConfigurationTypeDef",
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     "ListEventSourceMappingsResponseTypeDef",
     "GetFunctionResponseTypeDef",
     "ListFunctionsResponseTypeDef",
     "ListVersionsByFunctionResponseTypeDef",
 )
@@ -294,20 +281,22 @@
 
 class AddLayerVersionPermissionRequestRequestTypeDef(
     _RequiredAddLayerVersionPermissionRequestRequestTypeDef,
     _OptionalAddLayerVersionPermissionRequestRequestTypeDef,
 ):
     pass
 
-AddLayerVersionPermissionResponseTypeDef = TypedDict(
-    "AddLayerVersionPermissionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Statement": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredAddPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredAddPermissionRequestRequestTypeDef",
     {
         "FunctionName": str,
@@ -331,22 +320,14 @@
 )
 
 class AddPermissionRequestRequestTypeDef(
     _RequiredAddPermissionRequestRequestTypeDef, _OptionalAddPermissionRequestRequestTypeDef
 ):
     pass
 
-AddPermissionResponseTypeDef = TypedDict(
-    "AddPermissionResponseTypeDef",
-    {
-        "Statement": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AliasRoutingConfigurationOutputTypeDef = TypedDict(
     "AliasRoutingConfigurationOutputTypeDef",
     {
         "AdditionalVersionWeights": Dict[str, float],
     },
     total=False,
 )
@@ -369,54 +350,30 @@
 AllowedPublishersTypeDef = TypedDict(
     "AllowedPublishersTypeDef",
     {
         "SigningProfileVersionArns": Sequence[str],
     },
 )
 
-AmazonManagedKafkaEventSourceConfigOutputTypeDef = TypedDict(
-    "AmazonManagedKafkaEventSourceConfigOutputTypeDef",
-    {
-        "ConsumerGroupId": str,
-    },
-    total=False,
-)
-
 AmazonManagedKafkaEventSourceConfigTypeDef = TypedDict(
     "AmazonManagedKafkaEventSourceConfigTypeDef",
     {
         "ConsumerGroupId": str,
     },
     total=False,
 )
 
-CodeSigningPoliciesOutputTypeDef = TypedDict(
-    "CodeSigningPoliciesOutputTypeDef",
-    {
-        "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
-    },
-    total=False,
-)
-
 CodeSigningPoliciesTypeDef = TypedDict(
     "CodeSigningPoliciesTypeDef",
     {
         "UntrustedArtifactOnDeployment": CodeSigningPolicyType,
     },
     total=False,
 )
 
-ConcurrencyResponseMetadataTypeDef = TypedDict(
-    "ConcurrencyResponseMetadataTypeDef",
-    {
-        "ReservedConcurrentExecutions": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConcurrencyTypeDef = TypedDict(
     "ConcurrencyTypeDef",
     {
         "ReservedConcurrentExecutions": int,
     },
     total=False,
 )
@@ -564,22 +521,14 @@
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-DeadLetterConfigOutputTypeDef = TypedDict(
-    "DeadLetterConfigOutputTypeDef",
-    {
-        "TargetArn": str,
-    },
-    total=False,
-)
-
 DeleteAliasRequestRequestTypeDef = TypedDict(
     "DeleteAliasRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Name": str,
     },
 )
@@ -683,30 +632,14 @@
     "DeleteProvisionedConcurrencyConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Qualifier": str,
     },
 )
 
-OnFailureOutputTypeDef = TypedDict(
-    "OnFailureOutputTypeDef",
-    {
-        "Destination": str,
-    },
-    total=False,
-)
-
-OnSuccessOutputTypeDef = TypedDict(
-    "OnSuccessOutputTypeDef",
-    {
-        "Destination": str,
-    },
-    total=False,
-)
-
 OnFailureTypeDef = TypedDict(
     "OnFailureTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
@@ -715,96 +648,31 @@
     "OnSuccessTypeDef",
     {
         "Destination": str,
     },
     total=False,
 )
 
-DocumentDBEventSourceConfigOutputTypeDef = TypedDict(
-    "DocumentDBEventSourceConfigOutputTypeDef",
-    {
-        "DatabaseName": str,
-        "CollectionName": str,
-        "FullDocument": FullDocumentType,
-    },
-    total=False,
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentErrorTypeDef = TypedDict(
     "EnvironmentErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-EphemeralStorageOutputTypeDef = TypedDict(
-    "EphemeralStorageOutputTypeDef",
-    {
-        "Size": int,
-    },
-)
-
-ScalingConfigOutputTypeDef = TypedDict(
-    "ScalingConfigOutputTypeDef",
-    {
-        "MaximumConcurrency": int,
-    },
-    total=False,
-)
-
 SelfManagedEventSourceOutputTypeDef = TypedDict(
     "SelfManagedEventSourceOutputTypeDef",
     {
         "Endpoints": Dict[Literal["KAFKA_BOOTSTRAP_SERVERS"], List[str]],
     },
     total=False,
 )
 
-SelfManagedKafkaEventSourceConfigOutputTypeDef = TypedDict(
-    "SelfManagedKafkaEventSourceConfigOutputTypeDef",
-    {
-        "ConsumerGroupId": str,
-    },
-    total=False,
-)
-
-SourceAccessConfigurationOutputTypeDef = TypedDict(
-    "SourceAccessConfigurationOutputTypeDef",
-    {
-        "Type": SourceAccessTypeType,
-        "URI": str,
-    },
-    total=False,
-)
-
-FileSystemConfigOutputTypeDef = TypedDict(
-    "FileSystemConfigOutputTypeDef",
-    {
-        "Arn": str,
-        "LocalMountPath": str,
-    },
-)
-
-FilterOutputTypeDef = TypedDict(
-    "FilterOutputTypeDef",
-    {
-        "Pattern": str,
-    },
-    total=False,
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Pattern": str,
     },
     total=False,
 )
@@ -883,38 +751,21 @@
 GetFunctionCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "GetFunctionCodeSigningConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 
-GetFunctionCodeSigningConfigResponseTypeDef = TypedDict(
-    "GetFunctionCodeSigningConfigResponseTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-        "FunctionName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFunctionConcurrencyRequestRequestTypeDef = TypedDict(
     "GetFunctionConcurrencyRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 
-GetFunctionConcurrencyResponseTypeDef = TypedDict(
-    "GetFunctionConcurrencyResponseTypeDef",
-    {
-        "ReservedConcurrentExecutions": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
@@ -1010,23 +861,14 @@
     "GetLayerVersionPolicyRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
     },
 )
 
-GetLayerVersionPolicyResponseTypeDef = TypedDict(
-    "GetLayerVersionPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLayerVersionRequestRequestTypeDef = TypedDict(
     "GetLayerVersionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
     },
 )
@@ -1058,44 +900,22 @@
 )
 
 class GetPolicyRequestRequestTypeDef(
     _RequiredGetPolicyRequestRequestTypeDef, _OptionalGetPolicyRequestRequestTypeDef
 ):
     pass
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetProvisionedConcurrencyConfigRequestRequestTypeDef = TypedDict(
     "GetProvisionedConcurrencyConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "Qualifier": str,
     },
 )
 
-GetProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
-    "GetProvisionedConcurrencyConfigResponseTypeDef",
-    {
-        "RequestedProvisionedConcurrentExecutions": int,
-        "AvailableProvisionedConcurrentExecutions": int,
-        "AllocatedProvisionedConcurrentExecutions": int,
-        "Status": ProvisionedConcurrencyStatusEnumType,
-        "StatusReason": str,
-        "LastModified": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
     "_RequiredGetRuntimeManagementConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalGetRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
@@ -1108,24 +928,14 @@
 
 class GetRuntimeManagementConfigRequestRequestTypeDef(
     _RequiredGetRuntimeManagementConfigRequestRequestTypeDef,
     _OptionalGetRuntimeManagementConfigRequestRequestTypeDef,
 ):
     pass
 
-GetRuntimeManagementConfigResponseTypeDef = TypedDict(
-    "GetRuntimeManagementConfigResponseTypeDef",
-    {
-        "UpdateRuntimeOn": UpdateRuntimeOnType,
-        "RuntimeVersionArn": str,
-        "FunctionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ImageConfigErrorTypeDef = TypedDict(
     "ImageConfigErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -1160,42 +970,22 @@
 )
 
 class InvocationRequestRequestTypeDef(
     _RequiredInvocationRequestRequestTypeDef, _OptionalInvocationRequestRequestTypeDef
 ):
     pass
 
-InvocationResponseTypeDef = TypedDict(
-    "InvocationResponseTypeDef",
-    {
-        "StatusCode": int,
-        "FunctionError": str,
-        "LogResult": str,
-        "Payload": StreamingBody,
-        "ExecutedVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InvokeAsyncRequestRequestTypeDef = TypedDict(
     "InvokeAsyncRequestRequestTypeDef",
     {
         "FunctionName": str,
         "InvokeArgs": Union[str, bytes, IO[Any], StreamingBody],
     },
 )
 
-InvokeAsyncResponseTypeDef = TypedDict(
-    "InvokeAsyncResponseTypeDef",
-    {
-        "Status": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InvokeResponseStreamUpdateTypeDef = TypedDict(
     "InvokeResponseStreamUpdateTypeDef",
     {
         "Payload": bytes,
     },
     total=False,
 )
@@ -1255,35 +1045,24 @@
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
     },
     total=False,
 )
 
-_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
-    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "FunctionVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListAliasesRequestListAliasesPaginateTypeDef(
-    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
-    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAliasesRequestRequestTypeDef = TypedDict(
     "_RequiredListAliasesRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListAliasesRequestRequestTypeDef = TypedDict(
@@ -1297,72 +1076,34 @@
 )
 
 class ListAliasesRequestRequestTypeDef(
     _RequiredListAliasesRequestRequestTypeDef, _OptionalListAliasesRequestRequestTypeDef
 ):
     pass
 
-ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef = TypedDict(
-    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCodeSigningConfigsRequestRequestTypeDef = TypedDict(
     "ListCodeSigningConfigsRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef = TypedDict(
-    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
-    {
-        "EventSourceArn": str,
-        "FunctionName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEventSourceMappingsRequestRequestTypeDef = TypedDict(
     "ListEventSourceMappingsRequestRequestTypeDef",
     {
         "EventSourceArn": str,
         "FunctionName": str,
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(
-    _RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-    _OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListFunctionEventInvokeConfigsRequestRequestTypeDef = TypedDict(
@@ -1376,34 +1117,14 @@
 
 class ListFunctionEventInvokeConfigsRequestRequestTypeDef(
     _RequiredListFunctionEventInvokeConfigsRequestRequestTypeDef,
     _OptionalListFunctionEventInvokeConfigsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(
-    _RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-    _OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFunctionUrlConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionUrlConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListFunctionUrlConfigsRequestRequestTypeDef = TypedDict(
@@ -1417,34 +1138,14 @@
 
 class ListFunctionUrlConfigsRequestRequestTypeDef(
     _RequiredListFunctionUrlConfigsRequestRequestTypeDef,
     _OptionalListFunctionUrlConfigsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-    },
-)
-_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(
-    _RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-    _OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
-):
-    pass
-
 _RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef",
     {
         "CodeSigningConfigArn": str,
     },
 )
 _OptionalListFunctionsByCodeSigningConfigRequestRequestTypeDef = TypedDict(
@@ -1458,66 +1159,25 @@
 
 class ListFunctionsByCodeSigningConfigRequestRequestTypeDef(
     _RequiredListFunctionsByCodeSigningConfigRequestRequestTypeDef,
     _OptionalListFunctionsByCodeSigningConfigRequestRequestTypeDef,
 ):
     pass
 
-ListFunctionsByCodeSigningConfigResponseTypeDef = TypedDict(
-    "ListFunctionsByCodeSigningConfigResponseTypeDef",
-    {
-        "NextMarker": str,
-        "FunctionArns": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "MasterRegion": str,
-        "FunctionVersion": Literal["ALL"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFunctionsRequestRequestTypeDef = TypedDict(
     "ListFunctionsRequestRequestTypeDef",
     {
         "MasterRegion": str,
         "FunctionVersion": Literal["ALL"],
         "Marker": str,
         "MaxItems": int,
     },
     total=False,
 )
 
-_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    {
-        "LayerName": str,
-    },
-)
-_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
-    {
-        "CompatibleRuntime": RuntimeType,
-        "CompatibleArchitecture": ArchitectureType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(
-    _RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-    _OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListLayerVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLayerVersionsRequestRequestTypeDef",
     {
         "LayerName": str,
     },
 )
 _OptionalListLayerVersionsRequestRequestTypeDef = TypedDict(
@@ -1532,55 +1192,25 @@
 )
 
 class ListLayerVersionsRequestRequestTypeDef(
     _RequiredListLayerVersionsRequestRequestTypeDef, _OptionalListLayerVersionsRequestRequestTypeDef
 ):
     pass
 
-ListLayersRequestListLayersPaginateTypeDef = TypedDict(
-    "ListLayersRequestListLayersPaginateTypeDef",
-    {
-        "CompatibleRuntime": RuntimeType,
-        "CompatibleArchitecture": ArchitectureType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLayersRequestRequestTypeDef = TypedDict(
     "ListLayersRequestRequestTypeDef",
     {
         "CompatibleRuntime": RuntimeType,
         "Marker": str,
         "MaxItems": int,
         "CompatibleArchitecture": ArchitectureType,
     },
     total=False,
 )
 
-_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
-    "_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
-    "_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(
-    _RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-    _OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
-):
-    pass
-
 _RequiredListProvisionedConcurrencyConfigsRequestRequestTypeDef = TypedDict(
     "_RequiredListProvisionedConcurrencyConfigsRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListProvisionedConcurrencyConfigsRequestRequestTypeDef = TypedDict(
@@ -1615,42 +1245,14 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
-    "_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
-    {
-        "FunctionName": str,
-    },
-)
-_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
-    "_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(
-    _RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
-    _OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
-):
-    pass
-
 _RequiredListVersionsByFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredListVersionsByFunctionRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalListVersionsByFunctionRequestRequestTypeDef = TypedDict(
@@ -1664,24 +1266,14 @@
 
 class ListVersionsByFunctionRequestRequestTypeDef(
     _RequiredListVersionsByFunctionRequestRequestTypeDef,
     _OptionalListVersionsByFunctionRequestRequestTypeDef,
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
 _RequiredPublishVersionRequestRequestTypeDef = TypedDict(
     "_RequiredPublishVersionRequestRequestTypeDef",
     {
         "FunctionName": str,
     },
 )
 _OptionalPublishVersionRequestRequestTypeDef = TypedDict(
@@ -1703,23 +1295,14 @@
     "PutFunctionCodeSigningConfigRequestRequestTypeDef",
     {
         "CodeSigningConfigArn": str,
         "FunctionName": str,
     },
 )
 
-PutFunctionCodeSigningConfigResponseTypeDef = TypedDict(
-    "PutFunctionCodeSigningConfigResponseTypeDef",
-    {
-        "CodeSigningConfigArn": str,
-        "FunctionName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutFunctionConcurrencyRequestRequestTypeDef = TypedDict(
     "PutFunctionConcurrencyRequestRequestTypeDef",
     {
         "FunctionName": str,
         "ReservedConcurrentExecutions": int,
     },
 )
@@ -1729,27 +1312,14 @@
     {
         "FunctionName": str,
         "Qualifier": str,
         "ProvisionedConcurrentExecutions": int,
     },
 )
 
-PutProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
-    "PutProvisionedConcurrencyConfigResponseTypeDef",
-    {
-        "RequestedProvisionedConcurrentExecutions": int,
-        "AvailableProvisionedConcurrentExecutions": int,
-        "AllocatedProvisionedConcurrentExecutions": int,
-        "Status": ProvisionedConcurrencyStatusEnumType,
-        "StatusReason": str,
-        "LastModified": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutRuntimeManagementConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutRuntimeManagementConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
         "UpdateRuntimeOn": UpdateRuntimeOnType,
     },
 )
@@ -1764,24 +1334,14 @@
 
 class PutRuntimeManagementConfigRequestRequestTypeDef(
     _RequiredPutRuntimeManagementConfigRequestRequestTypeDef,
     _OptionalPutRuntimeManagementConfigRequestRequestTypeDef,
 ):
     pass
 
-PutRuntimeManagementConfigResponseTypeDef = TypedDict(
-    "PutRuntimeManagementConfigResponseTypeDef",
-    {
-        "UpdateRuntimeOn": UpdateRuntimeOnType,
-        "FunctionArn": str,
-        "RuntimeVersionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRemoveLayerVersionPermissionRequestRequestTypeDef = TypedDict(
     "_RequiredRemoveLayerVersionPermissionRequestRequestTypeDef",
     {
         "LayerName": str,
         "VersionNumber": int,
         "StatementId": str,
     },
@@ -1817,25 +1377,14 @@
 )
 
 class RemovePermissionRequestRequestTypeDef(
     _RequiredRemovePermissionRequestRequestTypeDef, _OptionalRemovePermissionRequestRequestTypeDef
 ):
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
 RuntimeVersionErrorTypeDef = TypedDict(
     "RuntimeVersionErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -1881,33 +1430,192 @@
 
 class UpdateFunctionCodeRequestRequestTypeDef(
     _RequiredUpdateFunctionCodeRequestRequestTypeDef,
     _OptionalUpdateFunctionCodeRequestRequestTypeDef,
 ):
     pass
 
+AddLayerVersionPermissionResponseTypeDef = TypedDict(
+    "AddLayerVersionPermissionResponseTypeDef",
+    {
+        "Statement": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddPermissionResponseTypeDef = TypedDict(
+    "AddPermissionResponseTypeDef",
+    {
+        "Statement": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConcurrencyResponseTypeDef = TypedDict(
+    "ConcurrencyResponseTypeDef",
+    {
+        "ReservedConcurrentExecutions": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetAccountSettingsResponseTypeDef = TypedDict(
     "GetAccountSettingsResponseTypeDef",
     {
         "AccountLimit": AccountLimitTypeDef,
         "AccountUsage": AccountUsageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionCodeSigningConfigResponseTypeDef = TypedDict(
+    "GetFunctionCodeSigningConfigResponseTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+        "FunctionName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFunctionConcurrencyResponseTypeDef = TypedDict(
+    "GetFunctionConcurrencyResponseTypeDef",
+    {
+        "ReservedConcurrentExecutions": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLayerVersionPolicyResponseTypeDef = TypedDict(
+    "GetLayerVersionPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
+    "GetProvisionedConcurrencyConfigResponseTypeDef",
+    {
+        "RequestedProvisionedConcurrentExecutions": int,
+        "AvailableProvisionedConcurrentExecutions": int,
+        "AllocatedProvisionedConcurrentExecutions": int,
+        "Status": ProvisionedConcurrencyStatusEnumType,
+        "StatusReason": str,
+        "LastModified": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRuntimeManagementConfigResponseTypeDef = TypedDict(
+    "GetRuntimeManagementConfigResponseTypeDef",
+    {
+        "UpdateRuntimeOn": UpdateRuntimeOnType,
+        "RuntimeVersionArn": str,
+        "FunctionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvocationResponseTypeDef = TypedDict(
+    "InvocationResponseTypeDef",
+    {
+        "StatusCode": int,
+        "FunctionError": str,
+        "LogResult": str,
+        "Payload": StreamingBody,
+        "ExecutedVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeAsyncResponseTypeDef = TypedDict(
+    "InvokeAsyncResponseTypeDef",
+    {
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFunctionsByCodeSigningConfigResponseTypeDef = TypedDict(
+    "ListFunctionsByCodeSigningConfigResponseTypeDef",
+    {
+        "NextMarker": str,
+        "FunctionArns": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AliasConfigurationResponseMetadataTypeDef = TypedDict(
-    "AliasConfigurationResponseMetadataTypeDef",
+PutFunctionCodeSigningConfigResponseTypeDef = TypedDict(
+    "PutFunctionCodeSigningConfigResponseTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+        "FunctionName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutProvisionedConcurrencyConfigResponseTypeDef = TypedDict(
+    "PutProvisionedConcurrencyConfigResponseTypeDef",
+    {
+        "RequestedProvisionedConcurrentExecutions": int,
+        "AvailableProvisionedConcurrentExecutions": int,
+        "AllocatedProvisionedConcurrentExecutions": int,
+        "Status": ProvisionedConcurrencyStatusEnumType,
+        "StatusReason": str,
+        "LastModified": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRuntimeManagementConfigResponseTypeDef = TypedDict(
+    "PutRuntimeManagementConfigResponseTypeDef",
+    {
+        "UpdateRuntimeOn": UpdateRuntimeOnType,
+        "FunctionArn": str,
+        "RuntimeVersionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AliasConfigurationResponseTypeDef = TypedDict(
+    "AliasConfigurationResponseTypeDef",
     {
         "AliasArn": str,
         "Name": str,
         "FunctionVersion": str,
         "Description": str,
         "RoutingConfig": AliasRoutingConfigurationOutputTypeDef,
         "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AliasConfigurationTypeDef = TypedDict(
     "AliasConfigurationTypeDef",
     {
         "AliasArn": str,
@@ -1967,15 +1675,15 @@
 
 _RequiredCodeSigningConfigTypeDef = TypedDict(
     "_RequiredCodeSigningConfigTypeDef",
     {
         "CodeSigningConfigId": str,
         "CodeSigningConfigArn": str,
         "AllowedPublishers": AllowedPublishersOutputTypeDef,
-        "CodeSigningPolicies": CodeSigningPoliciesOutputTypeDef,
+        "CodeSigningPolicies": CodeSigningPoliciesTypeDef,
         "LastModified": str,
     },
 )
 _OptionalCodeSigningConfigTypeDef = TypedDict(
     "_OptionalCodeSigningConfigTypeDef",
     {
         "Description": str,
@@ -2036,15 +1744,15 @@
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFunctionUrlConfigTypeDef = TypedDict(
     "_RequiredFunctionUrlConfigTypeDef",
     {
         "FunctionUrl": str,
@@ -2074,29 +1782,29 @@
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFunctionUrlConfigResponseTypeDef = TypedDict(
     "UpdateFunctionUrlConfigResponseTypeDef",
     {
         "FunctionUrl": str,
         "FunctionArn": str,
         "AuthType": FunctionUrlAuthTypeType,
         "Cors": CorsOutputTypeDef,
         "CreationTime": str,
         "LastModifiedTime": str,
         "InvokeMode": InvokeModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFunctionUrlConfigRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFunctionUrlConfigRequestRequestTypeDef",
     {
         "FunctionName": str,
@@ -2214,23 +1922,14 @@
 
 class UpdateFunctionConfigurationRequestRequestTypeDef(
     _RequiredUpdateFunctionConfigurationRequestRequestTypeDef,
     _OptionalUpdateFunctionConfigurationRequestRequestTypeDef,
 ):
     pass
 
-DestinationConfigOutputTypeDef = TypedDict(
-    "DestinationConfigOutputTypeDef",
-    {
-        "OnSuccess": OnSuccessOutputTypeDef,
-        "OnFailure": OnFailureOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationConfigTypeDef = TypedDict(
     "DestinationConfigTypeDef",
     {
         "OnSuccess": OnSuccessTypeDef,
         "OnFailure": OnFailureTypeDef,
     },
     total=False,
@@ -2244,15 +1943,15 @@
     },
     total=False,
 )
 
 FilterCriteriaOutputTypeDef = TypedDict(
     "FilterCriteriaOutputTypeDef",
     {
-        "Filters": List[FilterOutputTypeDef],
+        "Filters": List[FilterTypeDef],
     },
     total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
@@ -2395,15 +2094,15 @@
         "LayerVersionArn": str,
         "Description": str,
         "CreatedDate": str,
         "Version": int,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PublishLayerVersionResponseTypeDef = TypedDict(
     "PublishLayerVersionResponseTypeDef",
     {
         "Content": LayerVersionContentOutputTypeDef,
@@ -2411,15 +2110,15 @@
         "LayerVersionArn": str,
         "Description": str,
         "CreatedDate": str,
         "Version": int,
         "CompatibleRuntimes": List[RuntimeType],
         "LicenseInfo": str,
         "CompatibleArchitectures": List[ArchitectureType],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImageConfigResponseTypeDef = TypedDict(
     "ImageConfigResponseTypeDef",
     {
         "ImageConfig": ImageConfigOutputTypeDef,
@@ -2472,24 +2171,205 @@
 )
 
 ListLayerVersionsResponseTypeDef = TypedDict(
     "ListLayerVersionsResponseTypeDef",
     {
         "NextMarker": str,
         "LayerVersions": List[LayerVersionsListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_RequiredListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListAliasesRequestListAliasesPaginateTypeDef = TypedDict(
+    "_OptionalListAliasesRequestListAliasesPaginateTypeDef",
+    {
+        "FunctionVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAliasesRequestListAliasesPaginateTypeDef(
+    _RequiredListAliasesRequestListAliasesPaginateTypeDef,
+    _OptionalListAliasesRequestListAliasesPaginateTypeDef,
+):
+    pass
+
+ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef = TypedDict(
+    "ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef = TypedDict(
+    "ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef",
+    {
+        "EventSourceArn": str,
+        "FunctionName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef(
+    _RequiredListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+    _OptionalListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
     },
 )
+_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef(
+    _RequiredListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+    _OptionalListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+):
+    pass
+
+_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    {
+        "CodeSigningConfigArn": str,
+    },
+)
+_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef(
+    _RequiredListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+    _OptionalListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+):
+    pass
+
+ListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "MasterRegion": str,
+        "FunctionVersion": Literal["ALL"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    {
+        "LayerName": str,
+    },
+)
+_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef",
+    {
+        "CompatibleRuntime": RuntimeType,
+        "CompatibleArchitecture": ArchitectureType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListLayerVersionsRequestListLayerVersionsPaginateTypeDef(
+    _RequiredListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+    _OptionalListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+):
+    pass
+
+ListLayersRequestListLayersPaginateTypeDef = TypedDict(
+    "ListLayersRequestListLayersPaginateTypeDef",
+    {
+        "CompatibleRuntime": RuntimeType,
+        "CompatibleArchitecture": ArchitectureType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
+    "_RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef = TypedDict(
+    "_OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef(
+    _RequiredListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+    _OptionalListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+):
+    pass
+
+_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
+    "_RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
+    {
+        "FunctionName": str,
+    },
+)
+_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef = TypedDict(
+    "_OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef(
+    _RequiredListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
+    _OptionalListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
+):
+    pass
 
 ListProvisionedConcurrencyConfigsResponseTypeDef = TypedDict(
     "ListProvisionedConcurrencyConfigsResponseTypeDef",
     {
         "ProvisionedConcurrencyConfigs": List[ProvisionedConcurrencyConfigListItemTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuntimeVersionConfigTypeDef = TypedDict(
     "RuntimeVersionConfigTypeDef",
     {
         "RuntimeVersionArn": str,
@@ -2499,80 +2379,80 @@
 )
 
 ListAliasesResponseTypeDef = TypedDict(
     "ListAliasesResponseTypeDef",
     {
         "NextMarker": str,
         "Aliases": List[AliasConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCodeSigningConfigResponseTypeDef = TypedDict(
     "CreateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCodeSigningConfigResponseTypeDef = TypedDict(
     "GetCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCodeSigningConfigsResponseTypeDef = TypedDict(
     "ListCodeSigningConfigsResponseTypeDef",
     {
         "NextMarker": str,
         "CodeSigningConfigs": List[CodeSigningConfigTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCodeSigningConfigResponseTypeDef = TypedDict(
     "UpdateCodeSigningConfigResponseTypeDef",
     {
         "CodeSigningConfig": CodeSigningConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionUrlConfigsResponseTypeDef = TypedDict(
     "ListFunctionUrlConfigsResponseTypeDef",
     {
         "FunctionUrlConfigs": List[FunctionUrlConfigTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FunctionEventInvokeConfigResponseMetadataTypeDef = TypedDict(
-    "FunctionEventInvokeConfigResponseMetadataTypeDef",
+FunctionEventInvokeConfigResponseTypeDef = TypedDict(
+    "FunctionEventInvokeConfigResponseTypeDef",
     {
         "LastModified": datetime,
         "FunctionArn": str,
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
-        "DestinationConfig": DestinationConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DestinationConfig": DestinationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FunctionEventInvokeConfigTypeDef = TypedDict(
     "FunctionEventInvokeConfigTypeDef",
     {
         "LastModified": datetime,
         "FunctionArn": str,
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
-        "DestinationConfig": DestinationConfigOutputTypeDef,
+        "DestinationConfig": DestinationConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredPutFunctionEventInvokeConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutFunctionEventInvokeConfigRequestRequestTypeDef",
     {
@@ -2615,45 +2495,45 @@
 
 class UpdateFunctionEventInvokeConfigRequestRequestTypeDef(
     _RequiredUpdateFunctionEventInvokeConfigRequestRequestTypeDef,
     _OptionalUpdateFunctionEventInvokeConfigRequestRequestTypeDef,
 ):
     pass
 
-EventSourceMappingConfigurationResponseMetadataTypeDef = TypedDict(
-    "EventSourceMappingConfigurationResponseMetadataTypeDef",
+EventSourceMappingConfigurationResponseTypeDef = TypedDict(
+    "EventSourceMappingConfigurationResponseTypeDef",
     {
         "UUID": str,
         "StartingPosition": EventSourcePositionType,
         "StartingPositionTimestamp": datetime,
         "BatchSize": int,
         "MaximumBatchingWindowInSeconds": int,
         "ParallelizationFactor": int,
         "EventSourceArn": str,
         "FilterCriteria": FilterCriteriaOutputTypeDef,
         "FunctionArn": str,
         "LastModified": datetime,
         "LastProcessingResult": str,
         "State": str,
         "StateTransitionReason": str,
-        "DestinationConfig": DestinationConfigOutputTypeDef,
+        "DestinationConfig": DestinationConfigTypeDef,
         "Topics": List[str],
         "Queues": List[str],
-        "SourceAccessConfigurations": List[SourceAccessConfigurationOutputTypeDef],
+        "SourceAccessConfigurations": List[SourceAccessConfigurationTypeDef],
         "SelfManagedEventSource": SelfManagedEventSourceOutputTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
-        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigOutputTypeDef,
-        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigOutputTypeDef,
-        "ScalingConfig": ScalingConfigOutputTypeDef,
-        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
+        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
+        "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventSourceMappingConfigurationTypeDef = TypedDict(
     "EventSourceMappingConfigurationTypeDef",
     {
         "UUID": str,
@@ -2665,28 +2545,28 @@
         "EventSourceArn": str,
         "FilterCriteria": FilterCriteriaOutputTypeDef,
         "FunctionArn": str,
         "LastModified": datetime,
         "LastProcessingResult": str,
         "State": str,
         "StateTransitionReason": str,
-        "DestinationConfig": DestinationConfigOutputTypeDef,
+        "DestinationConfig": DestinationConfigTypeDef,
         "Topics": List[str],
         "Queues": List[str],
-        "SourceAccessConfigurations": List[SourceAccessConfigurationOutputTypeDef],
+        "SourceAccessConfigurations": List[SourceAccessConfigurationTypeDef],
         "SelfManagedEventSource": SelfManagedEventSourceOutputTypeDef,
         "MaximumRecordAgeInSeconds": int,
         "BisectBatchOnFunctionError": bool,
         "MaximumRetryAttempts": int,
         "TumblingWindowInSeconds": int,
         "FunctionResponseTypes": List[Literal["ReportBatchItemFailures"]],
-        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigOutputTypeDef,
-        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigOutputTypeDef,
-        "ScalingConfig": ScalingConfigOutputTypeDef,
-        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigOutputTypeDef,
+        "AmazonManagedKafkaEventSourceConfig": AmazonManagedKafkaEventSourceConfigTypeDef,
+        "SelfManagedKafkaEventSourceConfig": SelfManagedKafkaEventSourceConfigTypeDef,
+        "ScalingConfig": ScalingConfigTypeDef,
+        "DocumentDBEventSourceConfig": DocumentDBEventSourceConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateEventSourceMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEventSourceMappingRequestRequestTypeDef",
     {
@@ -2765,66 +2645,66 @@
 InvokeWithResponseStreamResponseTypeDef = TypedDict(
     "InvokeWithResponseStreamResponseTypeDef",
     {
         "StatusCode": int,
         "ExecutedVersion": str,
         "EventStream": "EventStream[InvokeWithResponseStreamResponseEventTypeDef]",
         "ResponseStreamContentType": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLayersResponseTypeDef = TypedDict(
     "ListLayersResponseTypeDef",
     {
         "NextMarker": str,
         "Layers": List[LayersListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-FunctionConfigurationResponseMetadataTypeDef = TypedDict(
-    "FunctionConfigurationResponseMetadataTypeDef",
+FunctionConfigurationResponseTypeDef = TypedDict(
+    "FunctionConfigurationResponseTypeDef",
     {
         "FunctionName": str,
         "FunctionArn": str,
         "Runtime": RuntimeType,
         "Role": str,
         "Handler": str,
         "CodeSize": int,
         "Description": str,
         "Timeout": int,
         "MemorySize": int,
         "LastModified": str,
         "CodeSha256": str,
         "Version": str,
         "VpcConfig": VpcConfigResponseTypeDef,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
         "Environment": EnvironmentResponseTypeDef,
         "KMSKeyArn": str,
         "TracingConfig": TracingConfigResponseTypeDef,
         "MasterArn": str,
         "RevisionId": str,
         "Layers": List[LayerTypeDef],
         "State": StateType,
         "StateReason": str,
         "StateReasonCode": StateReasonCodeType,
         "LastUpdateStatus": LastUpdateStatusType,
         "LastUpdateStatusReason": str,
         "LastUpdateStatusReasonCode": LastUpdateStatusReasonCodeType,
-        "FileSystemConfigs": List[FileSystemConfigOutputTypeDef],
+        "FileSystemConfigs": List[FileSystemConfigTypeDef],
         "PackageType": PackageTypeType,
         "ImageConfigResponse": ImageConfigResponseTypeDef,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
         "Architectures": List[ArchitectureType],
-        "EphemeralStorage": EphemeralStorageOutputTypeDef,
+        "EphemeralStorage": EphemeralStorageTypeDef,
         "SnapStart": SnapStartResponseTypeDef,
         "RuntimeVersionConfig": RuntimeVersionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FunctionConfigurationTypeDef = TypedDict(
     "FunctionConfigurationTypeDef",
     {
         "FunctionName": str,
@@ -2836,79 +2716,79 @@
         "Description": str,
         "Timeout": int,
         "MemorySize": int,
         "LastModified": str,
         "CodeSha256": str,
         "Version": str,
         "VpcConfig": VpcConfigResponseTypeDef,
-        "DeadLetterConfig": DeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": DeadLetterConfigTypeDef,
         "Environment": EnvironmentResponseTypeDef,
         "KMSKeyArn": str,
         "TracingConfig": TracingConfigResponseTypeDef,
         "MasterArn": str,
         "RevisionId": str,
         "Layers": List[LayerTypeDef],
         "State": StateType,
         "StateReason": str,
         "StateReasonCode": StateReasonCodeType,
         "LastUpdateStatus": LastUpdateStatusType,
         "LastUpdateStatusReason": str,
         "LastUpdateStatusReasonCode": LastUpdateStatusReasonCodeType,
-        "FileSystemConfigs": List[FileSystemConfigOutputTypeDef],
+        "FileSystemConfigs": List[FileSystemConfigTypeDef],
         "PackageType": PackageTypeType,
         "ImageConfigResponse": ImageConfigResponseTypeDef,
         "SigningProfileVersionArn": str,
         "SigningJobArn": str,
         "Architectures": List[ArchitectureType],
-        "EphemeralStorage": EphemeralStorageOutputTypeDef,
+        "EphemeralStorage": EphemeralStorageTypeDef,
         "SnapStart": SnapStartResponseTypeDef,
         "RuntimeVersionConfig": RuntimeVersionConfigTypeDef,
     },
     total=False,
 )
 
 ListFunctionEventInvokeConfigsResponseTypeDef = TypedDict(
     "ListFunctionEventInvokeConfigsResponseTypeDef",
     {
         "FunctionEventInvokeConfigs": List[FunctionEventInvokeConfigTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEventSourceMappingsResponseTypeDef = TypedDict(
     "ListEventSourceMappingsResponseTypeDef",
     {
         "NextMarker": str,
         "EventSourceMappings": List[EventSourceMappingConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFunctionResponseTypeDef = TypedDict(
     "GetFunctionResponseTypeDef",
     {
         "Configuration": FunctionConfigurationTypeDef,
         "Code": FunctionCodeLocationTypeDef,
         "Tags": Dict[str, str],
         "Concurrency": ConcurrencyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionsResponseTypeDef = TypedDict(
     "ListFunctionsResponseTypeDef",
     {
         "NextMarker": str,
         "Functions": List[FunctionConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVersionsByFunctionResponseTypeDef = TypedDict(
     "ListVersionsByFunctionResponseTypeDef",
     {
         "NextMarker": str,
         "Versions": List[FunctionConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/waiter.py` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda/waiter.pyi` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/PKG-INFO` & `mypy-boto3-lambda-1.28.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-lambda
-Version: 1.28.12
-Summary: Type annotations for boto3.Lambda 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 lambda type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-lambda"></a>
 
 # mypy-boto3-lambda
 
 [![PyPI - mypy-boto3-lambda](https://img.shields.io/pypi/v/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lambda.svg?color=blue)](https://pypi.org/project/mypy-boto3-lambda)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lambda)](https://pepy.tech/project/mypy-boto3-lambda)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lambda 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
+[boto3.Lambda 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lambda.html#Lambda)
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
 [mypy-boto3-lambda docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lambda/).
 
 See how it helps to find and fix potential bugs:
 
@@ -461,26 +429,22 @@
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lambda.type_defs import (
     AccountLimitTypeDef,
     AccountUsageTypeDef,
     AddLayerVersionPermissionRequestRequestTypeDef,
-    AddLayerVersionPermissionResponseTypeDef,
+    ResponseMetadataTypeDef,
     AddPermissionRequestRequestTypeDef,
-    AddPermissionResponseTypeDef,
     AliasRoutingConfigurationOutputTypeDef,
     AliasRoutingConfigurationTypeDef,
     AllowedPublishersOutputTypeDef,
     AllowedPublishersTypeDef,
-    AmazonManagedKafkaEventSourceConfigOutputTypeDef,
     AmazonManagedKafkaEventSourceConfigTypeDef,
-    CodeSigningPoliciesOutputTypeDef,
     CodeSigningPoliciesTypeDef,
-    ConcurrencyResponseMetadataTypeDef,
     ConcurrencyTypeDef,
     CorsOutputTypeDef,
     CorsTypeDef,
     DocumentDBEventSourceConfigTypeDef,
     ScalingConfigTypeDef,
     SelfManagedEventSourceTypeDef,
     SelfManagedKafkaEventSourceConfigTypeDef,
@@ -490,138 +454,118 @@
     EphemeralStorageTypeDef,
     FileSystemConfigTypeDef,
     FunctionCodeTypeDef,
     ImageConfigTypeDef,
     SnapStartTypeDef,
     TracingConfigTypeDef,
     VpcConfigTypeDef,
-    DeadLetterConfigOutputTypeDef,
     DeleteAliasRequestRequestTypeDef,
     DeleteCodeSigningConfigRequestRequestTypeDef,
     DeleteEventSourceMappingRequestRequestTypeDef,
     DeleteFunctionCodeSigningConfigRequestRequestTypeDef,
     DeleteFunctionConcurrencyRequestRequestTypeDef,
     DeleteFunctionEventInvokeConfigRequestRequestTypeDef,
     DeleteFunctionRequestRequestTypeDef,
     DeleteFunctionUrlConfigRequestRequestTypeDef,
     DeleteLayerVersionRequestRequestTypeDef,
     DeleteProvisionedConcurrencyConfigRequestRequestTypeDef,
-    OnFailureOutputTypeDef,
-    OnSuccessOutputTypeDef,
     OnFailureTypeDef,
     OnSuccessTypeDef,
-    DocumentDBEventSourceConfigOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnvironmentErrorTypeDef,
-    EphemeralStorageOutputTypeDef,
-    ScalingConfigOutputTypeDef,
     SelfManagedEventSourceOutputTypeDef,
-    SelfManagedKafkaEventSourceConfigOutputTypeDef,
-    SourceAccessConfigurationOutputTypeDef,
-    FileSystemConfigOutputTypeDef,
-    FilterOutputTypeDef,
     FilterTypeDef,
     FunctionCodeLocationTypeDef,
     LayerTypeDef,
     SnapStartResponseTypeDef,
     TracingConfigResponseTypeDef,
     VpcConfigResponseTypeDef,
     GetAliasRequestRequestTypeDef,
     GetCodeSigningConfigRequestRequestTypeDef,
     GetEventSourceMappingRequestRequestTypeDef,
     GetFunctionCodeSigningConfigRequestRequestTypeDef,
-    GetFunctionCodeSigningConfigResponseTypeDef,
     GetFunctionConcurrencyRequestRequestTypeDef,
-    GetFunctionConcurrencyResponseTypeDef,
     WaiterConfigTypeDef,
     GetFunctionConfigurationRequestRequestTypeDef,
     GetFunctionEventInvokeConfigRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetFunctionUrlConfigRequestRequestTypeDef,
     GetLayerVersionByArnRequestRequestTypeDef,
     GetLayerVersionPolicyRequestRequestTypeDef,
-    GetLayerVersionPolicyResponseTypeDef,
     GetLayerVersionRequestRequestTypeDef,
     LayerVersionContentOutputTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetProvisionedConcurrencyConfigRequestRequestTypeDef,
-    GetProvisionedConcurrencyConfigResponseTypeDef,
     GetRuntimeManagementConfigRequestRequestTypeDef,
-    GetRuntimeManagementConfigResponseTypeDef,
     ImageConfigErrorTypeDef,
     ImageConfigOutputTypeDef,
     InvocationRequestRequestTypeDef,
-    InvocationResponseTypeDef,
     InvokeAsyncRequestRequestTypeDef,
-    InvokeAsyncResponseTypeDef,
     InvokeResponseStreamUpdateTypeDef,
     InvokeWithResponseStreamCompleteEventTypeDef,
     InvokeWithResponseStreamRequestRequestTypeDef,
     LayerVersionContentInputTypeDef,
     LayerVersionsListItemTypeDef,
-    ListAliasesRequestListAliasesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAliasesRequestRequestTypeDef,
-    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
     ListCodeSigningConfigsRequestRequestTypeDef,
-    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
     ListEventSourceMappingsRequestRequestTypeDef,
-    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
     ListFunctionEventInvokeConfigsRequestRequestTypeDef,
-    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
     ListFunctionUrlConfigsRequestRequestTypeDef,
-    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
     ListFunctionsByCodeSigningConfigRequestRequestTypeDef,
-    ListFunctionsByCodeSigningConfigResponseTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
     ListLayerVersionsRequestRequestTypeDef,
-    ListLayersRequestListLayersPaginateTypeDef,
     ListLayersRequestRequestTypeDef,
-    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
     ListProvisionedConcurrencyConfigsRequestRequestTypeDef,
     ProvisionedConcurrencyConfigListItemTypeDef,
     ListTagsRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
-    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListVersionsByFunctionRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PublishVersionRequestRequestTypeDef,
     PutFunctionCodeSigningConfigRequestRequestTypeDef,
-    PutFunctionCodeSigningConfigResponseTypeDef,
     PutFunctionConcurrencyRequestRequestTypeDef,
     PutProvisionedConcurrencyConfigRequestRequestTypeDef,
-    PutProvisionedConcurrencyConfigResponseTypeDef,
     PutRuntimeManagementConfigRequestRequestTypeDef,
-    PutRuntimeManagementConfigResponseTypeDef,
     RemoveLayerVersionPermissionRequestRequestTypeDef,
     RemovePermissionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeVersionErrorTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFunctionCodeRequestRequestTypeDef,
+    AddLayerVersionPermissionResponseTypeDef,
+    AddPermissionResponseTypeDef,
+    ConcurrencyResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetAccountSettingsResponseTypeDef,
-    AliasConfigurationResponseMetadataTypeDef,
+    GetFunctionCodeSigningConfigResponseTypeDef,
+    GetFunctionConcurrencyResponseTypeDef,
+    GetLayerVersionPolicyResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetProvisionedConcurrencyConfigResponseTypeDef,
+    GetRuntimeManagementConfigResponseTypeDef,
+    InvocationResponseTypeDef,
+    InvokeAsyncResponseTypeDef,
+    ListFunctionsByCodeSigningConfigResponseTypeDef,
+    ListTagsResponseTypeDef,
+    PutFunctionCodeSigningConfigResponseTypeDef,
+    PutProvisionedConcurrencyConfigResponseTypeDef,
+    PutRuntimeManagementConfigResponseTypeDef,
+    AliasConfigurationResponseTypeDef,
     AliasConfigurationTypeDef,
     CreateAliasRequestRequestTypeDef,
     UpdateAliasRequestRequestTypeDef,
     CodeSigningConfigTypeDef,
     CreateCodeSigningConfigRequestRequestTypeDef,
     UpdateCodeSigningConfigRequestRequestTypeDef,
     CreateFunctionUrlConfigResponseTypeDef,
     FunctionUrlConfigTypeDef,
     GetFunctionUrlConfigResponseTypeDef,
     UpdateFunctionUrlConfigResponseTypeDef,
     CreateFunctionUrlConfigRequestRequestTypeDef,
     UpdateFunctionUrlConfigRequestRequestTypeDef,
     CreateFunctionRequestRequestTypeDef,
     UpdateFunctionConfigurationRequestRequestTypeDef,
-    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     EnvironmentResponseTypeDef,
     FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     GetFunctionConfigurationRequestFunctionActiveWaitTypeDef,
     GetFunctionConfigurationRequestFunctionUpdatedWaitTypeDef,
     GetFunctionConfigurationRequestPublishedVersionActiveWaitTypeDef,
@@ -631,33 +575,44 @@
     GetLayerVersionResponseTypeDef,
     PublishLayerVersionResponseTypeDef,
     ImageConfigResponseTypeDef,
     InvokeWithResponseStreamResponseEventTypeDef,
     PublishLayerVersionRequestRequestTypeDef,
     LayersListItemTypeDef,
     ListLayerVersionsResponseTypeDef,
+    ListAliasesRequestListAliasesPaginateTypeDef,
+    ListCodeSigningConfigsRequestListCodeSigningConfigsPaginateTypeDef,
+    ListEventSourceMappingsRequestListEventSourceMappingsPaginateTypeDef,
+    ListFunctionEventInvokeConfigsRequestListFunctionEventInvokeConfigsPaginateTypeDef,
+    ListFunctionUrlConfigsRequestListFunctionUrlConfigsPaginateTypeDef,
+    ListFunctionsByCodeSigningConfigRequestListFunctionsByCodeSigningConfigPaginateTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
+    ListLayerVersionsRequestListLayerVersionsPaginateTypeDef,
+    ListLayersRequestListLayersPaginateTypeDef,
+    ListProvisionedConcurrencyConfigsRequestListProvisionedConcurrencyConfigsPaginateTypeDef,
+    ListVersionsByFunctionRequestListVersionsByFunctionPaginateTypeDef,
     ListProvisionedConcurrencyConfigsResponseTypeDef,
     RuntimeVersionConfigTypeDef,
     ListAliasesResponseTypeDef,
     CreateCodeSigningConfigResponseTypeDef,
     GetCodeSigningConfigResponseTypeDef,
     ListCodeSigningConfigsResponseTypeDef,
     UpdateCodeSigningConfigResponseTypeDef,
     ListFunctionUrlConfigsResponseTypeDef,
-    FunctionEventInvokeConfigResponseMetadataTypeDef,
+    FunctionEventInvokeConfigResponseTypeDef,
     FunctionEventInvokeConfigTypeDef,
     PutFunctionEventInvokeConfigRequestRequestTypeDef,
     UpdateFunctionEventInvokeConfigRequestRequestTypeDef,
-    EventSourceMappingConfigurationResponseMetadataTypeDef,
+    EventSourceMappingConfigurationResponseTypeDef,
     EventSourceMappingConfigurationTypeDef,
     CreateEventSourceMappingRequestRequestTypeDef,
     UpdateEventSourceMappingRequestRequestTypeDef,
     InvokeWithResponseStreamResponseTypeDef,
     ListLayersResponseTypeDef,
-    FunctionConfigurationResponseMetadataTypeDef,
+    FunctionConfigurationResponseTypeDef,
     FunctionConfigurationTypeDef,
     ListFunctionEventInvokeConfigsResponseTypeDef,
     ListEventSourceMappingsResponseTypeDef,
     GetFunctionResponseTypeDef,
     ListFunctionsResponseTypeDef,
     ListVersionsByFunctionResponseTypeDef,
 )
```

### Comparing `mypy-boto3-lambda-1.28.12/mypy_boto3_lambda.egg-info/SOURCES.txt` & `mypy-boto3-lambda-1.28.15/mypy_boto3_lambda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lambda-1.28.12/setup.py` & `mypy-boto3-lambda-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lambda",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_lambda"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lambda 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Lambda 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

