# Comparing `tmp/mypy-boto3-redshift-data-1.28.12.tar.gz` & `tmp/mypy-boto3-redshift-data-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-data-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-data-1.28.15.tar", last modified: Fri Jul 28 20:43:33 2023, max compression
```

## Comparing `mypy-boto3-redshift-data-1.28.12.tar` & `mypy-boto3-redshift-data-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.701189 mypy-boto3-redshift-data-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-07-27 11:49:27.697189 mypy-boto3-redshift-data-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.697189 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16860 2023-07-27 11:44:25.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16831 2023-07-27 11:44:25.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.697189 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15050 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 11:49:27.000000 mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.701189 mypy-boto3-redshift-data-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-27 11:44:23.000000 mypy-boto3-redshift-data-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.209720 mypy-boto3-redshift-data-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-07-28 20:43:33.205720 mypy-boto3-redshift-data-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.201720 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13809 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8657 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8325 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16684 2023-07-28 20:36:40.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16655 2023-07-28 20:36:40.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.205720 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-07-28 20:43:32.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:43:32.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:32.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:32.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:32.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:32.000000 mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:33.209720 mypy-boto3-redshift-data-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-28 20:36:39.000000 mypy-boto3-redshift-data-1.28.15/setup.py
```

### Comparing `mypy-boto3-redshift-data-1.28.12/LICENSE` & `mypy-boto3-redshift-data-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/PKG-INFO` & `mypy-boto3-redshift-data-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-data
-Version: 1.28.12
-Summary: Type annotations for boto3.RedshiftDataAPIService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RedshiftDataAPIService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-data)](https://pepy.tech/project/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,41 +345,40 @@
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
-    SqlParameterOutputTypeDef,
+    SqlParameterTypeDef,
     SubStatementDataTypeDef,
     PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    SqlParameterTypeDef,
     FieldTypeDef,
     GetStatementResultRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
     BatchExecuteStatementOutputTypeDef,
     CancelStatementResponseTypeDef,
     ExecuteStatementOutputTypeDef,
     ListDatabasesResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
+    ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
     DescribeTableRequestDescribeTablePaginateTypeDef,
     GetStatementResultRequestGetStatementResultPaginateTypeDef,
     ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListStatementsRequestListStatementsPaginateTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
-    ExecuteStatementInputRequestTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
```

### Comparing `mypy-boto3-redshift-data-1.28.12/README.md` & `mypy-boto3-redshift-data-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-data)](https://pepy.tech/project/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,41 +313,40 @@
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
-    SqlParameterOutputTypeDef,
+    SqlParameterTypeDef,
     SubStatementDataTypeDef,
     PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    SqlParameterTypeDef,
     FieldTypeDef,
     GetStatementResultRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
     BatchExecuteStatementOutputTypeDef,
     CancelStatementResponseTypeDef,
     ExecuteStatementOutputTypeDef,
     ListDatabasesResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
+    ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
     DescribeTableRequestDescribeTablePaginateTypeDef,
     GetStatementResultRequestGetStatementResultPaginateTypeDef,
     ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListStatementsRequestListStatementsPaginateTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
-    ExecuteStatementInputRequestTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
```

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__init__.py` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__init__.pyi` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/__main__.py` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.RedshiftDataAPIService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.RedshiftDataAPIService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService\nOther"
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

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/client.py` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/client.pyi` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/literals.py` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/literals.pyi` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/paginator.py` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/paginator.pyi` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/type_defs.py` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,41 +25,40 @@
 
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
-    "SqlParameterOutputTypeDef",
+    "SqlParameterTypeDef",
     "SubStatementDataTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeTableRequestRequestTypeDef",
-    "SqlParameterTypeDef",
     "FieldTypeDef",
     "GetStatementResultRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "ListStatementsRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableMemberTypeDef",
     "BatchExecuteStatementOutputTypeDef",
     "CancelStatementResponseTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ListDatabasesResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeTableResponseTypeDef",
+    "ExecuteStatementInputRequestTypeDef",
     "StatementDataTypeDef",
     "DescribeStatementResponseTypeDef",
     "DescribeTableRequestDescribeTablePaginateTypeDef",
     "GetStatementResultRequestGetStatementResultPaginateTypeDef",
     "ListDatabasesRequestListDatabasesPaginateTypeDef",
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListStatementsRequestListStatementsPaginateTypeDef",
     "ListTablesRequestListTablesPaginateTypeDef",
-    "ExecuteStatementInputRequestTypeDef",
     "GetStatementResultResponseTypeDef",
     "ListTablesResponseTypeDef",
     "ListStatementsResponseTypeDef",
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
@@ -131,16 +130,16 @@
 DescribeStatementRequestRequestTypeDef = TypedDict(
     "DescribeStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-SqlParameterOutputTypeDef = TypedDict(
-    "SqlParameterOutputTypeDef",
+SqlParameterTypeDef = TypedDict(
+    "SqlParameterTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
 
 _RequiredSubStatementDataTypeDef = TypedDict(
@@ -206,22 +205,14 @@
 
 class DescribeTableRequestRequestTypeDef(
     _RequiredDescribeTableRequestRequestTypeDef, _OptionalDescribeTableRequestRequestTypeDef
 ):
     pass
 
 
-SqlParameterTypeDef = TypedDict(
-    "SqlParameterTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-)
-
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "blobValue": bytes,
         "booleanValue": bool,
         "doubleValue": float,
         "isNull": bool,
@@ -418,26 +409,55 @@
         "ColumnList": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "TableName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteStatementInputRequestTypeDef",
+    {
+        "Database": str,
+        "Sql": str,
+    },
+)
+_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteStatementInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "ClusterIdentifier": str,
+        "DbUser": str,
+        "Parameters": Sequence[SqlParameterTypeDef],
+        "SecretArn": str,
+        "StatementName": str,
+        "WithEvent": bool,
+        "WorkgroupName": str,
+    },
+    total=False,
+)
+
+
+class ExecuteStatementInputRequestTypeDef(
+    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
+):
+    pass
+
+
 _RequiredStatementDataTypeDef = TypedDict(
     "_RequiredStatementDataTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStatementDataTypeDef = TypedDict(
     "_OptionalStatementDataTypeDef",
     {
         "CreatedAt": datetime,
         "IsBatchStatement": bool,
-        "QueryParameters": List[SqlParameterOutputTypeDef],
+        "QueryParameters": List[SqlParameterTypeDef],
         "QueryString": str,
         "QueryStrings": List[str],
         "SecretArn": str,
         "StatementName": str,
         "Status": StatusStringType,
         "UpdatedAt": datetime,
     },
@@ -456,15 +476,15 @@
         "CreatedAt": datetime,
         "Database": str,
         "DbUser": str,
         "Duration": int,
         "Error": str,
         "HasResultSet": bool,
         "Id": str,
-        "QueryParameters": List[SqlParameterOutputTypeDef],
+        "QueryParameters": List[SqlParameterTypeDef],
         "QueryString": str,
         "RedshiftPid": int,
         "RedshiftQueryId": int,
         "ResultRows": int,
         "ResultSize": int,
         "SecretArn": str,
         "Status": StatusStringType,
@@ -616,43 +636,14 @@
 class ListTablesRequestListTablesPaginateTypeDef(
     _RequiredListTablesRequestListTablesPaginateTypeDef,
     _OptionalListTablesRequestListTablesPaginateTypeDef,
 ):
     pass
 
 
-_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteStatementInputRequestTypeDef",
-    {
-        "Database": str,
-        "Sql": str,
-    },
-)
-_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteStatementInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "ClusterIdentifier": str,
-        "DbUser": str,
-        "Parameters": Sequence[SqlParameterTypeDef],
-        "SecretArn": str,
-        "StatementName": str,
-        "WithEvent": bool,
-        "WorkgroupName": str,
-    },
-    total=False,
-)
-
-
-class ExecuteStatementInputRequestTypeDef(
-    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
-):
-    pass
-
-
 GetStatementResultResponseTypeDef = TypedDict(
     "GetStatementResultResponseTypeDef",
     {
         "ColumnMetadata": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "Records": List[List[FieldTypeDef]],
         "TotalNumRows": int,
```

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data/type_defs.pyi` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -24,41 +24,40 @@
 
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CancelStatementRequestRequestTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
-    "SqlParameterOutputTypeDef",
+    "SqlParameterTypeDef",
     "SubStatementDataTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeTableRequestRequestTypeDef",
-    "SqlParameterTypeDef",
     "FieldTypeDef",
     "GetStatementResultRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "ListStatementsRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableMemberTypeDef",
     "BatchExecuteStatementOutputTypeDef",
     "CancelStatementResponseTypeDef",
     "ExecuteStatementOutputTypeDef",
     "ListDatabasesResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "DescribeTableResponseTypeDef",
+    "ExecuteStatementInputRequestTypeDef",
     "StatementDataTypeDef",
     "DescribeStatementResponseTypeDef",
     "DescribeTableRequestDescribeTablePaginateTypeDef",
     "GetStatementResultRequestGetStatementResultPaginateTypeDef",
     "ListDatabasesRequestListDatabasesPaginateTypeDef",
     "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListStatementsRequestListStatementsPaginateTypeDef",
     "ListTablesRequestListTablesPaginateTypeDef",
-    "ExecuteStatementInputRequestTypeDef",
     "GetStatementResultResponseTypeDef",
     "ListTablesResponseTypeDef",
     "ListStatementsResponseTypeDef",
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
@@ -128,16 +127,16 @@
 DescribeStatementRequestRequestTypeDef = TypedDict(
     "DescribeStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-SqlParameterOutputTypeDef = TypedDict(
-    "SqlParameterOutputTypeDef",
+SqlParameterTypeDef = TypedDict(
+    "SqlParameterTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
 
 _RequiredSubStatementDataTypeDef = TypedDict(
@@ -199,22 +198,14 @@
 )
 
 class DescribeTableRequestRequestTypeDef(
     _RequiredDescribeTableRequestRequestTypeDef, _OptionalDescribeTableRequestRequestTypeDef
 ):
     pass
 
-SqlParameterTypeDef = TypedDict(
-    "SqlParameterTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-)
-
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "blobValue": bytes,
         "booleanValue": bool,
         "doubleValue": float,
         "isNull": bool,
@@ -403,26 +394,53 @@
         "ColumnList": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "TableName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
+    "_RequiredExecuteStatementInputRequestTypeDef",
+    {
+        "Database": str,
+        "Sql": str,
+    },
+)
+_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
+    "_OptionalExecuteStatementInputRequestTypeDef",
+    {
+        "ClientToken": str,
+        "ClusterIdentifier": str,
+        "DbUser": str,
+        "Parameters": Sequence[SqlParameterTypeDef],
+        "SecretArn": str,
+        "StatementName": str,
+        "WithEvent": bool,
+        "WorkgroupName": str,
+    },
+    total=False,
+)
+
+class ExecuteStatementInputRequestTypeDef(
+    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
+):
+    pass
+
 _RequiredStatementDataTypeDef = TypedDict(
     "_RequiredStatementDataTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalStatementDataTypeDef = TypedDict(
     "_OptionalStatementDataTypeDef",
     {
         "CreatedAt": datetime,
         "IsBatchStatement": bool,
-        "QueryParameters": List[SqlParameterOutputTypeDef],
+        "QueryParameters": List[SqlParameterTypeDef],
         "QueryString": str,
         "QueryStrings": List[str],
         "SecretArn": str,
         "StatementName": str,
         "Status": StatusStringType,
         "UpdatedAt": datetime,
     },
@@ -439,15 +457,15 @@
         "CreatedAt": datetime,
         "Database": str,
         "DbUser": str,
         "Duration": int,
         "Error": str,
         "HasResultSet": bool,
         "Id": str,
-        "QueryParameters": List[SqlParameterOutputTypeDef],
+        "QueryParameters": List[SqlParameterTypeDef],
         "QueryString": str,
         "RedshiftPid": int,
         "RedshiftQueryId": int,
         "ResultRows": int,
         "ResultSize": int,
         "SecretArn": str,
         "Status": StatusStringType,
@@ -589,41 +607,14 @@
 
 class ListTablesRequestListTablesPaginateTypeDef(
     _RequiredListTablesRequestListTablesPaginateTypeDef,
     _OptionalListTablesRequestListTablesPaginateTypeDef,
 ):
     pass
 
-_RequiredExecuteStatementInputRequestTypeDef = TypedDict(
-    "_RequiredExecuteStatementInputRequestTypeDef",
-    {
-        "Database": str,
-        "Sql": str,
-    },
-)
-_OptionalExecuteStatementInputRequestTypeDef = TypedDict(
-    "_OptionalExecuteStatementInputRequestTypeDef",
-    {
-        "ClientToken": str,
-        "ClusterIdentifier": str,
-        "DbUser": str,
-        "Parameters": Sequence[SqlParameterTypeDef],
-        "SecretArn": str,
-        "StatementName": str,
-        "WithEvent": bool,
-        "WorkgroupName": str,
-    },
-    total=False,
-)
-
-class ExecuteStatementInputRequestTypeDef(
-    _RequiredExecuteStatementInputRequestTypeDef, _OptionalExecuteStatementInputRequestTypeDef
-):
-    pass
-
 GetStatementResultResponseTypeDef = TypedDict(
     "GetStatementResultResponseTypeDef",
     {
         "ColumnMetadata": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "Records": List[List[FieldTypeDef]],
         "TotalNumRows": int,
```

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/PKG-INFO` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift-data
-Version: 1.28.12
-Summary: Type annotations for boto3.RedshiftDataAPIService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.RedshiftDataAPIService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift-data)](https://pepy.tech/project/mypy-boto3-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.RedshiftDataAPIService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
+[boto3.RedshiftDataAPIService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [mypy-boto3-redshift-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,41 +345,40 @@
 ```python
 from mypy_boto3_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
     ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
-    SqlParameterOutputTypeDef,
+    SqlParameterTypeDef,
     SubStatementDataTypeDef,
     PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    SqlParameterTypeDef,
     FieldTypeDef,
     GetStatementResultRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListSchemasRequestRequestTypeDef,
     ListStatementsRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
     BatchExecuteStatementOutputTypeDef,
     CancelStatementResponseTypeDef,
     ExecuteStatementOutputTypeDef,
     ListDatabasesResponseTypeDef,
     ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
+    ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
     DescribeTableRequestDescribeTablePaginateTypeDef,
     GetStatementResultRequestGetStatementResultPaginateTypeDef,
     ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListSchemasRequestListSchemasPaginateTypeDef,
     ListStatementsRequestListStatementsPaginateTypeDef,
     ListTablesRequestListTablesPaginateTypeDef,
-    ExecuteStatementInputRequestTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
 def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
```

### Comparing `mypy-boto3-redshift-data-1.28.12/mypy_boto3_redshift_data.egg-info/SOURCES.txt` & `mypy-boto3-redshift-data-1.28.15/mypy_boto3_redshift_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-data-1.28.12/setup.py` & `mypy-boto3-redshift-data-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift-data",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_redshift_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.RedshiftDataAPIService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.RedshiftDataAPIService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

