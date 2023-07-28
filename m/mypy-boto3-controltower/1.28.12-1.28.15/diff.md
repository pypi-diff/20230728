# Comparing `tmp/mypy-boto3-controltower-1.28.12.tar.gz` & `tmp/mypy-boto3-controltower-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-controltower-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
+gzip compressed data, was "mypy-boto3-controltower-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
```

## Comparing `mypy-boto3-controltower-1.28.12.tar` & `mypy-boto3-controltower-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.836542 mypy-boto3-controltower-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-27 05:34:31.832542 mypy-boto3-controltower-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.832542 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-27 05:19:51.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4469 2023-07-27 05:19:51.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-27 05:19:51.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:50.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.832542 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-27 05:34:31.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-27 05:34:31.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:31.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:31.000000 mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.836542 mypy-boto3-controltower-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-27 05:19:49.000000 mypy-boto3-controltower-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.724913 mypy-boto3-controltower-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-28 20:42:34.712913 mypy-boto3-controltower-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.708913 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.712913 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-28 20:42:34.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-28 20:42:34.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:34.000000 mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.724913 mypy-boto3-controltower-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-28 20:22:22.000000 mypy-boto3-controltower-1.28.15/setup.py
```

### Comparing `mypy-boto3-controltower-1.28.12/LICENSE` & `mypy-boto3-controltower-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-controltower-1.28.12/PKG-INFO` & `mypy-boto3-controltower-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-controltower
-Version: 1.28.12
-Summary: Type annotations for boto3.ControlTower 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ControlTower 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-controltower.svg?color=blue)](https://pypi.org/project/mypy-boto3-controltower)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-controltower)](https://pepy.tech/project/mypy-boto3-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ControlTower 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[boto3.ControlTower 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [mypy-boto3-controltower docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,25 +325,25 @@
 `mypy_boto3_controltower.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_controltower.type_defs import (
     ControlOperationTypeDef,
     DisableControlInputRequestTypeDef,
-    DisableControlOutputTypeDef,
+    ResponseMetadataTypeDef,
     EnableControlInputRequestTypeDef,
-    EnableControlOutputTypeDef,
     EnabledControlSummaryTypeDef,
     GetControlOperationInputRequestTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListEnabledControlsInputRequestTypeDef,
+    DisableControlOutputTypeDef,
+    EnableControlOutputTypeDef,
     GetControlOperationOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
+    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
 )
 
 
 def get_structure() -> ControlOperationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-controltower-1.28.12/README.md` & `mypy-boto3-controltower-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-controltower.svg?color=blue)](https://pypi.org/project/mypy-boto3-controltower)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-controltower)](https://pepy.tech/project/mypy-boto3-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ControlTower 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[boto3.ControlTower 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [mypy-boto3-controltower docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,25 +293,25 @@
 `mypy_boto3_controltower.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_controltower.type_defs import (
     ControlOperationTypeDef,
     DisableControlInputRequestTypeDef,
-    DisableControlOutputTypeDef,
+    ResponseMetadataTypeDef,
     EnableControlInputRequestTypeDef,
-    EnableControlOutputTypeDef,
     EnabledControlSummaryTypeDef,
     GetControlOperationInputRequestTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListEnabledControlsInputRequestTypeDef,
+    DisableControlOutputTypeDef,
+    EnableControlOutputTypeDef,
     GetControlOperationOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
+    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
 )
 
 
 def get_structure() -> ControlOperationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/__init__.py` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/__init__.pyi` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/__main__.py` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ControlTower 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ControlTower 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower\nOther"
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

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/client.py` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/client.pyi` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/literals.py` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/literals.pyi` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/paginator.py` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,31 +23,28 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEnabledControlsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEnabledControlsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListEnabledControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledcontrolspaginator)
     """
 
     def paginate(
-        self, *, targetIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, targetIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnabledControlsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledcontrolspaginator)
         """
