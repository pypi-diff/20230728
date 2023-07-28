# Comparing `tmp/mypy-boto3-finspace-data-1.28.12.tar.gz` & `tmp/mypy-boto3-finspace-data-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-finspace-data-1.28.12.tar", last modified: Thu Jul 27 05:34:41 2023, max compression
+gzip compressed data, was "mypy-boto3-finspace-data-1.28.15.tar", last modified: Fri Jul 28 20:42:47 2023, max compression
```

## Comparing `mypy-boto3-finspace-data-1.28.12.tar` & `mypy-boto3-finspace-data-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.480511 mypy-boto3-finspace-data-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-27 05:34:41.476511 mypy-boto3-finspace-data-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.472511 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25240 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36156 2023-07-27 05:22:17.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36101 2023-07-27 05:22:17.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:41.476511 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17374 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:41.000000 mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:41.480511 mypy-boto3-finspace-data-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 05:22:15.000000 mypy-boto3-finspace-data-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.237089 mypy-boto3-finspace-data-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-07-28 20:42:47.237089 mypy-boto3-finspace-data-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15794 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.229089 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25240 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25197 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10151 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35600 2023-07-28 20:25:51.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35545 2023-07-28 20:25:51.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:47.237089 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17304 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:47.000000 mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:47.237089 mypy-boto3-finspace-data-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-28 20:25:50.000000 mypy-boto3-finspace-data-1.28.15/setup.py
```

### Comparing `mypy-boto3-finspace-data-1.28.12/LICENSE` & `mypy-boto3-finspace-data-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.12/PKG-INFO` & `mypy-boto3-finspace-data-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace-data
-Version: 1.28.12
-Summary: Type annotations for boto3.FinSpaceData 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,93 +350,91 @@
 
 `mypy_boto3_finspace_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
-    AssociateUserToPermissionGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
-    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
     CreateChangesetRequestRequestTypeDef,
-    CreateChangesetResponseTypeDef,
     DataViewDestinationTypeParamsTypeDef,
-    CreateDataViewResponseTypeDef,
     DatasetOwnerInfoTypeDef,
-    CreateDatasetResponseTypeDef,
     CreatePermissionGroupRequestRequestTypeDef,
-    CreatePermissionGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
     CredentialsTypeDef,
     DataViewDestinationTypeParamsOutputTypeDef,
     DataViewErrorInfoTypeDef,
-    DatasetOwnerInfoOutputTypeDef,
     DeleteDatasetRequestRequestTypeDef,
-    DeleteDatasetResponseTypeDef,
     DeletePermissionGroupRequestRequestTypeDef,
-    DeletePermissionGroupResponseTypeDef,
     DisableUserRequestRequestTypeDef,
-    DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupRequestRequestTypeDef,
-    DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserRequestRequestTypeDef,
-    EnableUserResponseTypeDef,
     GetChangesetRequestRequestTypeDef,
     GetDataViewRequestRequestTypeDef,
     GetDatasetRequestRequestTypeDef,
     GetExternalDataViewAccessDetailsRequestRequestTypeDef,
     S3LocationTypeDef,
     GetPermissionGroupRequestRequestTypeDef,
     PermissionGroupTypeDef,
     GetProgrammaticAccessCredentialsRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
-    GetUserResponseTypeDef,
     GetWorkingLocationRequestRequestTypeDef,
-    GetWorkingLocationResponseTypeDef,
-    ListChangesetsRequestListChangesetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChangesetsRequestRequestTypeDef,
-    ListDataViewsRequestListDataViewsPaginateTypeDef,
     ListDataViewsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListPermissionGroupsByUserRequestRequestTypeDef,
     PermissionGroupByUserTypeDef,
-    ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef,
     ListPermissionGroupsRequestRequestTypeDef,
     ListUsersByPermissionGroupRequestRequestTypeDef,
     UserByPermissionGroupTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
-    PaginatorConfigTypeDef,
     ResourcePermissionTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResetUserPasswordResponseTypeDef,
-    ResponseMetadataTypeDef,
     UpdateChangesetRequestRequestTypeDef,
+    UpdatePermissionGroupRequestRequestTypeDef,
+    UpdateUserRequestRequestTypeDef,
+    AssociateUserToPermissionGroupResponseTypeDef,
+    CreateChangesetResponseTypeDef,
+    CreateDataViewResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreatePermissionGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DeleteDatasetResponseTypeDef,
+    DeletePermissionGroupResponseTypeDef,
+    DisableUserResponseTypeDef,
+    DisassociateUserFromPermissionGroupResponseTypeDef,
+    EnableUserResponseTypeDef,
+    GetUserResponseTypeDef,
+    GetWorkingLocationResponseTypeDef,
+    ResetUserPasswordResponseTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
-    UpdatePermissionGroupRequestRequestTypeDef,
     UpdatePermissionGroupResponseTypeDef,
-    UpdateUserRequestRequestTypeDef,
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
+    ListChangesetsRequestListChangesetsPaginateTypeDef,
+    ListDataViewsRequestListDataViewsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ListChangesetsResponseTypeDef,
     SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
```

### Comparing `mypy-boto3-finspace-data-1.28.12/README.md` & `mypy-boto3-finspace-data-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,93 +318,91 @@
 
 `mypy_boto3_finspace_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
-    AssociateUserToPermissionGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
-    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
     CreateChangesetRequestRequestTypeDef,
-    CreateChangesetResponseTypeDef,
     DataViewDestinationTypeParamsTypeDef,
-    CreateDataViewResponseTypeDef,
     DatasetOwnerInfoTypeDef,
-    CreateDatasetResponseTypeDef,
     CreatePermissionGroupRequestRequestTypeDef,
-    CreatePermissionGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
     CredentialsTypeDef,
     DataViewDestinationTypeParamsOutputTypeDef,
     DataViewErrorInfoTypeDef,
-    DatasetOwnerInfoOutputTypeDef,
     DeleteDatasetRequestRequestTypeDef,
-    DeleteDatasetResponseTypeDef,
     DeletePermissionGroupRequestRequestTypeDef,
-    DeletePermissionGroupResponseTypeDef,
     DisableUserRequestRequestTypeDef,
-    DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupRequestRequestTypeDef,
-    DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserRequestRequestTypeDef,
-    EnableUserResponseTypeDef,
     GetChangesetRequestRequestTypeDef,
     GetDataViewRequestRequestTypeDef,
     GetDatasetRequestRequestTypeDef,
     GetExternalDataViewAccessDetailsRequestRequestTypeDef,
     S3LocationTypeDef,
     GetPermissionGroupRequestRequestTypeDef,
     PermissionGroupTypeDef,
     GetProgrammaticAccessCredentialsRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
-    GetUserResponseTypeDef,
     GetWorkingLocationRequestRequestTypeDef,
-    GetWorkingLocationResponseTypeDef,
-    ListChangesetsRequestListChangesetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChangesetsRequestRequestTypeDef,
-    ListDataViewsRequestListDataViewsPaginateTypeDef,
     ListDataViewsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListPermissionGroupsByUserRequestRequestTypeDef,
     PermissionGroupByUserTypeDef,
-    ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef,
     ListPermissionGroupsRequestRequestTypeDef,
     ListUsersByPermissionGroupRequestRequestTypeDef,
     UserByPermissionGroupTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
-    PaginatorConfigTypeDef,
     ResourcePermissionTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResetUserPasswordResponseTypeDef,
-    ResponseMetadataTypeDef,
     UpdateChangesetRequestRequestTypeDef,
+    UpdatePermissionGroupRequestRequestTypeDef,
+    UpdateUserRequestRequestTypeDef,
+    AssociateUserToPermissionGroupResponseTypeDef,
+    CreateChangesetResponseTypeDef,
+    CreateDataViewResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreatePermissionGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DeleteDatasetResponseTypeDef,
+    DeletePermissionGroupResponseTypeDef,
+    DisableUserResponseTypeDef,
+    DisassociateUserFromPermissionGroupResponseTypeDef,
+    EnableUserResponseTypeDef,
+    GetUserResponseTypeDef,
+    GetWorkingLocationResponseTypeDef,
+    ResetUserPasswordResponseTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
-    UpdatePermissionGroupRequestRequestTypeDef,
     UpdatePermissionGroupResponseTypeDef,
-    UpdateUserRequestRequestTypeDef,
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
+    ListChangesetsRequestListChangesetsPaginateTypeDef,
+    ListDataViewsRequestListDataViewsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ListChangesetsResponseTypeDef,
     SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
```

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__init__.py` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__init__.pyi` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/__main__.py` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FinSpaceData 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.FinSpaceData 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData\nOther"
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

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/client.py` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/client.pyi` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/literals.py` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/literals.pyi` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/paginator.py` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,73 +62,73 @@
 class ListChangesetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListChangesets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, datasetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, datasetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChangesetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListChangesets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listchangesetspaginator)
         """
 
 
 class ListDataViewsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDataViews)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listdataviewspaginator)
     """
 
     def paginate(
-        self, *, datasetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, datasetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataViewsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDataViews.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listdataviewspaginator)
         """
 
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listdatasetspaginator)
         """
 
 
 class ListPermissionGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListPermissionGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listpermissiongroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListPermissionGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listpermissiongroupspaginator)
         """
 
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/paginator.pyi` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -59,69 +59,69 @@
 class ListChangesetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListChangesets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listchangesetspaginator)
     """
 
     def paginate(
-        self, *, datasetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, datasetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListChangesetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListChangesets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listchangesetspaginator)
         """
 
 class ListDataViewsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDataViews)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listdataviewspaginator)
     """
 
     def paginate(
-        self, *, datasetId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, datasetId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDataViewsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDataViews.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listdataviewspaginator)
         """
 
 class ListDatasetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDatasets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListDatasets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listdatasetspaginator)
         """
 
 class ListPermissionGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListPermissionGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listpermissiongroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListPermissionGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listpermissiongroupspaginator)
         """
 
 class ListUsersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListUsers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listuserspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/paginators/#listuserspaginator)
         """
