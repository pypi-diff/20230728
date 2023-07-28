# Comparing `tmp/mypy-boto3-keyspaces-1.28.12.tar.gz` & `tmp/mypy-boto3-keyspaces-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-keyspaces-1.28.12.tar", last modified: Thu Jul 27 05:34:53 2023, max compression
+gzip compressed data, was "mypy-boto3-keyspaces-1.28.15.tar", last modified: Fri Jul 28 20:43:05 2023, max compression
```

## Comparing `mypy-boto3-keyspaces-1.28.12.tar` & `mypy-boto3-keyspaces-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.204469 mypy-boto3-keyspaces-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-07-27 05:34:53.204469 mypy-boto3-keyspaces-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13468 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.200469 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-07-27 05:24:38.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19050 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.204469 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14963 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:53.000000 mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:53.204469 mypy-boto3-keyspaces-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:24:37.000000 mypy-boto3-keyspaces-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.025333 mypy-boto3-keyspaces-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-07-28 20:43:05.025333 mypy-boto3-keyspaces-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.009333 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13482 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13459 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9156 2023-07-28 20:29:09.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9154 2023-07-28 20:29:09.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17225 2023-07-28 20:29:09.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17193 2023-07-28 20:29:09.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.025333 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14676 2023-07-28 20:43:04.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:04.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:04.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:04.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:04.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:04.000000 mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:05.025333 mypy-boto3-keyspaces-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:29:08.000000 mypy-boto3-keyspaces-1.28.15/setup.py
```

### Comparing `mypy-boto3-keyspaces-1.28.12/LICENSE` & `mypy-boto3-keyspaces-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.12/PKG-INFO` & `mypy-boto3-keyspaces-1.28.15/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.28.12
-Summary: Type annotations for boto3.Keyspaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Keyspaces 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,62 +338,53 @@
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
-    ClientSideTimestampsOutputTypeDef,
     ClientSideTimestampsTypeDef,
-    ClusteringKeyOutputTypeDef,
     ClusteringKeyTypeDef,
-    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
-    CommentOutputTypeDef,
     CommentTypeDef,
     ReplicationSpecificationTypeDef,
     TagTypeDef,
-    CreateKeyspaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
-    CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
-    EncryptionSpecificationOutputTypeDef,
     GetKeyspaceRequestRequestTypeDef,
-    GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
-    TimeToLiveOutputTypeDef,
     KeyspaceSummaryTypeDef,
-    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKeyspacesRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreTableResponseTypeDef,
-    StaticColumnOutputTypeDef,
     StaticColumnTypeDef,
-    UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateKeyspaceResponseTypeDef,
+    CreateTableResponseTypeDef,
+    GetKeyspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RestoreTableResponseTypeDef,
+    UpdateTableResponseTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
+    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     GetTableResponseTypeDef,
     CreateTableRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-keyspaces-1.28.12/README.md` & `mypy-boto3-keyspaces-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,62 +306,53 @@
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
-    ClientSideTimestampsOutputTypeDef,
     ClientSideTimestampsTypeDef,
-    ClusteringKeyOutputTypeDef,
     ClusteringKeyTypeDef,
-    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
-    CommentOutputTypeDef,
     CommentTypeDef,
     ReplicationSpecificationTypeDef,
     TagTypeDef,
-    CreateKeyspaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
-    CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
-    EncryptionSpecificationOutputTypeDef,
     GetKeyspaceRequestRequestTypeDef,
-    GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
-    TimeToLiveOutputTypeDef,
     KeyspaceSummaryTypeDef,
-    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKeyspacesRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreTableResponseTypeDef,
-    StaticColumnOutputTypeDef,
     StaticColumnTypeDef,
-    UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateKeyspaceResponseTypeDef,
+    CreateTableResponseTypeDef,
+    GetKeyspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RestoreTableResponseTypeDef,
+    UpdateTableResponseTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
+    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     GetTableResponseTypeDef,
     CreateTableRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__init__.py` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__init__.pyi` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/__main__.py` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Keyspaces 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Keyspaces 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces\nOther"
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

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/client.py` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/client.pyi` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/literals.py` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/literals.pyi` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/paginator.py` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,61 +32,56 @@
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListKeyspacesPaginator", "ListTablesPaginator", "ListTagsForResourcePaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListKeyspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listkeyspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyspacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listkeyspacespaginator)
         """
 
-
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, keyspaceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, keyspaceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtablespaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/paginator.pyi` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,56 +32,61 @@
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListKeyspacesPaginator", "ListTablesPaginator", "ListTagsForResourcePaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListKeyspacesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listkeyspacespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListKeyspacesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListKeyspaces.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listkeyspacespaginator)
         """
 
