# Comparing `tmp/mypy-boto3-honeycode-1.28.12.tar.gz` & `tmp/mypy-boto3-honeycode-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-honeycode-1.28.12.tar", last modified: Thu Jul 27 05:34:46 2023, max compression
+gzip compressed data, was "mypy-boto3-honeycode-1.28.15.tar", last modified: Fri Jul 28 20:42:55 2023, max compression
```

## Comparing `mypy-boto3-honeycode-1.28.12.tar` & `mypy-boto3-honeycode-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-27 05:23:19.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22615 2023-07-27 05:23:19.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22578 2023-07-27 05:23:19.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:46.000000 mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:46.304494 mypy-boto3-honeycode-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:23:18.000000 mypy-boto3-honeycode-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:55.473202 mypy-boto3-honeycode-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-28 20:42:55.469202 mypy-boto3-honeycode-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13820 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:55.457202 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15516 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9243 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9241 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21303 2023-07-28 20:27:22.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21268 2023-07-28 20:27:22.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:55.469202 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:55.000000 mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:55.473202 mypy-boto3-honeycode-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:27:21.000000 mypy-boto3-honeycode-1.28.15/setup.py
```

### Comparing `mypy-boto3-honeycode-1.28.12/LICENSE` & `mypy-boto3-honeycode-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.12/PKG-INFO` & `mypy-boto3-honeycode-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.28.12
-Summary: Type annotations for boto3.Honeycode 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,63 +336,59 @@
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
-    DelimitedTextImportOptionsOutputTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
-    SourceDataColumnPropertiesOutputTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
-    ImportDataSourceConfigOutputTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
     DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
-    ImportDataSourceOutputTypeDef,
     ImportDataSourceTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
```

### Comparing `mypy-boto3-honeycode-1.28.12/README.md` & `mypy-boto3-honeycode-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,63 +304,59 @@
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
-    DelimitedTextImportOptionsOutputTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
-    SourceDataColumnPropertiesOutputTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
-    ImportDataSourceConfigOutputTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
     DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
-    ImportDataSourceOutputTypeDef,
     ImportDataSourceTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
