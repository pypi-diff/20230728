# Comparing `tmp/mypy-boto3-finspace-1.28.12.tar.gz` & `tmp/mypy-boto3-finspace-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-1.28.15.tar", last modified: Fri Jul 28 20:42:49 2023, max compression
```

## Comparing `mypy-boto3-finspace-1.28.12.tar` & `mypy-boto3-finspace-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39016 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    38974 2023-07-27 05:22:14.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16597 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 05:34:41.000000 mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.000509 mypy-boto3-finspace-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 05:22:13.000000 mypy-boto3-finspace-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14734 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24718 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9772 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9770 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    36402 2023-07-28 20:25:48.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36362 2023-07-28 20:25:48.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:42:49.000000 mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:49.257116 mypy-boto3-finspace-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:25:47.000000 mypy-boto3-finspace-1.28.15/setup.py
```

### Comparing `mypy-boto3-finspace-1.28.12/LICENSE` & `mypy-boto3-finspace-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.12/PKG-INFO` & `mypy-boto3-finspace-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.28.12
-Summary: Type annotations for boto3.finspace 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,116 +333,107 @@
 ### Typed dictionaries
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
-    AutoScalingConfigurationOutputTypeDef,
     AutoScalingConfigurationTypeDef,
-    CapacityConfigurationOutputTypeDef,
     CapacityConfigurationTypeDef,
-    ChangeRequestOutputTypeDef,
     ChangeRequestTypeDef,
-    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    CreateEnvironmentResponseTypeDef,
+    ResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
-    KxCacheStorageConfigurationOutputTypeDef,
-    KxCommandLineArgumentOutputTypeDef,
-    KxSavedownStorageConfigurationOutputTypeDef,
     VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
-    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
-    CreateKxUserResponseTypeDef,
-    CustomDNSServerOutputTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
     FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
-    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
-    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
-    TransitGatewayConfigurationOutputTypeDef,
+    TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
-    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
     KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
-    TransitGatewayConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    CreateKxDatabaseResponseTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
+    CreateKxUserResponseTypeDef,
+    GetKxConnectionStringResponseTypeDef,
+    GetKxDatabaseResponseTypeDef,
+    GetKxUserResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     EnvironmentTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
+    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
     KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
-    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationOutputTypeDef:
+def get_structure() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.12/README.md` & `mypy-boto3-finspace-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,116 +301,107 @@
 ### Typed dictionaries
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
-    AutoScalingConfigurationOutputTypeDef,
     AutoScalingConfigurationTypeDef,
-    CapacityConfigurationOutputTypeDef,
     CapacityConfigurationTypeDef,
-    ChangeRequestOutputTypeDef,
     ChangeRequestTypeDef,
-    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    CreateEnvironmentResponseTypeDef,
+    ResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
-    KxCacheStorageConfigurationOutputTypeDef,
-    KxCommandLineArgumentOutputTypeDef,
-    KxSavedownStorageConfigurationOutputTypeDef,
     VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
-    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
-    CreateKxUserResponseTypeDef,
-    CustomDNSServerOutputTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
     FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
-    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
-    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
-    TransitGatewayConfigurationOutputTypeDef,
+    TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
-    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
     KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
-    TransitGatewayConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    CreateKxDatabaseResponseTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
+    CreateKxUserResponseTypeDef,
+    GetKxConnectionStringResponseTypeDef,
+    GetKxDatabaseResponseTypeDef,
+    GetKxUserResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     EnvironmentTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
+    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
     KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
-    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationOutputTypeDef:
+def get_structure() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__init__.py` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__init__.pyi` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/__main__.py` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.finspace 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.finspace 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace\nOther"
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

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/client.py` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/client.pyi` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/literals.py` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/literals.pyi` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/paginator.py` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListKxEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/paginators/#listkxenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKxEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/paginators/#listkxenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/paginator.pyi` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListKxEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/paginators/#listkxenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKxEnvironmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace.Paginator.ListKxEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/paginators/#listkxenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/type_defs.py` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for finspace service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_finspace.type_defs import AutoScalingConfigurationOutputTypeDef
+    from mypy_boto3_finspace.type_defs import AutoScalingConfigurationTypeDef
 
-    data: AutoScalingConfigurationOutputTypeDef = {...}
+    data: AutoScalingConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -35,180 +35,127 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AutoScalingConfigurationOutputTypeDef",
     "AutoScalingConfigurationTypeDef",
-    "CapacityConfigurationOutputTypeDef",
     "CapacityConfigurationTypeDef",
-    "ChangeRequestOutputTypeDef",
     "ChangeRequestTypeDef",
-    "CodeConfigurationOutputTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
-    "CreateEnvironmentResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
-    "KxCacheStorageConfigurationOutputTypeDef",
-    "KxCommandLineArgumentOutputTypeDef",
-    "KxSavedownStorageConfigurationOutputTypeDef",
     "VpcConfigurationOutputTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
-    "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
-    "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserRequestRequestTypeDef",
-    "CreateKxUserResponseTypeDef",
-    "CustomDNSServerOutputTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
     "FederationParametersOutputTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
-    "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
-    "GetKxDatabaseResponseTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
-    "TransitGatewayConfigurationOutputTypeDef",
+    "TransitGatewayConfigurationTypeDef",
     "GetKxUserRequestRequestTypeDef",
-    "GetKxUserResponseTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
     "KxDatabaseCacheConfigurationOutputTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
     "ListKxClustersRequestRequestTypeDef",
     "ListKxDatabasesRequestRequestTypeDef",
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListKxEnvironmentsRequestRequestTypeDef",
     "ListKxUsersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TransitGatewayConfigurationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
-    "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
-    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
+    "CreateEnvironmentResponseTypeDef",
+    "CreateKxDatabaseResponseTypeDef",
+    "CreateKxEnvironmentResponseTypeDef",
+    "CreateKxUserResponseTypeDef",
+    "GetKxConnectionStringResponseTypeDef",
+    "GetKxDatabaseResponseTypeDef",
+    "GetKxUserResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateKxDatabaseResponseTypeDef",
+    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
     "EnvironmentTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
