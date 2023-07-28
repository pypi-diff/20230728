# Comparing `tmp/mypy-boto3-importexport-1.28.12.tar.gz` & `tmp/mypy-boto3-importexport-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-importexport-1.28.12.tar", last modified: Thu Jul 27 05:34:46 2023, max compression
+gzip compressed data, was "mypy-boto3-importexport-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
```

## Comparing `mypy-boto3-importexport-1.28.12.tar` & `mypy-boto3-importexport-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.920492 mypy-boto3-importexport-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-27 05:34:46.920492 mypy-boto3-importexport-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.916492 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-27 05:23:33.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-07-27 05:23:33.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-27 05:23:33.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:46.920492 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-27 05:34:46.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:46.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:46.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:46.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:46.000000 mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:46.920492 mypy-boto3-importexport-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:23:32.000000 mypy-boto3-importexport-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.349214 mypy-boto3-importexport-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:40.000000 mypy-boto3-importexport-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-28 20:42:56.349214 mypy-boto3-importexport-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-07-28 20:27:40.000000 mypy-boto3-importexport-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.349214 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-28 20:27:40.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-28 20:27:40.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:27:40.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-07-28 20:27:41.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-28 20:27:41.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-07-28 20:27:41.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-07-28 20:27:41.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-28 20:27:41.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-28 20:27:41.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:40.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-28 20:27:41.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-28 20:27:41.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:40.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.349214 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13210 2023-07-28 20:42:56.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:56.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:56.000000 mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.349214 mypy-boto3-importexport-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:27:40.000000 mypy-boto3-importexport-1.28.15/setup.py
```

### Comparing `mypy-boto3-importexport-1.28.12/LICENSE` & `mypy-boto3-importexport-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.28.12/PKG-INFO` & `mypy-boto3-importexport-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-importexport
-Version: 1.28.12
-Summary: Type annotations for boto3.ImportExport 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ImportExport 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-importexport)](https://pepy.tech/project/mypy-boto3-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ImportExport 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[boto3.ImportExport 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [mypy-boto3-importexport docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,29 +321,29 @@
 `mypy_boto3_importexport.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListJobsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListJobsInputRequestTypeDef,
     UpdateJobInputRequestTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
 def get_structure() -> ArtifactTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-importexport-1.28.12/README.md` & `mypy-boto3-importexport-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-importexport)](https://pepy.tech/project/mypy-boto3-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ImportExport 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[boto3.ImportExport 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [mypy-boto3-importexport docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,29 +289,29 @@
 `mypy_boto3_importexport.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListJobsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListJobsInputRequestTypeDef,
     UpdateJobInputRequestTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
 def get_structure() -> ArtifactTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/__init__.py` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/__init__.pyi` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/__main__.py` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ImportExport 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ImportExport 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport\nOther"
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

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/client.py` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/client.pyi` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/literals.py` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/literals.pyi` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/paginator.py` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, APIVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, APIVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/paginators/#listjobspaginator)
         """
```

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/paginator.pyi` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListJobsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/paginators/#listjobspaginator)
     """
 
     def paginate(
-        self, *, APIVersion: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, APIVersion: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/paginators/#listjobspaginator)
         """
```

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/type_defs.py` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,29 +22,29 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ArtifactTypeDef",
     "CancelJobInputRequestTypeDef",
-    "CancelJobOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateJobInputRequestTypeDef",
     "GetShippingLabelInputRequestTypeDef",
-    "GetShippingLabelOutputTypeDef",
     "GetStatusInputRequestTypeDef",
     "JobTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
-    "ListJobsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListJobsInputRequestTypeDef",
     "UpdateJobInputRequestTypeDef",
+    "CancelJobOutputTypeDef",
     "CreateJobOutputTypeDef",
+    "GetShippingLabelOutputTypeDef",
     "GetStatusOutputTypeDef",
     "UpdateJobOutputTypeDef",
     "ListJobsOutputTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
 )
 
 ArtifactTypeDef = TypedDict(
     "ArtifactTypeDef",
     {
         "Description": str,
         "URL": str,
@@ -69,19 +69,22 @@
 
 class CancelJobInputRequestTypeDef(
     _RequiredCancelJobInputRequestTypeDef, _OptionalCancelJobInputRequestTypeDef
 ):
     pass
 
 
-CancelJobOutputTypeDef = TypedDict(
-    "CancelJobOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Success": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateJobInputRequestTypeDef = TypedDict(
     "_RequiredCreateJobInputRequestTypeDef",
     {
         "JobType": JobTypeType,
@@ -132,23 +135,14 @@
 
 class GetShippingLabelInputRequestTypeDef(
     _RequiredGetShippingLabelInputRequestTypeDef, _OptionalGetShippingLabelInputRequestTypeDef
 ):
     pass
 
 
-GetShippingLabelOutputTypeDef = TypedDict(
-    "GetShippingLabelOutputTypeDef",
-    {
-        "ShippingLabelURL": str,
-        "Warning": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetStatusInputRequestTypeDef = TypedDict(
     "_RequiredGetStatusInputRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetStatusInputRequestTypeDef = TypedDict(
@@ -173,54 +167,34 @@
         "CreationDate": datetime,
         "IsCanceled": bool,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
-ListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "ListJobsInputListJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "APIVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListJobsInputRequestTypeDef = TypedDict(
     "ListJobsInputRequestTypeDef",
     {
         "MaxJobs": int,
         "Marker": str,
         "APIVersion": str,
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
 _RequiredUpdateJobInputRequestTypeDef = TypedDict(
     "_RequiredUpdateJobInputRequestTypeDef",
     {
         "JobId": str,
         "Manifest": str,
         "JobType": JobTypeType,
         "ValidateOnly": bool,
@@ -237,24 +211,41 @@
 
 class UpdateJobInputRequestTypeDef(
     _RequiredUpdateJobInputRequestTypeDef, _OptionalUpdateJobInputRequestTypeDef
 ):
     pass
 
 
+CancelJobOutputTypeDef = TypedDict(
+    "CancelJobOutputTypeDef",
+    {
+        "Success": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
         "JobId": str,
         "JobType": JobTypeType,
         "Signature": str,
         "SignatureFileContents": str,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetShippingLabelOutputTypeDef = TypedDict(
+    "GetShippingLabelOutputTypeDef",
+    {
+        "ShippingLabelURL": str,
+        "Warning": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStatusOutputTypeDef = TypedDict(
     "GetStatusOutputTypeDef",
     {
         "JobId": str,
@@ -269,29 +260,38 @@
         "LogKey": str,
         "ErrorCount": int,
         "Signature": str,
         "SignatureFileContents": str,
         "CurrentManifest": str,
         "CreationDate": datetime,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobOutputTypeDef = TypedDict(
     "UpdateJobOutputTypeDef",
     {
         "Success": bool,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "IsTruncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "ListJobsInputListJobsPaginateTypeDef",
+    {
+        "APIVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
```

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport/type_defs.pyi` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -21,29 +21,29 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ArtifactTypeDef",
     "CancelJobInputRequestTypeDef",
-    "CancelJobOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateJobInputRequestTypeDef",
     "GetShippingLabelInputRequestTypeDef",
-    "GetShippingLabelOutputTypeDef",
     "GetStatusInputRequestTypeDef",
     "JobTypeDef",
-    "ListJobsInputListJobsPaginateTypeDef",
-    "ListJobsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListJobsInputRequestTypeDef",
     "UpdateJobInputRequestTypeDef",
+    "CancelJobOutputTypeDef",
     "CreateJobOutputTypeDef",
+    "GetShippingLabelOutputTypeDef",
     "GetStatusOutputTypeDef",
     "UpdateJobOutputTypeDef",
     "ListJobsOutputTypeDef",
+    "ListJobsInputListJobsPaginateTypeDef",
 )
 
 ArtifactTypeDef = TypedDict(
     "ArtifactTypeDef",
     {
         "Description": str,
         "URL": str,
@@ -66,19 +66,22 @@
 )
 
 class CancelJobInputRequestTypeDef(
     _RequiredCancelJobInputRequestTypeDef, _OptionalCancelJobInputRequestTypeDef
 ):
     pass
 
-CancelJobOutputTypeDef = TypedDict(
-    "CancelJobOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Success": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateJobInputRequestTypeDef = TypedDict(
     "_RequiredCreateJobInputRequestTypeDef",
     {
         "JobType": JobTypeType,
@@ -125,23 +128,14 @@
 )
 
 class GetShippingLabelInputRequestTypeDef(
     _RequiredGetShippingLabelInputRequestTypeDef, _OptionalGetShippingLabelInputRequestTypeDef
 ):
     pass
 
-GetShippingLabelOutputTypeDef = TypedDict(
-    "GetShippingLabelOutputTypeDef",
-    {
-        "ShippingLabelURL": str,
-        "Warning": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetStatusInputRequestTypeDef = TypedDict(
     "_RequiredGetStatusInputRequestTypeDef",
     {
         "JobId": str,
     },
 )
 _OptionalGetStatusInputRequestTypeDef = TypedDict(
@@ -164,54 +158,34 @@
         "CreationDate": datetime,
         "IsCanceled": bool,
         "JobType": JobTypeType,
     },
     total=False,
 )
 
-ListJobsInputListJobsPaginateTypeDef = TypedDict(
-    "ListJobsInputListJobsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "APIVersion": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListJobsInputRequestTypeDef = TypedDict(
     "ListJobsInputRequestTypeDef",
     {
         "MaxJobs": int,
         "Marker": str,
         "APIVersion": str,
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
 _RequiredUpdateJobInputRequestTypeDef = TypedDict(
     "_RequiredUpdateJobInputRequestTypeDef",
     {
         "JobId": str,
         "Manifest": str,
         "JobType": JobTypeType,
         "ValidateOnly": bool,
@@ -226,24 +200,41 @@
 )
 
 class UpdateJobInputRequestTypeDef(
     _RequiredUpdateJobInputRequestTypeDef, _OptionalUpdateJobInputRequestTypeDef
 ):
     pass
 
+CancelJobOutputTypeDef = TypedDict(
+    "CancelJobOutputTypeDef",
+    {
+        "Success": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
         "JobId": str,
         "JobType": JobTypeType,
         "Signature": str,
         "SignatureFileContents": str,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetShippingLabelOutputTypeDef = TypedDict(
+    "GetShippingLabelOutputTypeDef",
+    {
+        "ShippingLabelURL": str,
+        "Warning": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStatusOutputTypeDef = TypedDict(
     "GetStatusOutputTypeDef",
     {
         "JobId": str,
@@ -258,29 +249,38 @@
         "LogKey": str,
         "ErrorCount": int,
         "Signature": str,
         "SignatureFileContents": str,
         "CurrentManifest": str,
         "CreationDate": datetime,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateJobOutputTypeDef = TypedDict(
     "UpdateJobOutputTypeDef",
     {
         "Success": bool,
         "WarningMessage": str,
         "ArtifactList": List[ArtifactTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsOutputTypeDef = TypedDict(
     "ListJobsOutputTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "IsTruncated": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListJobsInputListJobsPaginateTypeDef = TypedDict(
+    "ListJobsInputListJobsPaginateTypeDef",
+    {
+        "APIVersion": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
```

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/PKG-INFO` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-importexport
-Version: 1.28.12
-Summary: Type annotations for boto3.ImportExport 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ImportExport 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-importexport.svg?color=blue)](https://pypi.org/project/mypy-boto3-importexport)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-importexport)](https://pepy.tech/project/mypy-boto3-importexport)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ImportExport 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
+[boto3.ImportExport 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/importexport.html#ImportExport)
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
 [mypy-boto3-importexport docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_importexport/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,29 +321,29 @@
 `mypy_boto3_importexport.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_importexport.type_defs import (
     ArtifactTypeDef,
     CancelJobInputRequestTypeDef,
-    CancelJobOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateJobInputRequestTypeDef,
     GetShippingLabelInputRequestTypeDef,
-    GetShippingLabelOutputTypeDef,
     GetStatusInputRequestTypeDef,
     JobTypeDef,
-    ListJobsInputListJobsPaginateTypeDef,
-    ListJobsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListJobsInputRequestTypeDef,
     UpdateJobInputRequestTypeDef,
+    CancelJobOutputTypeDef,
     CreateJobOutputTypeDef,
+    GetShippingLabelOutputTypeDef,
     GetStatusOutputTypeDef,
     UpdateJobOutputTypeDef,
     ListJobsOutputTypeDef,
+    ListJobsInputListJobsPaginateTypeDef,
 )
 
 
 def get_structure() -> ArtifactTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-importexport-1.28.12/mypy_boto3_importexport.egg-info/SOURCES.txt` & `mypy-boto3-importexport-1.28.15/mypy_boto3_importexport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-importexport-1.28.12/setup.py` & `mypy-boto3-importexport-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-importexport",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_importexport"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ImportExport 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ImportExport 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

