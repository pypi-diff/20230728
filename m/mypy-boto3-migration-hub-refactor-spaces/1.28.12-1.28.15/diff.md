# Comparing `tmp/mypy-boto3-migration-hub-refactor-spaces-1.28.12.tar.gz` & `tmp/mypy-boto3-migration-hub-refactor-spaces-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.28.12.tar", last modified: Thu Jul 27 05:35:03 2023, max compression
+gzip compressed data, was "mypy-boto3-migration-hub-refactor-spaces-1.28.15.tar", last modified: Fri Jul 28 20:43:18 2023, max compression
```

## Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12.tar` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.180433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-07-27 05:35:03.172433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.168433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6936 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29910 2023-07-27 05:26:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29877 2023-07-27 05:26:40.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:03.172433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17337 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-27 05:35:03.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:03.180433 mypy-boto3-migration-hub-refactor-spaces-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-27 05:26:39.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15653 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22768 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10249 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    28978 2023-07-28 20:32:02.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28947 2023-07-28 20:32:01.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-28 20:43:18.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:18.757522 mypy-boto3-migration-hub-refactor-spaces-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-28 20:32:00.000000 mypy-boto3-migration-hub-refactor-spaces-1.28.15/setup.py
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/LICENSE` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,80 +349,77 @@
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
-    ApiGatewayProxyInputOutputTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
     UriPathRouteInputOutputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
-    LambdaEndpointInputOutputTypeDef,
-    UrlEndpointInputOutputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
-    DeleteRouteResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     EnvironmentVpcTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     LambdaEndpointConfigTypeDef,
     UrlEndpointConfigTypeDef,
     LambdaEndpointSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentVpcsRequestRequestTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListRoutesRequestListRoutesPaginateTypeDef,
     ListRoutesRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseTypeDef,
-    CreateApplicationResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    RouteSummaryTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    DeleteApplicationResponseTypeDef,
+    DeleteEnvironmentResponseTypeDef,
+    DeleteRouteResponseTypeDef,
+    DeleteServiceResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
-    RouteSummaryTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateRouteResponseTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
+    ListRoutesRequestListRoutesPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ServiceSummaryTypeDef,
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/README.md` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -317,80 +317,77 @@
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
-    ApiGatewayProxyInputOutputTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
     UriPathRouteInputOutputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
-    LambdaEndpointInputOutputTypeDef,
-    UrlEndpointInputOutputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
-    DeleteRouteResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     EnvironmentVpcTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     LambdaEndpointConfigTypeDef,
     UrlEndpointConfigTypeDef,
     LambdaEndpointSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentVpcsRequestRequestTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListRoutesRequestListRoutesPaginateTypeDef,
     ListRoutesRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseTypeDef,
-    CreateApplicationResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    RouteSummaryTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    DeleteApplicationResponseTypeDef,
+    DeleteEnvironmentResponseTypeDef,
+    DeleteRouteResponseTypeDef,
+    DeleteServiceResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
-    RouteSummaryTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateRouteResponseTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
+    ListRoutesRequestListRoutesPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ServiceSummaryTypeDef,
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__init__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/__main__.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces\nOther"
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

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/client.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/client.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/literals.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/literals.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/paginator.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,45 +62,45 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, EnvironmentIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EnvironmentIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listapplicationspaginator)
         """
 
 
 class ListEnvironmentVpcsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentvpcspaginator)
     """
 
     def paginate(
-        self, *, EnvironmentIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EnvironmentIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnvironmentVpcsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentvpcspaginator)
         """
 
 
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentspaginator)
         """
 
 
@@ -111,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listroutespaginator)
         """
 
 
@@ -130,13 +130,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -59,43 +59,43 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, EnvironmentIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EnvironmentIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listapplicationspaginator)
         """
 
 class ListEnvironmentVpcsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentvpcspaginator)
     """
 
     def paginate(
-        self, *, EnvironmentIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, EnvironmentIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnvironmentVpcsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironmentVpcs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentvpcspaginator)
         """
 
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listenvironmentspaginator)
         """
 
 class ListRoutesPaginator(Paginator):
@@ -105,15 +105,15 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listroutespaginator)
         """
 
 class ListServicesPaginator(Paginator):
@@ -123,13 +123,13 @@
     """
 
     def paginate(
         self,
         *,
         ApplicationIdentifier: str,
         EnvironmentIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces.Paginator.ListServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/paginators/#listservicespaginator)
         """
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/type_defs.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,80 +38,77 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApiGatewayProxyConfigTypeDef",
-    "ApiGatewayProxyInputOutputTypeDef",
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "CreateEnvironmentResponseTypeDef",
     "DefaultRouteInputTypeDef",
     "UriPathRouteInputTypeDef",
     "UriPathRouteInputOutputTypeDef",
     "LambdaEndpointInputTypeDef",
     "UrlEndpointInputTypeDef",