```

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__init__.py` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__init__.pyi` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/__main__.py` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Honeycode 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Honeycode 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
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

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/client.py` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/client.pyi` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/literals.py` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/literals.pyi` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/paginator.py` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 class ListTableColumnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablecolumnspaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, tableId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workbookId: str, tableId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTableColumnsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablecolumnspaginator)
         """
 
 
@@ -79,30 +79,30 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablerowspaginator)
         """
 
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workbookId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTablesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablespaginator)
         """
 
 
@@ -114,13 +114,13 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#querytablerowspaginator)
         """
```

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/paginator.pyi` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 class ListTableColumnsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablecolumnspaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, tableId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workbookId: str, tableId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTableColumnsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablecolumnspaginator)
         """
 
 class ListTableRowsPaginator(Paginator):
@@ -75,29 +75,29 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablerowspaginator)
         """
 
 class ListTablesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workbookId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTablesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#listtablespaginator)
         """
 
 class QueryTableRowsPaginator(Paginator):
@@ -108,13 +108,13 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[QueryTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/paginators/#querytablerowspaginator)
         """
```

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/type_defs.py` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,63 +31,59 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FailedBatchItemTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
     "ColumnMetadataTypeDef",
     "DataItemTypeDef",
-    "DelimitedTextImportOptionsOutputTypeDef",
     "DelimitedTextImportOptionsTypeDef",
     "DescribeTableDataImportJobRequestRequestTypeDef",
-    "SourceDataColumnPropertiesOutputTypeDef",
     "SourceDataColumnPropertiesTypeDef",
     "FilterTypeDef",
     "VariableValueTypeDef",
-    "ImportDataSourceConfigOutputTypeDef",
     "ImportDataSourceConfigTypeDef",
     "ImportJobSubmitterTypeDef",
-    "InvokeScreenAutomationResultTypeDef",
-    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListTableColumnsRequestRequestTypeDef",
     "TableColumnTypeDef",
-    "ListTableRowsRequestListTableRowsPaginateTypeDef",
     "ListTableRowsRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartTableDataImportJobResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchCreateTableRowsResultTypeDef",
     "BatchDeleteTableRowsResultTypeDef",
     "BatchUpdateTableRowsResultTypeDef",
+    "InvokeScreenAutomationResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "StartTableDataImportJobResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
     "DestinationOptionsOutputTypeDef",
     "DestinationOptionsTypeDef",
-    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
-    "ImportDataSourceOutputTypeDef",
     "ImportDataSourceTypeDef",
+    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    "ListTableRowsRequestListTableRowsPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
+    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
@@ -104,14 +100,25 @@
     "FailedBatchItemTypeDef",
     {
         "id": str,
         "errorMessage": str,
     },
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
 _RequiredBatchDeleteTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "rowIds": Sequence[str],
     },
@@ -175,38 +182,14 @@
         "overrideFormat": FormatType,
         "rawValue": str,
         "formattedValue": str,
     },
     total=False,
 )
 
-_RequiredDelimitedTextImportOptionsOutputTypeDef = TypedDict(
-    "_RequiredDelimitedTextImportOptionsOutputTypeDef",
-    {
-        "delimiter": str,
-    },
-)
-_OptionalDelimitedTextImportOptionsOutputTypeDef = TypedDict(
-    "_OptionalDelimitedTextImportOptionsOutputTypeDef",
-    {
-        "hasHeaderRow": bool,
-        "ignoreEmptyRows": bool,
-        "dataCharacterEncoding": ImportDataCharacterEncodingType,
-    },
-    total=False,
-)
-
-
-class DelimitedTextImportOptionsOutputTypeDef(
-    _RequiredDelimitedTextImportOptionsOutputTypeDef,
-    _OptionalDelimitedTextImportOptionsOutputTypeDef,
-):
-    pass
-
-
 _RequiredDelimitedTextImportOptionsTypeDef = TypedDict(
     "_RequiredDelimitedTextImportOptionsTypeDef",
     {
         "delimiter": str,
     },
 )
 _OptionalDelimitedTextImportOptionsTypeDef = TypedDict(
@@ -231,22 +214,14 @@
     {
         "workbookId": str,
         "tableId": str,
         "jobId": str,
     },
 )
 
-SourceDataColumnPropertiesOutputTypeDef = TypedDict(
-    "SourceDataColumnPropertiesOutputTypeDef",
-    {
-        "columnIndex": int,
-    },
-    total=False,
-)
-
 SourceDataColumnPropertiesTypeDef = TypedDict(
     "SourceDataColumnPropertiesTypeDef",
     {
         "columnIndex": int,
     },
     total=False,
 )
@@ -273,22 +248,14 @@
 VariableValueTypeDef = TypedDict(
     "VariableValueTypeDef",
     {
         "rawValue": str,
     },
 )
 
-ImportDataSourceConfigOutputTypeDef = TypedDict(
-    "ImportDataSourceConfigOutputTypeDef",
-    {
-        "dataSourceUrl": str,
-    },
-    total=False,
-)
-
 ImportDataSourceConfigTypeDef = TypedDict(
     "ImportDataSourceConfigTypeDef",
     {
         "dataSourceUrl": str,
     },
     total=False,
 )
@@ -298,45 +265,24 @@
     {
         "email": str,
         "userArn": str,
     },
     total=False,
 )
 
-InvokeScreenAutomationResultTypeDef = TypedDict(
-    "InvokeScreenAutomationResultTypeDef",
-    {
-        "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
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
-class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
-    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTableColumnsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableColumnsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -361,38 +307,14 @@
         "tableColumnId": str,
         "tableColumnName": str,
         "format": FormatType,
     },
     total=False,
 )
 
-_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "rowIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTableRowsRequestListTableRowsPaginateTypeDef(
-    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
-    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -409,36 +331,14 @@
 
 class ListTableRowsRequestRequestTypeDef(
     _RequiredListTableRowsRequestRequestTypeDef, _OptionalListTableRowsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "workbookId": str,
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
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -469,52 +369,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
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
-StartTableDataImportJobResultTypeDef = TypedDict(
-    "StartTableDataImportJobResultTypeDef",
-    {
-        "jobId": str,
-        "jobStatus": TableDataImportJobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -529,43 +391,68 @@
 
 BatchCreateTableRowsResultTypeDef = TypedDict(
     "BatchCreateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "createdRows": Dict[str, str],
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteTableRowsResultTypeDef = TypedDict(
     "BatchDeleteTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateTableRowsResultTypeDef = TypedDict(
     "BatchUpdateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeScreenAutomationResultTypeDef = TypedDict(
+    "InvokeScreenAutomationResultTypeDef",
+    {
+        "workbookCursor": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTableDataImportJobResultTypeDef = TypedDict(
+    "StartTableDataImportJobResultTypeDef",
+    {
+        "jobId": str,
+        "jobStatus": TableDataImportJobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpsertTableRowsResultTypeDef = TypedDict(
     "BatchUpsertTableRowsResultTypeDef",
     {
         "rows": Dict[str, UpsertRowsResultTypeDef],
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRowDataTypeDef = TypedDict(
     "CreateRowDataTypeDef",
     {
         "batchItemId": str,
@@ -607,51 +494,27 @@
 class ResultRowTypeDef(_RequiredResultRowTypeDef, _OptionalResultRowTypeDef):
     pass
 
 
 DestinationOptionsOutputTypeDef = TypedDict(
     "DestinationOptionsOutputTypeDef",
     {
-        "columnMap": Dict[str, SourceDataColumnPropertiesOutputTypeDef],
+        "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
 DestinationOptionsTypeDef = TypedDict(
     "DestinationOptionsTypeDef",
     {
         "columnMap": Mapping[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
-_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-        "filterFormula": FilterTypeDef,
-    },
-)
-_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
-    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredQueryTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "filterFormula": FilterTypeDef,
     },
@@ -729,45 +592,131 @@
 class InvokeScreenAutomationRequestRequestTypeDef(
     _RequiredInvokeScreenAutomationRequestRequestTypeDef,
     _OptionalInvokeScreenAutomationRequestRequestTypeDef,
 ):
     pass
 
 
-ImportDataSourceOutputTypeDef = TypedDict(
-    "ImportDataSourceOutputTypeDef",
+ImportDataSourceTypeDef = TypedDict(
+    "ImportDataSourceTypeDef",
     {
-        "dataSourceConfig": ImportDataSourceConfigOutputTypeDef,
+        "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
-ImportDataSourceTypeDef = TypedDict(
-    "ImportDataSourceTypeDef",
+_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
     {
-        "dataSourceConfig": ImportDataSourceConfigTypeDef,
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
+    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "rowIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTableRowsRequestListTableRowsPaginateTypeDef(
+    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
+    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "workbookId": str,
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
+_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+        "filterFormula": FilterTypeDef,
+    },
+)
+_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
+    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+):
+    pass
+
+
 ListTableColumnsResultTypeDef = TypedDict(
     "ListTableColumnsResultTypeDef",
     {
         "tableColumns": List[TableColumnTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResultTypeDef = TypedDict(
     "ListTablesResultTypeDef",
     {
         "tables": List[TableTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchCreateTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -819,26 +768,26 @@
     "ListTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "rowIdsNotFound": List[str],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryTableRowsResultTypeDef = TypedDict(
     "QueryTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
@@ -846,15 +795,15 @@
     },
 )
 
 ImportOptionsOutputTypeDef = TypedDict(
     "ImportOptionsOutputTypeDef",
     {
         "destinationOptions": DestinationOptionsOutputTypeDef,
-        "delimitedTextOptions": DelimitedTextImportOptionsOutputTypeDef,
+        "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
     },
     total=False,
 )
 
 ImportOptionsTypeDef = TypedDict(
     "ImportOptionsTypeDef",
     {
@@ -890,25 +839,25 @@
 
 GetScreenDataResultTypeDef = TypedDict(
     "GetScreenDataResultTypeDef",
     {
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableDataImportJobMetadataTypeDef = TypedDict(
     "TableDataImportJobMetadataTypeDef",
     {
         "submitter": ImportJobSubmitterTypeDef,
         "submitTime": datetime,
         "importOptions": ImportOptionsOutputTypeDef,
-        "dataSource": ImportDataSourceOutputTypeDef,
+        "dataSource": ImportDataSourceTypeDef,
     },
 )
 
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -923,10 +872,10 @@
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode/type_defs.pyi` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -30,63 +30,59 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FailedBatchItemTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
     "ColumnMetadataTypeDef",
     "DataItemTypeDef",
