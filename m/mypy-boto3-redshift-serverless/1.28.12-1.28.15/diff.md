# Comparing `tmp/mypy-boto3-redshift-serverless-1.28.12.tar.gz` & `tmp/mypy-boto3-redshift-serverless-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-serverless-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-serverless-1.28.15.tar", last modified: Fri Jul 28 20:43:33 2023, max compression
```

## Comparing `mypy-boto3-redshift-serverless-1.28.12.tar` & `mypy-boto3-redshift-serverless-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.181212 mypy-boto3-redshift-serverless-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-27 11:49:30.181212 mypy-boto3-redshift-serverless-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.169212 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32938 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34089 2023-07-27 11:44:27.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34058 2023-07-27 11:44:27.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.181212 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18401 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 11:49:29.000000 mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.181212 mypy-boto3-redshift-serverless-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 11:44:26.000000 mypy-boto3-redshift-serverless-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.749727 mypy-boto3-redshift-serverless-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:40.000000 mypy-boto3-redshift-serverless-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-28 20:43:33.741727 mypy-boto3-redshift-serverless-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16805 2023-07-28 20:36:40.000000 mypy-boto3-redshift-serverless-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.709727 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32992 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32938 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9409 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:41.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33722 2023-07-28 20:36:45.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33691 2023-07-28 20:36:42.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:40.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.741727 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-07-28 20:43:33.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 20:43:33.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:43:33.000000 mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:33.749727 mypy-boto3-redshift-serverless-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-28 20:36:40.000000 mypy-boto3-redshift-serverless-1.28.15/setup.py
```

### Comparing `mypy-boto3-redshift-serverless-1.28.12/LICENSE` & `mypy-boto3-redshift-serverless-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/PKG-INFO` & `mypy-boto3-redshift-serverless-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.28.12
-Summary: Type annotations for boto3.RedshiftServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RedshiftServerless 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,15 +353,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
-    ConfigParameterOutputTypeDef,
     ConfigParameterTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
@@ -388,15 +387,14 @@
     PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
@@ -408,14 +406,15 @@
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     GetCredentialsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -440,15 +439,14 @@
     ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -458,15 +456,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterOutputTypeDef:
+def get_structure() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.12/README.md` & `mypy-boto3-redshift-serverless-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,15 +321,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
-    ConfigParameterOutputTypeDef,
     ConfigParameterTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
@@ -356,15 +355,14 @@
     PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
@@ -376,14 +374,15 @@
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     GetCredentialsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -408,15 +407,14 @@
     ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -426,15 +424,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterOutputTypeDef:
+def get_structure() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__init__.py` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__init__.pyi` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/__main__.py` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftServerless 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.RedshiftServerless 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless\nOther"
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

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/client.py` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/client.pyi` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/literals.py` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/literals.pyi` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/paginator.py` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/paginator.pyi` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/type_defs.py` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for redshift-serverless service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_redshift_serverless.type_defs import ConfigParameterOutputTypeDef
+    from mypy_boto3_redshift_serverless.type_defs import ConfigParameterTypeDef
 
-    data: ConfigParameterOutputTypeDef = {...}
+    data: ConfigParameterTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -28,15 +28,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "ConfigParameterOutputTypeDef",
     "ConfigParameterTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateEndpointAccessRequestRequestTypeDef",
     "NamespaceTypeDef",
     "CreateUsageLimitRequestRequestTypeDef",
@@ -63,15 +62,14 @@
     "PaginatorConfigTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListRecoveryPointsRequestRequestTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
@@ -83,14 +81,15 @@
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetCredentialsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateNamespaceResponseTypeDef",
@@ -115,15 +114,14 @@
     "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -132,23 +130,14 @@
     "CreateWorkgroupResponseTypeDef",
     "DeleteWorkgroupResponseTypeDef",
     "GetWorkgroupResponseTypeDef",
     "ListWorkgroupsResponseTypeDef",
     "UpdateWorkgroupResponseTypeDef",
 )
 