```

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/paginator.pyi` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,28 +23,31 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListEnabledControlsOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListEnabledControlsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListEnabledControlsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledcontrolspaginator)
     """
 
     def paginate(
-        self, *, targetIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, targetIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnabledControlsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/paginators/#listenabledcontrolspaginator)
         """
```

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/type_defs.py` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,25 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ControlOperationTypeDef",
     "DisableControlInputRequestTypeDef",
-    "DisableControlOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EnableControlInputRequestTypeDef",
-    "EnableControlOutputTypeDef",
     "EnabledControlSummaryTypeDef",
     "GetControlOperationInputRequestTypeDef",
-    "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
-    "ListEnabledControlsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListEnabledControlsInputRequestTypeDef",
+    "DisableControlOutputTypeDef",
+    "EnableControlOutputTypeDef",
     "GetControlOperationOutputTypeDef",
     "ListEnabledControlsOutputTypeDef",
+    "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
 )
 
 ControlOperationTypeDef = TypedDict(
     "ControlOperationTypeDef",
     {
         "endTime": datetime,
         "operationType": ControlOperationTypeType,
@@ -55,38 +55,33 @@
     "DisableControlInputRequestTypeDef",
     {
         "controlIdentifier": str,
         "targetIdentifier": str,
     },
 )
 
-DisableControlOutputTypeDef = TypedDict(
-    "DisableControlOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "operationIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 EnableControlInputRequestTypeDef = TypedDict(
     "EnableControlInputRequestTypeDef",
     {
         "controlIdentifier": str,
         "targetIdentifier": str,
     },
 )
 
-EnableControlOutputTypeDef = TypedDict(
-    "EnableControlOutputTypeDef",
-    {
-        "operationIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnabledControlSummaryTypeDef = TypedDict(
     "EnabledControlSummaryTypeDef",
     {
         "controlIdentifier": str,
     },
     total=False,
 )
@@ -94,36 +89,24 @@
 GetControlOperationInputRequestTypeDef = TypedDict(
     "GetControlOperationInputRequestTypeDef",
     {
         "operationIdentifier": str,
     },
 )
 
-_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
-    "_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef",
-    {
-        "targetIdentifier": str,
-    },
-)
-_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
-    "_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef",
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
-class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(
-    _RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    _OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEnabledControlsInputRequestTypeDef = TypedDict(
     "_RequiredListEnabledControlsInputRequestTypeDef",
     {
         "targetIdentifier": str,
     },
 )
 _OptionalListEnabledControlsInputRequestTypeDef = TypedDict(
@@ -138,44 +121,60 @@
 
 class ListEnabledControlsInputRequestTypeDef(
     _RequiredListEnabledControlsInputRequestTypeDef, _OptionalListEnabledControlsInputRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DisableControlOutputTypeDef = TypedDict(
+    "DisableControlOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "operationIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EnableControlOutputTypeDef = TypedDict(
+    "EnableControlOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "operationIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetControlOperationOutputTypeDef = TypedDict(
     "GetControlOperationOutputTypeDef",
     {
         "controlOperation": ControlOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnabledControlsOutputTypeDef = TypedDict(
     "ListEnabledControlsOutputTypeDef",
     {
         "enabledControls": List[EnabledControlSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
+    "_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef",
+    {
+        "targetIdentifier": str,
+    },
+)
+_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
+    "_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(
+    _RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef,
+    _OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower/type_defs.pyi` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,25 +21,25 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ControlOperationTypeDef",
     "DisableControlInputRequestTypeDef",
-    "DisableControlOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EnableControlInputRequestTypeDef",
-    "EnableControlOutputTypeDef",
     "EnabledControlSummaryTypeDef",
     "GetControlOperationInputRequestTypeDef",
-    "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
-    "ListEnabledControlsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListEnabledControlsInputRequestTypeDef",
+    "DisableControlOutputTypeDef",
+    "EnableControlOutputTypeDef",
     "GetControlOperationOutputTypeDef",
     "ListEnabledControlsOutputTypeDef",
+    "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
 )
 
 ControlOperationTypeDef = TypedDict(
     "ControlOperationTypeDef",
     {
         "endTime": datetime,
         "operationType": ControlOperationTypeType,
@@ -54,38 +54,33 @@
     "DisableControlInputRequestTypeDef",
     {
         "controlIdentifier": str,
         "targetIdentifier": str,
     },
 )
 
-DisableControlOutputTypeDef = TypedDict(
-    "DisableControlOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "operationIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 EnableControlInputRequestTypeDef = TypedDict(
     "EnableControlInputRequestTypeDef",
     {
         "controlIdentifier": str,
         "targetIdentifier": str,
     },
 )
 
-EnableControlOutputTypeDef = TypedDict(
-    "EnableControlOutputTypeDef",
-    {
-        "operationIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnabledControlSummaryTypeDef = TypedDict(
     "EnabledControlSummaryTypeDef",
     {
         "controlIdentifier": str,
     },
     total=False,
 )
@@ -93,34 +88,24 @@
 GetControlOperationInputRequestTypeDef = TypedDict(
     "GetControlOperationInputRequestTypeDef",
     {
         "operationIdentifier": str,
     },
 )
 
-_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
-    "_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef",
-    {
-        "targetIdentifier": str,
-    },
-)
-_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
-    "_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef",
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
 
-class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(
-    _RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    _OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEnabledControlsInputRequestTypeDef = TypedDict(
     "_RequiredListEnabledControlsInputRequestTypeDef",
     {
         "targetIdentifier": str,
     },
 )
 _OptionalListEnabledControlsInputRequestTypeDef = TypedDict(
@@ -133,44 +118,59 @@
 )
 
 class ListEnabledControlsInputRequestTypeDef(
     _RequiredListEnabledControlsInputRequestTypeDef, _OptionalListEnabledControlsInputRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DisableControlOutputTypeDef = TypedDict(
+    "DisableControlOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "operationIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EnableControlOutputTypeDef = TypedDict(
+    "EnableControlOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "operationIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetControlOperationOutputTypeDef = TypedDict(
     "GetControlOperationOutputTypeDef",
     {
         "controlOperation": ControlOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnabledControlsOutputTypeDef = TypedDict(
     "ListEnabledControlsOutputTypeDef",
     {
         "enabledControls": List[EnabledControlSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
+    "_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef",
+    {
+        "targetIdentifier": str,
+    },
+)
+_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
+    "_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(
+    _RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef,
+    _OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef,
+):
+    pass
```

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/PKG-INFO` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-controltower
-Version: 1.28.12
-Summary: Type annotations for boto3.ControlTower 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ControlTower 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-controltower.svg?color=blue)](https://pypi.org/project/mypy-boto3-controltower)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-controltower)](https://pepy.tech/project/mypy-boto3-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ControlTower 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
+[boto3.ControlTower 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [mypy-boto3-controltower docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_controltower/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,25 +325,25 @@
 `mypy_boto3_controltower.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_controltower.type_defs import (
     ControlOperationTypeDef,
     DisableControlInputRequestTypeDef,
-    DisableControlOutputTypeDef,
+    ResponseMetadataTypeDef,
     EnableControlInputRequestTypeDef,
-    EnableControlOutputTypeDef,
     EnabledControlSummaryTypeDef,
     GetControlOperationInputRequestTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListEnabledControlsInputRequestTypeDef,
+    DisableControlOutputTypeDef,
+    EnableControlOutputTypeDef,
     GetControlOperationOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
+    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
 )
 
 
 def get_structure() -> ControlOperationTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-controltower-1.28.12/mypy_boto3_controltower.egg-info/SOURCES.txt` & `mypy-boto3-controltower-1.28.15/mypy_boto3_controltower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-controltower-1.28.12/setup.py` & `mypy-boto3-controltower-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-controltower",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_controltower"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ControlTower 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ControlTower 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