-    "DelimitedTextImportOptionsOutputTypeDef",
     "DelimitedTextImportOptionsTypeDef",
     "DescribeTableDataImportJobRequestRequestTypeDef",
-    "SourceDataColumnPropertiesOutputTypeDef",
     "SourceDataColumnPropertiesTypeDef",
     "FilterTypeDef",
     "VariableValueTypeDef",
-    "ImportDataSourceConfigOutputTypeDef",
     "ImportDataSourceConfigTypeDef",
     "ImportJobSubmitterTypeDef",
-    "InvokeScreenAutomationResultTypeDef",
-    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListTableColumnsRequestRequestTypeDef",
     "TableColumnTypeDef",
-    "ListTableRowsRequestListTableRowsPaginateTypeDef",
     "ListTableRowsRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartTableDataImportJobResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchCreateTableRowsResultTypeDef",
     "BatchDeleteTableRowsResultTypeDef",
     "BatchUpdateTableRowsResultTypeDef",
+    "InvokeScreenAutomationResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "StartTableDataImportJobResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
     "DestinationOptionsOutputTypeDef",
     "DestinationOptionsTypeDef",
-    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
-    "ImportDataSourceOutputTypeDef",
     "ImportDataSourceTypeDef",
+    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    "ListTableRowsRequestListTableRowsPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
+    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
@@ -103,14 +99,25 @@
     "FailedBatchItemTypeDef",
     {
         "id": str,
         "errorMessage": str,
     },
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
 _RequiredBatchDeleteTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "rowIds": Sequence[str],
     },
