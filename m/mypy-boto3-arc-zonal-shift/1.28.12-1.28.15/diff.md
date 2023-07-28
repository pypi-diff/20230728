# Comparing `tmp/mypy-boto3-arc-zonal-shift-1.28.12.tar.gz` & `tmp/mypy-boto3-arc-zonal-shift-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-arc-zonal-shift-1.28.12.tar", last modified: Thu Jul 27 05:34:20 2023, max compression
+gzip compressed data, was "mypy-boto3-arc-zonal-shift-1.28.15.tar", last modified: Fri Jul 28 20:42:19 2023, max compression
```

## Comparing `mypy-boto3-arc-zonal-shift-1.28.12.tar` & `mypy-boto3-arc-zonal-shift-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.588572 mypy-boto3-arc-zonal-shift-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-27 05:34:20.584572 mypy-boto3-arc-zonal-shift-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:20.584572 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:20.000000 mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:20.588572 mypy-boto3-arc-zonal-shift-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-27 05:17:40.000000 mypy-boto3-arc-zonal-shift-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.240695 mypy-boto3-arc-zonal-shift-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-28 20:42:19.232695 mypy-boto3-arc-zonal-shift-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.228695 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8532 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8662 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5848 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:19.232695 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13836 2023-07-28 20:42:18.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:42:19.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:18.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:18.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:18.000000 mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:19.240695 mypy-boto3-arc-zonal-shift-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-28 20:19:45.000000 mypy-boto3-arc-zonal-shift-1.28.15/setup.py
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/LICENSE` & `mypy-boto3-arc-zonal-shift-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/PKG-INFO` & `mypy-boto3-arc-zonal-shift-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-arc-zonal-shift
-Version: 1.28.12
-Summary: Type annotations for boto3.ARCZonalShift 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ARCZonalShift 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,27 +331,27 @@
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/README.md` & `mypy-boto3-arc-zonal-shift-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,27 +299,27 @@
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__init__.py` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__init__.pyi` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/__main__.py` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ARCZonalShift 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ARCZonalShift 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift\nOther"
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

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/client.py` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/client.pyi` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/literals.py` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/literals.pyi` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/paginator.py` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,31 +48,28 @@
 class ListManagedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
         """
 
 
 class ListZonalShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listzonalshiftspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        status: ZonalShiftStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: ZonalShiftStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListZonalShiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listzonalshiftspaginator)
         """
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/paginator.pyi` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -45,30 +45,27 @@
 class ListManagedResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListManagedResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listmanagedresourcespaginator)
         """
 
 class ListZonalShiftsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listzonalshiftspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        status: ZonalShiftStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: ZonalShiftStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListZonalShiftsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift.Paginator.ListZonalShifts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/paginators/#listzonalshiftspaginator)
         """
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/type_defs.py` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,30 @@
 from .literals import AppliedStatusType, ZonalShiftStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelZonalShiftRequestRequestTypeDef",
     "GetManagedResourceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ZonalShiftInResourceTypeDef",
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListManagedResourcesRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListZonalShiftsRequestRequestTypeDef",
     "ZonalShiftSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartZonalShiftRequestRequestTypeDef",
     "UpdateZonalShiftRequestRequestTypeDef",
     "ZonalShiftTypeDef",
     "GetManagedResourceResponseTypeDef",
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListManagedResourcesResponseTypeDef",
     "ListZonalShiftsResponseTypeDef",
 )
 
 CancelZonalShiftRequestRequestTypeDef = TypedDict(
     "CancelZonalShiftRequestRequestTypeDef",
     {
@@ -53,31 +52,44 @@
 GetManagedResourceRequestRequestTypeDef = TypedDict(
     "GetManagedResourceRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
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
 ZonalShiftInResourceTypeDef = TypedDict(
     "ZonalShiftInResourceTypeDef",
     {
         "appliedStatus": AppliedStatusType,
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "zonalShiftId": str,
     },
 )
 
-ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
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
 
 ListManagedResourcesRequestRequestTypeDef = TypedDict(
     "ListManagedResourcesRequestRequestTypeDef",
     {
@@ -98,30 +110,19 @@
     {
         "arn": str,
         "name": str,
     },
     total=False,
 )
 
-
 class ManagedResourceSummaryTypeDef(
     _RequiredManagedResourceSummaryTypeDef, _OptionalManagedResourceSummaryTypeDef
 ):
     pass
 
-
-ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
-    {
-        "status": ZonalShiftStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListZonalShiftsRequestRequestTypeDef = TypedDict(
     "ListZonalShiftsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "status": ZonalShiftStatusType,
     },
@@ -137,35 +138,14 @@
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
     },
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
 StartZonalShiftRequestRequestTypeDef = TypedDict(
     "StartZonalShiftRequestRequestTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiresIn": str,
         "resourceIdentifier": str,
@@ -183,56 +163,71 @@
     {
         "comment": str,
         "expiresIn": str,
     },
     total=False,
 )
 
-
 class UpdateZonalShiftRequestRequestTypeDef(
     _RequiredUpdateZonalShiftRequestRequestTypeDef, _OptionalUpdateZonalShiftRequestRequestTypeDef
 ):
     pass
 
-
 ZonalShiftTypeDef = TypedDict(
     "ZonalShiftTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetManagedResourceResponseTypeDef = TypedDict(
     "GetManagedResourceResponseTypeDef",
     {
         "appliedWeights": Dict[str, float],
         "arn": str,
         "name": str,
         "zonalShifts": List[ZonalShiftInResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
+    {
+        "status": ZonalShiftStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListManagedResourcesResponseTypeDef = TypedDict(
     "ListManagedResourcesResponseTypeDef",
     {
         "items": List[ManagedResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListZonalShiftsResponseTypeDef = TypedDict(
     "ListZonalShiftsResponseTypeDef",
     {
         "items": List[ZonalShiftSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift/type_defs.pyi` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,30 +18,31 @@
 from .literals import AppliedStatusType, ZonalShiftStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelZonalShiftRequestRequestTypeDef",
     "GetManagedResourceRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ZonalShiftInResourceTypeDef",
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListManagedResourcesRequestRequestTypeDef",
     "ManagedResourceSummaryTypeDef",
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListZonalShiftsRequestRequestTypeDef",
     "ZonalShiftSummaryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartZonalShiftRequestRequestTypeDef",
     "UpdateZonalShiftRequestRequestTypeDef",
     "ZonalShiftTypeDef",
     "GetManagedResourceResponseTypeDef",
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
     "ListManagedResourcesResponseTypeDef",
     "ListZonalShiftsResponseTypeDef",
 )
 
 CancelZonalShiftRequestRequestTypeDef = TypedDict(
     "CancelZonalShiftRequestRequestTypeDef",
     {
@@ -52,31 +53,44 @@
 GetManagedResourceRequestRequestTypeDef = TypedDict(
     "GetManagedResourceRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
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
 ZonalShiftInResourceTypeDef = TypedDict(
     "ZonalShiftInResourceTypeDef",
     {
         "appliedStatus": AppliedStatusType,
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "zonalShiftId": str,
     },
 )
 
-ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
-    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
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
 
 ListManagedResourcesRequestRequestTypeDef = TypedDict(
     "ListManagedResourcesRequestRequestTypeDef",
     {
@@ -97,27 +111,20 @@
     {
         "arn": str,
         "name": str,
     },
     total=False,
 )
 
+
 class ManagedResourceSummaryTypeDef(
     _RequiredManagedResourceSummaryTypeDef, _OptionalManagedResourceSummaryTypeDef
 ):
     pass
 
-ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
-    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
-    {
-        "status": ZonalShiftStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListZonalShiftsRequestRequestTypeDef = TypedDict(
     "ListZonalShiftsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "status": ZonalShiftStatusType,
@@ -134,35 +141,14 @@
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
     },
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
 StartZonalShiftRequestRequestTypeDef = TypedDict(
     "StartZonalShiftRequestRequestTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiresIn": str,
         "resourceIdentifier": str,
@@ -180,54 +166,73 @@
     {
         "comment": str,
         "expiresIn": str,
     },
     total=False,
 )
 
+
 class UpdateZonalShiftRequestRequestTypeDef(
     _RequiredUpdateZonalShiftRequestRequestTypeDef, _OptionalUpdateZonalShiftRequestRequestTypeDef
 ):
     pass
 
+
 ZonalShiftTypeDef = TypedDict(
     "ZonalShiftTypeDef",
     {
         "awayFrom": str,
         "comment": str,
         "expiryTime": datetime,
         "resourceIdentifier": str,
         "startTime": datetime,
         "status": ZonalShiftStatusType,
         "zonalShiftId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetManagedResourceResponseTypeDef = TypedDict(
     "GetManagedResourceResponseTypeDef",
     {
         "appliedWeights": Dict[str, float],
         "arn": str,
         "name": str,
         "zonalShifts": List[ZonalShiftInResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListManagedResourcesRequestListManagedResourcesPaginateTypeDef = TypedDict(
+    "ListManagedResourcesRequestListManagedResourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListZonalShiftsRequestListZonalShiftsPaginateTypeDef = TypedDict(
+    "ListZonalShiftsRequestListZonalShiftsPaginateTypeDef",
+    {
+        "status": ZonalShiftStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListManagedResourcesResponseTypeDef = TypedDict(
     "ListManagedResourcesResponseTypeDef",
     {
         "items": List[ManagedResourceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListZonalShiftsResponseTypeDef = TypedDict(
     "ListZonalShiftsResponseTypeDef",
     {
         "items": List[ZonalShiftSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-arc-zonal-shift
-Version: 1.28.12
-Summary: Type annotations for boto3.ARCZonalShift 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ARCZonalShift 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-arc-zonal-shift.svg?color=blue)](https://pypi.org/project/mypy-boto3-arc-zonal-shift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-arc-zonal-shift)](https://pepy.tech/project/mypy-boto3-arc-zonal-shift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ARCZonalShift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
+[boto3.ARCZonalShift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/arc-zonal-shift.html#ARCZonalShift)
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
 [mypy-boto3-arc-zonal-shift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_arc_zonal_shift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -331,27 +331,27 @@
 `mypy_boto3_arc_zonal_shift.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_arc_zonal_shift.type_defs import (
     CancelZonalShiftRequestRequestTypeDef,
     GetManagedResourceRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ZonalShiftInResourceTypeDef,
-    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListManagedResourcesRequestRequestTypeDef,
     ManagedResourceSummaryTypeDef,
-    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListZonalShiftsRequestRequestTypeDef,
     ZonalShiftSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartZonalShiftRequestRequestTypeDef,
     UpdateZonalShiftRequestRequestTypeDef,
     ZonalShiftTypeDef,
     GetManagedResourceResponseTypeDef,
+    ListManagedResourcesRequestListManagedResourcesPaginateTypeDef,
+    ListZonalShiftsRequestListZonalShiftsPaginateTypeDef,
     ListManagedResourcesResponseTypeDef,
     ListZonalShiftsResponseTypeDef,
 )
 
 
 def get_structure() -> CancelZonalShiftRequestRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt` & `mypy-boto3-arc-zonal-shift-1.28.15/mypy_boto3_arc_zonal_shift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-arc-zonal-shift-1.28.12/setup.py` & `mypy-boto3-arc-zonal-shift-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-arc-zonal-shift",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_arc_zonal_shift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ARCZonalShift 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ARCZonalShift 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