-    "LambdaEndpointInputOutputTypeDef",
-    "UrlEndpointInputOutputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
-    "DeleteApplicationResponseTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
-    "DeleteEnvironmentResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
-    "DeleteRouteResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
-    "DeleteServiceResponseTypeDef",
     "EnvironmentVpcTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetServiceRequestRequestTypeDef",
     "LambdaEndpointConfigTypeDef",
     "UrlEndpointConfigTypeDef",
     "LambdaEndpointSummaryTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
     "ListEnvironmentVpcsRequestRequestTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
-    "ListRoutesRequestListRoutesPaginateTypeDef",
     "ListRoutesRequestRequestTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UrlEndpointSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRouteRequestRequestTypeDef",
-    "UpdateRouteResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ApplicationSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
+    "RouteSummaryTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "CreateEnvironmentResponseTypeDef",
+    "DeleteApplicationResponseTypeDef",
+    "DeleteEnvironmentResponseTypeDef",
+    "DeleteRouteResponseTypeDef",
+    "DeleteServiceResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "GetEnvironmentResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetRouteResponseTypeDef",
-    "RouteSummaryTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateRouteResponseTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "ListEnvironmentVpcsResponseTypeDef",
     "GetServiceResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    "ListRoutesRequestListRoutesPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ServiceSummaryTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "ListRoutesResponseTypeDef",
     "ListServicesResponseTypeDef",
 )
 
@@ -125,23 +122,14 @@
         "ProxyUrl": str,
         "StageName": str,
         "VpcLinkId": str,
     },
     total=False,
 )
 
-ApiGatewayProxyInputOutputTypeDef = TypedDict(
-    "ApiGatewayProxyInputOutputTypeDef",
-    {
-        "EndpointType": ApiGatewayEndpointTypeType,
-        "StageName": str,
-    },
-    total=False,
-)
-
 ApiGatewayProxyInputTypeDef = TypedDict(
     "ApiGatewayProxyInputTypeDef",
     {
         "EndpointType": ApiGatewayEndpointTypeType,
         "StageName": str,
     },
     total=False,
@@ -170,14 +158,25 @@
         "Message": str,
         "ResourceIdentifier": str,
         "ResourceType": ErrorResourceTypeType,
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
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
     },
 )
@@ -194,31 +193,14 @@
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "Arn": str,
-        "CreatedTime": datetime,
-        "Description": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "NetworkFabricType": NetworkFabricTypeType,
-        "OwnerAccountId": str,
-        "State": EnvironmentStateType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DefaultRouteInputTypeDef = TypedDict(
     "DefaultRouteInputTypeDef",
     {
         "ActivationState": RouteActivationStateType,
     },
     total=False,
 )
@@ -293,82 +275,29 @@
 )
 
 
 class UrlEndpointInputTypeDef(_RequiredUrlEndpointInputTypeDef, _OptionalUrlEndpointInputTypeDef):
     pass
 
 
-LambdaEndpointInputOutputTypeDef = TypedDict(
-    "LambdaEndpointInputOutputTypeDef",
-    {
-        "Arn": str,
-    },
-)
-
-_RequiredUrlEndpointInputOutputTypeDef = TypedDict(
-    "_RequiredUrlEndpointInputOutputTypeDef",
-    {
-        "Url": str,
-    },
-)
-_OptionalUrlEndpointInputOutputTypeDef = TypedDict(
-    "_OptionalUrlEndpointInputOutputTypeDef",
-    {
-        "HealthUrl": str,
-    },
-    total=False,
-)
-
-
-class UrlEndpointInputOutputTypeDef(
-    _RequiredUrlEndpointInputOutputTypeDef, _OptionalUrlEndpointInputOutputTypeDef
-):
-    pass
-
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
 
