# Comparing `tmp/mypy-boto3-cur-1.28.12.tar.gz` & `tmp/mypy-boto3-cur-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cur-1.28.12.tar", last modified: Thu Jul 27 05:34:32 2023, max compression
+gzip compressed data, was "mypy-boto3-cur-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
```

## Comparing `mypy-boto3-cur-1.28.12.tar` & `mypy-boto3-cur-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.492540 mypy-boto3-cur-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-27 05:34:32.488540 mypy-boto3-cur-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.488540 mypy-boto3-cur-1.28.12/mypy_boto3_cur/
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:32.488540 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:32.000000 mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:32.492540 mypy-boto3-cur-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-27 05:19:51.000000 mypy-boto3-cur-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.884916 mypy-boto3-cur-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-28 20:42:34.884916 mypy-boto3-cur-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.880915 mypy-boto3-cur-1.28.15/mypy_boto3_cur/
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.884916 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13186 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:34.000000 mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.884916 mypy-boto3-cur-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 20:22:23.000000 mypy-boto3-cur-1.28.15/setup.py
```

### Comparing `mypy-boto3-cur-1.28.12/LICENSE` & `mypy-boto3-cur-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.12/PKG-INFO` & `mypy-boto3-cur-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.28.12
-Summary: Type annotations for boto3.CostandUsageReportService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,21 +328,21 @@
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResponseTypeDef,
-    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
     ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteReportDefinitionResponseTypeDef,
+    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
```

### Comparing `mypy-boto3-cur-1.28.12/README.md` & `mypy-boto3-cur-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,21 +296,21 @@
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResponseTypeDef,
-    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
     ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteReportDefinitionResponseTypeDef,
+    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
```

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/__init__.py` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/__init__.pyi` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/__main__.py` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CostandUsageReportService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CostandUsageReportService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService\nOther"
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

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/client.py` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/client.pyi` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/literals.py` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/literals.pyi` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/paginator.py` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class DescribeReportDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/paginators/#describereportdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeReportDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/paginators/#describereportdefinitionspaginator)
         """
```

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/paginator.pyi` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class DescribeReportDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/paginators/#describereportdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeReportDefinitionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService.Paginator.DescribeReportDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/paginators/#describereportdefinitionspaginator)
         """
```

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/type_defs.py` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,46 +28,51 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
-    "DeleteReportDefinitionResponseTypeDef",
-    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeReportDefinitionsRequestRequestTypeDef",
     "ReportDefinitionOutputTypeDef",
     "ReportDefinitionTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteReportDefinitionResponseTypeDef",
+    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
     },
     total=False,
 )
 
-DeleteReportDefinitionResponseTypeDef = TypedDict(
-    "DeleteReportDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
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
 
 DescribeReportDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeReportDefinitionsRequestRequestTypeDef",
     {
@@ -133,41 +138,36 @@
 )
 
 
 class ReportDefinitionTypeDef(_RequiredReportDefinitionTypeDef, _OptionalReportDefinitionTypeDef):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteReportDefinitionResponseTypeDef = TypedDict(
+    "DeleteReportDefinitionResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResponseMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 DescribeReportDefinitionsResponseTypeDef = TypedDict(
     "DescribeReportDefinitionsResponseTypeDef",
     {
         "ReportDefinitions": List[ReportDefinitionOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReportDefinitionRequestRequestTypeDef = TypedDict(
     "ModifyReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
```

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur/type_defs.pyi` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -27,46 +27,51 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
-    "DeleteReportDefinitionResponseTypeDef",
-    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeReportDefinitionsRequestRequestTypeDef",
     "ReportDefinitionOutputTypeDef",
     "ReportDefinitionTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "DeleteReportDefinitionResponseTypeDef",
+    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     "DescribeReportDefinitionsResponseTypeDef",
     "ModifyReportDefinitionRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
     },
     total=False,
 )
 
-DeleteReportDefinitionResponseTypeDef = TypedDict(
-    "DeleteReportDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = TypedDict(
-    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
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
 
 DescribeReportDefinitionsRequestRequestTypeDef = TypedDict(
     "DescribeReportDefinitionsRequestRequestTypeDef",
     {
@@ -128,41 +133,36 @@
     },
     total=False,
 )
 
 class ReportDefinitionTypeDef(_RequiredReportDefinitionTypeDef, _OptionalReportDefinitionTypeDef):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteReportDefinitionResponseTypeDef = TypedDict(
+    "DeleteReportDefinitionResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResponseMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef = TypedDict(
+    "DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 DescribeReportDefinitionsResponseTypeDef = TypedDict(
     "DescribeReportDefinitionsResponseTypeDef",
     {
         "ReportDefinitions": List[ReportDefinitionOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyReportDefinitionRequestRequestTypeDef = TypedDict(
     "ModifyReportDefinitionRequestRequestTypeDef",
     {
         "ReportName": str,
```

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/PKG-INFO` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cur
-Version: 1.28.12
-Summary: Type annotations for boto3.CostandUsageReportService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cur.svg?color=blue)](https://pypi.org/project/mypy-boto3-cur)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cur)](https://pepy.tech/project/mypy-boto3-cur)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CostandUsageReportService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
+[boto3.CostandUsageReportService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cur.html#CostandUsageReportService)
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
 [mypy-boto3-cur docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cur/).
 
 See how it helps to find and fix potential bugs:
 
@@ -328,21 +328,21 @@
 
 `mypy_boto3_cur.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cur.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResponseTypeDef,
-    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     DescribeReportDefinitionsRequestRequestTypeDef,
     ReportDefinitionOutputTypeDef,
     ReportDefinitionTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    DeleteReportDefinitionResponseTypeDef,
+    DescribeReportDefinitionsRequestDescribeReportDefinitionsPaginateTypeDef,
     DescribeReportDefinitionsResponseTypeDef,
     ModifyReportDefinitionRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
```

### Comparing `mypy-boto3-cur-1.28.12/mypy_boto3_cur.egg-info/SOURCES.txt` & `mypy-boto3-cur-1.28.15/mypy_boto3_cur.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cur-1.28.12/setup.py` & `mypy-boto3-cur-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cur",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cur"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CostandUsageReportService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CostandUsageReportService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

