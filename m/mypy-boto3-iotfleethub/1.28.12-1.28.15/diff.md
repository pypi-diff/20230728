# Comparing `tmp/mypy-boto3-iotfleethub-1.28.12.tar.gz` & `tmp/mypy-boto3-iotfleethub-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotfleethub-1.28.12.tar", last modified: Thu Jul 27 05:34:49 2023, max compression
+gzip compressed data, was "mypy-boto3-iotfleethub-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
```

## Comparing `mypy-boto3-iotfleethub-1.28.12.tar` & `mypy-boto3-iotfleethub-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-27 05:24:05.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-07-27 05:24:05.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-27 05:24:05.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:49.000000 mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:49.756482 mypy-boto3-iotfleethub-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 05:24:04.000000 mypy-boto3-iotfleethub-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.425256 mypy-boto3-iotfleethub-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:25.000000 mypy-boto3-iotfleethub-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-07-28 20:42:59.425256 mypy-boto3-iotfleethub-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-07-28 20:28:25.000000 mypy-boto3-iotfleethub-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.413256 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-28 20:28:25.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-28 20:28:25.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8347 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8202 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-28 20:28:26.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:25.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.425256 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-07-28 20:42:59.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:42:59.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:59.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:59.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:42:59.000000 mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.425256 mypy-boto3-iotfleethub-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:28:25.000000 mypy-boto3-iotfleethub-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotfleethub-1.28.12/LICENSE` & `mypy-boto3-iotfleethub-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.12/PKG-INFO` & `mypy-boto3-iotfleethub-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleethub
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTFleetHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTFleetHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,28 +321,28 @@
 `mypy_boto3_iotfleethub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotfleethub.type_defs import (
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
-    DescribeApplicationResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
 )
 
 
 def get_structure() -> ApplicationSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotfleethub-1.28.12/README.md` & `mypy-boto3-iotfleethub-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -289,28 +289,28 @@
 `mypy_boto3_iotfleethub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotfleethub.type_defs import (
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
-    DescribeApplicationResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
 )
 
 
 def get_structure() -> ApplicationSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__init__.py` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__init__.pyi` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/__main__.py` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTFleetHub 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTFleetHub 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub\nOther"
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

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/client.py` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/client.pyi` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/literals.py` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/literals.pyi` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/paginator.py` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/paginators/#listapplicationspaginator)
         """
```

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/paginator.pyi` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListApplicationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Paginator.ListApplications)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/paginators/#listapplicationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub.Paginator.ListApplications.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/paginators/#listapplicationspaginator)
         """
```

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/type_defs.py` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,28 +21,28 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
-    "DescribeApplicationResponseTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "DescribeApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
 )
 
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
         "applicationId": str,
         "applicationName": str,
@@ -87,20 +87,22 @@
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationId": str,
-        "applicationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredDeleteApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -124,37 +126,20 @@
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-DescribeApplicationResponseTypeDef = TypedDict(
-    "DescribeApplicationResponseTypeDef",
-    {
-        "applicationId": str,
-        "applicationArn": str,
-        "applicationName": str,
-        "applicationDescription": str,
-        "applicationUrl": str,
-        "applicationState": ApplicationStateType,
-        "applicationCreationDate": int,
-        "applicationLastUpdateDate": int,
-        "roleArn": str,
-        "ssoClientId": str,
-        "errorMessage": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
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
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
@@ -166,43 +151,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -234,15 +190,59 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationResponseTypeDef = TypedDict(
+    "DescribeApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationArn": str,
+        "applicationName": str,
+        "applicationDescription": str,
+        "applicationUrl": str,
+        "applicationState": ApplicationStateType,
+        "applicationCreationDate": int,
+        "applicationLastUpdateDate": int,
+        "roleArn": str,
+        "ssoClientId": str,
+        "errorMessage": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applicationSummaries": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
```

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub/type_defs.pyi` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,28 +20,28 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "CreateApplicationResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteApplicationRequestRequestTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
-    "DescribeApplicationResponseTypeDef",
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
+    "CreateApplicationResponseTypeDef",
+    "DescribeApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
 )
 
 _RequiredApplicationSummaryTypeDef = TypedDict(
     "_RequiredApplicationSummaryTypeDef",
     {
         "applicationId": str,
         "applicationName": str,
@@ -82,20 +82,22 @@
 )
 
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-CreateApplicationResponseTypeDef = TypedDict(
-    "CreateApplicationResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "applicationId": str,
-        "applicationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredDeleteApplicationRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
@@ -117,37 +119,20 @@
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "applicationId": str,
     },
 )
 
-DescribeApplicationResponseTypeDef = TypedDict(
-    "DescribeApplicationResponseTypeDef",
-    {
-        "applicationId": str,
-        "applicationArn": str,
-        "applicationName": str,
-        "applicationDescription": str,
-        "applicationUrl": str,
-        "applicationState": ApplicationStateType,
-        "applicationCreationDate": int,
-        "applicationLastUpdateDate": int,
-        "roleArn": str,
-        "ssoClientId": str,
-        "errorMessage": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
-    "ListApplicationsRequestListApplicationsPaginateTypeDef",
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
 
 ListApplicationsRequestRequestTypeDef = TypedDict(
     "ListApplicationsRequestRequestTypeDef",
     {
@@ -159,43 +144,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -225,15 +181,59 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
+CreateApplicationResponseTypeDef = TypedDict(
+    "CreateApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeApplicationResponseTypeDef = TypedDict(
+    "DescribeApplicationResponseTypeDef",
+    {
+        "applicationId": str,
+        "applicationArn": str,
+        "applicationName": str,
+        "applicationDescription": str,
+        "applicationUrl": str,
+        "applicationState": ApplicationStateType,
+        "applicationCreationDate": int,
+        "applicationLastUpdateDate": int,
+        "roleArn": str,
+        "ssoClientId": str,
+        "errorMessage": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "applicationSummaries": List[ApplicationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationsRequestListApplicationsPaginateTypeDef = TypedDict(
+    "ListApplicationsRequestListApplicationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
```

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/PKG-INFO` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotfleethub
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTFleetHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTFleetHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotfleethub.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotfleethub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotfleethub)](https://pepy.tech/project/mypy-boto3-iotfleethub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTFleetHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
+[boto3.IoTFleetHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotfleethub.html#IoTFleetHub)
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
 [mypy-boto3-iotfleethub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotfleethub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -321,28 +321,28 @@
 `mypy_boto3_iotfleethub.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotfleethub.type_defs import (
     ApplicationSummaryTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationRequestRequestTypeDef,
     DescribeApplicationRequestRequestTypeDef,
-    DescribeApplicationResponseTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApplicationRequestRequestTypeDef,
+    CreateApplicationResponseTypeDef,
+    DescribeApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListApplicationsRequestListApplicationsPaginateTypeDef,
 )
 
 
 def get_structure() -> ApplicationSummaryTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iotfleethub-1.28.12/mypy_boto3_iotfleethub.egg-info/SOURCES.txt` & `mypy-boto3-iotfleethub-1.28.15/mypy_boto3_iotfleethub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotfleethub-1.28.12/setup.py` & `mypy-boto3-iotfleethub-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotfleethub",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotfleethub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTFleetHub 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.IoTFleetHub 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