```

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/type_defs.py` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,93 +35,91 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateUserToPermissionGroupRequestRequestTypeDef",
-    "AssociateUserToPermissionGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AwsCredentialsTypeDef",
     "ChangesetErrorInfoTypeDef",
-    "ColumnDefinitionOutputTypeDef",
     "ColumnDefinitionTypeDef",
     "CreateChangesetRequestRequestTypeDef",
-    "CreateChangesetResponseTypeDef",
     "DataViewDestinationTypeParamsTypeDef",
-    "CreateDataViewResponseTypeDef",
     "DatasetOwnerInfoTypeDef",
-    "CreateDatasetResponseTypeDef",
     "CreatePermissionGroupRequestRequestTypeDef",
-    "CreatePermissionGroupResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "CreateUserResponseTypeDef",
     "CredentialsTypeDef",
     "DataViewDestinationTypeParamsOutputTypeDef",
     "DataViewErrorInfoTypeDef",
-    "DatasetOwnerInfoOutputTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
-    "DeleteDatasetResponseTypeDef",
     "DeletePermissionGroupRequestRequestTypeDef",
-    "DeletePermissionGroupResponseTypeDef",
     "DisableUserRequestRequestTypeDef",
-    "DisableUserResponseTypeDef",
     "DisassociateUserFromPermissionGroupRequestRequestTypeDef",
-    "DisassociateUserFromPermissionGroupResponseTypeDef",
     "EnableUserRequestRequestTypeDef",
-    "EnableUserResponseTypeDef",
     "GetChangesetRequestRequestTypeDef",
     "GetDataViewRequestRequestTypeDef",
     "GetDatasetRequestRequestTypeDef",
     "GetExternalDataViewAccessDetailsRequestRequestTypeDef",
     "S3LocationTypeDef",
     "GetPermissionGroupRequestRequestTypeDef",
     "PermissionGroupTypeDef",
     "GetProgrammaticAccessCredentialsRequestRequestTypeDef",
     "GetUserRequestRequestTypeDef",
-    "GetUserResponseTypeDef",
     "GetWorkingLocationRequestRequestTypeDef",
-    "GetWorkingLocationResponseTypeDef",
-    "ListChangesetsRequestListChangesetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChangesetsRequestRequestTypeDef",
-    "ListDataViewsRequestListDataViewsPaginateTypeDef",
     "ListDataViewsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListPermissionGroupsByUserRequestRequestTypeDef",
     "PermissionGroupByUserTypeDef",
-    "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
     "ListPermissionGroupsRequestRequestTypeDef",
     "ListUsersByPermissionGroupRequestRequestTypeDef",
     "UserByPermissionGroupTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourcePermissionTypeDef",
     "ResetUserPasswordRequestRequestTypeDef",
-    "ResetUserPasswordResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateChangesetRequestRequestTypeDef",
+    "UpdatePermissionGroupRequestRequestTypeDef",
+    "UpdateUserRequestRequestTypeDef",
+    "AssociateUserToPermissionGroupResponseTypeDef",
+    "CreateChangesetResponseTypeDef",
+    "CreateDataViewResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreatePermissionGroupResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "DeleteDatasetResponseTypeDef",
+    "DeletePermissionGroupResponseTypeDef",
+    "DisableUserResponseTypeDef",
+    "DisassociateUserFromPermissionGroupResponseTypeDef",
+    "EnableUserResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "GetWorkingLocationResponseTypeDef",
+    "ResetUserPasswordResponseTypeDef",
     "UpdateChangesetResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
-    "UpdatePermissionGroupRequestRequestTypeDef",
     "UpdatePermissionGroupResponseTypeDef",
-    "UpdateUserRequestRequestTypeDef",
     "UpdateUserResponseTypeDef",
     "ChangesetSummaryTypeDef",
     "GetChangesetResponseTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateDataViewRequestRequestTypeDef",
     "GetProgrammaticAccessCredentialsResponseTypeDef",
     "DataViewSummaryTypeDef",
     "GetDataViewResponseTypeDef",
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     "GetPermissionGroupResponseTypeDef",
     "ListPermissionGroupsResponseTypeDef",
+    "ListChangesetsRequestListChangesetsPaginateTypeDef",
+    "ListDataViewsRequestListDataViewsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListPermissionGroupsByUserResponseTypeDef",
     "ListUsersByPermissionGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "PermissionGroupParamsTypeDef",
     "ListChangesetsResponseTypeDef",
     "SchemaUnionOutputTypeDef",
     "SchemaUnionTypeDef",
