# Comparing `tmp/mypy-boto3-cloudcontrol-1.28.12.tar.gz` & `tmp/mypy-boto3-cloudcontrol-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloudcontrol-1.28.12.tar", last modified: Thu Jul 27 05:34:24 2023, max compression
+gzip compressed data, was "mypy-boto3-cloudcontrol-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-cloudcontrol-1.28.12.tar` & `mypy-boto3-cloudcontrol-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.956563 mypy-boto3-cloudcontrol-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-27 05:34:24.952563 mypy-boto3-cloudcontrol-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.952563 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9706 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-27 05:18:26.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.952563 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:24.000000 mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:24.956563 mypy-boto3-cloudcontrol-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-27 05:18:25.000000 mypy-boto3-cloudcontrol-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.400781 mypy-boto3-cloudcontrol-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-28 20:42:25.392780 mypy-boto3-cloudcontrol-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13222 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.384780 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10839 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9292 2023-07-28 20:20:51.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9290 2023-07-28 20:20:51.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-07-28 20:20:51.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-07-28 20:20:51.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.392780 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14732 2023-07-28 20:42:25.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-28 20:42:25.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:42:25.000000 mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.400781 mypy-boto3-cloudcontrol-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-28 20:20:50.000000 mypy-boto3-cloudcontrol-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloudcontrol-1.28.12/LICENSE` & `mypy-boto3-cloudcontrol-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/PKG-INFO` & `mypy-boto3-cloudcontrol-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudcontrol
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudControlApi 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudControlApi 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudcontrol)](https://pepy.tech/project/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,35 +354,35 @@
 `mypy_boto3_cloudcontrol.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
+    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
 def get_structure() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudcontrol-1.28.12/README.md` & `mypy-boto3-cloudcontrol-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudcontrol)](https://pepy.tech/project/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,35 +322,35 @@
 `mypy_boto3_cloudcontrol.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
+    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
 def get_structure() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__init__.py` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__init__.pyi` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/__main__.py` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CloudControlApi 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.CloudControlApi 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi\nOther"
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

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/client.py` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/client.pyi` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/literals.py` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/literals.pyi` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/paginator.py` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcerequestspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcerequestspaginator)
         """
 
 
@@ -72,13 +72,13 @@
     def paginate(
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ResourceModel: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcespaginator)
         """
```

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/paginator.pyi` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcerequestspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcerequestspaginator)
         """
 
 class ListResourcesPaginator(Paginator):
@@ -68,13 +68,13 @@
     def paginate(
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ResourceModel: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/paginators/#listresourcespaginator)
         """
```

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/type_defs.py` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,35 +22,35 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelResourceRequestInputRequestTypeDef",
     "ProgressEventTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateResourceInputRequestTypeDef",
     "DeleteResourceInputRequestTypeDef",
     "GetResourceInputRequestTypeDef",
     "ResourceDescriptionTypeDef",
     "GetResourceRequestStatusInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceRequestStatusFilterTypeDef",
-    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourcesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateResourceInputRequestTypeDef",
     "CancelResourceRequestOutputTypeDef",
     "CreateResourceOutputTypeDef",
     "DeleteResourceOutputTypeDef",
     "GetResourceRequestStatusOutputTypeDef",
     "ListResourceRequestsOutputTypeDef",
     "UpdateResourceOutputTypeDef",
     "GetResourceOutputTypeDef",
     "ListResourcesOutputTypeDef",
     "GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