@@ -172,36 +179,14 @@
         "overrideFormat": FormatType,
         "rawValue": str,
         "formattedValue": str,
     },
     total=False,
 )
 
-_RequiredDelimitedTextImportOptionsOutputTypeDef = TypedDict(
-    "_RequiredDelimitedTextImportOptionsOutputTypeDef",
-    {
-        "delimiter": str,
-    },
-)
-_OptionalDelimitedTextImportOptionsOutputTypeDef = TypedDict(
-    "_OptionalDelimitedTextImportOptionsOutputTypeDef",
-    {
-        "hasHeaderRow": bool,
-        "ignoreEmptyRows": bool,
-        "dataCharacterEncoding": ImportDataCharacterEncodingType,
-    },
-    total=False,
-)
-
-class DelimitedTextImportOptionsOutputTypeDef(
-    _RequiredDelimitedTextImportOptionsOutputTypeDef,
-    _OptionalDelimitedTextImportOptionsOutputTypeDef,
-):
-    pass
-
 _RequiredDelimitedTextImportOptionsTypeDef = TypedDict(
     "_RequiredDelimitedTextImportOptionsTypeDef",
     {
         "delimiter": str,
     },
 )
 _OptionalDelimitedTextImportOptionsTypeDef = TypedDict(
@@ -224,22 +209,14 @@
     {
         "workbookId": str,
         "tableId": str,
         "jobId": str,
     },
 )
 