-ConfigParameterOutputTypeDef = TypedDict(
-    "ConfigParameterOutputTypeDef",
-    {
-        "parameterKey": str,
-        "parameterValue": str,
-    },
-    total=False,
-)
-
 ConfigParameterTypeDef = TypedDict(
     "ConfigParameterTypeDef",
     {
         "parameterKey": str,
         "parameterValue": str,
     },
     total=False,
@@ -542,22 +531,14 @@
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
 ListUsageLimitsRequestRequestTypeDef = TypedDict(
     "ListUsageLimitsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "resourceArn": str,
         "usageType": UsageLimitUsageTypeType,
@@ -902,14 +883,22 @@
         "dbUser": str,
         "expiration": datetime,
         "nextRefreshTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConvertRecoveryPointToSnapshotResponseTypeDef = TypedDict(
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1181,22 +1170,14 @@
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "vpcEndpointId": str,
         "vpcId": str,
     },
@@ -1271,15 +1252,15 @@
     },
 )
 
 WorkgroupTypeDef = TypedDict(
     "WorkgroupTypeDef",
     {
         "baseCapacity": int,
-        "configParameters": List[ConfigParameterOutputTypeDef],
+        "configParameters": List[ConfigParameterTypeDef],
         "creationDate": datetime,
         "endpoint": EndpointTypeDef,
         "enhancedVpcRouting": bool,
         "namespaceName": str,
         "port": int,
         "publiclyAccessible": bool,
         "securityGroupIds": List[str],
```

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless/type_defs.pyi` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for redshift-serverless service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_redshift_serverless.type_defs import ConfigParameterOutputTypeDef
+    from mypy_boto3_redshift_serverless.type_defs import ConfigParameterTypeDef
 
-    data: ConfigParameterOutputTypeDef = {...}
+    data: ConfigParameterTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -27,15 +27,14 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "ConfigParameterOutputTypeDef",
     "ConfigParameterTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "SnapshotTypeDef",
     "CreateEndpointAccessRequestRequestTypeDef",
     "NamespaceTypeDef",
     "CreateUsageLimitRequestRequestTypeDef",
@@ -62,15 +61,14 @@
     "PaginatorConfigTypeDef",
     "ListEndpointAccessRequestRequestTypeDef",
     "ListNamespacesRequestRequestTypeDef",
     "ListRecoveryPointsRequestRequestTypeDef",
     "ListSnapshotsRequestRequestTypeDef",
     "ListTableRestoreStatusRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListUsageLimitsRequestRequestTypeDef",
     "ListWorkgroupsRequestRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RestoreFromRecoveryPointRequestRequestTypeDef",
     "RestoreFromSnapshotRequestRequestTypeDef",
     "RestoreTableFromSnapshotRequestRequestTypeDef",
@@ -82,14 +80,15 @@
     "UpdateWorkgroupRequestRequestTypeDef",
     "ConvertRecoveryPointToSnapshotRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateSnapshotRequestRequestTypeDef",
     "CreateWorkgroupRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetCredentialsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     "CreateSnapshotResponseTypeDef",
     "DeleteSnapshotResponseTypeDef",
     "GetSnapshotResponseTypeDef",
     "ListSnapshotsResponseTypeDef",
     "UpdateSnapshotResponseTypeDef",
     "CreateNamespaceResponseTypeDef",
@@ -114,15 +113,14 @@
     "ListEndpointAccessRequestListEndpointAccessPaginateTypeDef",
     "ListNamespacesRequestListNamespacesPaginateTypeDef",
     "ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef",
     "ListSnapshotsRequestListSnapshotsPaginateTypeDef",
     "ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef",
     "ListUsageLimitsRequestListUsageLimitsPaginateTypeDef",
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "VpcEndpointTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "CreateEndpointAccessResponseTypeDef",
     "DeleteEndpointAccessResponseTypeDef",
     "GetEndpointAccessResponseTypeDef",
     "ListEndpointAccessResponseTypeDef",
@@ -131,23 +129,14 @@
     "CreateWorkgroupResponseTypeDef",
     "DeleteWorkgroupResponseTypeDef",
     "GetWorkgroupResponseTypeDef",
     "ListWorkgroupsResponseTypeDef",
     "UpdateWorkgroupResponseTypeDef",
 )
 
-ConfigParameterOutputTypeDef = TypedDict(
-    "ConfigParameterOutputTypeDef",
-    {
-        "parameterKey": str,
-        "parameterValue": str,
-    },
-    total=False,
-)
-
 ConfigParameterTypeDef = TypedDict(
     "ConfigParameterTypeDef",
     {
         "parameterKey": str,
         "parameterValue": str,
     },
     total=False,
@@ -533,22 +522,14 @@
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
 ListUsageLimitsRequestRequestTypeDef = TypedDict(
     "ListUsageLimitsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "resourceArn": str,
         "usageType": UsageLimitUsageTypeType,
@@ -871,14 +852,22 @@
         "dbUser": str,
         "expiration": datetime,
         "nextRefreshTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConvertRecoveryPointToSnapshotResponseTypeDef = TypedDict(
     "ConvertRecoveryPointToSnapshotResponseTypeDef",
     {
         "snapshot": SnapshotTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1150,22 +1139,14 @@
     "ListWorkgroupsRequestListWorkgroupsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "networkInterfaces": List[NetworkInterfaceTypeDef],
         "vpcEndpointId": str,
         "vpcId": str,
     },
@@ -1240,15 +1221,15 @@
     },
 )
 
 WorkgroupTypeDef = TypedDict(
     "WorkgroupTypeDef",
     {
         "baseCapacity": int,
-        "configParameters": List[ConfigParameterOutputTypeDef],
+        "configParameters": List[ConfigParameterTypeDef],
         "creationDate": datetime,
         "endpoint": EndpointTypeDef,
         "enhancedVpcRouting": bool,
         "namespaceName": str,
         "port": int,
         "publiclyAccessible": bool,
         "securityGroupIds": List[str],
```

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/PKG-INFO` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-serverless
-Version: 1.28.12
-Summary: Type annotations for boto3.RedshiftServerless 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RedshiftServerless 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-serverless.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-serverless)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-serverless)](https://pepy.tech/project/mypy-boto3-redshift-serverless)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftServerless 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
+[boto3.RedshiftServerless 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-serverless.html#RedshiftServerless)
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
 [mypy-boto3-redshift-serverless docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_serverless/).
 
 See how it helps to find and fix potential bugs:
 
@@ -353,15 +353,14 @@
 ### Typed dictionaries
 
 `mypy_boto3_redshift_serverless.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_redshift_serverless.type_defs import (
-    ConfigParameterOutputTypeDef,
     ConfigParameterTypeDef,
     TagTypeDef,
     ResponseMetadataTypeDef,
     SnapshotTypeDef,
     CreateEndpointAccessRequestRequestTypeDef,
     NamespaceTypeDef,
     CreateUsageLimitRequestRequestTypeDef,
@@ -388,15 +387,14 @@
     PaginatorConfigTypeDef,
     ListEndpointAccessRequestRequestTypeDef,
     ListNamespacesRequestRequestTypeDef,
     ListRecoveryPointsRequestRequestTypeDef,
     ListSnapshotsRequestRequestTypeDef,
     ListTableRestoreStatusRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListUsageLimitsRequestRequestTypeDef,
     ListWorkgroupsRequestRequestTypeDef,
     NetworkInterfaceTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RestoreFromRecoveryPointRequestRequestTypeDef,
     RestoreFromSnapshotRequestRequestTypeDef,
     RestoreTableFromSnapshotRequestRequestTypeDef,
@@ -408,14 +406,15 @@
     UpdateWorkgroupRequestRequestTypeDef,
     ConvertRecoveryPointToSnapshotRequestRequestTypeDef,
     CreateNamespaceRequestRequestTypeDef,
     CreateSnapshotRequestRequestTypeDef,
     CreateWorkgroupRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     GetCredentialsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ConvertRecoveryPointToSnapshotResponseTypeDef,
     CreateSnapshotResponseTypeDef,
     DeleteSnapshotResponseTypeDef,
     GetSnapshotResponseTypeDef,
     ListSnapshotsResponseTypeDef,
     UpdateSnapshotResponseTypeDef,
     CreateNamespaceResponseTypeDef,
@@ -440,15 +439,14 @@
     ListEndpointAccessRequestListEndpointAccessPaginateTypeDef,
     ListNamespacesRequestListNamespacesPaginateTypeDef,
     ListRecoveryPointsRequestListRecoveryPointsPaginateTypeDef,
     ListSnapshotsRequestListSnapshotsPaginateTypeDef,
     ListTableRestoreStatusRequestListTableRestoreStatusPaginateTypeDef,
     ListUsageLimitsRequestListUsageLimitsPaginateTypeDef,
     ListWorkgroupsRequestListWorkgroupsPaginateTypeDef,
-    ListTagsForResourceResponseTypeDef,
     VpcEndpointTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     CreateEndpointAccessResponseTypeDef,
     DeleteEndpointAccessResponseTypeDef,
     GetEndpointAccessResponseTypeDef,
     ListEndpointAccessResponseTypeDef,
@@ -458,15 +456,15 @@
     DeleteWorkgroupResponseTypeDef,
     GetWorkgroupResponseTypeDef,
     ListWorkgroupsResponseTypeDef,
     UpdateWorkgroupResponseTypeDef,
 )
 
 
-def get_structure() -> ConfigParameterOutputTypeDef:
+def get_structure() -> ConfigParameterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-redshift-serverless-1.28.12/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt` & `mypy-boto3-redshift-serverless-1.28.15/mypy_boto3_redshift_serverless.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-serverless-1.28.12/setup.py` & `mypy-boto3-redshift-serverless-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift-serverless",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_redshift_serverless"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RedshiftServerless 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.RedshiftServerless 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

