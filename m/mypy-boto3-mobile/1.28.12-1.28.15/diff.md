# Comparing `tmp/mypy-boto3-mobile-1.28.12.tar.gz` & `tmp/mypy-boto3-mobile-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mobile-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
+gzip compressed data, was "mypy-boto3-mobile-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
```

## Comparing `mypy-boto3-mobile-1.28.12.tar` & `mypy-boto3-mobile-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.188429 mypy-boto3-mobile-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-27 05:35:04.188429 mypy-boto3-mobile-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.180429 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-07-27 05:26:46.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-27 05:26:46.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.188429 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-27 05:35:04.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:35:04.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:35:04.000000 mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.188429 mypy-boto3-mobile-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:26:45.000000 mypy-boto3-mobile-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.089554 mypy-boto3-mobile-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-28 20:43:21.089554 mypy-boto3-mobile-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.077554 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9113 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8050 2023-07-28 20:32:10.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-07-28 20:32:10.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-07-28 20:32:10.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.089554 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13449 2023-07-28 20:43:20.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:43:20.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:20.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:20.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:43:20.000000 mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.089554 mypy-boto3-mobile-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:32:09.000000 mypy-boto3-mobile-1.28.15/setup.py
```

### Comparing `mypy-boto3-mobile-1.28.12/LICENSE` & `mypy-boto3-mobile-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.12/PKG-INFO` & `mypy-boto3-mobile-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mobile
-Version: 1.28.12
-Summary: Type annotations for boto3.Mobile 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Mobile 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mobile.svg?color=blue)](https://pypi.org/project/mypy-boto3-mobile)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mobile)](https://pepy.tech/project/mypy-boto3-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Mobile 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[boto3.Mobile 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [mypy-boto3-mobile docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,34 +323,34 @@
 `mypy_boto3_mobile.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mobile.type_defs import (
     BundleDetailsTypeDef,
     CreateProjectRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProjectRequestRequestTypeDef,
     ResourceTypeDef,
     DescribeBundleRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ExportBundleRequestRequestTypeDef,
-    ExportBundleResultTypeDef,
     ExportProjectRequestRequestTypeDef,
-    ExportProjectResultTypeDef,
-    ListBundlesRequestListBundlesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBundlesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeBundleResultTypeDef,
+    ExportBundleResultTypeDef,
+    ExportProjectResultTypeDef,
     ListBundlesResultTypeDef,
     DeleteProjectResultTypeDef,
     ProjectDetailsTypeDef,
+    ListBundlesRequestListBundlesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsResultTypeDef,
     CreateProjectResultTypeDef,
     DescribeProjectResultTypeDef,
     UpdateProjectResultTypeDef,
 )
```

### Comparing `mypy-boto3-mobile-1.28.12/README.md` & `mypy-boto3-mobile-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mobile.svg?color=blue)](https://pypi.org/project/mypy-boto3-mobile)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mobile)](https://pepy.tech/project/mypy-boto3-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Mobile 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[boto3.Mobile 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [mypy-boto3-mobile docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,34 +291,34 @@
 `mypy_boto3_mobile.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mobile.type_defs import (
     BundleDetailsTypeDef,
     CreateProjectRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProjectRequestRequestTypeDef,
     ResourceTypeDef,
     DescribeBundleRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ExportBundleRequestRequestTypeDef,
-    ExportBundleResultTypeDef,
     ExportProjectRequestRequestTypeDef,
-    ExportProjectResultTypeDef,
-    ListBundlesRequestListBundlesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBundlesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeBundleResultTypeDef,
+    ExportBundleResultTypeDef,
+    ExportProjectResultTypeDef,
     ListBundlesResultTypeDef,
     DeleteProjectResultTypeDef,
     ProjectDetailsTypeDef,
+    ListBundlesRequestListBundlesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsResultTypeDef,
     CreateProjectResultTypeDef,
     DescribeProjectResultTypeDef,
     UpdateProjectResultTypeDef,
 )
```

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/__init__.py` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/__init__.pyi` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/__main__.py` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Mobile 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Mobile 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile\nOther"
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

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/client.py` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/client.pyi` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/literals.py` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/literals.pyi` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/paginator.py` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,28 +43,28 @@
 class ListBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/paginators/#listbundlespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/paginators/#listbundlespaginator)
         """
 
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/paginator.pyi` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,27 +40,27 @@
 class ListBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/paginators/#listbundlespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/paginators/#listbundlespaginator)
         """
 
 class ListProjectsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListProjects)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/paginators/#listprojectspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProjectsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile.Paginator.ListProjects.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/paginators/#listprojectspaginator)
         """
```

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/type_defs.py` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -20,38 +20,37 @@
 from .literals import PlatformType, ProjectStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BundleDetailsTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "ResourceTypeDef",
     "DescribeBundleRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ExportBundleRequestRequestTypeDef",
-    "ExportBundleResultTypeDef",
     "ExportProjectRequestRequestTypeDef",
-    "ExportProjectResultTypeDef",
-    "ListBundlesRequestListBundlesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBundlesRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeBundleResultTypeDef",
+    "ExportBundleResultTypeDef",
+    "ExportProjectResultTypeDef",
     "ListBundlesResultTypeDef",
     "DeleteProjectResultTypeDef",
     "ProjectDetailsTypeDef",
+    "ListBundlesRequestListBundlesPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "CreateProjectResultTypeDef",
     "DescribeProjectResultTypeDef",
     "UpdateProjectResultTypeDef",
 )
 
 BundleDetailsTypeDef = TypedDict(
@@ -74,14 +73,25 @@
         "region": str,
         "contents": Union[str, bytes, IO[Any], StreamingBody],
         "snapshotId": str,
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
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 
@@ -114,21 +124,19 @@
     "_OptionalDescribeProjectRequestRequestTypeDef",
     {
         "syncFromResources": bool,
     },
     total=False,
 )
 
-
 class DescribeProjectRequestRequestTypeDef(
     _RequiredDescribeProjectRequestRequestTypeDef, _OptionalDescribeProjectRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredExportBundleRequestRequestTypeDef = TypedDict(
     "_RequiredExportBundleRequestRequestTypeDef",
     {
         "bundleId": str,
     },
 )
 _OptionalExportBundleRequestRequestTypeDef = TypedDict(
@@ -136,71 +144,45 @@
     {
         "projectId": str,
         "platform": PlatformType,
     },
     total=False,
 )
 
-
 class ExportBundleRequestRequestTypeDef(
     _RequiredExportBundleRequestRequestTypeDef, _OptionalExportBundleRequestRequestTypeDef
 ):
     pass
 
-
-ExportBundleResultTypeDef = TypedDict(
-    "ExportBundleResultTypeDef",
-    {
-        "downloadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ExportProjectRequestRequestTypeDef = TypedDict(
     "ExportProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 
-ExportProjectResultTypeDef = TypedDict(
-    "ExportProjectResultTypeDef",
-    {
-        "downloadUrl": str,
-        "shareUrl": str,
-        "snapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBundlesRequestListBundlesPaginateTypeDef = TypedDict(
-    "ListBundlesRequestListBundlesPaginateTypeDef",
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
 
 ListBundlesRequestRequestTypeDef = TypedDict(
     "ListBundlesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -211,79 +193,74 @@
     {
         "name": str,
         "projectId": str,
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
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateProjectRequestRequestTypeDef",
     {
         "contents": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
-
 DescribeBundleResultTypeDef = TypedDict(
     "DescribeBundleResultTypeDef",
     {
         "details": BundleDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportBundleResultTypeDef = TypedDict(
+    "ExportBundleResultTypeDef",
+    {
+        "downloadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportProjectResultTypeDef = TypedDict(
+    "ExportProjectResultTypeDef",
+    {
+        "downloadUrl": str,
+        "shareUrl": str,
+        "snapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBundlesResultTypeDef = TypedDict(
     "ListBundlesResultTypeDef",
     {
         "bundleList": List[BundleDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteProjectResultTypeDef = TypedDict(
     "DeleteProjectResultTypeDef",
     {
         "deletedResources": List[ResourceTypeDef],
         "orphanedResources": List[ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProjectDetailsTypeDef = TypedDict(
     "ProjectDetailsTypeDef",
     {
         "name": str,
@@ -294,39 +271,55 @@
         "lastUpdatedDate": datetime,
         "consoleUrl": str,
         "resources": List[ResourceTypeDef],
     },
     total=False,
 )
 
+ListBundlesRequestListBundlesPaginateTypeDef = TypedDict(
+    "ListBundlesRequestListBundlesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProjectResultTypeDef = TypedDict(
     "CreateProjectResultTypeDef",
     {
         "details": ProjectDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProjectResultTypeDef = TypedDict(
     "DescribeProjectResultTypeDef",
     {
         "details": ProjectDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectResultTypeDef = TypedDict(
     "UpdateProjectResultTypeDef",
     {
         "details": ProjectDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile/type_defs.pyi` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,37 +20,38 @@
 from .literals import PlatformType, ProjectStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BundleDetailsTypeDef",
     "CreateProjectRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "ResourceTypeDef",
     "DescribeBundleRequestRequestTypeDef",
     "DescribeProjectRequestRequestTypeDef",
     "ExportBundleRequestRequestTypeDef",
-    "ExportBundleResultTypeDef",
     "ExportProjectRequestRequestTypeDef",
-    "ExportProjectResultTypeDef",
-    "ListBundlesRequestListBundlesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBundlesRequestRequestTypeDef",
-    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsRequestRequestTypeDef",
     "ProjectSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeBundleResultTypeDef",
+    "ExportBundleResultTypeDef",
+    "ExportProjectResultTypeDef",
     "ListBundlesResultTypeDef",
     "DeleteProjectResultTypeDef",
     "ProjectDetailsTypeDef",
+    "ListBundlesRequestListBundlesPaginateTypeDef",
+    "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListProjectsResultTypeDef",
     "CreateProjectResultTypeDef",
     "DescribeProjectResultTypeDef",
     "UpdateProjectResultTypeDef",
 )
 
 BundleDetailsTypeDef = TypedDict(
@@ -73,14 +74,25 @@
         "region": str,
         "contents": Union[str, bytes, IO[Any], StreamingBody],
         "snapshotId": str,
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
 DeleteProjectRequestRequestTypeDef = TypedDict(
     "DeleteProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 
@@ -113,19 +125,21 @@
     "_OptionalDescribeProjectRequestRequestTypeDef",
     {
         "syncFromResources": bool,
     },
     total=False,
 )
 
+
 class DescribeProjectRequestRequestTypeDef(
     _RequiredDescribeProjectRequestRequestTypeDef, _OptionalDescribeProjectRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredExportBundleRequestRequestTypeDef = TypedDict(
     "_RequiredExportBundleRequestRequestTypeDef",
     {
         "bundleId": str,
     },
 )
 _OptionalExportBundleRequestRequestTypeDef = TypedDict(
@@ -133,69 +147,47 @@
     {
         "projectId": str,
         "platform": PlatformType,
     },
     total=False,
 )
 
+
 class ExportBundleRequestRequestTypeDef(
     _RequiredExportBundleRequestRequestTypeDef, _OptionalExportBundleRequestRequestTypeDef
 ):
     pass
 
-ExportBundleResultTypeDef = TypedDict(
-    "ExportBundleResultTypeDef",
-    {
-        "downloadUrl": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ExportProjectRequestRequestTypeDef = TypedDict(
     "ExportProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 
-ExportProjectResultTypeDef = TypedDict(
-    "ExportProjectResultTypeDef",
-    {
-        "downloadUrl": str,
-        "shareUrl": str,
-        "snapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListBundlesRequestListBundlesPaginateTypeDef = TypedDict(
-    "ListBundlesRequestListBundlesPaginateTypeDef",
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
 
 ListBundlesRequestRequestTypeDef = TypedDict(
     "ListBundlesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
-    "ListProjectsRequestListProjectsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProjectsRequestRequestTypeDef = TypedDict(
     "ListProjectsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -206,77 +198,76 @@
     {
         "name": str,
         "projectId": str,
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
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectId": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateProjectRequestRequestTypeDef",
     {
         "contents": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
+
 class UpdateProjectRequestRequestTypeDef(
     _RequiredUpdateProjectRequestRequestTypeDef, _OptionalUpdateProjectRequestRequestTypeDef
 ):
     pass
 
+
 DescribeBundleResultTypeDef = TypedDict(
     "DescribeBundleResultTypeDef",
     {
         "details": BundleDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportBundleResultTypeDef = TypedDict(
+    "ExportBundleResultTypeDef",
+    {
+        "downloadUrl": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportProjectResultTypeDef = TypedDict(
+    "ExportProjectResultTypeDef",
+    {
+        "downloadUrl": str,
+        "shareUrl": str,
+        "snapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBundlesResultTypeDef = TypedDict(
     "ListBundlesResultTypeDef",
     {
         "bundleList": List[BundleDetailsTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteProjectResultTypeDef = TypedDict(
     "DeleteProjectResultTypeDef",
     {
         "deletedResources": List[ResourceTypeDef],
         "orphanedResources": List[ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProjectDetailsTypeDef = TypedDict(
     "ProjectDetailsTypeDef",
     {
         "name": str,
@@ -287,39 +278,55 @@
         "lastUpdatedDate": datetime,
         "consoleUrl": str,
         "resources": List[ResourceTypeDef],
     },
     total=False,
 )
 
+ListBundlesRequestListBundlesPaginateTypeDef = TypedDict(
+    "ListBundlesRequestListBundlesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProjectsRequestListProjectsPaginateTypeDef = TypedDict(
+    "ListProjectsRequestListProjectsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListProjectsResultTypeDef = TypedDict(
     "ListProjectsResultTypeDef",
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProjectResultTypeDef = TypedDict(
     "CreateProjectResultTypeDef",
     {
         "details": ProjectDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeProjectResultTypeDef = TypedDict(
     "DescribeProjectResultTypeDef",
     {
         "details": ProjectDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateProjectResultTypeDef = TypedDict(
     "UpdateProjectResultTypeDef",
     {
         "details": ProjectDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/PKG-INFO` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mobile
-Version: 1.28.12
-Summary: Type annotations for boto3.Mobile 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Mobile 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mobile.svg?color=blue)](https://pypi.org/project/mypy-boto3-mobile)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mobile)](https://pepy.tech/project/mypy-boto3-mobile)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Mobile 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
+[boto3.Mobile 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mobile.html#Mobile)
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
 [mypy-boto3-mobile docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mobile/).
 
 See how it helps to find and fix potential bugs:
 
@@ -323,34 +323,34 @@
 `mypy_boto3_mobile.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mobile.type_defs import (
     BundleDetailsTypeDef,
     CreateProjectRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DeleteProjectRequestRequestTypeDef,
     ResourceTypeDef,
     DescribeBundleRequestRequestTypeDef,
     DescribeProjectRequestRequestTypeDef,
     ExportBundleRequestRequestTypeDef,
-    ExportBundleResultTypeDef,
     ExportProjectRequestRequestTypeDef,
-    ExportProjectResultTypeDef,
-    ListBundlesRequestListBundlesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBundlesRequestRequestTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsRequestRequestTypeDef,
     ProjectSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateProjectRequestRequestTypeDef,
     DescribeBundleResultTypeDef,
+    ExportBundleResultTypeDef,
+    ExportProjectResultTypeDef,
     ListBundlesResultTypeDef,
     DeleteProjectResultTypeDef,
     ProjectDetailsTypeDef,
+    ListBundlesRequestListBundlesPaginateTypeDef,
+    ListProjectsRequestListProjectsPaginateTypeDef,
     ListProjectsResultTypeDef,
     CreateProjectResultTypeDef,
     DescribeProjectResultTypeDef,
     UpdateProjectResultTypeDef,
 )
```

### Comparing `mypy-boto3-mobile-1.28.12/mypy_boto3_mobile.egg-info/SOURCES.txt` & `mypy-boto3-mobile-1.28.15/mypy_boto3_mobile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mobile-1.28.12/setup.py` & `mypy-boto3-mobile-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mobile",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mobile"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Mobile 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Mobile 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