-SourceDataColumnPropertiesOutputTypeDef = TypedDict(
-    "SourceDataColumnPropertiesOutputTypeDef",
-    {
-        "columnIndex": int,
-    },
-    total=False,
-)
-
 SourceDataColumnPropertiesTypeDef = TypedDict(
     "SourceDataColumnPropertiesTypeDef",
     {
         "columnIndex": int,
     },
     total=False,
 )
@@ -264,22 +241,14 @@
 VariableValueTypeDef = TypedDict(
     "VariableValueTypeDef",
     {
         "rawValue": str,
     },
 )
 
-ImportDataSourceConfigOutputTypeDef = TypedDict(
-    "ImportDataSourceConfigOutputTypeDef",
-    {
-        "dataSourceUrl": str,
-    },
-    total=False,
-)
-
 ImportDataSourceConfigTypeDef = TypedDict(
     "ImportDataSourceConfigTypeDef",
     {
         "dataSourceUrl": str,
     },
     total=False,
 )
@@ -289,43 +258,24 @@
     {
         "email": str,
         "userArn": str,
     },
     total=False,
 )
 
-InvokeScreenAutomationResultTypeDef = TypedDict(
-    "InvokeScreenAutomationResultTypeDef",
-    {
-        "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
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
 
-class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
-    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTableColumnsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableColumnsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -348,36 +298,14 @@
         "tableColumnId": str,
         "tableColumnName": str,
         "format": FormatType,
     },
     total=False,
 )
 