+    "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
     "KxDatabaseConfigurationOutputTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
-    "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
     "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
-AutoScalingConfigurationOutputTypeDef = TypedDict(
-    "AutoScalingConfigurationOutputTypeDef",
-    {
-        "minNodeCount": int,
-        "maxNodeCount": int,
-        "autoScalingMetric": Literal["CPU_UTILIZATION_PERCENTAGE"],
-        "metricTarget": float,
-        "scaleInCooldownSeconds": float,
-        "scaleOutCooldownSeconds": float,
-    },
-    total=False,
-)
-
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
         "minNodeCount": int,
         "maxNodeCount": int,
         "autoScalingMetric": Literal["CPU_UTILIZATION_PERCENTAGE"],
         "metricTarget": float,
         "scaleInCooldownSeconds": float,
         "scaleOutCooldownSeconds": float,
     },
     total=False,
 )
 
-CapacityConfigurationOutputTypeDef = TypedDict(
-    "CapacityConfigurationOutputTypeDef",
-    {
-        "nodeType": str,
-        "nodeCount": int,
-    },
-    total=False,
-)
-
 CapacityConfigurationTypeDef = TypedDict(
     "CapacityConfigurationTypeDef",
     {
         "nodeType": str,
         "nodeCount": int,
     },
     total=False,
 )
 
-_RequiredChangeRequestOutputTypeDef = TypedDict(
-    "_RequiredChangeRequestOutputTypeDef",
-    {
-        "changeType": ChangeTypeType,
-        "dbPath": str,
-    },
-)
-_OptionalChangeRequestOutputTypeDef = TypedDict(
-    "_OptionalChangeRequestOutputTypeDef",
-    {
-        "s3Path": str,
-    },
-    total=False,
-)
-
-
-class ChangeRequestOutputTypeDef(
-    _RequiredChangeRequestOutputTypeDef, _OptionalChangeRequestOutputTypeDef
-):
-    pass
-
-
 _RequiredChangeRequestTypeDef = TypedDict(
     "_RequiredChangeRequestTypeDef",
     {
         "changeType": ChangeTypeType,
         "dbPath": str,
     },
 )
@@ -221,24 +168,14 @@
 )
 
 
 class ChangeRequestTypeDef(_RequiredChangeRequestTypeDef, _OptionalChangeRequestTypeDef):
     pass
 
 
-CodeConfigurationOutputTypeDef = TypedDict(
-    "CodeConfigurationOutputTypeDef",
-    {
-        "s3Bucket": str,
-        "s3Key": str,
-        "s3ObjectVersion": str,
-    },
-    total=False,
-)
-
 CodeConfigurationTypeDef = TypedDict(
     "CodeConfigurationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "s3ObjectVersion": str,
     },
@@ -263,21 +200,22 @@
     {
         "emailAddress": str,
         "firstName": str,
         "lastName": str,
     },
 )
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "environmentId": str,
-        "environmentArn": str,
-        "environmentUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "errorMessage": str,
@@ -318,39 +256,14 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "ipAddressType": Literal["IP_V4"],
     },
     total=False,
 )
 