@@ -152,19 +150,22 @@
 class AssociateUserToPermissionGroupRequestRequestTypeDef(
     _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef,
     _OptionalAssociateUserToPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateUserToPermissionGroupResponseTypeDef = TypedDict(
-    "AssociateUserToPermissionGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "statusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AwsCredentialsTypeDef = TypedDict(
     "AwsCredentialsTypeDef",
     {
         "accessKeyId": str,
@@ -180,24 +181,14 @@
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
 )
 
-ColumnDefinitionOutputTypeDef = TypedDict(
-    "ColumnDefinitionOutputTypeDef",
-    {
-        "dataType": ColumnDataTypeType,
-        "columnName": str,
-        "columnDescription": str,
-    },
-    total=False,
-)
-
 ColumnDefinitionTypeDef = TypedDict(
     "ColumnDefinitionTypeDef",
     {
         "dataType": ColumnDataTypeType,
         "columnName": str,
         "columnDescription": str,
     },
@@ -224,23 +215,14 @@
 
 class CreateChangesetRequestRequestTypeDef(
     _RequiredCreateChangesetRequestRequestTypeDef, _OptionalCreateChangesetRequestRequestTypeDef
 ):
     pass
 
 
-CreateChangesetResponseTypeDef = TypedDict(
-    "CreateChangesetResponseTypeDef",
-    {
-        "datasetId": str,
-        "changesetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDataViewDestinationTypeParamsTypeDef = TypedDict(
     "_RequiredDataViewDestinationTypeParamsTypeDef",
     {
         "destinationType": str,
     },
 )
 _OptionalDataViewDestinationTypeParamsTypeDef = TypedDict(
@@ -255,41 +237,24 @@
 
 class DataViewDestinationTypeParamsTypeDef(
     _RequiredDataViewDestinationTypeParamsTypeDef, _OptionalDataViewDestinationTypeParamsTypeDef
 ):
     pass
 
 
-CreateDataViewResponseTypeDef = TypedDict(
-    "CreateDataViewResponseTypeDef",
-    {
-        "datasetId": str,
-        "dataViewId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DatasetOwnerInfoTypeDef = TypedDict(
     "DatasetOwnerInfoTypeDef",
     {
         "name": str,
         "phoneNumber": str,
         "email": str,
     },
     total=False,
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "datasetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionGroupRequestRequestTypeDef",
     {
         "name": str,
         "applicationPermissions": Sequence[ApplicationPermissionType],
     },
 )
@@ -306,22 +271,14 @@
 class CreatePermissionGroupRequestRequestTypeDef(
     _RequiredCreatePermissionGroupRequestRequestTypeDef,
     _OptionalCreatePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
 
-CreatePermissionGroupResponseTypeDef = TypedDict(
-    "CreatePermissionGroupResponseTypeDef",
-    {
-        "permissionGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "emailAddress": str,
         "type": UserTypeType,
     },
 )
@@ -340,22 +297,14 @@
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "userId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "accessKeyId": str,
         "secretAccessKey": str,
         "sessionToken": str,
     },
@@ -390,24 +339,14 @@
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
 )
 
-DatasetOwnerInfoOutputTypeDef = TypedDict(
-    "DatasetOwnerInfoOutputTypeDef",
-    {
-        "name": str,
-        "phoneNumber": str,
-        "email": str,
-    },
-    total=False,
-)
-
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalDeleteDatasetRequestRequestTypeDef = TypedDict(
@@ -421,22 +360,14 @@
 
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
 
-DeleteDatasetResponseTypeDef = TypedDict(
-    "DeleteDatasetResponseTypeDef",
-    {
-        "datasetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
     },
 )
 _OptionalDeletePermissionGroupRequestRequestTypeDef = TypedDict(
@@ -451,22 +382,14 @@
 class DeletePermissionGroupRequestRequestTypeDef(
     _RequiredDeletePermissionGroupRequestRequestTypeDef,
     _OptionalDeletePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
 
-DeletePermissionGroupResponseTypeDef = TypedDict(
-    "DeletePermissionGroupResponseTypeDef",
-    {
-        "permissionGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisableUserRequestRequestTypeDef = TypedDict(
     "_RequiredDisableUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalDisableUserRequestRequestTypeDef = TypedDict(
@@ -480,22 +403,14 @@
 
 class DisableUserRequestRequestTypeDef(
     _RequiredDisableUserRequestRequestTypeDef, _OptionalDisableUserRequestRequestTypeDef
 ):
     pass
 
 
-DisableUserResponseTypeDef = TypedDict(
-    "DisableUserResponseTypeDef",
-    {
-        "userId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
         "userId": str,
     },
 )
@@ -511,22 +426,14 @@
 class DisassociateUserFromPermissionGroupRequestRequestTypeDef(
     _RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef,
     _OptionalDisassociateUserFromPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
 
-DisassociateUserFromPermissionGroupResponseTypeDef = TypedDict(
-    "DisassociateUserFromPermissionGroupResponseTypeDef",
-    {
-        "statusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableUserRequestRequestTypeDef = TypedDict(
     "_RequiredEnableUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalEnableUserRequestRequestTypeDef = TypedDict(
@@ -540,22 +447,14 @@
 
 class EnableUserRequestRequestTypeDef(
     _RequiredEnableUserRequestRequestTypeDef, _OptionalEnableUserRequestRequestTypeDef
 ):
     pass
 
 
-EnableUserResponseTypeDef = TypedDict(
-    "EnableUserResponseTypeDef",
-    {
-        "userId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChangesetRequestRequestTypeDef = TypedDict(
     "GetChangesetRequestRequestTypeDef",
     {
         "datasetId": str,
         "changesetId": str,
     },
 )
@@ -637,74 +536,32 @@
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
-    {
-        "userId": str,
-        "status": UserStatusType,
-        "firstName": str,
-        "lastName": str,
-        "emailAddress": str,
-        "type": UserTypeType,
-        "apiAccess": ApiAccessType,
-        "apiAccessPrincipalArn": str,
-        "createTime": int,
-        "lastEnabledTime": int,
-        "lastDisabledTime": int,
-        "lastModifiedTime": int,
-        "lastLoginTime": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkingLocationRequestRequestTypeDef = TypedDict(
     "GetWorkingLocationRequestRequestTypeDef",
     {
         "locationType": locationTypeType,
     },
     total=False,
 )
 
-GetWorkingLocationResponseTypeDef = TypedDict(
-    "GetWorkingLocationResponseTypeDef",
-    {
-        "s3Uri": str,
-        "s3Path": str,
-        "s3Bucket": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListChangesetsRequestListChangesetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangesetsRequestListChangesetsPaginateTypeDef",
-    {
-        "datasetId": str,
-    },
-)
-_OptionalListChangesetsRequestListChangesetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangesetsRequestListChangesetsPaginateTypeDef",
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
-class ListChangesetsRequestListChangesetsPaginateTypeDef(
-    _RequiredListChangesetsRequestListChangesetsPaginateTypeDef,
-    _OptionalListChangesetsRequestListChangesetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListChangesetsRequestRequestTypeDef = TypedDict(
     "_RequiredListChangesetsRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalListChangesetsRequestRequestTypeDef = TypedDict(
@@ -719,36 +576,14 @@
 
 class ListChangesetsRequestRequestTypeDef(
     _RequiredListChangesetsRequestRequestTypeDef, _OptionalListChangesetsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
-    "_RequiredListDataViewsRequestListDataViewsPaginateTypeDef",
-    {
-        "datasetId": str,
-    },
-)
-_OptionalListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
-    "_OptionalListDataViewsRequestListDataViewsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDataViewsRequestListDataViewsPaginateTypeDef(
-    _RequiredListDataViewsRequestListDataViewsPaginateTypeDef,
-    _OptionalListDataViewsRequestListDataViewsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDataViewsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataViewsRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalListDataViewsRequestRequestTypeDef = TypedDict(
@@ -763,22 +598,14 @@
 
 class ListDataViewsRequestRequestTypeDef(
     _RequiredListDataViewsRequestRequestTypeDef, _OptionalListDataViewsRequestRequestTypeDef
 ):
     pass
 
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -813,22 +640,14 @@
         "permissionGroupId": str,
         "name": str,
         "membershipStatus": PermissionGroupMembershipStatusType,
     },
     total=False,
 )
 
-ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef = TypedDict(
-    "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListPermissionGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
     },
 )
 _OptionalListPermissionGroupsRequestRequestTypeDef = TypedDict(
@@ -882,22 +701,14 @@
         "apiAccess": ApiAccessType,
         "apiAccessPrincipalArn": str,
         "membershipStatus": PermissionGroupMembershipStatusType,
     },
     total=False,
 )
 
-ListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "ListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "maxResults": int,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -931,24 +742,14 @@
         "lastDisabledTime": int,
         "lastModifiedTime": int,
         "lastLoginTime": int,
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
 ResourcePermissionTypeDef = TypedDict(
     "ResourcePermissionTypeDef",
     {
         "permission": str,
     },
     total=False,
 )
@@ -970,34 +771,14 @@
 
 class ResetUserPasswordRequestRequestTypeDef(
     _RequiredResetUserPasswordRequestRequestTypeDef, _OptionalResetUserPasswordRequestRequestTypeDef
 ):
     pass
 
 
-ResetUserPasswordResponseTypeDef = TypedDict(
-    "ResetUserPasswordResponseTypeDef",
-    {
-        "userId": str,
-        "temporaryPassword": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredUpdateChangesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChangesetRequestRequestTypeDef",
     {
         "datasetId": str,
         "changesetId": str,
         "sourceParams": Mapping[str, str],
         "formatParams": Mapping[str, str],
@@ -1014,31 +795,14 @@
 
 class UpdateChangesetRequestRequestTypeDef(
     _RequiredUpdateChangesetRequestRequestTypeDef, _OptionalUpdateChangesetRequestRequestTypeDef
 ):
     pass
 
 
-UpdateChangesetResponseTypeDef = TypedDict(
-    "UpdateChangesetResponseTypeDef",
-    {
-        "changesetId": str,
-        "datasetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDatasetResponseTypeDef = TypedDict(
-    "UpdateDatasetResponseTypeDef",
-    {
-        "datasetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
     },
 )
 _OptionalUpdatePermissionGroupRequestRequestTypeDef = TypedDict(
@@ -1056,22 +820,14 @@
 class UpdatePermissionGroupRequestRequestTypeDef(
     _RequiredUpdatePermissionGroupRequestRequestTypeDef,
     _OptionalUpdatePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
 
-UpdatePermissionGroupResponseTypeDef = TypedDict(
-    "UpdatePermissionGroupResponseTypeDef",
-    {
-        "permissionGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalUpdateUserRequestRequestTypeDef = TypedDict(
@@ -1090,19 +846,173 @@
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
 
+AssociateUserToPermissionGroupResponseTypeDef = TypedDict(
+    "AssociateUserToPermissionGroupResponseTypeDef",
+    {
+        "statusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChangesetResponseTypeDef = TypedDict(
+    "CreateChangesetResponseTypeDef",
+    {
+        "datasetId": str,
+        "changesetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataViewResponseTypeDef = TypedDict(
+    "CreateDataViewResponseTypeDef",
+    {
+        "datasetId": str,
+        "dataViewId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "datasetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePermissionGroupResponseTypeDef = TypedDict(
+    "CreatePermissionGroupResponseTypeDef",
+    {
+        "permissionGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "userId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDatasetResponseTypeDef = TypedDict(
+    "DeleteDatasetResponseTypeDef",
+    {
+        "datasetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePermissionGroupResponseTypeDef = TypedDict(
+    "DeletePermissionGroupResponseTypeDef",
+    {
+        "permissionGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableUserResponseTypeDef = TypedDict(
+    "DisableUserResponseTypeDef",
+    {
+        "userId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateUserFromPermissionGroupResponseTypeDef = TypedDict(
+    "DisassociateUserFromPermissionGroupResponseTypeDef",
+    {
+        "statusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableUserResponseTypeDef = TypedDict(
+    "EnableUserResponseTypeDef",
+    {
+        "userId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
+    {
+        "userId": str,
+        "status": UserStatusType,
+        "firstName": str,
+        "lastName": str,
+        "emailAddress": str,
+        "type": UserTypeType,
+        "apiAccess": ApiAccessType,
+        "apiAccessPrincipalArn": str,
+        "createTime": int,
+        "lastEnabledTime": int,
+        "lastDisabledTime": int,
+        "lastModifiedTime": int,
+        "lastLoginTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkingLocationResponseTypeDef = TypedDict(
+    "GetWorkingLocationResponseTypeDef",
+    {
+        "s3Uri": str,
+        "s3Path": str,
+        "s3Bucket": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResetUserPasswordResponseTypeDef = TypedDict(
+    "ResetUserPasswordResponseTypeDef",
+    {
+        "userId": str,
+        "temporaryPassword": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChangesetResponseTypeDef = TypedDict(
+    "UpdateChangesetResponseTypeDef",
+    {
+        "changesetId": str,
+        "datasetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
+    {
+        "datasetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePermissionGroupResponseTypeDef = TypedDict(
+    "UpdatePermissionGroupResponseTypeDef",
+    {
+        "permissionGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "userId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangesetSummaryTypeDef = TypedDict(
     "ChangesetSummaryTypeDef",
     {
         "changesetId": str,
@@ -1134,22 +1044,22 @@
         "createTime": int,
         "status": IngestionStatusType,
         "errorInfo": ChangesetErrorInfoTypeDef,
         "activeUntilTimestamp": int,
         "activeFromTimestamp": int,
         "updatesChangesetId": str,
         "updatedByChangesetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SchemaDefinitionOutputTypeDef = TypedDict(
     "SchemaDefinitionOutputTypeDef",
     {
-        "columns": List[ColumnDefinitionOutputTypeDef],
+        "columns": List[ColumnDefinitionTypeDef],
         "primaryKeyColumns": List[str],
     },
     total=False,
 )
 
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
@@ -1187,15 +1097,15 @@
 
 
 GetProgrammaticAccessCredentialsResponseTypeDef = TypedDict(
     "GetProgrammaticAccessCredentialsResponseTypeDef",
     {
         "credentials": CredentialsTypeDef,
         "durationInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataViewSummaryTypeDef = TypedDict(
     "DataViewSummaryTypeDef",
     {
         "dataViewId": str,
@@ -1225,68 +1135,136 @@
         "lastModifiedTime": int,
         "createTime": int,
         "sortColumns": List[str],
         "dataViewId": str,
         "dataViewArn": str,
         "destinationTypeParams": DataViewDestinationTypeParamsOutputTypeDef,
         "status": DataViewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExternalDataViewAccessDetailsResponseTypeDef = TypedDict(
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     {
         "credentials": AwsCredentialsTypeDef,
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPermissionGroupResponseTypeDef = TypedDict(
     "GetPermissionGroupResponseTypeDef",
     {
         "permissionGroup": PermissionGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionGroupsResponseTypeDef = TypedDict(
     "ListPermissionGroupsResponseTypeDef",
     {
         "permissionGroups": List[PermissionGroupTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListChangesetsRequestListChangesetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangesetsRequestListChangesetsPaginateTypeDef",
+    {
+        "datasetId": str,
+    },
+)
+_OptionalListChangesetsRequestListChangesetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangesetsRequestListChangesetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListChangesetsRequestListChangesetsPaginateTypeDef(
+    _RequiredListChangesetsRequestListChangesetsPaginateTypeDef,
+    _OptionalListChangesetsRequestListChangesetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
+    "_RequiredListDataViewsRequestListDataViewsPaginateTypeDef",
+    {
+        "datasetId": str,
+    },
+)
+_OptionalListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
+    "_OptionalListDataViewsRequestListDataViewsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDataViewsRequestListDataViewsPaginateTypeDef(
+    _RequiredListDataViewsRequestListDataViewsPaginateTypeDef,
+    _OptionalListDataViewsRequestListDataViewsPaginateTypeDef,
+):
+    pass
+
+
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef = TypedDict(
+    "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "ListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPermissionGroupsByUserResponseTypeDef = TypedDict(
     "ListPermissionGroupsByUserResponseTypeDef",
     {
         "permissionGroups": List[PermissionGroupByUserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersByPermissionGroupResponseTypeDef = TypedDict(
     "ListUsersByPermissionGroupResponseTypeDef",
     {
         "users": List[UserByPermissionGroupTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "users": List[UserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PermissionGroupParamsTypeDef = TypedDict(
     "PermissionGroupParamsTypeDef",
     {
         "permissionGroupId": str,
@@ -1296,15 +1274,15 @@
 )
 
 ListChangesetsResponseTypeDef = TypedDict(
     "ListChangesetsResponseTypeDef",
     {
         "changesets": List[ChangesetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SchemaUnionOutputTypeDef = TypedDict(
     "SchemaUnionOutputTypeDef",
     {
         "tabularSchemaConfig": SchemaDefinitionOutputTypeDef,
@@ -1321,27 +1299,27 @@
 )
 
 ListDataViewsResponseTypeDef = TypedDict(
     "ListDataViewsResponseTypeDef",
     {
         "nextToken": str,
         "dataViews": List[DataViewSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetTypeDef = TypedDict(
     "DatasetTypeDef",
     {
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
-        "ownerInfo": DatasetOwnerInfoOutputTypeDef,
+        "ownerInfo": DatasetOwnerInfoTypeDef,
         "createTime": int,
         "lastModifiedTime": int,
         "schemaDefinition": SchemaUnionOutputTypeDef,
         "alias": str,
     },
     total=False,
 )
@@ -1355,15 +1333,15 @@
         "kind": DatasetKindType,
         "datasetDescription": str,
         "createTime": int,
         "lastModifiedTime": int,
         "schemaDefinition": SchemaUnionOutputTypeDef,
         "alias": str,
         "status": DatasetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetTitle": str,
@@ -1417,10 +1395,10 @@
 
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasets": List[DatasetTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data/type_defs.pyi` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -34,93 +34,91 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateUserToPermissionGroupRequestRequestTypeDef",
-    "AssociateUserToPermissionGroupResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AwsCredentialsTypeDef",
     "ChangesetErrorInfoTypeDef",
-    "ColumnDefinitionOutputTypeDef",
     "ColumnDefinitionTypeDef",
     "CreateChangesetRequestRequestTypeDef",
-    "CreateChangesetResponseTypeDef",
     "DataViewDestinationTypeParamsTypeDef",
-    "CreateDataViewResponseTypeDef",
     "DatasetOwnerInfoTypeDef",
-    "CreateDatasetResponseTypeDef",
     "CreatePermissionGroupRequestRequestTypeDef",
-    "CreatePermissionGroupResponseTypeDef",
     "CreateUserRequestRequestTypeDef",
-    "CreateUserResponseTypeDef",
     "CredentialsTypeDef",
     "DataViewDestinationTypeParamsOutputTypeDef",
     "DataViewErrorInfoTypeDef",
-    "DatasetOwnerInfoOutputTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
-    "DeleteDatasetResponseTypeDef",
     "DeletePermissionGroupRequestRequestTypeDef",
-    "DeletePermissionGroupResponseTypeDef",
     "DisableUserRequestRequestTypeDef",
-    "DisableUserResponseTypeDef",
     "DisassociateUserFromPermissionGroupRequestRequestTypeDef",
-    "DisassociateUserFromPermissionGroupResponseTypeDef",
     "EnableUserRequestRequestTypeDef",
-    "EnableUserResponseTypeDef",
     "GetChangesetRequestRequestTypeDef",
     "GetDataViewRequestRequestTypeDef",
     "GetDatasetRequestRequestTypeDef",
     "GetExternalDataViewAccessDetailsRequestRequestTypeDef",
     "S3LocationTypeDef",
     "GetPermissionGroupRequestRequestTypeDef",
     "PermissionGroupTypeDef",
     "GetProgrammaticAccessCredentialsRequestRequestTypeDef",
     "GetUserRequestRequestTypeDef",
-    "GetUserResponseTypeDef",
     "GetWorkingLocationRequestRequestTypeDef",
-    "GetWorkingLocationResponseTypeDef",
-    "ListChangesetsRequestListChangesetsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListChangesetsRequestRequestTypeDef",
-    "ListDataViewsRequestListDataViewsPaginateTypeDef",
     "ListDataViewsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "ListPermissionGroupsByUserRequestRequestTypeDef",
     "PermissionGroupByUserTypeDef",
-    "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
     "ListPermissionGroupsRequestRequestTypeDef",
     "ListUsersByPermissionGroupRequestRequestTypeDef",
     "UserByPermissionGroupTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "UserTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourcePermissionTypeDef",
     "ResetUserPasswordRequestRequestTypeDef",
-    "ResetUserPasswordResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateChangesetRequestRequestTypeDef",
+    "UpdatePermissionGroupRequestRequestTypeDef",
+    "UpdateUserRequestRequestTypeDef",
+    "AssociateUserToPermissionGroupResponseTypeDef",
+    "CreateChangesetResponseTypeDef",
+    "CreateDataViewResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreatePermissionGroupResponseTypeDef",
+    "CreateUserResponseTypeDef",
+    "DeleteDatasetResponseTypeDef",
+    "DeletePermissionGroupResponseTypeDef",
+    "DisableUserResponseTypeDef",
+    "DisassociateUserFromPermissionGroupResponseTypeDef",
+    "EnableUserResponseTypeDef",
+    "GetUserResponseTypeDef",
+    "GetWorkingLocationResponseTypeDef",
+    "ResetUserPasswordResponseTypeDef",
     "UpdateChangesetResponseTypeDef",
     "UpdateDatasetResponseTypeDef",
-    "UpdatePermissionGroupRequestRequestTypeDef",
     "UpdatePermissionGroupResponseTypeDef",
-    "UpdateUserRequestRequestTypeDef",
     "UpdateUserResponseTypeDef",
     "ChangesetSummaryTypeDef",
     "GetChangesetResponseTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "CreateDataViewRequestRequestTypeDef",
     "GetProgrammaticAccessCredentialsResponseTypeDef",
     "DataViewSummaryTypeDef",
     "GetDataViewResponseTypeDef",
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     "GetPermissionGroupResponseTypeDef",
     "ListPermissionGroupsResponseTypeDef",
+    "ListChangesetsRequestListChangesetsPaginateTypeDef",
+    "ListDataViewsRequestListDataViewsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "ListPermissionGroupsByUserResponseTypeDef",
     "ListUsersByPermissionGroupResponseTypeDef",
     "ListUsersResponseTypeDef",
     "PermissionGroupParamsTypeDef",
     "ListChangesetsResponseTypeDef",
     "SchemaUnionOutputTypeDef",
     "SchemaUnionTypeDef",
@@ -149,19 +147,22 @@
 
 class AssociateUserToPermissionGroupRequestRequestTypeDef(
     _RequiredAssociateUserToPermissionGroupRequestRequestTypeDef,
     _OptionalAssociateUserToPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-AssociateUserToPermissionGroupResponseTypeDef = TypedDict(
-    "AssociateUserToPermissionGroupResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "statusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AwsCredentialsTypeDef = TypedDict(
     "AwsCredentialsTypeDef",
     {
         "accessKeyId": str,
@@ -177,24 +178,14 @@
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
 )
 
-ColumnDefinitionOutputTypeDef = TypedDict(
-    "ColumnDefinitionOutputTypeDef",
-    {
-        "dataType": ColumnDataTypeType,
-        "columnName": str,
-        "columnDescription": str,
-    },
-    total=False,
-)
-
 ColumnDefinitionTypeDef = TypedDict(
     "ColumnDefinitionTypeDef",
     {
         "dataType": ColumnDataTypeType,
         "columnName": str,
         "columnDescription": str,
     },
@@ -219,23 +210,14 @@
 )
 
 class CreateChangesetRequestRequestTypeDef(
     _RequiredCreateChangesetRequestRequestTypeDef, _OptionalCreateChangesetRequestRequestTypeDef
 ):
     pass
 
-CreateChangesetResponseTypeDef = TypedDict(
-    "CreateChangesetResponseTypeDef",
-    {
-        "datasetId": str,
-        "changesetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDataViewDestinationTypeParamsTypeDef = TypedDict(
     "_RequiredDataViewDestinationTypeParamsTypeDef",
     {
         "destinationType": str,
     },
 )
 _OptionalDataViewDestinationTypeParamsTypeDef = TypedDict(
@@ -248,41 +230,24 @@
 )
 
 class DataViewDestinationTypeParamsTypeDef(
     _RequiredDataViewDestinationTypeParamsTypeDef, _OptionalDataViewDestinationTypeParamsTypeDef
 ):
     pass
 
-CreateDataViewResponseTypeDef = TypedDict(
-    "CreateDataViewResponseTypeDef",
-    {
-        "datasetId": str,
-        "dataViewId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DatasetOwnerInfoTypeDef = TypedDict(
     "DatasetOwnerInfoTypeDef",
     {
         "name": str,
         "phoneNumber": str,
         "email": str,
     },
     total=False,
 )
 
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "datasetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePermissionGroupRequestRequestTypeDef",
     {
         "name": str,
         "applicationPermissions": Sequence[ApplicationPermissionType],
     },
 )
@@ -297,22 +262,14 @@
 
 class CreatePermissionGroupRequestRequestTypeDef(
     _RequiredCreatePermissionGroupRequestRequestTypeDef,
     _OptionalCreatePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-CreatePermissionGroupResponseTypeDef = TypedDict(
-    "CreatePermissionGroupResponseTypeDef",
-    {
-        "permissionGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateUserRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserRequestRequestTypeDef",
     {
         "emailAddress": str,
         "type": UserTypeType,
     },
 )
@@ -329,22 +286,14 @@
 )
 
 class CreateUserRequestRequestTypeDef(
     _RequiredCreateUserRequestRequestTypeDef, _OptionalCreateUserRequestRequestTypeDef
 ):
     pass
 
-CreateUserResponseTypeDef = TypedDict(
-    "CreateUserResponseTypeDef",
-    {
-        "userId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CredentialsTypeDef = TypedDict(
     "CredentialsTypeDef",
     {
         "accessKeyId": str,
         "secretAccessKey": str,
         "sessionToken": str,
     },
@@ -377,24 +326,14 @@
     {
         "errorMessage": str,
         "errorCategory": ErrorCategoryType,
     },
     total=False,
 )
 
-DatasetOwnerInfoOutputTypeDef = TypedDict(
-    "DatasetOwnerInfoOutputTypeDef",
-    {
-        "name": str,
-        "phoneNumber": str,
-        "email": str,
-    },
-    total=False,
-)
-
 _RequiredDeleteDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteDatasetRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalDeleteDatasetRequestRequestTypeDef = TypedDict(
@@ -406,22 +345,14 @@
 )
 
 class DeleteDatasetRequestRequestTypeDef(
     _RequiredDeleteDatasetRequestRequestTypeDef, _OptionalDeleteDatasetRequestRequestTypeDef
 ):
     pass
 
-DeleteDatasetResponseTypeDef = TypedDict(
-    "DeleteDatasetResponseTypeDef",
-    {
-        "datasetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeletePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDeletePermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
     },
 )
 _OptionalDeletePermissionGroupRequestRequestTypeDef = TypedDict(
@@ -434,22 +365,14 @@
 
 class DeletePermissionGroupRequestRequestTypeDef(
     _RequiredDeletePermissionGroupRequestRequestTypeDef,
     _OptionalDeletePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-DeletePermissionGroupResponseTypeDef = TypedDict(
-    "DeletePermissionGroupResponseTypeDef",
-    {
-        "permissionGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisableUserRequestRequestTypeDef = TypedDict(
     "_RequiredDisableUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalDisableUserRequestRequestTypeDef = TypedDict(
@@ -461,22 +384,14 @@
 )
 
 class DisableUserRequestRequestTypeDef(
     _RequiredDisableUserRequestRequestTypeDef, _OptionalDisableUserRequestRequestTypeDef
 ):
     pass
 
-DisableUserResponseTypeDef = TypedDict(
-    "DisableUserResponseTypeDef",
-    {
-        "userId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
         "userId": str,
     },
 )
@@ -490,22 +405,14 @@
 
 class DisassociateUserFromPermissionGroupRequestRequestTypeDef(
     _RequiredDisassociateUserFromPermissionGroupRequestRequestTypeDef,
     _OptionalDisassociateUserFromPermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-DisassociateUserFromPermissionGroupResponseTypeDef = TypedDict(
-    "DisassociateUserFromPermissionGroupResponseTypeDef",
-    {
-        "statusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableUserRequestRequestTypeDef = TypedDict(
     "_RequiredEnableUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalEnableUserRequestRequestTypeDef = TypedDict(
@@ -517,22 +424,14 @@
 )
 
 class EnableUserRequestRequestTypeDef(
     _RequiredEnableUserRequestRequestTypeDef, _OptionalEnableUserRequestRequestTypeDef
 ):
     pass
 
-EnableUserResponseTypeDef = TypedDict(
-    "EnableUserResponseTypeDef",
-    {
-        "userId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetChangesetRequestRequestTypeDef = TypedDict(
     "GetChangesetRequestRequestTypeDef",
     {
         "datasetId": str,
         "changesetId": str,
     },
 )
@@ -612,72 +511,32 @@
 GetUserRequestRequestTypeDef = TypedDict(
     "GetUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 
-GetUserResponseTypeDef = TypedDict(
-    "GetUserResponseTypeDef",
-    {
-        "userId": str,
-        "status": UserStatusType,
-        "firstName": str,
-        "lastName": str,
-        "emailAddress": str,
-        "type": UserTypeType,
-        "apiAccess": ApiAccessType,
-        "apiAccessPrincipalArn": str,
-        "createTime": int,
-        "lastEnabledTime": int,
-        "lastDisabledTime": int,
-        "lastModifiedTime": int,
-        "lastLoginTime": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetWorkingLocationRequestRequestTypeDef = TypedDict(
     "GetWorkingLocationRequestRequestTypeDef",
     {
         "locationType": locationTypeType,
     },
     total=False,
 )
 
-GetWorkingLocationResponseTypeDef = TypedDict(
-    "GetWorkingLocationResponseTypeDef",
-    {
-        "s3Uri": str,
-        "s3Path": str,
-        "s3Bucket": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListChangesetsRequestListChangesetsPaginateTypeDef = TypedDict(
-    "_RequiredListChangesetsRequestListChangesetsPaginateTypeDef",
-    {
-        "datasetId": str,
-    },
-)
-_OptionalListChangesetsRequestListChangesetsPaginateTypeDef = TypedDict(
-    "_OptionalListChangesetsRequestListChangesetsPaginateTypeDef",
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
 
-class ListChangesetsRequestListChangesetsPaginateTypeDef(
-    _RequiredListChangesetsRequestListChangesetsPaginateTypeDef,
-    _OptionalListChangesetsRequestListChangesetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListChangesetsRequestRequestTypeDef = TypedDict(
     "_RequiredListChangesetsRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalListChangesetsRequestRequestTypeDef = TypedDict(
@@ -690,34 +549,14 @@
 )
 
 class ListChangesetsRequestRequestTypeDef(
     _RequiredListChangesetsRequestRequestTypeDef, _OptionalListChangesetsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
-    "_RequiredListDataViewsRequestListDataViewsPaginateTypeDef",
-    {
-        "datasetId": str,
-    },
-)
-_OptionalListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
-    "_OptionalListDataViewsRequestListDataViewsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDataViewsRequestListDataViewsPaginateTypeDef(
-    _RequiredListDataViewsRequestListDataViewsPaginateTypeDef,
-    _OptionalListDataViewsRequestListDataViewsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDataViewsRequestRequestTypeDef = TypedDict(
     "_RequiredListDataViewsRequestRequestTypeDef",
     {
         "datasetId": str,
     },
 )
 _OptionalListDataViewsRequestRequestTypeDef = TypedDict(
@@ -730,22 +569,14 @@
 )
 
 class ListDataViewsRequestRequestTypeDef(
     _RequiredListDataViewsRequestRequestTypeDef, _OptionalListDataViewsRequestRequestTypeDef
 ):
     pass
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -778,22 +609,14 @@
         "permissionGroupId": str,
         "name": str,
         "membershipStatus": PermissionGroupMembershipStatusType,
     },
     total=False,
 )
 
-ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef = TypedDict(
-    "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListPermissionGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListPermissionGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
     },
 )
 _OptionalListPermissionGroupsRequestRequestTypeDef = TypedDict(
@@ -843,22 +666,14 @@
         "apiAccess": ApiAccessType,
         "apiAccessPrincipalArn": str,
         "membershipStatus": PermissionGroupMembershipStatusType,
     },
     total=False,
 )
 
-ListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "ListUsersRequestListUsersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "maxResults": int,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -890,24 +705,14 @@
         "lastDisabledTime": int,
         "lastModifiedTime": int,
         "lastLoginTime": int,
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
 ResourcePermissionTypeDef = TypedDict(
     "ResourcePermissionTypeDef",
     {
         "permission": str,
     },
     total=False,
 )
@@ -927,34 +732,14 @@
 )
 
 class ResetUserPasswordRequestRequestTypeDef(
     _RequiredResetUserPasswordRequestRequestTypeDef, _OptionalResetUserPasswordRequestRequestTypeDef
 ):
     pass
 
-ResetUserPasswordResponseTypeDef = TypedDict(
-    "ResetUserPasswordResponseTypeDef",
-    {
-        "userId": str,
-        "temporaryPassword": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 _RequiredUpdateChangesetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChangesetRequestRequestTypeDef",
     {
         "datasetId": str,
         "changesetId": str,
         "sourceParams": Mapping[str, str],
         "formatParams": Mapping[str, str],
@@ -969,31 +754,14 @@
 )
 
 class UpdateChangesetRequestRequestTypeDef(
     _RequiredUpdateChangesetRequestRequestTypeDef, _OptionalUpdateChangesetRequestRequestTypeDef
 ):
     pass
 
-UpdateChangesetResponseTypeDef = TypedDict(
-    "UpdateChangesetResponseTypeDef",
-    {
-        "changesetId": str,
-        "datasetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDatasetResponseTypeDef = TypedDict(
-    "UpdateDatasetResponseTypeDef",
-    {
-        "datasetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdatePermissionGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePermissionGroupRequestRequestTypeDef",
     {
         "permissionGroupId": str,
     },
 )
 _OptionalUpdatePermissionGroupRequestRequestTypeDef = TypedDict(
@@ -1009,22 +777,14 @@
 
 class UpdatePermissionGroupRequestRequestTypeDef(
     _RequiredUpdatePermissionGroupRequestRequestTypeDef,
     _OptionalUpdatePermissionGroupRequestRequestTypeDef,
 ):
     pass
 
-UpdatePermissionGroupResponseTypeDef = TypedDict(
-    "UpdatePermissionGroupResponseTypeDef",
-    {
-        "permissionGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateUserRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateUserRequestRequestTypeDef",
     {
         "userId": str,
     },
 )
 _OptionalUpdateUserRequestRequestTypeDef = TypedDict(
@@ -1041,19 +801,173 @@
 )
 
 class UpdateUserRequestRequestTypeDef(
     _RequiredUpdateUserRequestRequestTypeDef, _OptionalUpdateUserRequestRequestTypeDef
 ):
     pass
 
+AssociateUserToPermissionGroupResponseTypeDef = TypedDict(
+    "AssociateUserToPermissionGroupResponseTypeDef",
+    {
+        "statusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateChangesetResponseTypeDef = TypedDict(
+    "CreateChangesetResponseTypeDef",
+    {
+        "datasetId": str,
+        "changesetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataViewResponseTypeDef = TypedDict(
+    "CreateDataViewResponseTypeDef",
+    {
+        "datasetId": str,
+        "dataViewId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "datasetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePermissionGroupResponseTypeDef = TypedDict(
+    "CreatePermissionGroupResponseTypeDef",
+    {
+        "permissionGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserResponseTypeDef = TypedDict(
+    "CreateUserResponseTypeDef",
+    {
+        "userId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDatasetResponseTypeDef = TypedDict(
+    "DeleteDatasetResponseTypeDef",
+    {
+        "datasetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeletePermissionGroupResponseTypeDef = TypedDict(
+    "DeletePermissionGroupResponseTypeDef",
+    {
+        "permissionGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableUserResponseTypeDef = TypedDict(
+    "DisableUserResponseTypeDef",
+    {
+        "userId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateUserFromPermissionGroupResponseTypeDef = TypedDict(
+    "DisassociateUserFromPermissionGroupResponseTypeDef",
+    {
+        "statusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableUserResponseTypeDef = TypedDict(
+    "EnableUserResponseTypeDef",
+    {
+        "userId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetUserResponseTypeDef = TypedDict(
+    "GetUserResponseTypeDef",
+    {
+        "userId": str,
+        "status": UserStatusType,
+        "firstName": str,
+        "lastName": str,
+        "emailAddress": str,
+        "type": UserTypeType,
+        "apiAccess": ApiAccessType,
+        "apiAccessPrincipalArn": str,
+        "createTime": int,
+        "lastEnabledTime": int,
+        "lastDisabledTime": int,
+        "lastModifiedTime": int,
+        "lastLoginTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetWorkingLocationResponseTypeDef = TypedDict(
+    "GetWorkingLocationResponseTypeDef",
+    {
+        "s3Uri": str,
+        "s3Path": str,
+        "s3Bucket": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ResetUserPasswordResponseTypeDef = TypedDict(
+    "ResetUserPasswordResponseTypeDef",
+    {
+        "userId": str,
+        "temporaryPassword": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateChangesetResponseTypeDef = TypedDict(
+    "UpdateChangesetResponseTypeDef",
+    {
+        "changesetId": str,
+        "datasetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDatasetResponseTypeDef = TypedDict(
+    "UpdateDatasetResponseTypeDef",
+    {
+        "datasetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePermissionGroupResponseTypeDef = TypedDict(
+    "UpdatePermissionGroupResponseTypeDef",
+    {
+        "permissionGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateUserResponseTypeDef = TypedDict(
     "UpdateUserResponseTypeDef",
     {
         "userId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangesetSummaryTypeDef = TypedDict(
     "ChangesetSummaryTypeDef",
     {
         "changesetId": str,
@@ -1085,22 +999,22 @@
         "createTime": int,
         "status": IngestionStatusType,
         "errorInfo": ChangesetErrorInfoTypeDef,
         "activeUntilTimestamp": int,
         "activeFromTimestamp": int,
         "updatesChangesetId": str,
         "updatedByChangesetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SchemaDefinitionOutputTypeDef = TypedDict(
     "SchemaDefinitionOutputTypeDef",
     {
-        "columns": List[ColumnDefinitionOutputTypeDef],
+        "columns": List[ColumnDefinitionTypeDef],
         "primaryKeyColumns": List[str],
     },
     total=False,
 )
 
 SchemaDefinitionTypeDef = TypedDict(
     "SchemaDefinitionTypeDef",
@@ -1136,15 +1050,15 @@
     pass
 
 GetProgrammaticAccessCredentialsResponseTypeDef = TypedDict(
     "GetProgrammaticAccessCredentialsResponseTypeDef",
     {
         "credentials": CredentialsTypeDef,
         "durationInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DataViewSummaryTypeDef = TypedDict(
     "DataViewSummaryTypeDef",
     {
         "dataViewId": str,
@@ -1174,68 +1088,132 @@
         "lastModifiedTime": int,
         "createTime": int,
         "sortColumns": List[str],
         "dataViewId": str,
         "dataViewArn": str,
         "destinationTypeParams": DataViewDestinationTypeParamsOutputTypeDef,
         "status": DataViewStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExternalDataViewAccessDetailsResponseTypeDef = TypedDict(
     "GetExternalDataViewAccessDetailsResponseTypeDef",
     {
         "credentials": AwsCredentialsTypeDef,
         "s3Location": S3LocationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPermissionGroupResponseTypeDef = TypedDict(
     "GetPermissionGroupResponseTypeDef",
     {
         "permissionGroup": PermissionGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPermissionGroupsResponseTypeDef = TypedDict(
     "ListPermissionGroupsResponseTypeDef",
     {
         "permissionGroups": List[PermissionGroupTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListChangesetsRequestListChangesetsPaginateTypeDef = TypedDict(
+    "_RequiredListChangesetsRequestListChangesetsPaginateTypeDef",
+    {
+        "datasetId": str,
+    },
+)
+_OptionalListChangesetsRequestListChangesetsPaginateTypeDef = TypedDict(
+    "_OptionalListChangesetsRequestListChangesetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListChangesetsRequestListChangesetsPaginateTypeDef(
+    _RequiredListChangesetsRequestListChangesetsPaginateTypeDef,
+    _OptionalListChangesetsRequestListChangesetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
+    "_RequiredListDataViewsRequestListDataViewsPaginateTypeDef",
+    {
+        "datasetId": str,
+    },
+)
+_OptionalListDataViewsRequestListDataViewsPaginateTypeDef = TypedDict(
+    "_OptionalListDataViewsRequestListDataViewsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDataViewsRequestListDataViewsPaginateTypeDef(
+    _RequiredListDataViewsRequestListDataViewsPaginateTypeDef,
+    _OptionalListDataViewsRequestListDataViewsPaginateTypeDef,
+):
+    pass
+
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef = TypedDict(
+    "ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "ListUsersRequestListUsersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListPermissionGroupsByUserResponseTypeDef = TypedDict(
     "ListPermissionGroupsByUserResponseTypeDef",
     {
         "permissionGroups": List[PermissionGroupByUserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersByPermissionGroupResponseTypeDef = TypedDict(
     "ListUsersByPermissionGroupResponseTypeDef",
     {
         "users": List[UserByPermissionGroupTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "users": List[UserTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PermissionGroupParamsTypeDef = TypedDict(
     "PermissionGroupParamsTypeDef",
     {
         "permissionGroupId": str,
@@ -1245,15 +1223,15 @@
 )
 
 ListChangesetsResponseTypeDef = TypedDict(
     "ListChangesetsResponseTypeDef",
     {
         "changesets": List[ChangesetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SchemaUnionOutputTypeDef = TypedDict(
     "SchemaUnionOutputTypeDef",
     {
         "tabularSchemaConfig": SchemaDefinitionOutputTypeDef,
@@ -1270,27 +1248,27 @@
 )
 
 ListDataViewsResponseTypeDef = TypedDict(
     "ListDataViewsResponseTypeDef",
     {
         "nextToken": str,
         "dataViews": List[DataViewSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DatasetTypeDef = TypedDict(
     "DatasetTypeDef",
     {
         "datasetId": str,
         "datasetArn": str,
         "datasetTitle": str,
         "kind": DatasetKindType,
         "datasetDescription": str,
-        "ownerInfo": DatasetOwnerInfoOutputTypeDef,
+        "ownerInfo": DatasetOwnerInfoTypeDef,
         "createTime": int,
         "lastModifiedTime": int,
         "schemaDefinition": SchemaUnionOutputTypeDef,
         "alias": str,
     },
     total=False,
 )
@@ -1304,15 +1282,15 @@
         "kind": DatasetKindType,
         "datasetDescription": str,
         "createTime": int,
         "lastModifiedTime": int,
         "schemaDefinition": SchemaUnionOutputTypeDef,
         "alias": str,
         "status": DatasetStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "datasetTitle": str,
@@ -1362,10 +1340,10 @@
     pass
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "datasets": List[DatasetTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/PKG-INFO` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-finspace-data
-Version: 1.28.12
-Summary: Type annotations for boto3.FinSpaceData 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-finspace-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-finspace-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-finspace-data)](https://pepy.tech/project/mypy-boto3-finspace-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FinSpaceData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
+[boto3.FinSpaceData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/finspace-data.html#FinSpaceData)
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
 [mypy-boto3-finspace-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_finspace_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,93 +350,91 @@
 
 `mypy_boto3_finspace_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_finspace_data.type_defs import (
     AssociateUserToPermissionGroupRequestRequestTypeDef,
-    AssociateUserToPermissionGroupResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsCredentialsTypeDef,
     ChangesetErrorInfoTypeDef,
-    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
     CreateChangesetRequestRequestTypeDef,
-    CreateChangesetResponseTypeDef,
     DataViewDestinationTypeParamsTypeDef,
-    CreateDataViewResponseTypeDef,
     DatasetOwnerInfoTypeDef,
-    CreateDatasetResponseTypeDef,
     CreatePermissionGroupRequestRequestTypeDef,
-    CreatePermissionGroupResponseTypeDef,
     CreateUserRequestRequestTypeDef,
-    CreateUserResponseTypeDef,
     CredentialsTypeDef,
     DataViewDestinationTypeParamsOutputTypeDef,
     DataViewErrorInfoTypeDef,
-    DatasetOwnerInfoOutputTypeDef,
     DeleteDatasetRequestRequestTypeDef,
-    DeleteDatasetResponseTypeDef,
     DeletePermissionGroupRequestRequestTypeDef,
-    DeletePermissionGroupResponseTypeDef,
     DisableUserRequestRequestTypeDef,
-    DisableUserResponseTypeDef,
     DisassociateUserFromPermissionGroupRequestRequestTypeDef,
-    DisassociateUserFromPermissionGroupResponseTypeDef,
     EnableUserRequestRequestTypeDef,
-    EnableUserResponseTypeDef,
     GetChangesetRequestRequestTypeDef,
     GetDataViewRequestRequestTypeDef,
     GetDatasetRequestRequestTypeDef,
     GetExternalDataViewAccessDetailsRequestRequestTypeDef,
     S3LocationTypeDef,
     GetPermissionGroupRequestRequestTypeDef,
     PermissionGroupTypeDef,
     GetProgrammaticAccessCredentialsRequestRequestTypeDef,
     GetUserRequestRequestTypeDef,
-    GetUserResponseTypeDef,
     GetWorkingLocationRequestRequestTypeDef,
-    GetWorkingLocationResponseTypeDef,
-    ListChangesetsRequestListChangesetsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListChangesetsRequestRequestTypeDef,
-    ListDataViewsRequestListDataViewsPaginateTypeDef,
     ListDataViewsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     ListPermissionGroupsByUserRequestRequestTypeDef,
     PermissionGroupByUserTypeDef,
-    ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef,
     ListPermissionGroupsRequestRequestTypeDef,
     ListUsersByPermissionGroupRequestRequestTypeDef,
     UserByPermissionGroupTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     UserTypeDef,
-    PaginatorConfigTypeDef,
     ResourcePermissionTypeDef,
     ResetUserPasswordRequestRequestTypeDef,
-    ResetUserPasswordResponseTypeDef,
-    ResponseMetadataTypeDef,
     UpdateChangesetRequestRequestTypeDef,
+    UpdatePermissionGroupRequestRequestTypeDef,
+    UpdateUserRequestRequestTypeDef,
+    AssociateUserToPermissionGroupResponseTypeDef,
+    CreateChangesetResponseTypeDef,
+    CreateDataViewResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreatePermissionGroupResponseTypeDef,
+    CreateUserResponseTypeDef,
+    DeleteDatasetResponseTypeDef,
+    DeletePermissionGroupResponseTypeDef,
+    DisableUserResponseTypeDef,
+    DisassociateUserFromPermissionGroupResponseTypeDef,
+    EnableUserResponseTypeDef,
+    GetUserResponseTypeDef,
+    GetWorkingLocationResponseTypeDef,
+    ResetUserPasswordResponseTypeDef,
     UpdateChangesetResponseTypeDef,
     UpdateDatasetResponseTypeDef,
-    UpdatePermissionGroupRequestRequestTypeDef,
     UpdatePermissionGroupResponseTypeDef,
-    UpdateUserRequestRequestTypeDef,
     UpdateUserResponseTypeDef,
     ChangesetSummaryTypeDef,
     GetChangesetResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     CreateDataViewRequestRequestTypeDef,
     GetProgrammaticAccessCredentialsResponseTypeDef,
     DataViewSummaryTypeDef,
     GetDataViewResponseTypeDef,
     GetExternalDataViewAccessDetailsResponseTypeDef,
     GetPermissionGroupResponseTypeDef,
     ListPermissionGroupsResponseTypeDef,
+    ListChangesetsRequestListChangesetsPaginateTypeDef,
+    ListDataViewsRequestListDataViewsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListPermissionGroupsRequestListPermissionGroupsPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     ListPermissionGroupsByUserResponseTypeDef,
     ListUsersByPermissionGroupResponseTypeDef,
     ListUsersResponseTypeDef,
     PermissionGroupParamsTypeDef,
     ListChangesetsResponseTypeDef,
     SchemaUnionOutputTypeDef,
     SchemaUnionTypeDef,
```

### Comparing `mypy-boto3-finspace-data-1.28.12/mypy_boto3_finspace_data.egg-info/SOURCES.txt` & `mypy-boto3-finspace-data-1.28.15/mypy_boto3_finspace_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-finspace-data-1.28.12/setup.py` & `mypy-boto3-finspace-data-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-finspace-data",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_finspace_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FinSpaceData 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.FinSpaceData 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