-_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "rowIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTableRowsRequestListTableRowsPaginateTypeDef(
-    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
-    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -392,34 +320,14 @@
 )
 
 class ListTableRowsRequestRequestTypeDef(
     _RequiredListTableRowsRequestRequestTypeDef, _OptionalListTableRowsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "workbookId": str,
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
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -448,52 +356,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
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
-StartTableDataImportJobResultTypeDef = TypedDict(
-    "StartTableDataImportJobResultTypeDef",
-    {
-        "jobId": str,
-        "jobStatus": TableDataImportJobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -508,43 +378,68 @@
 
 BatchCreateTableRowsResultTypeDef = TypedDict(
     "BatchCreateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "createdRows": Dict[str, str],
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteTableRowsResultTypeDef = TypedDict(
     "BatchDeleteTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateTableRowsResultTypeDef = TypedDict(
     "BatchUpdateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeScreenAutomationResultTypeDef = TypedDict(
+    "InvokeScreenAutomationResultTypeDef",
+    {
+        "workbookCursor": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTableDataImportJobResultTypeDef = TypedDict(
+    "StartTableDataImportJobResultTypeDef",
+    {
+        "jobId": str,
+        "jobStatus": TableDataImportJobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpsertTableRowsResultTypeDef = TypedDict(
     "BatchUpsertTableRowsResultTypeDef",
     {
         "rows": Dict[str, UpsertRowsResultTypeDef],
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRowDataTypeDef = TypedDict(
     "CreateRowDataTypeDef",
     {
         "batchItemId": str,
@@ -584,49 +479,27 @@
 
 class ResultRowTypeDef(_RequiredResultRowTypeDef, _OptionalResultRowTypeDef):
     pass
 
 DestinationOptionsOutputTypeDef = TypedDict(
     "DestinationOptionsOutputTypeDef",
     {
-        "columnMap": Dict[str, SourceDataColumnPropertiesOutputTypeDef],
+        "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
 DestinationOptionsTypeDef = TypedDict(
     "DestinationOptionsTypeDef",
     {
         "columnMap": Mapping[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
-_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-        "filterFormula": FilterTypeDef,
-    },
-)
-_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
-    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-):
-    pass
-
 _RequiredQueryTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "filterFormula": FilterTypeDef,
     },
@@ -698,45 +571,123 @@
 
 class InvokeScreenAutomationRequestRequestTypeDef(
     _RequiredInvokeScreenAutomationRequestRequestTypeDef,
     _OptionalInvokeScreenAutomationRequestRequestTypeDef,
 ):
     pass
 
-ImportDataSourceOutputTypeDef = TypedDict(
-    "ImportDataSourceOutputTypeDef",
+ImportDataSourceTypeDef = TypedDict(
+    "ImportDataSourceTypeDef",
     {
-        "dataSourceConfig": ImportDataSourceConfigOutputTypeDef,
+        "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
-ImportDataSourceTypeDef = TypedDict(
-    "ImportDataSourceTypeDef",
+_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
     {
-        "dataSourceConfig": ImportDataSourceConfigTypeDef,
+        "workbookId": str,
+        "tableId": str,
     },
 )
+_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
+    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
+):
+    pass
+
+_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "rowIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTableRowsRequestListTableRowsPaginateTypeDef(
+    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
+    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
+):
+    pass
+
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "workbookId": str,
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
+_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+        "filterFormula": FilterTypeDef,
+    },
+)
+_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
+    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+):
+    pass
 
 ListTableColumnsResultTypeDef = TypedDict(
     "ListTableColumnsResultTypeDef",
     {
         "tableColumns": List[TableColumnTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResultTypeDef = TypedDict(
     "ListTablesResultTypeDef",
     {
         "tables": List[TableTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchCreateTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -784,26 +735,26 @@
     "ListTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "rowIdsNotFound": List[str],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryTableRowsResultTypeDef = TypedDict(
     "QueryTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
@@ -811,15 +762,15 @@
     },
 )
 
 ImportOptionsOutputTypeDef = TypedDict(
     "ImportOptionsOutputTypeDef",
     {
         "destinationOptions": DestinationOptionsOutputTypeDef,
-        "delimitedTextOptions": DelimitedTextImportOptionsOutputTypeDef,
+        "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
     },
     total=False,
 )
 
 ImportOptionsTypeDef = TypedDict(
     "ImportOptionsTypeDef",
     {
@@ -853,25 +804,25 @@
 
 GetScreenDataResultTypeDef = TypedDict(
     "GetScreenDataResultTypeDef",
     {
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TableDataImportJobMetadataTypeDef = TypedDict(
     "TableDataImportJobMetadataTypeDef",
     {
         "submitter": ImportJobSubmitterTypeDef,
         "submitTime": datetime,
         "importOptions": ImportOptionsOutputTypeDef,
-        "dataSource": ImportDataSourceOutputTypeDef,
+        "dataSource": ImportDataSourceTypeDef,
     },
 )
 
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -886,10 +837,10 @@
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/PKG-INFO` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-honeycode
-Version: 1.28.12
-Summary: Type annotations for boto3.Honeycode 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-honeycode.svg?color=blue)](https://pypi.org/project/mypy-boto3-honeycode)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-honeycode)](https://pepy.tech/project/mypy-boto3-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Honeycode 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
+[boto3.Honeycode 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [mypy-boto3-honeycode docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_honeycode/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,63 +336,59 @@
 
 `mypy_boto3_honeycode.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_honeycode.type_defs import (
     FailedBatchItemTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
-    DelimitedTextImportOptionsOutputTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
-    SourceDataColumnPropertiesOutputTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
-    ImportDataSourceConfigOutputTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
     DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
-    ImportDataSourceOutputTypeDef,
     ImportDataSourceTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
```

### Comparing `mypy-boto3-honeycode-1.28.12/mypy_boto3_honeycode.egg-info/SOURCES.txt` & `mypy-boto3-honeycode-1.28.15/mypy_boto3_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-honeycode-1.28.12/setup.py` & `mypy-boto3-honeycode-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-honeycode",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Honeycode 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Honeycode 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

