# Comparing `tmp/mypy-boto3-mediastore-data-1.28.12.tar.gz` & `tmp/mypy-boto3-mediastore-data-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediastore-data-1.28.12.tar", last modified: Thu Jul 27 05:35:01 2023, max compression
+gzip compressed data, was "mypy-boto3-mediastore-data-1.28.15.tar", last modified: Fri Jul 28 20:43:17 2023, max compression
```

## Comparing `mypy-boto3-mediastore-data-1.28.12.tar` & `mypy-boto3-mediastore-data-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.800438 mypy-boto3-mediastore-data-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-27 05:35:01.792438 mypy-boto3-mediastore-data-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.792438 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-07-27 05:26:26.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:01.792438 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:01.800438 mypy-boto3-mediastore-data-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-data-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.237501 mypy-boto3-mediastore-data-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-28 20:43:17.229501 mypy-boto3-mediastore-data-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.229501 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6708 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6695 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.229501 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13374 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:17.237501 mypy-boto3-mediastore-data-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-07-28 20:31:42.000000 mypy-boto3-mediastore-data-1.28.15/setup.py
```

### Comparing `mypy-boto3-mediastore-data-1.28.12/LICENSE` & `mypy-boto3-mediastore-data-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.12/PKG-INFO` & `mypy-boto3-mediastore-data-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore-data
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaStoreData 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaStoreData 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,25 +325,25 @@
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
-    DescribeObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetObjectRequestRequestTypeDef,
-    GetObjectResponseTypeDef,
     ItemTypeDef,
-    ListItemsRequestListItemsPaginateTypeDef,
-    ListItemsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListItemsRequestRequestTypeDef,
     PutObjectRequestRequestTypeDef,
+    DescribeObjectResponseTypeDef,
+    GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     ListItemsResponseTypeDef,
+    ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteObjectRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediastore-data-1.28.12/README.md` & `mypy-boto3-mediastore-data-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,25 +293,25 @@
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
-    DescribeObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetObjectRequestRequestTypeDef,
-    GetObjectResponseTypeDef,
     ItemTypeDef,
-    ListItemsRequestListItemsPaginateTypeDef,
-    ListItemsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListItemsRequestRequestTypeDef,
     PutObjectRequestRequestTypeDef,
+    DescribeObjectResponseTypeDef,
+    GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     ListItemsResponseTypeDef,
+    ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteObjectRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__init__.py` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__init__.pyi` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/__main__.py` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaStoreData 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MediaStoreData 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData\nOther"
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

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/client.py` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/client.pyi` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/literals.py` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/literals.pyi` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/paginator.py` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/paginators/#listitemspaginator)
     """
 
     def paginate(
-        self, *, Path: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Path: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/paginators/#listitemspaginator)
         """
```

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/paginator.pyi` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListItemsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/paginators/#listitemspaginator)
     """
 
     def paginate(
-        self, *, Path: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Path: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData.Paginator.ListItems.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/paginators/#listitemspaginator)
         """
```

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/type_defs.py` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,25 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteObjectRequestRequestTypeDef",
     "DescribeObjectRequestRequestTypeDef",
-    "DescribeObjectResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetObjectRequestRequestTypeDef",
-    "GetObjectResponseTypeDef",
     "ItemTypeDef",
-    "ListItemsRequestListItemsPaginateTypeDef",
-    "ListItemsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "ListItemsRequestRequestTypeDef",
     "PutObjectRequestRequestTypeDef",
+    "DescribeObjectResponseTypeDef",
+    "GetObjectResponseTypeDef",
     "PutObjectResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "ListItemsResponseTypeDef",