+    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     "ListResourceRequestsInputRequestTypeDef",
 )
 
 CancelResourceRequestInputRequestTypeDef = TypedDict(
     "CancelResourceRequestInputRequestTypeDef",
     {
@@ -71,14 +71,25 @@
         "StatusMessage": str,
         "ErrorCode": HandlerErrorCodeType,
         "RetryAfter": datetime,
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
 _RequiredCreateResourceInputRequestTypeDef = TypedDict(
     "_RequiredCreateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "DesiredState": str,
     },
 )
@@ -167,48 +178,33 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-ResourceRequestStatusFilterTypeDef = TypedDict(
-    "ResourceRequestStatusFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Operations": Sequence[OperationType],
-        "OperationStatuses": Sequence[OperationStatusType],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
-    {
-        "TypeName": str,
-    },
-)
-_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+ResourceRequestStatusFilterTypeDef = TypedDict(
+    "ResourceRequestStatusFilterTypeDef",
     {
-        "TypeVersionId": str,
-        "RoleArn": str,
-        "ResourceModel": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Operations": Sequence[OperationType],
+        "OperationStatuses": Sequence[OperationStatusType],
     },
     total=False,
 )
 
-
-class ListResourcesInputListResourcesPaginateTypeDef(
-    _RequiredListResourcesInputListResourcesPaginateTypeDef,
-    _OptionalListResourcesInputListResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesInputRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalListResourcesInputRequestTypeDef = TypedDict(
@@ -226,35 +222,14 @@
 
 class ListResourcesInputRequestTypeDef(
     _RequiredListResourcesInputRequestTypeDef, _OptionalListResourcesInputRequestTypeDef
 ):
     pass
 
 
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
 _RequiredUpdateResourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "Identifier": str,
         "PatchDocument": str,
     },
@@ -276,75 +251,75 @@
     pass
 
 
 CancelResourceRequestOutputTypeDef = TypedDict(
     "CancelResourceRequestOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResourceOutputTypeDef = TypedDict(
     "CreateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResourceOutputTypeDef = TypedDict(
     "DeleteResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceRequestStatusOutputTypeDef = TypedDict(
     "GetResourceRequestStatusOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceRequestsOutputTypeDef = TypedDict(
     "ListResourceRequestsOutputTypeDef",
     {
         "ResourceRequestStatusSummaries": List[ProgressEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceOutputTypeDef = TypedDict(
     "UpdateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceOutputTypeDef = TypedDict(
     "GetResourceOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescription": ResourceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesOutputTypeDef = TypedDict(
     "ListResourcesOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescriptions": List[ResourceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef = TypedDict(
     "_RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
     {
         "RequestToken": str,
@@ -362,19 +337,44 @@
 class GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef(
     _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
     _OptionalGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
 ):
     pass
 
 
+_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeName": str,
+    },
+)
+_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeVersionId": str,
+        "RoleArn": str,
+        "ResourceModel": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourcesInputListResourcesPaginateTypeDef(
+    _RequiredListResourcesInputListResourcesPaginateTypeDef,
+    _OptionalListResourcesInputListResourcesPaginateTypeDef,
+):
+    pass
+
+
 ListResourceRequestsInputListResourceRequestsPaginateTypeDef = TypedDict(
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     {
         "ResourceRequestStatusFilter": ResourceRequestStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListResourceRequestsInputRequestTypeDef = TypedDict(
     "ListResourceRequestsInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/type_defs.pyi` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,35 +21,35 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelResourceRequestInputRequestTypeDef",
     "ProgressEventTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateResourceInputRequestTypeDef",
     "DeleteResourceInputRequestTypeDef",
     "GetResourceInputRequestTypeDef",
     "ResourceDescriptionTypeDef",
     "GetResourceRequestStatusInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceRequestStatusFilterTypeDef",
-    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourcesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateResourceInputRequestTypeDef",
     "CancelResourceRequestOutputTypeDef",
     "CreateResourceOutputTypeDef",
     "DeleteResourceOutputTypeDef",
     "GetResourceRequestStatusOutputTypeDef",
     "ListResourceRequestsOutputTypeDef",
     "UpdateResourceOutputTypeDef",
     "GetResourceOutputTypeDef",
     "ListResourcesOutputTypeDef",
     "GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
+    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     "ListResourceRequestsInputRequestTypeDef",
 )
 
 CancelResourceRequestInputRequestTypeDef = TypedDict(
     "CancelResourceRequestInputRequestTypeDef",
     {
@@ -70,14 +70,25 @@
         "StatusMessage": str,
         "ErrorCode": HandlerErrorCodeType,
         "RetryAfter": datetime,
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
 _RequiredCreateResourceInputRequestTypeDef = TypedDict(
     "_RequiredCreateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "DesiredState": str,
     },
 )
@@ -160,46 +171,33 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-ResourceRequestStatusFilterTypeDef = TypedDict(
-    "ResourceRequestStatusFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Operations": Sequence[OperationType],
-        "OperationStatuses": Sequence[OperationStatusType],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
-    {
-        "TypeName": str,
-    },
-)
-_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+ResourceRequestStatusFilterTypeDef = TypedDict(
+    "ResourceRequestStatusFilterTypeDef",
     {
-        "TypeVersionId": str,
-        "RoleArn": str,
-        "ResourceModel": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Operations": Sequence[OperationType],
+        "OperationStatuses": Sequence[OperationStatusType],
     },
     total=False,
 )
 
-class ListResourcesInputListResourcesPaginateTypeDef(
-    _RequiredListResourcesInputListResourcesPaginateTypeDef,
-    _OptionalListResourcesInputListResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesInputRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalListResourcesInputRequestTypeDef = TypedDict(
@@ -215,35 +213,14 @@
 )
 
 class ListResourcesInputRequestTypeDef(
     _RequiredListResourcesInputRequestTypeDef, _OptionalListResourcesInputRequestTypeDef
 ):
     pass
 
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
 _RequiredUpdateResourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "Identifier": str,
         "PatchDocument": str,
     },
@@ -263,75 +240,75 @@
 ):
     pass
 
 CancelResourceRequestOutputTypeDef = TypedDict(
     "CancelResourceRequestOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResourceOutputTypeDef = TypedDict(
     "CreateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResourceOutputTypeDef = TypedDict(
     "DeleteResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceRequestStatusOutputTypeDef = TypedDict(
     "GetResourceRequestStatusOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceRequestsOutputTypeDef = TypedDict(
     "ListResourceRequestsOutputTypeDef",
     {
         "ResourceRequestStatusSummaries": List[ProgressEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceOutputTypeDef = TypedDict(
     "UpdateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceOutputTypeDef = TypedDict(
     "GetResourceOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescription": ResourceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesOutputTypeDef = TypedDict(
     "ListResourcesOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescriptions": List[ResourceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef = TypedDict(
     "_RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
     {
         "RequestToken": str,
@@ -347,19 +324,42 @@
 
 class GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef(
     _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
     _OptionalGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
 ):
     pass
 
+_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeName": str,
+    },
+)
+_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeVersionId": str,
+        "RoleArn": str,
+        "ResourceModel": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourcesInputListResourcesPaginateTypeDef(
+    _RequiredListResourcesInputListResourcesPaginateTypeDef,
+    _OptionalListResourcesInputListResourcesPaginateTypeDef,
+):
+    pass
+
 ListResourceRequestsInputListResourceRequestsPaginateTypeDef = TypedDict(
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     {
         "ResourceRequestStatusFilter": ResourceRequestStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListResourceRequestsInputRequestTypeDef = TypedDict(
     "ListResourceRequestsInputRequestTypeDef",
     {
```

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/waiter.py` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol/waiter.pyi` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/PKG-INFO` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloudcontrol
-Version: 1.28.12
-Summary: Type annotations for boto3.CloudControlApi 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.CloudControlApi 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloudcontrol.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloudcontrol)](https://pepy.tech/project/mypy-boto3-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CloudControlApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
+[boto3.CloudControlApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [mypy-boto3-cloudcontrol docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloudcontrol/).
 
 See how it helps to find and fix potential bugs:
 
@@ -354,35 +354,35 @@
 `mypy_boto3_cloudcontrol.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
+    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
 def get_structure() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
```

### Comparing `mypy-boto3-cloudcontrol-1.28.12/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt` & `mypy-boto3-cloudcontrol-1.28.15/mypy_boto3_cloudcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloudcontrol-1.28.12/setup.py` & `mypy-boto3-cloudcontrol-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloudcontrol",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloudcontrol"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CloudControlApi 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.CloudControlApi 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

