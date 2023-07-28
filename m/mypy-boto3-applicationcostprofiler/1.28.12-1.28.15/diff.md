# Comparing `tmp/mypy-boto3-applicationcostprofiler-1.28.12.tar.gz` & `tmp/mypy-boto3-applicationcostprofiler-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-applicationcostprofiler-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
+gzip compressed data, was "mypy-boto3-applicationcostprofiler-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-applicationcostprofiler-1.28.12.tar` & `mypy-boto3-applicationcostprofiler-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.480577 mypy-boto3-applicationcostprofiler-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-07-27 05:34:18.480577 mypy-boto3-applicationcostprofiler-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12677 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.472577 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5827 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.480577 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-07-27 05:34:18.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-27 05:34:18.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 05:34:18.000000 mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.480577 mypy-boto3-applicationcostprofiler-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-27 05:17:26.000000 mypy-boto3-applicationcostprofiler-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.208654 mypy-boto3-applicationcostprofiler-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-07-28 20:42:16.208654 mypy-boto3-applicationcostprofiler-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.204654 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-07-28 20:19:26.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.208654 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-07-28 20:42:15.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-28 20:42:16.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:15.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 20:42:15.000000 mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.208654 mypy-boto3-applicationcostprofiler-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-28 20:19:25.000000 mypy-boto3-applicationcostprofiler-1.28.15/setup.py
```

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/LICENSE` & `mypy-boto3-applicationcostprofiler-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/PKG-INFO` & `mypy-boto3-applicationcostprofiler-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-applicationcostprofiler
-Version: 1.28.12
-Summary: Type annotations for boto3.ApplicationCostProfiler 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApplicationCostProfiler 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-applicationcostprofiler)](https://pepy.tech/project/mypy-boto3-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationCostProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[boto3.ApplicationCostProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
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
 [mypy-boto3-applicationcostprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,31 +325,30 @@
 
 `mypy_boto3_applicationcostprofiler.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
+    ResponseMetadataTypeDef,
     GetReportDefinitionRequestRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     SourceS3LocationTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    S3LocationTypeDef,
+    ListReportDefinitionsRequestRequestTypeDef,
+    DeleteReportDefinitionResultTypeDef,
+    ImportApplicationUsageResultTypeDef,
     PutReportDefinitionResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateReportDefinitionResultTypeDef,
     GetReportDefinitionResultTypeDef,
-    ReportDefinitionTypeDef,
-    ImportApplicationUsageRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
+    ReportDefinitionTypeDef,
     UpdateReportDefinitionRequestRequestTypeDef,