-KxCacheStorageConfigurationOutputTypeDef = TypedDict(
-    "KxCacheStorageConfigurationOutputTypeDef",
-    {
-        "type": str,
-        "size": int,
-    },
-)
-
-KxCommandLineArgumentOutputTypeDef = TypedDict(
-    "KxCommandLineArgumentOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
-KxSavedownStorageConfigurationOutputTypeDef = TypedDict(
-    "KxSavedownStorageConfigurationOutputTypeDef",
-    {
-        "type": Literal["SDS01"],
-        "size": int,
-    },
-)
-
 VpcConfigurationOutputTypeDef = TypedDict(
     "VpcConfigurationOutputTypeDef",
     {
         "vpcId": str,
         "securityGroupIds": List[str],
         "subnetIds": List[str],
         "ipAddressType": Literal["IP_V4"],
@@ -378,27 +291,14 @@
 
 class CreateKxDatabaseRequestRequestTypeDef(
     _RequiredCreateKxDatabaseRequestRequestTypeDef, _OptionalCreateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
 
-CreateKxDatabaseResponseTypeDef = TypedDict(
-    "CreateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxEnvironmentRequestRequestTypeDef",
     {
         "name": str,
         "kmsKeyId": str,
     },
 )
@@ -416,28 +316,14 @@
 class CreateKxEnvironmentRequestRequestTypeDef(
     _RequiredCreateKxEnvironmentRequestRequestTypeDef,
     _OptionalCreateKxEnvironmentRequestRequestTypeDef,
 ):
     pass
 
 
-CreateKxEnvironmentResponseTypeDef = TypedDict(
-    "CreateKxEnvironmentResponseTypeDef",
-    {
-        "name": str,
-        "status": EnvironmentStatusType,
-        "environmentId": str,
-        "description": str,
-        "environmentArn": str,
-        "kmsKeyId": str,
-        "creationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKxUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxUserRequestRequestTypeDef",
     {
         "environmentId": str,
         "userName": str,
         "iamRole": str,
     },
@@ -454,33 +340,14 @@
 
 class CreateKxUserRequestRequestTypeDef(
     _RequiredCreateKxUserRequestRequestTypeDef, _OptionalCreateKxUserRequestRequestTypeDef
 ):
     pass
 
 
-CreateKxUserResponseTypeDef = TypedDict(
-    "CreateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CustomDNSServerOutputTypeDef = TypedDict(
-    "CustomDNSServerOutputTypeDef",
-    {
-        "customDNSServerName": str,
-        "customDNSServerIP": str,
-    },
-)
-
 CustomDNSServerTypeDef = TypedDict(
     "CustomDNSServerTypeDef",
     {
         "customDNSServerName": str,
         "customDNSServerIP": str,
     },
 )
@@ -580,81 +447,45 @@
     {
         "userArn": str,
         "environmentId": str,
         "clusterName": str,
     },
 )
 
-GetKxConnectionStringResponseTypeDef = TypedDict(
-    "GetKxConnectionStringResponseTypeDef",
-    {
-        "signedConnectionString": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKxDatabaseRequestRequestTypeDef = TypedDict(
     "GetKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
     },
 )
 
-GetKxDatabaseResponseTypeDef = TypedDict(
-    "GetKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "lastCompletedChangesetId": str,
-        "numBytes": int,
-        "numChangesets": int,
-        "numFiles": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKxEnvironmentRequestRequestTypeDef = TypedDict(
     "GetKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-TransitGatewayConfigurationOutputTypeDef = TypedDict(
-    "TransitGatewayConfigurationOutputTypeDef",
+TransitGatewayConfigurationTypeDef = TypedDict(
+    "TransitGatewayConfigurationTypeDef",
     {
         "transitGatewayID": str,
         "routableCIDRSpace": str,
     },
 )
 
 GetKxUserRequestRequestTypeDef = TypedDict(
     "GetKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
-GetKxUserResponseTypeDef = TypedDict(
-    "GetKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KxChangesetListEntryTypeDef = TypedDict(
     "KxChangesetListEntryTypeDef",
     {
         "changesetId": str,
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
@@ -827,18 +658,20 @@
 
 class ListKxDatabasesRequestRequestTypeDef(
     _RequiredListKxDatabasesRequestRequestTypeDef, _OptionalListKxDatabasesRequestRequestTypeDef
 ):
     pass
 
 
-ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
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
 
 ListKxEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListKxEnvironmentsRequestRequestTypeDef",
     {
@@ -873,59 +706,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
 
-TransitGatewayConfigurationTypeDef = TypedDict(
-    "TransitGatewayConfigurationTypeDef",
-    {
-        "transitGatewayID": str,
-        "routableCIDRSpace": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -949,25 +745,14 @@
 
 class UpdateKxDatabaseRequestRequestTypeDef(
     _RequiredUpdateKxDatabaseRequestRequestTypeDef, _OptionalUpdateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
 
-UpdateKxDatabaseResponseTypeDef = TypedDict(
-    "UpdateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "environmentId": str,
-        "description": str,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
@@ -1007,25 +792,14 @@
 
 class UpdateKxUserRequestRequestTypeDef(
     _RequiredUpdateKxUserRequestRequestTypeDef, _OptionalUpdateKxUserRequestRequestTypeDef
 ):
     pass
 
 
-UpdateKxUserResponseTypeDef = TypedDict(
-    "UpdateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateKxChangesetRequestRequestTypeDef = TypedDict(
     "CreateKxChangesetRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
@@ -1079,42 +853,156 @@
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "environmentArn": str,
+        "environmentUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxDatabaseResponseTypeDef = TypedDict(
+    "CreateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxEnvironmentResponseTypeDef = TypedDict(
+    "CreateKxEnvironmentResponseTypeDef",
+    {
+        "name": str,
+        "status": EnvironmentStatusType,
+        "environmentId": str,
+        "description": str,
+        "environmentArn": str,
+        "kmsKeyId": str,
+        "creationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxUserResponseTypeDef = TypedDict(
+    "CreateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxConnectionStringResponseTypeDef = TypedDict(
+    "GetKxConnectionStringResponseTypeDef",
+    {
+        "signedConnectionString": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxDatabaseResponseTypeDef = TypedDict(
+    "GetKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "lastCompletedChangesetId": str,
+        "numBytes": int,
+        "numChangesets": int,
+        "numFiles": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxUserResponseTypeDef = TypedDict(
+    "GetKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKxDatabaseResponseTypeDef = TypedDict(
+    "UpdateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "environmentId": str,
+        "description": str,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKxUserResponseTypeDef = TypedDict(
+    "UpdateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateKxChangesetResponseTypeDef = TypedDict(
     "CreateKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
-        "changeRequests": List[ChangeRequestOutputTypeDef],
+        "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKxChangesetResponseTypeDef = TypedDict(
     "GetKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
-        "changeRequests": List[ChangeRequestOutputTypeDef],
+        "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "name": str,
@@ -1143,21 +1031,21 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KxEnvironmentTypeDef = TypedDict(
     "KxEnvironmentTypeDef",
     {
         "name": str,
@@ -1167,44 +1055,68 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
     },
     total=False,
 )
 
+_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    {
+        "environmentId": str,
+    },
+)
+_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    {
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
+    _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
+    _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateKxEnvironmentNetworkResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateKxEnvironmentResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentResponseTypeDef",
     {
         "name": str,
@@ -1214,38 +1126,38 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxChangesetsResponseTypeDef = TypedDict(
     "ListKxChangesetsResponseTypeDef",
     {
         "kxChangesets": List[KxChangesetListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxClustersResponseTypeDef = TypedDict(
     "ListKxClustersResponseTypeDef",
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKxDatabaseConfigurationOutputTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationOutputTypeDef",
     {
         "databaseName": str,
@@ -1290,146 +1202,130 @@
 
 
 ListKxDatabasesResponseTypeDef = TypedDict(
     "ListKxDatabasesResponseTypeDef",
     {
         "kxDatabases": List[KxDatabaseListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxClusterNodesResponseTypeDef = TypedDict(
     "ListKxClusterNodesResponseTypeDef",
     {
         "nodes": List[KxNodeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxUsersResponseTypeDef = TypedDict(
     "ListKxUsersResponseTypeDef",
     {
         "users": List[KxUserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef",
-    {
-        "environmentId": str,
-    },
-)
-_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     {
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
-        "clientToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
-    _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
-    _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
-):
-    pass
-
-
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEnvironmentResponseTypeDef = TypedDict(
     "UpdateEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxEnvironmentsResponseTypeDef = TypedDict(
     "ListKxEnvironmentsResponseTypeDef",
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKxClusterResponseTypeDef = TypedDict(
     "CreateKxClusterResponseTypeDef",
     {
         "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
         "databases": List[KxDatabaseConfigurationOutputTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationOutputTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationOutputTypeDef,
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
-        "capacityConfiguration": CapacityConfigurationOutputTypeDef,
+        "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
         "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentOutputTypeDef],
-        "code": CodeConfigurationOutputTypeDef,
+        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
-        "savedownStorageConfiguration": KxSavedownStorageConfigurationOutputTypeDef,
+        "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKxClusterResponseTypeDef = TypedDict(
     "GetKxClusterResponseTypeDef",
     {
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
         "databases": List[KxDatabaseConfigurationOutputTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationOutputTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationOutputTypeDef,
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
-        "capacityConfiguration": CapacityConfigurationOutputTypeDef,
+        "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
         "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentOutputTypeDef],
-        "code": CodeConfigurationOutputTypeDef,
+        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
-        "savedownStorageConfiguration": KxSavedownStorageConfigurationOutputTypeDef,
+        "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
         "environmentId": str,
```

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace/type_defs.pyi` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for finspace service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_finspace.type_defs import AutoScalingConfigurationOutputTypeDef
+    from mypy_boto3_finspace.type_defs import AutoScalingConfigurationTypeDef
 
-    data: AutoScalingConfigurationOutputTypeDef = {...}
+    data: AutoScalingConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -34,178 +34,127 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AutoScalingConfigurationOutputTypeDef",
     "AutoScalingConfigurationTypeDef",
-    "CapacityConfigurationOutputTypeDef",
     "CapacityConfigurationTypeDef",
-    "ChangeRequestOutputTypeDef",
     "ChangeRequestTypeDef",
-    "CodeConfigurationOutputTypeDef",
     "CodeConfigurationTypeDef",
     "FederationParametersTypeDef",
     "SuperuserParametersTypeDef",
-    "CreateEnvironmentResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ErrorInfoTypeDef",
     "KxCacheStorageConfigurationTypeDef",
     "KxCommandLineArgumentTypeDef",
     "KxSavedownStorageConfigurationTypeDef",
     "VpcConfigurationTypeDef",
-    "KxCacheStorageConfigurationOutputTypeDef",
-    "KxCommandLineArgumentOutputTypeDef",
-    "KxSavedownStorageConfigurationOutputTypeDef",
     "VpcConfigurationOutputTypeDef",
     "CreateKxDatabaseRequestRequestTypeDef",
-    "CreateKxDatabaseResponseTypeDef",
     "CreateKxEnvironmentRequestRequestTypeDef",
-    "CreateKxEnvironmentResponseTypeDef",
     "CreateKxUserRequestRequestTypeDef",
-    "CreateKxUserResponseTypeDef",
-    "CustomDNSServerOutputTypeDef",
     "CustomDNSServerTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
     "DeleteKxClusterRequestRequestTypeDef",
     "DeleteKxDatabaseRequestRequestTypeDef",
     "DeleteKxEnvironmentRequestRequestTypeDef",
     "DeleteKxUserRequestRequestTypeDef",
     "FederationParametersOutputTypeDef",
     "GetEnvironmentRequestRequestTypeDef",
     "GetKxChangesetRequestRequestTypeDef",
     "GetKxClusterRequestRequestTypeDef",
     "GetKxConnectionStringRequestRequestTypeDef",
-    "GetKxConnectionStringResponseTypeDef",
     "GetKxDatabaseRequestRequestTypeDef",
-    "GetKxDatabaseResponseTypeDef",
     "GetKxEnvironmentRequestRequestTypeDef",
-    "TransitGatewayConfigurationOutputTypeDef",
+    "TransitGatewayConfigurationTypeDef",
     "GetKxUserRequestRequestTypeDef",
-    "GetKxUserResponseTypeDef",
     "KxChangesetListEntryTypeDef",
     "KxClusterTypeDef",
     "KxDatabaseCacheConfigurationOutputTypeDef",
     "KxDatabaseCacheConfigurationTypeDef",
     "KxDatabaseListEntryTypeDef",
     "KxNodeTypeDef",
     "KxUserTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
     "ListKxChangesetsRequestRequestTypeDef",
     "ListKxClusterNodesRequestRequestTypeDef",
     "ListKxClustersRequestRequestTypeDef",
     "ListKxDatabasesRequestRequestTypeDef",
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListKxEnvironmentsRequestRequestTypeDef",
     "ListKxUsersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "TransitGatewayConfigurationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateKxDatabaseRequestRequestTypeDef",
-    "UpdateKxDatabaseResponseTypeDef",
     "UpdateKxEnvironmentRequestRequestTypeDef",
     "UpdateKxUserRequestRequestTypeDef",
-    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentRequestRequestTypeDef",
+    "CreateEnvironmentResponseTypeDef",
+    "CreateKxDatabaseResponseTypeDef",
+    "CreateKxEnvironmentResponseTypeDef",
+    "CreateKxUserResponseTypeDef",
+    "GetKxConnectionStringResponseTypeDef",
+    "GetKxDatabaseResponseTypeDef",
+    "GetKxUserResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateKxDatabaseResponseTypeDef",
+    "UpdateKxUserResponseTypeDef",
     "CreateKxChangesetResponseTypeDef",
     "GetKxChangesetResponseTypeDef",
     "EnvironmentTypeDef",
     "GetKxEnvironmentResponseTypeDef",
     "KxEnvironmentTypeDef",
+    "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     "UpdateKxEnvironmentResponseTypeDef",
     "ListKxChangesetsResponseTypeDef",
     "ListKxClustersResponseTypeDef",
     "KxDatabaseConfigurationOutputTypeDef",
     "KxDatabaseConfigurationTypeDef",
     "ListKxDatabasesResponseTypeDef",
     "ListKxClusterNodesResponseTypeDef",
     "ListKxUsersResponseTypeDef",
-    "UpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     "GetEnvironmentResponseTypeDef",
     "ListEnvironmentsResponseTypeDef",
     "UpdateEnvironmentResponseTypeDef",
     "ListKxEnvironmentsResponseTypeDef",
     "CreateKxClusterResponseTypeDef",
     "GetKxClusterResponseTypeDef",
     "CreateKxClusterRequestRequestTypeDef",
     "UpdateKxClusterDatabasesRequestRequestTypeDef",
 )
 
-AutoScalingConfigurationOutputTypeDef = TypedDict(
-    "AutoScalingConfigurationOutputTypeDef",
-    {
-        "minNodeCount": int,
-        "maxNodeCount": int,
-        "autoScalingMetric": Literal["CPU_UTILIZATION_PERCENTAGE"],
-        "metricTarget": float,
-        "scaleInCooldownSeconds": float,
-        "scaleOutCooldownSeconds": float,
-    },
-    total=False,
-)
-
 AutoScalingConfigurationTypeDef = TypedDict(
     "AutoScalingConfigurationTypeDef",
     {
         "minNodeCount": int,
         "maxNodeCount": int,
         "autoScalingMetric": Literal["CPU_UTILIZATION_PERCENTAGE"],
         "metricTarget": float,
         "scaleInCooldownSeconds": float,
         "scaleOutCooldownSeconds": float,
     },
     total=False,
 )
 
-CapacityConfigurationOutputTypeDef = TypedDict(
-    "CapacityConfigurationOutputTypeDef",
-    {
-        "nodeType": str,
-        "nodeCount": int,
-    },
-    total=False,
-)
-
 CapacityConfigurationTypeDef = TypedDict(
     "CapacityConfigurationTypeDef",
     {
         "nodeType": str,
         "nodeCount": int,
     },
     total=False,
 )
 
-_RequiredChangeRequestOutputTypeDef = TypedDict(
-    "_RequiredChangeRequestOutputTypeDef",
-    {
-        "changeType": ChangeTypeType,
-        "dbPath": str,
-    },
-)
-_OptionalChangeRequestOutputTypeDef = TypedDict(
-    "_OptionalChangeRequestOutputTypeDef",
-    {
-        "s3Path": str,
-    },
-    total=False,
-)
-
-class ChangeRequestOutputTypeDef(
-    _RequiredChangeRequestOutputTypeDef, _OptionalChangeRequestOutputTypeDef
-):
-    pass
-
 _RequiredChangeRequestTypeDef = TypedDict(
     "_RequiredChangeRequestTypeDef",
     {
         "changeType": ChangeTypeType,
         "dbPath": str,
     },
 )
@@ -216,24 +165,14 @@
     },
     total=False,
 )
 
 class ChangeRequestTypeDef(_RequiredChangeRequestTypeDef, _OptionalChangeRequestTypeDef):
     pass
 
-CodeConfigurationOutputTypeDef = TypedDict(
-    "CodeConfigurationOutputTypeDef",
-    {
-        "s3Bucket": str,
-        "s3Key": str,
-        "s3ObjectVersion": str,
-    },
-    total=False,
-)
-
 CodeConfigurationTypeDef = TypedDict(
     "CodeConfigurationTypeDef",
     {
         "s3Bucket": str,
         "s3Key": str,
         "s3ObjectVersion": str,
     },
@@ -258,21 +197,22 @@
     {
         "emailAddress": str,
         "firstName": str,
         "lastName": str,
     },
 )
 
-CreateEnvironmentResponseTypeDef = TypedDict(
-    "CreateEnvironmentResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "environmentId": str,
-        "environmentArn": str,
-        "environmentUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ErrorInfoTypeDef = TypedDict(
     "ErrorInfoTypeDef",
     {
         "errorMessage": str,
@@ -313,39 +253,14 @@
         "securityGroupIds": Sequence[str],
         "subnetIds": Sequence[str],
         "ipAddressType": Literal["IP_V4"],
     },
     total=False,
 )
 
-KxCacheStorageConfigurationOutputTypeDef = TypedDict(
-    "KxCacheStorageConfigurationOutputTypeDef",
-    {
-        "type": str,
-        "size": int,
-    },
-)
-
-KxCommandLineArgumentOutputTypeDef = TypedDict(
-    "KxCommandLineArgumentOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
-KxSavedownStorageConfigurationOutputTypeDef = TypedDict(
-    "KxSavedownStorageConfigurationOutputTypeDef",
-    {
-        "type": Literal["SDS01"],
-        "size": int,
-    },
-)
-
 VpcConfigurationOutputTypeDef = TypedDict(
     "VpcConfigurationOutputTypeDef",
     {
         "vpcId": str,
         "securityGroupIds": List[str],
         "subnetIds": List[str],
         "ipAddressType": Literal["IP_V4"],
@@ -371,27 +286,14 @@
 )
 
 class CreateKxDatabaseRequestRequestTypeDef(
     _RequiredCreateKxDatabaseRequestRequestTypeDef, _OptionalCreateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
-CreateKxDatabaseResponseTypeDef = TypedDict(
-    "CreateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxEnvironmentRequestRequestTypeDef",
     {
         "name": str,
         "kmsKeyId": str,
     },
 )
@@ -407,28 +309,14 @@
 
 class CreateKxEnvironmentRequestRequestTypeDef(
     _RequiredCreateKxEnvironmentRequestRequestTypeDef,
     _OptionalCreateKxEnvironmentRequestRequestTypeDef,
 ):
     pass
 
-CreateKxEnvironmentResponseTypeDef = TypedDict(
-    "CreateKxEnvironmentResponseTypeDef",
-    {
-        "name": str,
-        "status": EnvironmentStatusType,
-        "environmentId": str,
-        "description": str,
-        "environmentArn": str,
-        "kmsKeyId": str,
-        "creationTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKxUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxUserRequestRequestTypeDef",
     {
         "environmentId": str,
         "userName": str,
         "iamRole": str,
     },
@@ -443,33 +331,14 @@
 )
 
 class CreateKxUserRequestRequestTypeDef(
     _RequiredCreateKxUserRequestRequestTypeDef, _OptionalCreateKxUserRequestRequestTypeDef
 ):
     pass
 
-CreateKxUserResponseTypeDef = TypedDict(
-    "CreateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CustomDNSServerOutputTypeDef = TypedDict(
-    "CustomDNSServerOutputTypeDef",
-    {
-        "customDNSServerName": str,
-        "customDNSServerIP": str,
-    },
-)
-
 CustomDNSServerTypeDef = TypedDict(
     "CustomDNSServerTypeDef",
     {
         "customDNSServerName": str,
         "customDNSServerIP": str,
     },
 )
@@ -567,81 +436,45 @@
     {
         "userArn": str,
         "environmentId": str,
         "clusterName": str,
     },
 )
 
-GetKxConnectionStringResponseTypeDef = TypedDict(
-    "GetKxConnectionStringResponseTypeDef",
-    {
-        "signedConnectionString": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKxDatabaseRequestRequestTypeDef = TypedDict(
     "GetKxDatabaseRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
     },
 )
 
-GetKxDatabaseResponseTypeDef = TypedDict(
-    "GetKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "databaseArn": str,
-        "environmentId": str,
-        "description": str,
-        "createdTimestamp": datetime,
-        "lastModifiedTimestamp": datetime,
-        "lastCompletedChangesetId": str,
-        "numBytes": int,
-        "numChangesets": int,
-        "numFiles": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetKxEnvironmentRequestRequestTypeDef = TypedDict(
     "GetKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-TransitGatewayConfigurationOutputTypeDef = TypedDict(
-    "TransitGatewayConfigurationOutputTypeDef",
+TransitGatewayConfigurationTypeDef = TypedDict(
+    "TransitGatewayConfigurationTypeDef",
     {
         "transitGatewayID": str,
         "routableCIDRSpace": str,
     },
 )
 
 GetKxUserRequestRequestTypeDef = TypedDict(
     "GetKxUserRequestRequestTypeDef",
     {
         "userName": str,
         "environmentId": str,
     },
 )
 
-GetKxUserResponseTypeDef = TypedDict(
-    "GetKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 KxChangesetListEntryTypeDef = TypedDict(
     "KxChangesetListEntryTypeDef",
     {
         "changesetId": str,
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
@@ -806,18 +639,20 @@
 )
 
 class ListKxDatabasesRequestRequestTypeDef(
     _RequiredListKxDatabasesRequestRequestTypeDef, _OptionalListKxDatabasesRequestRequestTypeDef
 ):
     pass
 
-ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
-    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
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
 
 ListKxEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListKxEnvironmentsRequestRequestTypeDef",
     {
@@ -850,59 +685,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
 
-TransitGatewayConfigurationTypeDef = TypedDict(
-    "TransitGatewayConfigurationTypeDef",
-    {
-        "transitGatewayID": str,
-        "routableCIDRSpace": str,
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -924,25 +722,14 @@
 )
 
 class UpdateKxDatabaseRequestRequestTypeDef(
     _RequiredUpdateKxDatabaseRequestRequestTypeDef, _OptionalUpdateKxDatabaseRequestRequestTypeDef
 ):
     pass
 
-UpdateKxDatabaseResponseTypeDef = TypedDict(
-    "UpdateKxDatabaseResponseTypeDef",
-    {
-        "databaseName": str,
-        "environmentId": str,
-        "description": str,
-        "lastModifiedTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateKxEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 _OptionalUpdateKxEnvironmentRequestRequestTypeDef = TypedDict(
@@ -978,25 +765,14 @@
 )
 
 class UpdateKxUserRequestRequestTypeDef(
     _RequiredUpdateKxUserRequestRequestTypeDef, _OptionalUpdateKxUserRequestRequestTypeDef
 ):
     pass
 
-UpdateKxUserResponseTypeDef = TypedDict(
-    "UpdateKxUserResponseTypeDef",
-    {
-        "userName": str,
-        "userArn": str,
-        "environmentId": str,
-        "iamRole": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateKxChangesetRequestRequestTypeDef = TypedDict(
     "CreateKxChangesetRequestRequestTypeDef",
     {
         "environmentId": str,
         "databaseName": str,
         "changeRequests": Sequence[ChangeRequestTypeDef],
         "clientToken": str,
@@ -1046,42 +822,156 @@
 )
 
 class CreateEnvironmentRequestRequestTypeDef(
     _RequiredCreateEnvironmentRequestRequestTypeDef, _OptionalCreateEnvironmentRequestRequestTypeDef
 ):
     pass
 
+CreateEnvironmentResponseTypeDef = TypedDict(
+    "CreateEnvironmentResponseTypeDef",
+    {
+        "environmentId": str,
+        "environmentArn": str,
+        "environmentUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxDatabaseResponseTypeDef = TypedDict(
+    "CreateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxEnvironmentResponseTypeDef = TypedDict(
+    "CreateKxEnvironmentResponseTypeDef",
+    {
+        "name": str,
+        "status": EnvironmentStatusType,
+        "environmentId": str,
+        "description": str,
+        "environmentArn": str,
+        "kmsKeyId": str,
+        "creationTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateKxUserResponseTypeDef = TypedDict(
+    "CreateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxConnectionStringResponseTypeDef = TypedDict(
+    "GetKxConnectionStringResponseTypeDef",
+    {
+        "signedConnectionString": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxDatabaseResponseTypeDef = TypedDict(
+    "GetKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "databaseArn": str,
+        "environmentId": str,
+        "description": str,
+        "createdTimestamp": datetime,
+        "lastModifiedTimestamp": datetime,
+        "lastCompletedChangesetId": str,
+        "numBytes": int,
+        "numChangesets": int,
+        "numFiles": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKxUserResponseTypeDef = TypedDict(
+    "GetKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKxDatabaseResponseTypeDef = TypedDict(
+    "UpdateKxDatabaseResponseTypeDef",
+    {
+        "databaseName": str,
+        "environmentId": str,
+        "description": str,
+        "lastModifiedTimestamp": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateKxUserResponseTypeDef = TypedDict(
+    "UpdateKxUserResponseTypeDef",
+    {
+        "userName": str,
+        "userArn": str,
+        "environmentId": str,
+        "iamRole": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateKxChangesetResponseTypeDef = TypedDict(
     "CreateKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
-        "changeRequests": List[ChangeRequestOutputTypeDef],
+        "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKxChangesetResponseTypeDef = TypedDict(
     "GetKxChangesetResponseTypeDef",
     {
         "changesetId": str,
         "databaseName": str,
         "environmentId": str,
-        "changeRequests": List[ChangeRequestOutputTypeDef],
+        "changeRequests": List[ChangeRequestTypeDef],
         "createdTimestamp": datetime,
         "activeFromTimestamp": datetime,
         "lastModifiedTimestamp": datetime,
         "status": ChangesetStatusType,
         "errorInfo": ErrorInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnvironmentTypeDef = TypedDict(
     "EnvironmentTypeDef",
     {
         "name": str,
@@ -1110,21 +1000,21 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KxEnvironmentTypeDef = TypedDict(
     "KxEnvironmentTypeDef",
     {
         "name": str,
@@ -1134,44 +1024,66 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
         "certificateAuthorityArn": str,
     },
     total=False,
 )
 
+_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    {
+        "environmentId": str,
+    },
+)
+_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+    {
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
+    _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
+    _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
+):
+    pass
+
 UpdateKxEnvironmentNetworkResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentNetworkResponseTypeDef",
     {
         "name": str,
         "environmentId": str,
         "awsAccountId": str,
         "status": EnvironmentStatusType,
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateKxEnvironmentResponseTypeDef = TypedDict(
     "UpdateKxEnvironmentResponseTypeDef",
     {
         "name": str,
@@ -1181,38 +1093,38 @@
         "tgwStatus": tgwStatusType,
         "dnsStatus": dnsStatusType,
         "errorMessage": str,
         "description": str,
         "environmentArn": str,
         "kmsKeyId": str,
         "dedicatedServiceAccountId": str,
-        "transitGatewayConfiguration": TransitGatewayConfigurationOutputTypeDef,
-        "customDNSConfiguration": List[CustomDNSServerOutputTypeDef],
+        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
+        "customDNSConfiguration": List[CustomDNSServerTypeDef],
         "creationTimestamp": datetime,
         "updateTimestamp": datetime,
         "availabilityZoneIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxChangesetsResponseTypeDef = TypedDict(
     "ListKxChangesetsResponseTypeDef",
     {
         "kxChangesets": List[KxChangesetListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxClustersResponseTypeDef = TypedDict(
     "ListKxClustersResponseTypeDef",
     {
         "kxClusterSummaries": List[KxClusterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKxDatabaseConfigurationOutputTypeDef = TypedDict(
     "_RequiredKxDatabaseConfigurationOutputTypeDef",
     {
         "databaseName": str,
@@ -1253,144 +1165,130 @@
     pass
 
 ListKxDatabasesResponseTypeDef = TypedDict(
     "ListKxDatabasesResponseTypeDef",
     {
         "kxDatabases": List[KxDatabaseListEntryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxClusterNodesResponseTypeDef = TypedDict(
     "ListKxClusterNodesResponseTypeDef",
     {
         "nodes": List[KxNodeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxUsersResponseTypeDef = TypedDict(
     "ListKxUsersResponseTypeDef",
     {
         "users": List[KxUserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef",
-    {
-        "environmentId": str,
-    },
-)
-_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef",
+ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef = TypedDict(
+    "ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef",
     {
-        "transitGatewayConfiguration": TransitGatewayConfigurationTypeDef,
-        "customDNSConfiguration": Sequence[CustomDNSServerTypeDef],
-        "clientToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class UpdateKxEnvironmentNetworkRequestRequestTypeDef(
-    _RequiredUpdateKxEnvironmentNetworkRequestRequestTypeDef,
-    _OptionalUpdateKxEnvironmentNetworkRequestRequestTypeDef,
-):
-    pass
-
 GetEnvironmentResponseTypeDef = TypedDict(
     "GetEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnvironmentsResponseTypeDef = TypedDict(
     "ListEnvironmentsResponseTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEnvironmentResponseTypeDef = TypedDict(
     "UpdateEnvironmentResponseTypeDef",
     {
         "environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListKxEnvironmentsResponseTypeDef = TypedDict(
     "ListKxEnvironmentsResponseTypeDef",
     {
         "environments": List[KxEnvironmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKxClusterResponseTypeDef = TypedDict(
     "CreateKxClusterResponseTypeDef",
     {
         "environmentId": str,
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
         "databases": List[KxDatabaseConfigurationOutputTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationOutputTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationOutputTypeDef,
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
-        "capacityConfiguration": CapacityConfigurationOutputTypeDef,
+        "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
         "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentOutputTypeDef],
-        "code": CodeConfigurationOutputTypeDef,
+        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
-        "savedownStorageConfiguration": KxSavedownStorageConfigurationOutputTypeDef,
+        "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKxClusterResponseTypeDef = TypedDict(
     "GetKxClusterResponseTypeDef",
     {
         "status": KxClusterStatusType,
         "statusReason": str,
         "clusterName": str,
         "clusterType": KxClusterTypeType,
         "databases": List[KxDatabaseConfigurationOutputTypeDef],
-        "cacheStorageConfigurations": List[KxCacheStorageConfigurationOutputTypeDef],
-        "autoScalingConfiguration": AutoScalingConfigurationOutputTypeDef,
+        "cacheStorageConfigurations": List[KxCacheStorageConfigurationTypeDef],
+        "autoScalingConfiguration": AutoScalingConfigurationTypeDef,
         "clusterDescription": str,
-        "capacityConfiguration": CapacityConfigurationOutputTypeDef,
+        "capacityConfiguration": CapacityConfigurationTypeDef,
         "releaseLabel": str,
         "vpcConfiguration": VpcConfigurationOutputTypeDef,
         "initializationScript": str,
-        "commandLineArguments": List[KxCommandLineArgumentOutputTypeDef],
-        "code": CodeConfigurationOutputTypeDef,
+        "commandLineArguments": List[KxCommandLineArgumentTypeDef],
+        "code": CodeConfigurationTypeDef,
         "executionRole": str,
         "lastModifiedTimestamp": datetime,
-        "savedownStorageConfiguration": KxSavedownStorageConfigurationOutputTypeDef,
+        "savedownStorageConfiguration": KxSavedownStorageConfigurationTypeDef,
         "azMode": KxAzModeType,
         "availabilityZoneId": str,
         "createdTimestamp": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateKxClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKxClusterRequestRequestTypeDef",
     {
         "environmentId": str,
```

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/PKG-INFO` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace
-Version: 1.28.12
-Summary: Type annotations for boto3.finspace 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace)](https://pepy.tech/project/mypy-boto3-finspace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.finspace 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
+[boto3.finspace 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace.html#finspace)
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
 [mypy-boto3-finspace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -333,116 +333,107 @@
 ### Typed dictionaries
 
 `mypy_boto3_finspace.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace.type_defs import (
-    AutoScalingConfigurationOutputTypeDef,
     AutoScalingConfigurationTypeDef,
-    CapacityConfigurationOutputTypeDef,
     CapacityConfigurationTypeDef,
-    ChangeRequestOutputTypeDef,
     ChangeRequestTypeDef,
-    CodeConfigurationOutputTypeDef,
     CodeConfigurationTypeDef,
     FederationParametersTypeDef,
     SuperuserParametersTypeDef,
-    CreateEnvironmentResponseTypeDef,
+    ResponseMetadataTypeDef,
     ErrorInfoTypeDef,
     KxCacheStorageConfigurationTypeDef,
     KxCommandLineArgumentTypeDef,
     KxSavedownStorageConfigurationTypeDef,
     VpcConfigurationTypeDef,
-    KxCacheStorageConfigurationOutputTypeDef,
-    KxCommandLineArgumentOutputTypeDef,
-    KxSavedownStorageConfigurationOutputTypeDef,
     VpcConfigurationOutputTypeDef,
     CreateKxDatabaseRequestRequestTypeDef,
-    CreateKxDatabaseResponseTypeDef,
     CreateKxEnvironmentRequestRequestTypeDef,
-    CreateKxEnvironmentResponseTypeDef,
     CreateKxUserRequestRequestTypeDef,
-    CreateKxUserResponseTypeDef,
-    CustomDNSServerOutputTypeDef,
     CustomDNSServerTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
     DeleteKxClusterRequestRequestTypeDef,
     DeleteKxDatabaseRequestRequestTypeDef,
     DeleteKxEnvironmentRequestRequestTypeDef,
     DeleteKxUserRequestRequestTypeDef,
     FederationParametersOutputTypeDef,
     GetEnvironmentRequestRequestTypeDef,
     GetKxChangesetRequestRequestTypeDef,
     GetKxClusterRequestRequestTypeDef,
     GetKxConnectionStringRequestRequestTypeDef,
-    GetKxConnectionStringResponseTypeDef,
     GetKxDatabaseRequestRequestTypeDef,
-    GetKxDatabaseResponseTypeDef,
     GetKxEnvironmentRequestRequestTypeDef,
-    TransitGatewayConfigurationOutputTypeDef,
+    TransitGatewayConfigurationTypeDef,
     GetKxUserRequestRequestTypeDef,
-    GetKxUserResponseTypeDef,
     KxChangesetListEntryTypeDef,
     KxClusterTypeDef,
     KxDatabaseCacheConfigurationOutputTypeDef,
     KxDatabaseCacheConfigurationTypeDef,
     KxDatabaseListEntryTypeDef,
     KxNodeTypeDef,
     KxUserTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
     ListKxChangesetsRequestRequestTypeDef,
     ListKxClusterNodesRequestRequestTypeDef,
     ListKxClustersRequestRequestTypeDef,
     ListKxDatabasesRequestRequestTypeDef,
-    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKxEnvironmentsRequestRequestTypeDef,
     ListKxUsersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
-    TransitGatewayConfigurationTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateKxDatabaseRequestRequestTypeDef,
-    UpdateKxDatabaseResponseTypeDef,
     UpdateKxEnvironmentRequestRequestTypeDef,
     UpdateKxUserRequestRequestTypeDef,
-    UpdateKxUserResponseTypeDef,
     CreateKxChangesetRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentRequestRequestTypeDef,
+    CreateEnvironmentResponseTypeDef,
+    CreateKxDatabaseResponseTypeDef,
+    CreateKxEnvironmentResponseTypeDef,
+    CreateKxUserResponseTypeDef,
+    GetKxConnectionStringResponseTypeDef,
+    GetKxDatabaseResponseTypeDef,
+    GetKxUserResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateKxDatabaseResponseTypeDef,
+    UpdateKxUserResponseTypeDef,
     CreateKxChangesetResponseTypeDef,
     GetKxChangesetResponseTypeDef,
     EnvironmentTypeDef,
     GetKxEnvironmentResponseTypeDef,
     KxEnvironmentTypeDef,
+    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
     UpdateKxEnvironmentNetworkResponseTypeDef,
     UpdateKxEnvironmentResponseTypeDef,
     ListKxChangesetsResponseTypeDef,
     ListKxClustersResponseTypeDef,
     KxDatabaseConfigurationOutputTypeDef,
     KxDatabaseConfigurationTypeDef,
     ListKxDatabasesResponseTypeDef,
     ListKxClusterNodesResponseTypeDef,
     ListKxUsersResponseTypeDef,
-    UpdateKxEnvironmentNetworkRequestRequestTypeDef,
+    ListKxEnvironmentsRequestListKxEnvironmentsPaginateTypeDef,
     GetEnvironmentResponseTypeDef,
     ListEnvironmentsResponseTypeDef,
     UpdateEnvironmentResponseTypeDef,
     ListKxEnvironmentsResponseTypeDef,
     CreateKxClusterResponseTypeDef,
     GetKxClusterResponseTypeDef,
     CreateKxClusterRequestRequestTypeDef,
     UpdateKxClusterDatabasesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AutoScalingConfigurationOutputTypeDef:
+def get_structure() -> AutoScalingConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-finspace-1.28.12/mypy_boto3_finspace.egg-info/SOURCES.txt` & `mypy-boto3-finspace-1.28.15/mypy_boto3_finspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-1.28.12/setup.py` & `mypy-boto3-finspace-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_finspace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.finspace 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.finspace 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