-DeleteApplicationResponseTypeDef = TypedDict(
-    "DeleteApplicationResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "State": ApplicationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 
-DeleteEnvironmentResponseTypeDef = TypedDict(
-    "DeleteEnvironmentResponseTypeDef",
-    {
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "State": EnvironmentStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -377,50 +306,23 @@
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
 )
 
-DeleteRouteResponseTypeDef = TypedDict(
-    "DeleteRouteResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "LastUpdatedTime": datetime,
-        "RouteId": str,
-        "ServiceId": str,
-        "State": RouteStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "ServiceIdentifier": str,
     },
 )
 
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "ServiceId": str,
-        "State": ServiceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentVpcTypeDef = TypedDict(
     "EnvironmentVpcTypeDef",
     {
         "AccountId": str,
         "CidrBlocks": List[str],
         "CreatedTime": datetime,
         "EnvironmentId": str,
@@ -449,22 +351,14 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRouteRequestRequestTypeDef = TypedDict(
     "GetRouteRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
@@ -500,36 +394,24 @@
     "LambdaEndpointSummaryTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-_RequiredListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationsRequestListApplicationsPaginateTypeDef",
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
-class ListApplicationsRequestListApplicationsPaginateTypeDef(
-    _RequiredListApplicationsRequestListApplicationsPaginateTypeDef,
-    _OptionalListApplicationsRequestListApplicationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApplicationsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationsRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 _OptionalListApplicationsRequestRequestTypeDef = TypedDict(
@@ -544,36 +426,14 @@
 
 class ListApplicationsRequestRequestTypeDef(
     _RequiredListApplicationsRequestRequestTypeDef, _OptionalListApplicationsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    {
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(
-    _RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    _OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEnvironmentVpcsRequestRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentVpcsRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 _OptionalListEnvironmentVpcsRequestRequestTypeDef = TypedDict(
@@ -589,54 +449,23 @@
 class ListEnvironmentVpcsRequestRequestTypeDef(
     _RequiredListEnvironmentVpcsRequestRequestTypeDef,
     _OptionalListEnvironmentVpcsRequestRequestTypeDef,
 ):
     pass
 
 
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesRequestListRoutesPaginateTypeDef",
-    {
-        "ApplicationIdentifier": str,
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesRequestListRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRoutesRequestListRoutesPaginateTypeDef(
-    _RequiredListRoutesRequestListRoutesPaginateTypeDef,
-    _OptionalListRoutesRequestListRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutesRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -652,37 +481,14 @@
 
 class ListRoutesRequestRequestTypeDef(
     _RequiredListRoutesRequestRequestTypeDef, _OptionalListRoutesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "_RequiredListServicesRequestListServicesPaginateTypeDef",
-    {
-        "ApplicationIdentifier": str,
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "_OptionalListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListServicesRequestListServicesPaginateTypeDef(
-    _RequiredListServicesRequestListServicesPaginateTypeDef,
-    _OptionalListServicesRequestListServicesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListServicesRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -705,51 +511,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
         "ResourceArn": str,
     },
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
 UrlEndpointSummaryTypeDef = TypedDict(
     "UrlEndpointSummaryTypeDef",
     {
         "HealthUrl": str,
         "Url": str,
     },
     total=False,
@@ -777,47 +554,14 @@
         "ActivationState": RouteActivationStateType,
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
 )
 
-UpdateRouteResponseTypeDef = TypedDict(
-    "UpdateRouteResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "LastUpdatedTime": datetime,
-        "RouteId": str,
-        "ServiceId": str,
-        "State": RouteStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "ApiGatewayProxy": ApiGatewayProxyInputOutputTypeDef,
-        "ApplicationId": str,
-        "Arn": str,
-        "CreatedByAccountId": str,
-        "CreatedTime": datetime,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "OwnerAccountId": str,
-        "ProxyType": Literal["API_GATEWAY"],
-        "State": ApplicationStateType,
-        "Tags": Dict[str, str],
-        "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
         "Name": str,
         "ProxyType": Literal["API_GATEWAY"],
         "VpcId": str,
@@ -876,14 +620,128 @@
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
     },
     total=False,
 )
 
+RouteSummaryTypeDef = TypedDict(
+    "RouteSummaryTypeDef",
+    {
+        "AppendSourcePath": bool,
+        "ApplicationId": str,
+        "Arn": str,
+        "CreatedByAccountId": str,
+        "CreatedTime": datetime,
+        "EnvironmentId": str,
+        "Error": ErrorResponseTypeDef,
+        "IncludeChildPaths": bool,
+        "LastUpdatedTime": datetime,
+        "Methods": List[HttpMethodType],
+        "OwnerAccountId": str,
+        "PathResourceToId": Dict[str, str],
+        "RouteId": str,
+        "RouteType": RouteTypeType,
+        "ServiceId": str,
+        "SourcePath": str,
+        "State": RouteStateType,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "ApiGatewayProxy": ApiGatewayProxyInputTypeDef,
+        "ApplicationId": str,
+        "Arn": str,
+        "CreatedByAccountId": str,
+        "CreatedTime": datetime,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "OwnerAccountId": str,
+        "ProxyType": Literal["API_GATEWAY"],
+        "State": ApplicationStateType,
+        "Tags": Dict[str, str],
+        "VpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedTime": datetime,
+        "Description": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "NetworkFabricType": NetworkFabricTypeType,
+        "OwnerAccountId": str,
+        "State": EnvironmentStateType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationResponseTypeDef = TypedDict(
+    "DeleteApplicationResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "State": ApplicationStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEnvironmentResponseTypeDef = TypedDict(
+    "DeleteEnvironmentResponseTypeDef",
+    {
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "State": EnvironmentStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRouteResponseTypeDef = TypedDict(
+    "DeleteRouteResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "LastUpdatedTime": datetime,
+        "RouteId": str,
+        "ServiceId": str,
+        "State": RouteStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "ServiceId": str,
+        "State": ServiceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApiGatewayProxy": ApiGatewayProxyConfigTypeDef,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
@@ -893,15 +751,15 @@
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ProxyType": Literal["API_GATEWAY"],
         "State": ApplicationStateType,
         "Tags": Dict[str, str],
         "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "Arn": str,
@@ -912,15 +770,23 @@
         "LastUpdatedTime": datetime,
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponseTypeDef = TypedDict(
     "GetRouteResponseTypeDef",
     {
         "AppendSourcePath": bool,
@@ -937,41 +803,37 @@
         "PathResourceToId": Dict[str, str],
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "SourcePath": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RouteSummaryTypeDef = TypedDict(
-    "RouteSummaryTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRouteResponseTypeDef = TypedDict(
+    "UpdateRouteResponseTypeDef",
     {
-        "AppendSourcePath": bool,
         "ApplicationId": str,
         "Arn": str,
-        "CreatedByAccountId": str,
-        "CreatedTime": datetime,
-        "EnvironmentId": str,
-        "Error": ErrorResponseTypeDef,
-        "IncludeChildPaths": bool,
         "LastUpdatedTime": datetime,
-        "Methods": List[HttpMethodType],
-        "OwnerAccountId": str,
-        "PathResourceToId": Dict[str, str],
         "RouteId": str,
-        "RouteType": RouteTypeType,
         "ServiceId": str,
-        "SourcePath": str,
         "State": RouteStateType,
-        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
@@ -1008,15 +870,15 @@
         "OwnerAccountId": str,
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
         "UriPathRoute": UriPathRouteInputOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
@@ -1051,33 +913,33 @@
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "Description": str,
         "EndpointType": ServiceEndpointTypeType,
         "EnvironmentId": str,
-        "LambdaEndpoint": LambdaEndpointInputOutputTypeDef,
+        "LambdaEndpoint": LambdaEndpointInputTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
-        "UrlEndpoint": UrlEndpointInputOutputTypeDef,
+        "UrlEndpoint": UrlEndpointInputTypeDef,
         "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentVpcsResponseTypeDef = TypedDict(
     "ListEnvironmentVpcsResponseTypeDef",
     {
         "EnvironmentVpcList": List[EnvironmentVpcTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "ApplicationId": str,
@@ -1093,18 +955,116 @@
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
         "UrlEndpoint": UrlEndpointConfigTypeDef,
         "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListApplicationsRequestListApplicationsPaginateTypeDef(
+    _RequiredListApplicationsRequestListApplicationsPaginateTypeDef,
+    _OptionalListApplicationsRequestListApplicationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    {
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(
+    _RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+    _OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+):
+    pass
+
+
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesRequestListRoutesPaginateTypeDef",
+    {
+        "ApplicationIdentifier": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesRequestListRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListRoutesRequestListRoutesPaginateTypeDef(
+    _RequiredListRoutesRequestListRoutesPaginateTypeDef,
+    _OptionalListRoutesRequestListRoutesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "_RequiredListServicesRequestListServicesPaginateTypeDef",
+    {
+        "ApplicationIdentifier": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "_OptionalListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListServicesRequestListServicesPaginateTypeDef(
+    _RequiredListServicesRequestListServicesPaginateTypeDef,
+    _OptionalListServicesRequestListServicesPaginateTypeDef,
+):
+    pass
+
+
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
@@ -1126,37 +1086,37 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaryList": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "EnvironmentSummaryList": List[EnvironmentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoutesResponseTypeDef = TypedDict(
     "ListRoutesResponseTypeDef",
     {
         "NextToken": str,
         "RouteSummaryList": List[RouteSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,80 +37,77 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiGatewayProxyConfigTypeDef",
-    "ApiGatewayProxyInputOutputTypeDef",
     "ApiGatewayProxyInputTypeDef",
     "ApiGatewayProxySummaryTypeDef",
     "ErrorResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
-    "CreateEnvironmentResponseTypeDef",
     "DefaultRouteInputTypeDef",
     "UriPathRouteInputTypeDef",
     "UriPathRouteInputOutputTypeDef",
     "LambdaEndpointInputTypeDef",
     "UrlEndpointInputTypeDef",
-    "LambdaEndpointInputOutputTypeDef",
-    "UrlEndpointInputOutputTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
-    "DeleteApplicationResponseTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
-    "DeleteEnvironmentResponseTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
-    "DeleteRouteResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
-    "DeleteServiceResponseTypeDef",
     "EnvironmentVpcTypeDef",
     "GetApplicationRequestRequestTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetServiceRequestRequestTypeDef",
     "LambdaEndpointConfigTypeDef",
     "UrlEndpointConfigTypeDef",
     "LambdaEndpointSummaryTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
-    "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
     "ListEnvironmentVpcsRequestRequestTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
-    "ListRoutesRequestListRoutesPaginateTypeDef",
     "ListRoutesRequestRequestTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UrlEndpointSummaryTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateRouteRequestRequestTypeDef",
-    "UpdateRouteResponseTypeDef",
-    "CreateApplicationResponseTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ApplicationSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
+    "RouteSummaryTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "CreateEnvironmentResponseTypeDef",
+    "DeleteApplicationResponseTypeDef",
+    "DeleteEnvironmentResponseTypeDef",
+    "DeleteRouteResponseTypeDef",
+    "DeleteServiceResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "GetEnvironmentResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "GetRouteResponseTypeDef",
-    "RouteSummaryTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateRouteResponseTypeDef",
     "CreateRouteRequestRequestTypeDef",
     "CreateRouteResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "CreateServiceResponseTypeDef",
     "ListEnvironmentVpcsResponseTypeDef",
     "GetServiceResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    "ListRoutesRequestListRoutesPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
     "ServiceSummaryTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "ListRoutesResponseTypeDef",
     "ListServicesResponseTypeDef",
 )
 
@@ -124,23 +121,14 @@
         "ProxyUrl": str,
         "StageName": str,
         "VpcLinkId": str,
     },
     total=False,
 )
 
-ApiGatewayProxyInputOutputTypeDef = TypedDict(
-    "ApiGatewayProxyInputOutputTypeDef",
-    {
-        "EndpointType": ApiGatewayEndpointTypeType,
-        "StageName": str,
-    },
-    total=False,
-)
-
 ApiGatewayProxyInputTypeDef = TypedDict(
     "ApiGatewayProxyInputTypeDef",
     {
         "EndpointType": ApiGatewayEndpointTypeType,
         "StageName": str,
     },
     total=False,
@@ -169,14 +157,25 @@
         "Message": str,
         "ResourceIdentifier": str,
         "ResourceType": ErrorResourceTypeType,
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
 _RequiredCreateEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEnvironmentRequestRequestTypeDef",
     {
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
     },
 )
@@ -191,31 +190,14 @@
 )
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
-    {
-        "Arn": str,
-        "CreatedTime": datetime,
-        "Description": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "NetworkFabricType": NetworkFabricTypeType,
-        "OwnerAccountId": str,
-        "State": EnvironmentStateType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DefaultRouteInputTypeDef = TypedDict(
     "DefaultRouteInputTypeDef",
     {
         "ActivationState": RouteActivationStateType,
     },
     total=False,
 )
@@ -284,80 +266,29 @@
     },
     total=False,
 )
 
 class UrlEndpointInputTypeDef(_RequiredUrlEndpointInputTypeDef, _OptionalUrlEndpointInputTypeDef):
     pass
 
-LambdaEndpointInputOutputTypeDef = TypedDict(
-    "LambdaEndpointInputOutputTypeDef",
-    {
-        "Arn": str,
-    },
-)
-
-_RequiredUrlEndpointInputOutputTypeDef = TypedDict(
-    "_RequiredUrlEndpointInputOutputTypeDef",
-    {
-        "Url": str,
-    },
-)
-_OptionalUrlEndpointInputOutputTypeDef = TypedDict(
-    "_OptionalUrlEndpointInputOutputTypeDef",
-    {
-        "HealthUrl": str,
-    },
-    total=False,
-)
-
-class UrlEndpointInputOutputTypeDef(
-    _RequiredUrlEndpointInputOutputTypeDef, _OptionalUrlEndpointInputOutputTypeDef
-):
-    pass
-
 DeleteApplicationRequestRequestTypeDef = TypedDict(
     "DeleteApplicationRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
 
-DeleteApplicationResponseTypeDef = TypedDict(
-    "DeleteApplicationResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "State": ApplicationStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 
-DeleteEnvironmentResponseTypeDef = TypedDict(
-    "DeleteEnvironmentResponseTypeDef",
-    {
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "State": EnvironmentStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -366,50 +297,23 @@
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
 )
 
-DeleteRouteResponseTypeDef = TypedDict(
-    "DeleteRouteResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "LastUpdatedTime": datetime,
-        "RouteId": str,
-        "ServiceId": str,
-        "State": RouteStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "ServiceIdentifier": str,
     },
 )
 
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "ServiceId": str,
-        "State": ServiceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnvironmentVpcTypeDef = TypedDict(
     "EnvironmentVpcTypeDef",
     {
         "AccountId": str,
         "CidrBlocks": List[str],
         "CreatedTime": datetime,
         "EnvironmentId": str,
@@ -438,22 +342,14 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRouteRequestRequestTypeDef = TypedDict(
     "GetRouteRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
@@ -489,34 +385,24 @@
     "LambdaEndpointSummaryTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-_RequiredListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "_RequiredListApplicationsRequestListApplicationsPaginateTypeDef",
-    {
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "_OptionalListApplicationsRequestListApplicationsPaginateTypeDef",
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
 
-class ListApplicationsRequestListApplicationsPaginateTypeDef(
-    _RequiredListApplicationsRequestListApplicationsPaginateTypeDef,
-    _OptionalListApplicationsRequestListApplicationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListApplicationsRequestRequestTypeDef = TypedDict(
     "_RequiredListApplicationsRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 _OptionalListApplicationsRequestRequestTypeDef = TypedDict(
@@ -529,34 +415,14 @@
 )
 
 class ListApplicationsRequestRequestTypeDef(
     _RequiredListApplicationsRequestRequestTypeDef, _OptionalListApplicationsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
-    "_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    {
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
-    "_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(
-    _RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-    _OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEnvironmentVpcsRequestRequestTypeDef = TypedDict(
     "_RequiredListEnvironmentVpcsRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
     },
 )
 _OptionalListEnvironmentVpcsRequestRequestTypeDef = TypedDict(
@@ -570,52 +436,23 @@
 
 class ListEnvironmentVpcsRequestRequestTypeDef(
     _RequiredListEnvironmentVpcsRequestRequestTypeDef,
     _OptionalListEnvironmentVpcsRequestRequestTypeDef,
 ):
     pass
 
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesRequestListRoutesPaginateTypeDef",
-    {
-        "ApplicationIdentifier": str,
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesRequestListRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRoutesRequestListRoutesPaginateTypeDef(
-    _RequiredListRoutesRequestListRoutesPaginateTypeDef,
-    _OptionalListRoutesRequestListRoutesPaginateTypeDef,
-):
-    pass
-
 _RequiredListRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredListRoutesRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -629,35 +466,14 @@
 )
 
 class ListRoutesRequestRequestTypeDef(
     _RequiredListRoutesRequestRequestTypeDef, _OptionalListRoutesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "_RequiredListServicesRequestListServicesPaginateTypeDef",
-    {
-        "ApplicationIdentifier": str,
-        "EnvironmentIdentifier": str,
-    },
-)
-_OptionalListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "_OptionalListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListServicesRequestListServicesPaginateTypeDef(
-    _RequiredListServicesRequestListServicesPaginateTypeDef,
-    _OptionalListServicesRequestListServicesPaginateTypeDef,
-):
-    pass
-
 _RequiredListServicesRequestRequestTypeDef = TypedDict(
     "_RequiredListServicesRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
     },
 )
@@ -678,51 +494,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
         "ResourceArn": str,
     },
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
 UrlEndpointSummaryTypeDef = TypedDict(
     "UrlEndpointSummaryTypeDef",
     {
         "HealthUrl": str,
         "Url": str,
     },
     total=False,
@@ -750,47 +537,14 @@
         "ActivationState": RouteActivationStateType,
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
         "RouteIdentifier": str,
     },
 )
 
-UpdateRouteResponseTypeDef = TypedDict(
-    "UpdateRouteResponseTypeDef",
-    {
-        "ApplicationId": str,
-        "Arn": str,
-        "LastUpdatedTime": datetime,
-        "RouteId": str,
-        "ServiceId": str,
-        "State": RouteStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
-    {
-        "ApiGatewayProxy": ApiGatewayProxyInputOutputTypeDef,
-        "ApplicationId": str,
-        "Arn": str,
-        "CreatedByAccountId": str,
-        "CreatedTime": datetime,
-        "EnvironmentId": str,
-        "LastUpdatedTime": datetime,
-        "Name": str,
-        "OwnerAccountId": str,
-        "ProxyType": Literal["API_GATEWAY"],
-        "State": ApplicationStateType,
-        "Tags": Dict[str, str],
-        "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApplicationRequestRequestTypeDef",
     {
         "EnvironmentIdentifier": str,
         "Name": str,
         "ProxyType": Literal["API_GATEWAY"],
         "VpcId": str,
@@ -847,14 +601,128 @@
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
     },
     total=False,
 )
 
+RouteSummaryTypeDef = TypedDict(
+    "RouteSummaryTypeDef",
+    {
+        "AppendSourcePath": bool,
+        "ApplicationId": str,
+        "Arn": str,
+        "CreatedByAccountId": str,
+        "CreatedTime": datetime,
+        "EnvironmentId": str,
+        "Error": ErrorResponseTypeDef,
+        "IncludeChildPaths": bool,
+        "LastUpdatedTime": datetime,
+        "Methods": List[HttpMethodType],
+        "OwnerAccountId": str,
+        "PathResourceToId": Dict[str, str],
+        "RouteId": str,
+        "RouteType": RouteTypeType,
+        "ServiceId": str,
+        "SourcePath": str,
+        "State": RouteStateType,
+        "Tags": Dict[str, str],
+    },
+    total=False,
+)
+
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "ApiGatewayProxy": ApiGatewayProxyInputTypeDef,
+        "ApplicationId": str,
+        "Arn": str,
+        "CreatedByAccountId": str,
+        "CreatedTime": datetime,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "OwnerAccountId": str,
+        "ProxyType": Literal["API_GATEWAY"],
+        "State": ApplicationStateType,
+        "Tags": Dict[str, str],
+        "VpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "Arn": str,
+        "CreatedTime": datetime,
+        "Description": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "NetworkFabricType": NetworkFabricTypeType,
+        "OwnerAccountId": str,
+        "State": EnvironmentStateType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteApplicationResponseTypeDef = TypedDict(
+    "DeleteApplicationResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "State": ApplicationStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEnvironmentResponseTypeDef = TypedDict(
+    "DeleteEnvironmentResponseTypeDef",
+    {
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "State": EnvironmentStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteRouteResponseTypeDef = TypedDict(
+    "DeleteRouteResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "LastUpdatedTime": datetime,
+        "RouteId": str,
+        "ServiceId": str,
+        "State": RouteStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
+    {
+        "ApplicationId": str,
+        "Arn": str,
+        "EnvironmentId": str,
+        "LastUpdatedTime": datetime,
+        "Name": str,
+        "ServiceId": str,
+        "State": ServiceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetApplicationResponseTypeDef = TypedDict(
     "GetApplicationResponseTypeDef",
     {
         "ApiGatewayProxy": ApiGatewayProxyConfigTypeDef,
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
@@ -864,15 +732,15 @@
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ProxyType": Literal["API_GATEWAY"],
         "State": ApplicationStateType,
         "Tags": Dict[str, str],
         "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "Arn": str,
@@ -883,15 +751,23 @@
         "LastUpdatedTime": datetime,
         "Name": str,
         "NetworkFabricType": NetworkFabricTypeType,
         "OwnerAccountId": str,
         "State": EnvironmentStateType,
         "Tags": Dict[str, str],
         "TransitGatewayId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponseTypeDef = TypedDict(
     "GetRouteResponseTypeDef",
     {
         "AppendSourcePath": bool,
@@ -908,41 +784,37 @@
         "PathResourceToId": Dict[str, str],
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "SourcePath": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RouteSummaryTypeDef = TypedDict(
-    "RouteSummaryTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRouteResponseTypeDef = TypedDict(
+    "UpdateRouteResponseTypeDef",
     {
-        "AppendSourcePath": bool,
         "ApplicationId": str,
         "Arn": str,
-        "CreatedByAccountId": str,
-        "CreatedTime": datetime,
-        "EnvironmentId": str,
-        "Error": ErrorResponseTypeDef,
-        "IncludeChildPaths": bool,
         "LastUpdatedTime": datetime,
-        "Methods": List[HttpMethodType],
-        "OwnerAccountId": str,
-        "PathResourceToId": Dict[str, str],
         "RouteId": str,
-        "RouteType": RouteTypeType,
         "ServiceId": str,
-        "SourcePath": str,
         "State": RouteStateType,
-        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
         "EnvironmentIdentifier": str,
@@ -977,15 +849,15 @@
         "OwnerAccountId": str,
         "RouteId": str,
         "RouteType": RouteTypeType,
         "ServiceId": str,
         "State": RouteStateType,
         "Tags": Dict[str, str],
         "UriPathRoute": UriPathRouteInputOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "ApplicationIdentifier": str,
@@ -1018,33 +890,33 @@
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
         "Description": str,
         "EndpointType": ServiceEndpointTypeType,
         "EnvironmentId": str,
-        "LambdaEndpoint": LambdaEndpointInputOutputTypeDef,
+        "LambdaEndpoint": LambdaEndpointInputTypeDef,
         "LastUpdatedTime": datetime,
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
-        "UrlEndpoint": UrlEndpointInputOutputTypeDef,
+        "UrlEndpoint": UrlEndpointInputTypeDef,
         "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentVpcsResponseTypeDef = TypedDict(
     "ListEnvironmentVpcsResponseTypeDef",
     {
         "EnvironmentVpcList": List[EnvironmentVpcTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "ApplicationId": str,
@@ -1060,18 +932,108 @@
         "Name": str,
         "OwnerAccountId": str,
         "ServiceId": str,
         "State": ServiceStateType,
         "Tags": Dict[str, str],
         "UrlEndpoint": UrlEndpointConfigTypeDef,
         "VpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "_RequiredListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "_OptionalListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListApplicationsRequestListApplicationsPaginateTypeDef(
+    _RequiredListApplicationsRequestListApplicationsPaginateTypeDef,
+    _OptionalListApplicationsRequestListApplicationsPaginateTypeDef,
+):
+    pass
+
+_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
+    "_RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    {
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef = TypedDict(
+    "_OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef(
+    _RequiredListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+    _OptionalListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+):
+    pass
+
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesRequestListRoutesPaginateTypeDef",
+    {
+        "ApplicationIdentifier": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListRoutesRequestListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesRequestListRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRoutesRequestListRoutesPaginateTypeDef(
+    _RequiredListRoutesRequestListRoutesPaginateTypeDef,
+    _OptionalListRoutesRequestListRoutesPaginateTypeDef,
+):
+    pass
+
+_RequiredListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "_RequiredListServicesRequestListServicesPaginateTypeDef",
+    {
+        "ApplicationIdentifier": str,
+        "EnvironmentIdentifier": str,
+    },
+)
+_OptionalListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "_OptionalListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListServicesRequestListServicesPaginateTypeDef(
+    _RequiredListServicesRequestListServicesPaginateTypeDef,
+    _OptionalListServicesRequestListServicesPaginateTypeDef,
+):
+    pass
+
 ServiceSummaryTypeDef = TypedDict(
     "ServiceSummaryTypeDef",
     {
         "ApplicationId": str,
         "Arn": str,
         "CreatedByAccountId": str,
         "CreatedTime": datetime,
@@ -1093,37 +1055,37 @@
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaryList": List[ApplicationSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "EnvironmentSummaryList": List[EnvironmentSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoutesResponseTypeDef = TypedDict(
     "ListRoutesResponseTypeDef",
     {
         "NextToken": str,
         "RouteSummaryList": List[RouteSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "NextToken": str,
         "ServiceSummaryList": List[ServiceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-migration-hub-refactor-spaces
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-migration-hub-refactor-spaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-migration-hub-refactor-spaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-migration-hub-refactor-spaces)](https://pepy.tech/project/mypy-boto3-migration-hub-refactor-spaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHubRefactorSpaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
+[boto3.MigrationHubRefactorSpaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migration-hub-refactor-spaces.html#MigrationHubRefactorSpaces)
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
 [mypy-boto3-migration-hub-refactor-spaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_migration_hub_refactor_spaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,80 +349,77 @@
 
 `mypy_boto3_migration_hub_refactor_spaces.type_defs` module contains structures
 and shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_migration_hub_refactor_spaces.type_defs import (
     ApiGatewayProxyConfigTypeDef,
-    ApiGatewayProxyInputOutputTypeDef,
     ApiGatewayProxyInputTypeDef,
     ApiGatewayProxySummaryTypeDef,
     ErrorResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentResponseTypeDef,
     DefaultRouteInputTypeDef,
     UriPathRouteInputTypeDef,
     UriPathRouteInputOutputTypeDef,
     LambdaEndpointInputTypeDef,
     UrlEndpointInputTypeDef,
-    LambdaEndpointInputOutputTypeDef,
-    UrlEndpointInputOutputTypeDef,
     DeleteApplicationRequestRequestTypeDef,
-    DeleteApplicationResponseTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DeleteEnvironmentResponseTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
-    DeleteRouteResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     EnvironmentVpcTypeDef,
     GetApplicationRequestRequestTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteRequestRequestTypeDef,
     GetServiceRequestRequestTypeDef,
     LambdaEndpointConfigTypeDef,
     UrlEndpointConfigTypeDef,
     LambdaEndpointSummaryTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
-    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
     ListEnvironmentVpcsRequestRequestTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListRoutesRequestListRoutesPaginateTypeDef,
     ListRoutesRequestRequestTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UrlEndpointSummaryTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateRouteRequestRequestTypeDef,
-    UpdateRouteResponseTypeDef,
-    CreateApplicationResponseTypeDef,
     CreateApplicationRequestRequestTypeDef,
     ApplicationSummaryTypeDef,
     EnvironmentSummaryTypeDef,
+    RouteSummaryTypeDef,
+    CreateApplicationResponseTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    DeleteApplicationResponseTypeDef,
+    DeleteEnvironmentResponseTypeDef,
+    DeleteRouteResponseTypeDef,
+    DeleteServiceResponseTypeDef,
     GetApplicationResponseTypeDef,
     GetEnvironmentResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
     GetRouteResponseTypeDef,
-    RouteSummaryTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateRouteResponseTypeDef,
     CreateRouteRequestRequestTypeDef,
     CreateRouteResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     CreateServiceResponseTypeDef,
     ListEnvironmentVpcsResponseTypeDef,
     GetServiceResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    ListEnvironmentVpcsRequestListEnvironmentVpcsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
+    ListRoutesRequestListRoutesPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
     ServiceSummaryTypeDef,
     ListApplicationsResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     ListRoutesResponseTypeDef,
     ListServicesResponseTypeDef,
 )
```

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/mypy_boto3_migration_hub_refactor_spaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-migration-hub-refactor-spaces-1.28.12/setup.py` & `mypy-boto3-migration-hub-refactor-spaces-1.28.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-migration-hub-refactor-spaces",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_migration_hub_refactor_spaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MigrationHubRefactorSpaces 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