+    ImportApplicationUsageRequestRequestTypeDef,
+    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
     ListReportDefinitionsResultTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/README.md` & `mypy-boto3-applicationcostprofiler-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-applicationcostprofiler)](https://pepy.tech/project/mypy-boto3-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationCostProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[boto3.ApplicationCostProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
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
 [mypy-boto3-applicationcostprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,31 +293,30 @@
 
 `mypy_boto3_applicationcostprofiler.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
+    ResponseMetadataTypeDef,
     GetReportDefinitionRequestRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     SourceS3LocationTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    S3LocationTypeDef,
+    ListReportDefinitionsRequestRequestTypeDef,
+    DeleteReportDefinitionResultTypeDef,
+    ImportApplicationUsageResultTypeDef,
     PutReportDefinitionResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateReportDefinitionResultTypeDef,
     GetReportDefinitionResultTypeDef,
-    ReportDefinitionTypeDef,
-    ImportApplicationUsageRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
+    ReportDefinitionTypeDef,
     UpdateReportDefinitionRequestRequestTypeDef,
+    ImportApplicationUsageRequestRequestTypeDef,
+    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
     ListReportDefinitionsResultTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/__init__.py` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/__init__.pyi` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/__main__.py` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApplicationCostProfiler 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ApplicationCostProfiler 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler\nOther"
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

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/client.py` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/client.pyi` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/literals.py` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/literals.pyi` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/paginator.py` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListReportDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/paginators/#listreportdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReportDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/paginators/#listreportdefinitionspaginator)
         """
```

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/paginator.pyi` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListReportDefinitionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/paginators/#listreportdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListReportDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/paginators/#listreportdefinitionspaginator)
         """
```

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/type_defs.py` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -18,61 +18,62 @@
 from .literals import FormatType, ReportFrequencyType, S3BucketRegionType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
-    "DeleteReportDefinitionResultTypeDef",
+    "ResponseMetadataTypeDef",
     "GetReportDefinitionRequestRequestTypeDef",
-    "S3LocationOutputTypeDef",
+    "S3LocationTypeDef",
     "SourceS3LocationTypeDef",
-    "ImportApplicationUsageResultTypeDef",
-    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
-    "ListReportDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "S3LocationTypeDef",
+    "ListReportDefinitionsRequestRequestTypeDef",
+    "DeleteReportDefinitionResultTypeDef",
+    "ImportApplicationUsageResultTypeDef",
     "PutReportDefinitionResultTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateReportDefinitionResultTypeDef",
     "GetReportDefinitionResultTypeDef",
-    "ReportDefinitionTypeDef",
-    "ImportApplicationUsageRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
+    "ReportDefinitionTypeDef",
     "UpdateReportDefinitionRequestRequestTypeDef",
+    "ImportApplicationUsageRequestRequestTypeDef",
+    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
     "ListReportDefinitionsResultTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-DeleteReportDefinitionResultTypeDef = TypedDict(
-    "DeleteReportDefinitionResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetReportDefinitionRequestRequestTypeDef = TypedDict(
     "GetReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
 )
 
 _RequiredSourceS3LocationTypeDef = TypedDict(
@@ -86,147 +87,134 @@
     "_OptionalSourceS3LocationTypeDef",
     {
         "region": S3BucketRegionType,
     },
     total=False,
 )
 
-
 class SourceS3LocationTypeDef(_RequiredSourceS3LocationTypeDef, _OptionalSourceS3LocationTypeDef):
     pass
 
-
-ImportApplicationUsageResultTypeDef = TypedDict(
-    "ImportApplicationUsageResultTypeDef",
-    {
-        "importId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef = TypedDict(
-    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
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
 
 ListReportDefinitionsRequestRequestTypeDef = TypedDict(
     "ListReportDefinitionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteReportDefinitionResultTypeDef = TypedDict(
+    "DeleteReportDefinitionResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+ImportApplicationUsageResultTypeDef = TypedDict(
+    "ImportApplicationUsageResultTypeDef",
     {
-        "bucket": str,
-        "prefix": str,
+        "importId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutReportDefinitionResultTypeDef = TypedDict(
     "PutReportDefinitionResultTypeDef",
     {
         "reportId": str,
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReportDefinitionResultTypeDef = TypedDict(
     "UpdateReportDefinitionResultTypeDef",
     {
         "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReportDefinitionResultTypeDef = TypedDict(
     "GetReportDefinitionResultTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
-        "destinationS3Location": S3LocationOutputTypeDef,
+        "destinationS3Location": S3LocationTypeDef,
         "createdAt": datetime,
         "lastUpdated": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportDefinitionTypeDef = TypedDict(
-    "ReportDefinitionTypeDef",
+PutReportDefinitionRequestRequestTypeDef = TypedDict(
+    "PutReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
-        "destinationS3Location": S3LocationOutputTypeDef,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-    },
-    total=False,
-)
-
-ImportApplicationUsageRequestRequestTypeDef = TypedDict(
-    "ImportApplicationUsageRequestRequestTypeDef",
-    {
-        "sourceS3Location": SourceS3LocationTypeDef,
+        "destinationS3Location": S3LocationTypeDef,
     },
 )
 
-PutReportDefinitionRequestRequestTypeDef = TypedDict(
-    "PutReportDefinitionRequestRequestTypeDef",
+ReportDefinitionTypeDef = TypedDict(
+    "ReportDefinitionTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
         "destinationS3Location": S3LocationTypeDef,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
     },
+    total=False,
 )
 
 UpdateReportDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
         "destinationS3Location": S3LocationTypeDef,
     },
 )
 
+ImportApplicationUsageRequestRequestTypeDef = TypedDict(
+    "ImportApplicationUsageRequestRequestTypeDef",
+    {
+        "sourceS3Location": SourceS3LocationTypeDef,
+    },
+)
+
+ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef = TypedDict(
+    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListReportDefinitionsResultTypeDef = TypedDict(
     "ListReportDefinitionsResultTypeDef",
     {
         "reportDefinitions": List[ReportDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler/type_defs.pyi` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,60 +18,63 @@
 from .literals import FormatType, ReportFrequencyType, S3BucketRegionType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
-    "DeleteReportDefinitionResultTypeDef",
+    "ResponseMetadataTypeDef",
     "GetReportDefinitionRequestRequestTypeDef",
-    "S3LocationOutputTypeDef",
+    "S3LocationTypeDef",
     "SourceS3LocationTypeDef",
-    "ImportApplicationUsageResultTypeDef",
-    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
-    "ListReportDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "S3LocationTypeDef",
+    "ListReportDefinitionsRequestRequestTypeDef",
+    "DeleteReportDefinitionResultTypeDef",
+    "ImportApplicationUsageResultTypeDef",
     "PutReportDefinitionResultTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateReportDefinitionResultTypeDef",
     "GetReportDefinitionResultTypeDef",
-    "ReportDefinitionTypeDef",
-    "ImportApplicationUsageRequestRequestTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
+    "ReportDefinitionTypeDef",
     "UpdateReportDefinitionRequestRequestTypeDef",
+    "ImportApplicationUsageRequestRequestTypeDef",
+    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
     "ListReportDefinitionsResultTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-DeleteReportDefinitionResultTypeDef = TypedDict(
-    "DeleteReportDefinitionResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetReportDefinitionRequestRequestTypeDef = TypedDict(
     "GetReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
 )
 
 _RequiredSourceS3LocationTypeDef = TypedDict(
@@ -85,145 +88,136 @@
     "_OptionalSourceS3LocationTypeDef",
     {
         "region": S3BucketRegionType,
     },
     total=False,
 )
 
+
 class SourceS3LocationTypeDef(_RequiredSourceS3LocationTypeDef, _OptionalSourceS3LocationTypeDef):
     pass
 
-ImportApplicationUsageResultTypeDef = TypedDict(
-    "ImportApplicationUsageResultTypeDef",
-    {
-        "importId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef = TypedDict(
-    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
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
 
 ListReportDefinitionsRequestRequestTypeDef = TypedDict(
     "ListReportDefinitionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteReportDefinitionResultTypeDef = TypedDict(
+    "DeleteReportDefinitionResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+ImportApplicationUsageResultTypeDef = TypedDict(
+    "ImportApplicationUsageResultTypeDef",
     {
-        "bucket": str,
-        "prefix": str,
+        "importId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutReportDefinitionResultTypeDef = TypedDict(
     "PutReportDefinitionResultTypeDef",
     {
         "reportId": str,
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReportDefinitionResultTypeDef = TypedDict(
     "UpdateReportDefinitionResultTypeDef",
     {
         "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReportDefinitionResultTypeDef = TypedDict(
     "GetReportDefinitionResultTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
-        "destinationS3Location": S3LocationOutputTypeDef,
+        "destinationS3Location": S3LocationTypeDef,
         "createdAt": datetime,
         "lastUpdated": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReportDefinitionTypeDef = TypedDict(
-    "ReportDefinitionTypeDef",
+PutReportDefinitionRequestRequestTypeDef = TypedDict(
+    "PutReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
-        "destinationS3Location": S3LocationOutputTypeDef,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-    },
-    total=False,
-)
-
-ImportApplicationUsageRequestRequestTypeDef = TypedDict(
-    "ImportApplicationUsageRequestRequestTypeDef",
-    {
-        "sourceS3Location": SourceS3LocationTypeDef,
+        "destinationS3Location": S3LocationTypeDef,
     },
 )
 
-PutReportDefinitionRequestRequestTypeDef = TypedDict(
-    "PutReportDefinitionRequestRequestTypeDef",
+ReportDefinitionTypeDef = TypedDict(
+    "ReportDefinitionTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
         "destinationS3Location": S3LocationTypeDef,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
     },
+    total=False,
 )
 
 UpdateReportDefinitionRequestRequestTypeDef = TypedDict(
     "UpdateReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
         "destinationS3Location": S3LocationTypeDef,
     },
 )
 
+ImportApplicationUsageRequestRequestTypeDef = TypedDict(
+    "ImportApplicationUsageRequestRequestTypeDef",
+    {
+        "sourceS3Location": SourceS3LocationTypeDef,
+    },
+)
+
+ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef = TypedDict(
+    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListReportDefinitionsResultTypeDef = TypedDict(
     "ListReportDefinitionsResultTypeDef",
     {
         "reportDefinitions": List[ReportDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/PKG-INFO` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-applicationcostprofiler
-Version: 1.28.12
-Summary: Type annotations for boto3.ApplicationCostProfiler 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApplicationCostProfiler 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/mypy-boto3-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-applicationcostprofiler)](https://pepy.tech/project/mypy-boto3-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApplicationCostProfiler 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
+[boto3.ApplicationCostProfiler 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
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
 [mypy-boto3-applicationcostprofiler docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_applicationcostprofiler/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,31 +325,30 @@
 
 `mypy_boto3_applicationcostprofiler.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
+    ResponseMetadataTypeDef,
     GetReportDefinitionRequestRequestTypeDef,
-    S3LocationOutputTypeDef,
+    S3LocationTypeDef,
     SourceS3LocationTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    S3LocationTypeDef,
+    ListReportDefinitionsRequestRequestTypeDef,
+    DeleteReportDefinitionResultTypeDef,
+    ImportApplicationUsageResultTypeDef,
     PutReportDefinitionResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateReportDefinitionResultTypeDef,
     GetReportDefinitionResultTypeDef,
-    ReportDefinitionTypeDef,
-    ImportApplicationUsageRequestRequestTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
+    ReportDefinitionTypeDef,
     UpdateReportDefinitionRequestRequestTypeDef,
+    ImportApplicationUsageRequestRequestTypeDef,
+    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
     ListReportDefinitionsResultTypeDef,
 )
 
 
 def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/mypy_boto3_applicationcostprofiler.egg-info/SOURCES.txt` & `mypy-boto3-applicationcostprofiler-1.28.15/mypy_boto3_applicationcostprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-applicationcostprofiler-1.28.12/setup.py` & `mypy-boto3-applicationcostprofiler-1.28.15/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-applicationcostprofiler",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_applicationcostprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApplicationCostProfiler 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ApplicationCostProfiler 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