+    "ListItemsRequestListItemsPaginateTypeDef",
 )
 
 DeleteObjectRequestRequestTypeDef = TypedDict(
     "DeleteObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
@@ -55,23 +55,22 @@
 DescribeObjectRequestRequestTypeDef = TypedDict(
     "DescribeObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 
-DescribeObjectResponseTypeDef = TypedDict(
-    "DescribeObjectResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ETag": str,
-        "ContentType": str,
-        "ContentLength": int,
-        "CacheControl": str,
-        "LastModified": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredGetObjectRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectRequestRequestTypeDef",
     {
         "Path": str,
@@ -88,71 +87,47 @@
 
 class GetObjectRequestRequestTypeDef(
     _RequiredGetObjectRequestRequestTypeDef, _OptionalGetObjectRequestRequestTypeDef
 ):
     pass
 
 
-GetObjectResponseTypeDef = TypedDict(
-    "GetObjectResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "CacheControl": str,
-        "ContentRange": str,
-        "ContentLength": int,
-        "ContentType": str,
-        "ETag": str,
-        "LastModified": datetime,
-        "StatusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "Name": str,
         "Type": ItemTypeType,
         "ETag": str,
         "LastModified": datetime,
         "ContentType": str,
         "ContentLength": int,
     },
     total=False,
 )
 
-ListItemsRequestListItemsPaginateTypeDef = TypedDict(
-    "ListItemsRequestListItemsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Path": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListItemsRequestRequestTypeDef = TypedDict(
     "ListItemsRequestRequestTypeDef",
     {
         "Path": str,
         "MaxResults": int,
         "NextToken": str,
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
 _RequiredPutObjectRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectRequestRequestTypeDef",
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "Path": str,
     },
 )
@@ -170,36 +145,61 @@
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
 
-PutObjectResponseTypeDef = TypedDict(
-    "PutObjectResponseTypeDef",
+DescribeObjectResponseTypeDef = TypedDict(
+    "DescribeObjectResponseTypeDef",
     {
-        "ContentSHA256": str,
         "ETag": str,
-        "StorageClass": Literal["TEMPORAL"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ContentType": str,
+        "ContentLength": int,
+        "CacheControl": str,
+        "LastModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetObjectResponseTypeDef = TypedDict(
+    "GetObjectResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Body": StreamingBody,
+        "CacheControl": str,
+        "ContentRange": str,
+        "ContentLength": int,
+        "ContentType": str,
+        "ETag": str,
+        "LastModified": datetime,
+        "StatusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectResponseTypeDef = TypedDict(
+    "PutObjectResponseTypeDef",
+    {
+        "ContentSHA256": str,
+        "ETag": str,
+        "StorageClass": Literal["TEMPORAL"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListItemsResponseTypeDef = TypedDict(
     "ListItemsResponseTypeDef",
     {
         "Items": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListItemsRequestListItemsPaginateTypeDef = TypedDict(
+    "ListItemsRequestListItemsPaginateTypeDef",
+    {
+        "Path": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
```

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data/type_defs.pyi` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -27,25 +27,25 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteObjectRequestRequestTypeDef",
     "DescribeObjectRequestRequestTypeDef",
-    "DescribeObjectResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "GetObjectRequestRequestTypeDef",
-    "GetObjectResponseTypeDef",
     "ItemTypeDef",
-    "ListItemsRequestListItemsPaginateTypeDef",
-    "ListItemsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "ListItemsRequestRequestTypeDef",
     "PutObjectRequestRequestTypeDef",
+    "DescribeObjectResponseTypeDef",
+    "GetObjectResponseTypeDef",
     "PutObjectResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "ListItemsResponseTypeDef",
+    "ListItemsRequestListItemsPaginateTypeDef",
 )
 
 DeleteObjectRequestRequestTypeDef = TypedDict(
     "DeleteObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
@@ -54,23 +54,22 @@
 DescribeObjectRequestRequestTypeDef = TypedDict(
     "DescribeObjectRequestRequestTypeDef",
     {
         "Path": str,
     },
 )
 
-DescribeObjectResponseTypeDef = TypedDict(
-    "DescribeObjectResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ETag": str,
-        "ContentType": str,
-        "ContentLength": int,
-        "CacheControl": str,
-        "LastModified": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredGetObjectRequestRequestTypeDef = TypedDict(
     "_RequiredGetObjectRequestRequestTypeDef",
     {
         "Path": str,
@@ -85,71 +84,47 @@
 )
 
 class GetObjectRequestRequestTypeDef(
     _RequiredGetObjectRequestRequestTypeDef, _OptionalGetObjectRequestRequestTypeDef
 ):
     pass
 
-GetObjectResponseTypeDef = TypedDict(
-    "GetObjectResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "CacheControl": str,
-        "ContentRange": str,
-        "ContentLength": int,
-        "ContentType": str,
-        "ETag": str,
-        "LastModified": datetime,
-        "StatusCode": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "Name": str,
         "Type": ItemTypeType,
         "ETag": str,
         "LastModified": datetime,
         "ContentType": str,
         "ContentLength": int,
     },
     total=False,
 )
 
-ListItemsRequestListItemsPaginateTypeDef = TypedDict(
-    "ListItemsRequestListItemsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Path": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListItemsRequestRequestTypeDef = TypedDict(
     "ListItemsRequestRequestTypeDef",
     {
         "Path": str,
         "MaxResults": int,
         "NextToken": str,
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
 _RequiredPutObjectRequestRequestTypeDef = TypedDict(
     "_RequiredPutObjectRequestRequestTypeDef",
     {
         "Body": Union[str, bytes, IO[Any], StreamingBody],
         "Path": str,
     },
 )
@@ -165,36 +140,61 @@
 )
 
 class PutObjectRequestRequestTypeDef(
     _RequiredPutObjectRequestRequestTypeDef, _OptionalPutObjectRequestRequestTypeDef
 ):
     pass
 
-PutObjectResponseTypeDef = TypedDict(
-    "PutObjectResponseTypeDef",
+DescribeObjectResponseTypeDef = TypedDict(
+    "DescribeObjectResponseTypeDef",
     {
-        "ContentSHA256": str,
         "ETag": str,
-        "StorageClass": Literal["TEMPORAL"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ContentType": str,
+        "ContentLength": int,
+        "CacheControl": str,
+        "LastModified": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetObjectResponseTypeDef = TypedDict(
+    "GetObjectResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Body": StreamingBody,
+        "CacheControl": str,
+        "ContentRange": str,
+        "ContentLength": int,
+        "ContentType": str,
+        "ETag": str,
+        "LastModified": datetime,
+        "StatusCode": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectResponseTypeDef = TypedDict(
+    "PutObjectResponseTypeDef",
+    {
+        "ContentSHA256": str,
+        "ETag": str,
+        "StorageClass": Literal["TEMPORAL"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListItemsResponseTypeDef = TypedDict(
     "ListItemsResponseTypeDef",
     {
         "Items": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListItemsRequestListItemsPaginateTypeDef = TypedDict(
+    "ListItemsRequestListItemsPaginateTypeDef",
+    {
+        "Path": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
```

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/PKG-INFO` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore-data
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaStoreData 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaStoreData 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore-data.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore-data)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore-data)](https://pepy.tech/project/mypy-boto3-mediastore-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStoreData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
+[boto3.MediaStoreData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore-data.html#MediaStoreData)
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
 [mypy-boto3-mediastore-data docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,25 +325,25 @@
 `mypy_boto3_mediastore_data.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mediastore_data.type_defs import (
     DeleteObjectRequestRequestTypeDef,
     DescribeObjectRequestRequestTypeDef,
-    DescribeObjectResponseTypeDef,
+    ResponseMetadataTypeDef,
     GetObjectRequestRequestTypeDef,
-    GetObjectResponseTypeDef,
     ItemTypeDef,
-    ListItemsRequestListItemsPaginateTypeDef,
-    ListItemsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListItemsRequestRequestTypeDef,
     PutObjectRequestRequestTypeDef,
+    DescribeObjectResponseTypeDef,
+    GetObjectResponseTypeDef,
     PutObjectResponseTypeDef,
-    ResponseMetadataTypeDef,
     ListItemsResponseTypeDef,
+    ListItemsRequestListItemsPaginateTypeDef,
 )
 
 
 def get_structure() -> DeleteObjectRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mediastore-data-1.28.12/mypy_boto3_mediastore_data.egg-info/SOURCES.txt` & `mypy-boto3-mediastore-data-1.28.15/mypy_boto3_mediastore_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-data-1.28.12/setup.py` & `mypy-boto3-mediastore-data-1.28.15/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediastore-data",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mediastore_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaStoreData 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MediaStoreData 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