+
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, keyspaceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, keyspaceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtablespaginator)
         """
 
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/type_defs.py` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,62 +33,53 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
-    "ClientSideTimestampsOutputTypeDef",
     "ClientSideTimestampsTypeDef",
-    "ClusteringKeyOutputTypeDef",
     "ClusteringKeyTypeDef",
-    "ColumnDefinitionOutputTypeDef",
     "ColumnDefinitionTypeDef",
-    "CommentOutputTypeDef",
     "CommentTypeDef",
     "ReplicationSpecificationTypeDef",
     "TagTypeDef",
-    "CreateKeyspaceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "EncryptionSpecificationTypeDef",
     "PointInTimeRecoveryTypeDef",
     "TimeToLiveTypeDef",
-    "CreateTableResponseTypeDef",
     "DeleteKeyspaceRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
-    "EncryptionSpecificationOutputTypeDef",
     "GetKeyspaceRequestRequestTypeDef",
-    "GetKeyspaceResponseTypeDef",
     "GetTableRequestRequestTypeDef",
     "PointInTimeRecoverySummaryTypeDef",
-    "TimeToLiveOutputTypeDef",
     "KeyspaceSummaryTypeDef",
-    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListKeyspacesRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableSummaryTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "PartitionKeyOutputTypeDef",
     "PartitionKeyTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreTableResponseTypeDef",
-    "StaticColumnOutputTypeDef",
     "StaticColumnTypeDef",
-    "UpdateTableResponseTypeDef",
     "CreateKeyspaceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateKeyspaceResponseTypeDef",
+    "CreateTableResponseTypeDef",
+    "GetKeyspaceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RestoreTableResponseTypeDef",
+    "UpdateTableResponseTypeDef",
     "RestoreTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "ListKeyspacesResponseTypeDef",
+    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTablesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "GetTableResponseTypeDef",
     "CreateTableRequestRequestTypeDef",
 )
 
 _RequiredCapacitySpecificationSummaryTypeDef = TypedDict(
@@ -132,67 +123,37 @@
 
 class CapacitySpecificationTypeDef(
     _RequiredCapacitySpecificationTypeDef, _OptionalCapacitySpecificationTypeDef
 ):
     pass
 
 
-ClientSideTimestampsOutputTypeDef = TypedDict(
-    "ClientSideTimestampsOutputTypeDef",
-    {
-        "status": Literal["ENABLED"],
-    },
-)
-
 ClientSideTimestampsTypeDef = TypedDict(
     "ClientSideTimestampsTypeDef",
     {
         "status": Literal["ENABLED"],
     },
 )
 
-ClusteringKeyOutputTypeDef = TypedDict(
-    "ClusteringKeyOutputTypeDef",
-    {
-        "name": str,
-        "orderBy": SortOrderType,
-    },
-)
-
 ClusteringKeyTypeDef = TypedDict(
     "ClusteringKeyTypeDef",
     {
         "name": str,
         "orderBy": SortOrderType,
     },
 )
 
-ColumnDefinitionOutputTypeDef = TypedDict(
-    "ColumnDefinitionOutputTypeDef",
-    {
-        "name": str,
-        "type": str,
-    },
-)
-
 ColumnDefinitionTypeDef = TypedDict(
     "ColumnDefinitionTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 
-CommentOutputTypeDef = TypedDict(
-    "CommentOutputTypeDef",
-    {
-        "message": str,
-    },
-)
-
 CommentTypeDef = TypedDict(
     "CommentTypeDef",
     {
         "message": str,
     },
 )
 
@@ -221,19 +182,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-CreateKeyspaceResponseTypeDef = TypedDict(
-    "CreateKeyspaceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredEncryptionSpecificationTypeDef = TypedDict(
     "_RequiredEncryptionSpecificationTypeDef",
     {
         "type": EncryptionTypeType,
@@ -264,22 +228,14 @@
 TimeToLiveTypeDef = TypedDict(
     "TimeToLiveTypeDef",
     {
         "status": Literal["ENABLED"],
     },
 )
 
-CreateTableResponseTypeDef = TypedDict(
-    "CreateTableResponseTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteKeyspaceRequestRequestTypeDef = TypedDict(
     "DeleteKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
@@ -287,53 +243,21 @@
     "DeleteTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
 
-_RequiredEncryptionSpecificationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionSpecificationOutputTypeDef",
-    {
-        "type": EncryptionTypeType,
-    },
-)
-_OptionalEncryptionSpecificationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionSpecificationOutputTypeDef",
-    {
-        "kmsKeyIdentifier": str,
-    },
-    total=False,
-)
-
-
-class EncryptionSpecificationOutputTypeDef(
-    _RequiredEncryptionSpecificationOutputTypeDef, _OptionalEncryptionSpecificationOutputTypeDef
-):
-    pass
-
-
 GetKeyspaceRequestRequestTypeDef = TypedDict(
     "GetKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
-GetKeyspaceResponseTypeDef = TypedDict(
-    "GetKeyspaceResponseTypeDef",
-    {
-        "keyspaceName": str,
-        "resourceArn": str,
-        "replicationStrategy": rsType,
-        "replicationRegions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTableRequestRequestTypeDef = TypedDict(
     "GetTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
@@ -355,21 +279,14 @@
 
 class PointInTimeRecoverySummaryTypeDef(
     _RequiredPointInTimeRecoverySummaryTypeDef, _OptionalPointInTimeRecoverySummaryTypeDef
 ):
     pass
 
 
-TimeToLiveOutputTypeDef = TypedDict(
-    "TimeToLiveOutputTypeDef",
-    {
-        "status": Literal["ENABLED"],
-    },
-)
-
 _RequiredKeyspaceSummaryTypeDef = TypedDict(
     "_RequiredKeyspaceSummaryTypeDef",
     {
         "keyspaceName": str,
         "resourceArn": str,
         "replicationStrategy": rsType,
     },
@@ -383,53 +300,33 @@
 )
 
 
 class KeyspaceSummaryTypeDef(_RequiredKeyspaceSummaryTypeDef, _OptionalKeyspaceSummaryTypeDef):
     pass
 
 
-ListKeyspacesRequestListKeyspacesPaginateTypeDef = TypedDict(
-    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
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
 
 ListKeyspacesRequestRequestTypeDef = TypedDict(
     "ListKeyspacesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "keyspaceName": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -453,36 +350,14 @@
     {
         "keyspaceName": str,
         "tableName": str,
         "resourceArn": str,
     },
 )
 
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
@@ -498,87 +373,28 @@
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
-PartitionKeyOutputTypeDef = TypedDict(
-    "PartitionKeyOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
 PartitionKeyTypeDef = TypedDict(
     "PartitionKeyTypeDef",
     {
         "name": str,
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
-RestoreTableResponseTypeDef = TypedDict(
-    "RestoreTableResponseTypeDef",
-    {
-        "restoredTableARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StaticColumnOutputTypeDef = TypedDict(
-    "StaticColumnOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
 StaticColumnTypeDef = TypedDict(
     "StaticColumnTypeDef",
     {
         "name": str,
     },
 )
 
-UpdateTableResponseTypeDef = TypedDict(
-    "UpdateTableResponseTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKeyspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 _OptionalCreateKeyspaceRequestRequestTypeDef = TypedDict(
@@ -609,14 +425,66 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+CreateKeyspaceResponseTypeDef = TypedDict(
+    "CreateKeyspaceResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTableResponseTypeDef = TypedDict(
+    "CreateTableResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyspaceResponseTypeDef = TypedDict(
+    "GetKeyspaceResponseTypeDef",
+    {
+        "keyspaceName": str,
+        "resourceArn": str,
+        "replicationStrategy": rsType,
+        "replicationRegions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreTableResponseTypeDef = TypedDict(
+    "RestoreTableResponseTypeDef",
+    {
+        "restoredTableARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTableResponseTypeDef = TypedDict(
+    "UpdateTableResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredRestoreTableRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreTableRequestRequestTypeDef",
     {
         "sourceKeyspaceName": str,
         "sourceTableName": str,
         "targetKeyspaceName": str,
         "targetTableName": str,
@@ -670,48 +538,91 @@
 
 
 ListKeyspacesResponseTypeDef = TypedDict(
     "ListKeyspacesResponseTypeDef",
     {
         "nextToken": str,
         "keyspaces": List[KeyspaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTablesResponseTypeDef = TypedDict(
-    "ListTablesResponseTypeDef",
+ListKeyspacesRequestListKeyspacesPaginateTypeDef = TypedDict(
+    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     {
-        "nextToken": str,
-        "tables": List[TableSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "keyspaceName": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTablesRequestListTablesPaginateTypeDef(
+    _RequiredListTablesRequestListTablesPaginateTypeDef,
+    _OptionalListTablesRequestListTablesPaginateTypeDef,
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
+ListTablesResponseTypeDef = TypedDict(
+    "ListTablesResponseTypeDef",
     {
         "nextToken": str,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tables": List[TableSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSchemaDefinitionOutputTypeDef = TypedDict(
     "_RequiredSchemaDefinitionOutputTypeDef",
     {
-        "allColumns": List[ColumnDefinitionOutputTypeDef],
-        "partitionKeys": List[PartitionKeyOutputTypeDef],
+        "allColumns": List[ColumnDefinitionTypeDef],
+        "partitionKeys": List[PartitionKeyTypeDef],
     },
 )
 _OptionalSchemaDefinitionOutputTypeDef = TypedDict(
     "_OptionalSchemaDefinitionOutputTypeDef",
     {
-        "clusteringKeys": List[ClusteringKeyOutputTypeDef],
-        "staticColumns": List[StaticColumnOutputTypeDef],
+        "clusteringKeys": List[ClusteringKeyTypeDef],
+        "staticColumns": List[StaticColumnTypeDef],
     },
     total=False,
 )
 
 
 class SchemaDefinitionOutputTypeDef(
     _RequiredSchemaDefinitionOutputTypeDef, _OptionalSchemaDefinitionOutputTypeDef
@@ -746,21 +657,21 @@
         "keyspaceName": str,
         "tableName": str,
         "resourceArn": str,
         "creationTimestamp": datetime,
         "status": TableStatusType,
         "schemaDefinition": SchemaDefinitionOutputTypeDef,
         "capacitySpecification": CapacitySpecificationSummaryTypeDef,
-        "encryptionSpecification": EncryptionSpecificationOutputTypeDef,
+        "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
-        "ttl": TimeToLiveOutputTypeDef,
+        "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
-        "comment": CommentOutputTypeDef,
-        "clientSideTimestamps": ClientSideTimestampsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "comment": CommentTypeDef,
+        "clientSideTimestamps": ClientSideTimestampsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
```

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces/type_defs.pyi` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -32,62 +32,53 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CapacitySpecificationSummaryTypeDef",
     "CapacitySpecificationTypeDef",
-    "ClientSideTimestampsOutputTypeDef",
     "ClientSideTimestampsTypeDef",
-    "ClusteringKeyOutputTypeDef",
     "ClusteringKeyTypeDef",
-    "ColumnDefinitionOutputTypeDef",
     "ColumnDefinitionTypeDef",
-    "CommentOutputTypeDef",
     "CommentTypeDef",
     "ReplicationSpecificationTypeDef",
     "TagTypeDef",
-    "CreateKeyspaceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "EncryptionSpecificationTypeDef",
     "PointInTimeRecoveryTypeDef",
     "TimeToLiveTypeDef",
-    "CreateTableResponseTypeDef",
     "DeleteKeyspaceRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
-    "EncryptionSpecificationOutputTypeDef",
     "GetKeyspaceRequestRequestTypeDef",
-    "GetKeyspaceResponseTypeDef",
     "GetTableRequestRequestTypeDef",
     "PointInTimeRecoverySummaryTypeDef",
-    "TimeToLiveOutputTypeDef",
     "KeyspaceSummaryTypeDef",
-    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListKeyspacesRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableSummaryTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "PartitionKeyOutputTypeDef",
     "PartitionKeyTypeDef",
-    "ResponseMetadataTypeDef",
-    "RestoreTableResponseTypeDef",
-    "StaticColumnOutputTypeDef",
     "StaticColumnTypeDef",
-    "UpdateTableResponseTypeDef",
     "CreateKeyspaceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateKeyspaceResponseTypeDef",
+    "CreateTableResponseTypeDef",
+    "GetKeyspaceResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "RestoreTableResponseTypeDef",
+    "UpdateTableResponseTypeDef",
     "RestoreTableRequestRequestTypeDef",
     "UpdateTableRequestRequestTypeDef",
     "ListKeyspacesResponseTypeDef",
+    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTablesResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "SchemaDefinitionOutputTypeDef",
     "SchemaDefinitionTypeDef",
     "GetTableResponseTypeDef",
     "CreateTableRequestRequestTypeDef",
 )
 
 _RequiredCapacitySpecificationSummaryTypeDef = TypedDict(
@@ -127,67 +118,37 @@
 )
 
 class CapacitySpecificationTypeDef(
     _RequiredCapacitySpecificationTypeDef, _OptionalCapacitySpecificationTypeDef
 ):
     pass
 
-ClientSideTimestampsOutputTypeDef = TypedDict(
-    "ClientSideTimestampsOutputTypeDef",
-    {
-        "status": Literal["ENABLED"],
-    },
-)
-
 ClientSideTimestampsTypeDef = TypedDict(
     "ClientSideTimestampsTypeDef",
     {
         "status": Literal["ENABLED"],
     },
 )
 
-ClusteringKeyOutputTypeDef = TypedDict(
-    "ClusteringKeyOutputTypeDef",
-    {
-        "name": str,
-        "orderBy": SortOrderType,
-    },
-)
-
 ClusteringKeyTypeDef = TypedDict(
     "ClusteringKeyTypeDef",
     {
         "name": str,
         "orderBy": SortOrderType,
     },
 )
 
-ColumnDefinitionOutputTypeDef = TypedDict(
-    "ColumnDefinitionOutputTypeDef",
-    {
-        "name": str,
-        "type": str,
-    },
-)
-
 ColumnDefinitionTypeDef = TypedDict(
     "ColumnDefinitionTypeDef",
     {
         "name": str,
         "type": str,
     },
 )
 
-CommentOutputTypeDef = TypedDict(
-    "CommentOutputTypeDef",
-    {
-        "message": str,
-    },
-)
-
 CommentTypeDef = TypedDict(
     "CommentTypeDef",
     {
         "message": str,
     },
 )
 
@@ -214,19 +175,22 @@
     "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-CreateKeyspaceResponseTypeDef = TypedDict(
-    "CreateKeyspaceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredEncryptionSpecificationTypeDef = TypedDict(
     "_RequiredEncryptionSpecificationTypeDef",
     {
         "type": EncryptionTypeType,
@@ -255,22 +219,14 @@
 TimeToLiveTypeDef = TypedDict(
     "TimeToLiveTypeDef",
     {
         "status": Literal["ENABLED"],
     },
 )
 
-CreateTableResponseTypeDef = TypedDict(
-    "CreateTableResponseTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteKeyspaceRequestRequestTypeDef = TypedDict(
     "DeleteKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
@@ -278,51 +234,21 @@
     "DeleteTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
 
-_RequiredEncryptionSpecificationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionSpecificationOutputTypeDef",
-    {
-        "type": EncryptionTypeType,
-    },
-)
-_OptionalEncryptionSpecificationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionSpecificationOutputTypeDef",
-    {
-        "kmsKeyIdentifier": str,
-    },
-    total=False,
-)
-
-class EncryptionSpecificationOutputTypeDef(
-    _RequiredEncryptionSpecificationOutputTypeDef, _OptionalEncryptionSpecificationOutputTypeDef
-):
-    pass
-
 GetKeyspaceRequestRequestTypeDef = TypedDict(
     "GetKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 
-GetKeyspaceResponseTypeDef = TypedDict(
-    "GetKeyspaceResponseTypeDef",
-    {
-        "keyspaceName": str,
-        "resourceArn": str,
-        "replicationStrategy": rsType,
-        "replicationRegions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTableRequestRequestTypeDef = TypedDict(
     "GetTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
         "tableName": str,
     },
 )
@@ -342,21 +268,14 @@
 )
 
 class PointInTimeRecoverySummaryTypeDef(
     _RequiredPointInTimeRecoverySummaryTypeDef, _OptionalPointInTimeRecoverySummaryTypeDef
 ):
     pass
 
-TimeToLiveOutputTypeDef = TypedDict(
-    "TimeToLiveOutputTypeDef",
-    {
-        "status": Literal["ENABLED"],
-    },
-)
-
 _RequiredKeyspaceSummaryTypeDef = TypedDict(
     "_RequiredKeyspaceSummaryTypeDef",
     {
         "keyspaceName": str,
         "resourceArn": str,
         "replicationStrategy": rsType,
     },
@@ -368,51 +287,33 @@
     },
     total=False,
 )
 
 class KeyspaceSummaryTypeDef(_RequiredKeyspaceSummaryTypeDef, _OptionalKeyspaceSummaryTypeDef):
     pass
 
-ListKeyspacesRequestListKeyspacesPaginateTypeDef = TypedDict(
-    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
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
 
 ListKeyspacesRequestRequestTypeDef = TypedDict(
     "ListKeyspacesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "keyspaceName": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
-):
-    pass
-
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -434,34 +335,14 @@
     {
         "keyspaceName": str,
         "tableName": str,
         "resourceArn": str,
     },
 )
 
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
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -475,87 +356,28 @@
 
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
-PartitionKeyOutputTypeDef = TypedDict(
-    "PartitionKeyOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
 PartitionKeyTypeDef = TypedDict(
     "PartitionKeyTypeDef",
     {
         "name": str,
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
-RestoreTableResponseTypeDef = TypedDict(
-    "RestoreTableResponseTypeDef",
-    {
-        "restoredTableARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StaticColumnOutputTypeDef = TypedDict(
-    "StaticColumnOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-
 StaticColumnTypeDef = TypedDict(
     "StaticColumnTypeDef",
     {
         "name": str,
     },
 )
 
-UpdateTableResponseTypeDef = TypedDict(
-    "UpdateTableResponseTypeDef",
-    {
-        "resourceArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateKeyspaceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateKeyspaceRequestRequestTypeDef",
     {
         "keyspaceName": str,
     },
 )
 _OptionalCreateKeyspaceRequestRequestTypeDef = TypedDict(
@@ -584,14 +406,66 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+CreateKeyspaceResponseTypeDef = TypedDict(
+    "CreateKeyspaceResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTableResponseTypeDef = TypedDict(
+    "CreateTableResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetKeyspaceResponseTypeDef = TypedDict(
+    "GetKeyspaceResponseTypeDef",
+    {
+        "keyspaceName": str,
+        "resourceArn": str,
+        "replicationStrategy": rsType,
+        "replicationRegions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RestoreTableResponseTypeDef = TypedDict(
+    "RestoreTableResponseTypeDef",
+    {
+        "restoredTableARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateTableResponseTypeDef = TypedDict(
+    "UpdateTableResponseTypeDef",
+    {
+        "resourceArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredRestoreTableRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreTableRequestRequestTypeDef",
     {
         "sourceKeyspaceName": str,
         "sourceTableName": str,
         "targetKeyspaceName": str,
         "targetTableName": str,
@@ -641,48 +515,87 @@
     pass
 
 ListKeyspacesResponseTypeDef = TypedDict(
     "ListKeyspacesResponseTypeDef",
     {
         "nextToken": str,
         "keyspaces": List[KeyspaceSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTablesResponseTypeDef = TypedDict(
-    "ListTablesResponseTypeDef",
+ListKeyspacesRequestListKeyspacesPaginateTypeDef = TypedDict(
+    "ListKeyspacesRequestListKeyspacesPaginateTypeDef",
     {
-        "nextToken": str,
-        "tables": List[TableSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "keyspaceName": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTablesRequestListTablesPaginateTypeDef(
+    _RequiredListTablesRequestListTablesPaginateTypeDef,
+    _OptionalListTablesRequestListTablesPaginateTypeDef,
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
+
+ListTablesResponseTypeDef = TypedDict(
+    "ListTablesResponseTypeDef",
     {
         "nextToken": str,
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tables": List[TableSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSchemaDefinitionOutputTypeDef = TypedDict(
     "_RequiredSchemaDefinitionOutputTypeDef",
     {
-        "allColumns": List[ColumnDefinitionOutputTypeDef],
-        "partitionKeys": List[PartitionKeyOutputTypeDef],
+        "allColumns": List[ColumnDefinitionTypeDef],
+        "partitionKeys": List[PartitionKeyTypeDef],
     },
 )
 _OptionalSchemaDefinitionOutputTypeDef = TypedDict(
     "_OptionalSchemaDefinitionOutputTypeDef",
     {
-        "clusteringKeys": List[ClusteringKeyOutputTypeDef],
-        "staticColumns": List[StaticColumnOutputTypeDef],
+        "clusteringKeys": List[ClusteringKeyTypeDef],
+        "staticColumns": List[StaticColumnTypeDef],
     },
     total=False,
 )
 
 class SchemaDefinitionOutputTypeDef(
     _RequiredSchemaDefinitionOutputTypeDef, _OptionalSchemaDefinitionOutputTypeDef
 ):
@@ -713,21 +626,21 @@
         "keyspaceName": str,
         "tableName": str,
         "resourceArn": str,
         "creationTimestamp": datetime,
         "status": TableStatusType,
         "schemaDefinition": SchemaDefinitionOutputTypeDef,
         "capacitySpecification": CapacitySpecificationSummaryTypeDef,
-        "encryptionSpecification": EncryptionSpecificationOutputTypeDef,
+        "encryptionSpecification": EncryptionSpecificationTypeDef,
         "pointInTimeRecovery": PointInTimeRecoverySummaryTypeDef,
-        "ttl": TimeToLiveOutputTypeDef,
+        "ttl": TimeToLiveTypeDef,
         "defaultTimeToLive": int,
-        "comment": CommentOutputTypeDef,
-        "clientSideTimestamps": ClientSideTimestampsOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "comment": CommentTypeDef,
+        "clientSideTimestamps": ClientSideTimestampsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "keyspaceName": str,
```

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/PKG-INFO` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-keyspaces
-Version: 1.28.12
-Summary: Type annotations for boto3.Keyspaces 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Keyspaces 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-keyspaces.svg?color=blue)](https://pypi.org/project/mypy-boto3-keyspaces)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-keyspaces)](https://pepy.tech/project/mypy-boto3-keyspaces)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Keyspaces 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
+[boto3.Keyspaces 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/keyspaces.html#Keyspaces)
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
 [mypy-boto3-keyspaces docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_keyspaces/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,62 +338,53 @@
 `mypy_boto3_keyspaces.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_keyspaces.type_defs import (
     CapacitySpecificationSummaryTypeDef,
     CapacitySpecificationTypeDef,
-    ClientSideTimestampsOutputTypeDef,
     ClientSideTimestampsTypeDef,
-    ClusteringKeyOutputTypeDef,
     ClusteringKeyTypeDef,
-    ColumnDefinitionOutputTypeDef,
     ColumnDefinitionTypeDef,
-    CommentOutputTypeDef,
     CommentTypeDef,
     ReplicationSpecificationTypeDef,
     TagTypeDef,
-    CreateKeyspaceResponseTypeDef,
+    ResponseMetadataTypeDef,
     EncryptionSpecificationTypeDef,
     PointInTimeRecoveryTypeDef,
     TimeToLiveTypeDef,
-    CreateTableResponseTypeDef,
     DeleteKeyspaceRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
-    EncryptionSpecificationOutputTypeDef,
     GetKeyspaceRequestRequestTypeDef,
-    GetKeyspaceResponseTypeDef,
     GetTableRequestRequestTypeDef,
     PointInTimeRecoverySummaryTypeDef,
-    TimeToLiveOutputTypeDef,
     KeyspaceSummaryTypeDef,
-    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListKeyspacesRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    PartitionKeyOutputTypeDef,
     PartitionKeyTypeDef,
-    ResponseMetadataTypeDef,
-    RestoreTableResponseTypeDef,
-    StaticColumnOutputTypeDef,
     StaticColumnTypeDef,
-    UpdateTableResponseTypeDef,
     CreateKeyspaceRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateKeyspaceResponseTypeDef,
+    CreateTableResponseTypeDef,
+    GetKeyspaceResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    RestoreTableResponseTypeDef,
+    UpdateTableResponseTypeDef,
     RestoreTableRequestRequestTypeDef,
     UpdateTableRequestRequestTypeDef,
     ListKeyspacesResponseTypeDef,
+    ListKeyspacesRequestListKeyspacesPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTablesResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     SchemaDefinitionOutputTypeDef,
     SchemaDefinitionTypeDef,
     GetTableResponseTypeDef,
     CreateTableRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-keyspaces-1.28.12/mypy_boto3_keyspaces.egg-info/SOURCES.txt` & `mypy-boto3-keyspaces-1.28.15/mypy_boto3_keyspaces.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-keyspaces-1.28.12/setup.py` & `mypy-boto3-keyspaces-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-keyspaces",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_keyspaces"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Keyspaces 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Keyspaces 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

