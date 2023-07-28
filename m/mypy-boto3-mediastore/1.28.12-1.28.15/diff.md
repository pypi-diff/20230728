# Comparing `tmp/mypy-boto3-mediastore-1.28.12.tar.gz` & `tmp/mypy-boto3-mediastore-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mediastore-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
+gzip compressed data, was "mypy-boto3-mediastore-1.28.15.tar", last modified: Fri Jul 28 20:43:17 2023, max compression
```

## Comparing `mypy-boto3-mediastore-1.28.12.tar` & `mypy-boto3-mediastore-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.036437 mypy-boto3-mediastore-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-07-27 05:35:02.032437 mypy-boto3-mediastore-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12683 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.028437 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10904 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.032437 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14182 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 05:35:01.000000 mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.036437 mypy-boto3-mediastore-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-27 05:26:25.000000 mypy-boto3-mediastore-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.785508 mypy-boto3-mediastore-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-28 20:43:17.777508 mypy-boto3-mediastore-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.777508 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14585 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14556 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8258 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10348 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10335 2023-07-28 20:31:39.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:17.777508 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14125 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:17.000000 mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:17.785508 mypy-boto3-mediastore-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-28 20:31:38.000000 mypy-boto3-mediastore-1.28.15/setup.py
```

### Comparing `mypy-boto3-mediastore-1.28.12/LICENSE` & `mypy-boto3-mediastore-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.12/PKG-INFO` & `mypy-boto3-mediastore-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaStore 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,47 +325,45 @@
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
     CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteContainerInputRequestTypeDef,
     DeleteContainerPolicyInputRequestTypeDef,
     DeleteCorsPolicyInputRequestTypeDef,
     DeleteLifecyclePolicyInputRequestTypeDef,
     DeleteMetricPolicyInputRequestTypeDef,
     DescribeContainerInputRequestTypeDef,
     GetContainerPolicyInputRequestTypeDef,
-    GetContainerPolicyOutputTypeDef,
     GetCorsPolicyInputRequestTypeDef,
     GetLifecyclePolicyInputRequestTypeDef,
-    GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyInputRequestTypeDef,
-    ListContainersInputListContainersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContainersInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
-    MetricPolicyRuleOutputTypeDef,
     MetricPolicyRuleTypeDef,
-    PaginatorConfigTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    CreateContainerOutputTypeDef,
-    DescribeContainerOutputTypeDef,
-    ListContainersOutputTypeDef,
-    GetCorsPolicyOutputTypeDef,
     PutCorsPolicyInputRequestTypeDef,
     CreateContainerInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateContainerOutputTypeDef,
+    DescribeContainerOutputTypeDef,
+    GetContainerPolicyOutputTypeDef,
+    GetCorsPolicyOutputTypeDef,
+    GetLifecyclePolicyOutputTypeDef,
+    ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    ListContainersInputListContainersPaginateTypeDef,
     MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
     GetMetricPolicyOutputTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-mediastore-1.28.12/README.md` & `mypy-boto3-mediastore-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,47 +293,45 @@
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
     CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteContainerInputRequestTypeDef,
     DeleteContainerPolicyInputRequestTypeDef,
     DeleteCorsPolicyInputRequestTypeDef,
     DeleteLifecyclePolicyInputRequestTypeDef,
     DeleteMetricPolicyInputRequestTypeDef,
     DescribeContainerInputRequestTypeDef,
     GetContainerPolicyInputRequestTypeDef,
-    GetContainerPolicyOutputTypeDef,
     GetCorsPolicyInputRequestTypeDef,
     GetLifecyclePolicyInputRequestTypeDef,
-    GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyInputRequestTypeDef,
-    ListContainersInputListContainersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContainersInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
-    MetricPolicyRuleOutputTypeDef,
     MetricPolicyRuleTypeDef,
-    PaginatorConfigTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    CreateContainerOutputTypeDef,
-    DescribeContainerOutputTypeDef,
-    ListContainersOutputTypeDef,
-    GetCorsPolicyOutputTypeDef,
     PutCorsPolicyInputRequestTypeDef,
     CreateContainerInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateContainerOutputTypeDef,
+    DescribeContainerOutputTypeDef,
+    GetContainerPolicyOutputTypeDef,
+    GetCorsPolicyOutputTypeDef,
+    GetLifecyclePolicyOutputTypeDef,
+    ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    ListContainersInputListContainersPaginateTypeDef,
     MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
     GetMetricPolicyOutputTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__init__.py` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__init__.pyi` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/__main__.py` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaStore 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.MediaStore 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore\nOther"
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

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/client.py` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/client.pyi` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/literals.py` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/literals.pyi` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/paginator.py` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,31 +23,28 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListContainersOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListContainersPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListContainersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Paginator.ListContainers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/paginators/#listcontainerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContainersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Paginator.ListContainers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/paginators/#listcontainerspaginator)
         """
```

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/paginator.pyi` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,28 +23,31 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import ListContainersOutputTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListContainersPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListContainersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Paginator.ListContainers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/paginators/#listcontainerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListContainersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore.Paginator.ListContainers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/paginators/#listcontainerspaginator)
         """
```

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/type_defs.py` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,47 +24,45 @@
 
 
 __all__ = (
     "ContainerTypeDef",
     "CorsRuleOutputTypeDef",
     "CorsRuleTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteContainerInputRequestTypeDef",
     "DeleteContainerPolicyInputRequestTypeDef",
     "DeleteCorsPolicyInputRequestTypeDef",
     "DeleteLifecyclePolicyInputRequestTypeDef",
     "DeleteMetricPolicyInputRequestTypeDef",
     "DescribeContainerInputRequestTypeDef",
     "GetContainerPolicyInputRequestTypeDef",
-    "GetContainerPolicyOutputTypeDef",
     "GetCorsPolicyInputRequestTypeDef",
     "GetLifecyclePolicyInputRequestTypeDef",
-    "GetLifecyclePolicyOutputTypeDef",
     "GetMetricPolicyInputRequestTypeDef",
-    "ListContainersInputListContainersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListContainersInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
-    "MetricPolicyRuleOutputTypeDef",
     "MetricPolicyRuleTypeDef",
-    "PaginatorConfigTypeDef",
     "PutContainerPolicyInputRequestTypeDef",
     "PutLifecyclePolicyInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAccessLoggingInputRequestTypeDef",
     "StopAccessLoggingInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "CreateContainerOutputTypeDef",
-    "DescribeContainerOutputTypeDef",
-    "ListContainersOutputTypeDef",
-    "GetCorsPolicyOutputTypeDef",
     "PutCorsPolicyInputRequestTypeDef",
     "CreateContainerInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateContainerOutputTypeDef",
+    "DescribeContainerOutputTypeDef",
+    "GetContainerPolicyOutputTypeDef",
+    "GetCorsPolicyOutputTypeDef",
+    "GetLifecyclePolicyOutputTypeDef",
+    "ListContainersOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "ListContainersInputListContainersPaginateTypeDef",
     "MetricPolicyOutputTypeDef",
     "MetricPolicyTypeDef",
     "GetMetricPolicyOutputTypeDef",
     "PutMetricPolicyInputRequestTypeDef",
 )
 
 ContainerTypeDef = TypedDict(
@@ -139,14 +137,25 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
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
 DeleteContainerInputRequestTypeDef = TypedDict(
     "DeleteContainerInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
@@ -189,55 +198,41 @@
 GetContainerPolicyInputRequestTypeDef = TypedDict(
     "GetContainerPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
-GetContainerPolicyOutputTypeDef = TypedDict(
-    "GetContainerPolicyOutputTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCorsPolicyInputRequestTypeDef = TypedDict(
     "GetCorsPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
 GetLifecyclePolicyInputRequestTypeDef = TypedDict(
     "GetLifecyclePolicyInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
-GetLifecyclePolicyOutputTypeDef = TypedDict(
-    "GetLifecyclePolicyOutputTypeDef",
-    {
-        "LifecyclePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMetricPolicyInputRequestTypeDef = TypedDict(
     "GetMetricPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
-ListContainersInputListContainersPaginateTypeDef = TypedDict(
-    "ListContainersInputListContainersPaginateTypeDef",
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
 
 ListContainersInputRequestTypeDef = TypedDict(
     "ListContainersInputRequestTypeDef",
     {
@@ -250,59 +245,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
-MetricPolicyRuleOutputTypeDef = TypedDict(
-    "MetricPolicyRuleOutputTypeDef",
-    {
-        "ObjectGroup": str,
-        "ObjectGroupName": str,
-    },
-)
-
 MetricPolicyRuleTypeDef = TypedDict(
     "MetricPolicyRuleTypeDef",
     {
         "ObjectGroup": str,
         "ObjectGroupName": str,
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
 PutContainerPolicyInputRequestTypeDef = TypedDict(
     "PutContainerPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "Policy": str,
     },
 )
@@ -311,25 +269,14 @@
     "PutLifecyclePolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "LifecyclePolicy": str,
     },
 )
 
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
 StartAccessLoggingInputRequestTypeDef = TypedDict(
     "StartAccessLoggingInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
@@ -344,47 +291,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": Sequence[str],
     },
 )
 
-CreateContainerOutputTypeDef = TypedDict(
-    "CreateContainerOutputTypeDef",
-    {
-        "Container": ContainerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeContainerOutputTypeDef = TypedDict(
-    "DescribeContainerOutputTypeDef",
-    {
-        "Container": ContainerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListContainersOutputTypeDef = TypedDict(
-    "ListContainersOutputTypeDef",
-    {
-        "Containers": List[ContainerTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetCorsPolicyOutputTypeDef = TypedDict(
-    "GetCorsPolicyOutputTypeDef",
-    {
-        "CorsPolicy": List[CorsRuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutCorsPolicyInputRequestTypeDef = TypedDict(
     "PutCorsPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "CorsPolicy": Sequence[CorsRuleTypeDef],
     },
 )
@@ -414,32 +328,89 @@
     "TagResourceInputRequestTypeDef",
     {
         "Resource": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateContainerOutputTypeDef = TypedDict(
+    "CreateContainerOutputTypeDef",
+    {
+        "Container": ContainerTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeContainerOutputTypeDef = TypedDict(
+    "DescribeContainerOutputTypeDef",
+    {
+        "Container": ContainerTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerPolicyOutputTypeDef = TypedDict(
+    "GetContainerPolicyOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCorsPolicyOutputTypeDef = TypedDict(
+    "GetCorsPolicyOutputTypeDef",
+    {
+        "CorsPolicy": List[CorsRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLifecyclePolicyOutputTypeDef = TypedDict(
+    "GetLifecyclePolicyOutputTypeDef",
+    {
+        "LifecyclePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContainersOutputTypeDef = TypedDict(
+    "ListContainersOutputTypeDef",
+    {
+        "Containers": List[ContainerTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContainersInputListContainersPaginateTypeDef = TypedDict(
+    "ListContainersInputListContainersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 _RequiredMetricPolicyOutputTypeDef = TypedDict(
     "_RequiredMetricPolicyOutputTypeDef",
     {
         "ContainerLevelMetrics": ContainerLevelMetricsType,
     },
 )
 _OptionalMetricPolicyOutputTypeDef = TypedDict(
     "_OptionalMetricPolicyOutputTypeDef",
     {
-        "MetricPolicyRules": List[MetricPolicyRuleOutputTypeDef],
+        "MetricPolicyRules": List[MetricPolicyRuleTypeDef],
     },
     total=False,
 )
 
 
 class MetricPolicyOutputTypeDef(
     _RequiredMetricPolicyOutputTypeDef, _OptionalMetricPolicyOutputTypeDef
@@ -466,15 +437,15 @@
     pass
 
 
 GetMetricPolicyOutputTypeDef = TypedDict(
     "GetMetricPolicyOutputTypeDef",
     {
         "MetricPolicy": MetricPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetricPolicyInputRequestTypeDef = TypedDict(
     "PutMetricPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
```

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore/type_defs.pyi` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -23,47 +23,45 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "ContainerTypeDef",
     "CorsRuleOutputTypeDef",
     "CorsRuleTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteContainerInputRequestTypeDef",
     "DeleteContainerPolicyInputRequestTypeDef",
     "DeleteCorsPolicyInputRequestTypeDef",
     "DeleteLifecyclePolicyInputRequestTypeDef",
     "DeleteMetricPolicyInputRequestTypeDef",
     "DescribeContainerInputRequestTypeDef",
     "GetContainerPolicyInputRequestTypeDef",
-    "GetContainerPolicyOutputTypeDef",
     "GetCorsPolicyInputRequestTypeDef",
     "GetLifecyclePolicyInputRequestTypeDef",
-    "GetLifecyclePolicyOutputTypeDef",
     "GetMetricPolicyInputRequestTypeDef",
-    "ListContainersInputListContainersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListContainersInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagOutputTypeDef",
-    "MetricPolicyRuleOutputTypeDef",
     "MetricPolicyRuleTypeDef",
-    "PaginatorConfigTypeDef",
     "PutContainerPolicyInputRequestTypeDef",
     "PutLifecyclePolicyInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartAccessLoggingInputRequestTypeDef",
     "StopAccessLoggingInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "CreateContainerOutputTypeDef",
-    "DescribeContainerOutputTypeDef",
-    "ListContainersOutputTypeDef",
-    "GetCorsPolicyOutputTypeDef",
     "PutCorsPolicyInputRequestTypeDef",
     "CreateContainerInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateContainerOutputTypeDef",
+    "DescribeContainerOutputTypeDef",
+    "GetContainerPolicyOutputTypeDef",
+    "GetCorsPolicyOutputTypeDef",
+    "GetLifecyclePolicyOutputTypeDef",
+    "ListContainersOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
+    "ListContainersInputListContainersPaginateTypeDef",
     "MetricPolicyOutputTypeDef",
     "MetricPolicyTypeDef",
     "GetMetricPolicyOutputTypeDef",
     "PutMetricPolicyInputRequestTypeDef",
 )
 
 ContainerTypeDef = TypedDict(
@@ -132,14 +130,25 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
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
 DeleteContainerInputRequestTypeDef = TypedDict(
     "DeleteContainerInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
@@ -182,55 +191,41 @@
 GetContainerPolicyInputRequestTypeDef = TypedDict(
     "GetContainerPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
-GetContainerPolicyOutputTypeDef = TypedDict(
-    "GetContainerPolicyOutputTypeDef",
-    {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCorsPolicyInputRequestTypeDef = TypedDict(
     "GetCorsPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
 GetLifecyclePolicyInputRequestTypeDef = TypedDict(
     "GetLifecyclePolicyInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
-GetLifecyclePolicyOutputTypeDef = TypedDict(
-    "GetLifecyclePolicyOutputTypeDef",
-    {
-        "LifecyclePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMetricPolicyInputRequestTypeDef = TypedDict(
     "GetMetricPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
-ListContainersInputListContainersPaginateTypeDef = TypedDict(
-    "ListContainersInputListContainersPaginateTypeDef",
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
 
 ListContainersInputRequestTypeDef = TypedDict(
     "ListContainersInputRequestTypeDef",
     {
@@ -243,57 +238,22 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "Resource": str,
     },
 )
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-MetricPolicyRuleOutputTypeDef = TypedDict(
-    "MetricPolicyRuleOutputTypeDef",
-    {
-        "ObjectGroup": str,
-        "ObjectGroupName": str,
-    },
-)
-
 MetricPolicyRuleTypeDef = TypedDict(
     "MetricPolicyRuleTypeDef",
     {
         "ObjectGroup": str,
         "ObjectGroupName": str,
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
 PutContainerPolicyInputRequestTypeDef = TypedDict(
     "PutContainerPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "Policy": str,
     },
 )
@@ -302,25 +262,14 @@
     "PutLifecyclePolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "LifecyclePolicy": str,
     },
 )
 
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
 StartAccessLoggingInputRequestTypeDef = TypedDict(
     "StartAccessLoggingInputRequestTypeDef",
     {
         "ContainerName": str,
     },
 )
 
@@ -335,47 +284,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "Resource": str,
         "TagKeys": Sequence[str],
     },
 )
 
-CreateContainerOutputTypeDef = TypedDict(
-    "CreateContainerOutputTypeDef",
-    {
-        "Container": ContainerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeContainerOutputTypeDef = TypedDict(
-    "DescribeContainerOutputTypeDef",
-    {
-        "Container": ContainerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListContainersOutputTypeDef = TypedDict(
-    "ListContainersOutputTypeDef",
-    {
-        "Containers": List[ContainerTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetCorsPolicyOutputTypeDef = TypedDict(
-    "GetCorsPolicyOutputTypeDef",
-    {
-        "CorsPolicy": List[CorsRuleOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutCorsPolicyInputRequestTypeDef = TypedDict(
     "PutCorsPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
         "CorsPolicy": Sequence[CorsRuleTypeDef],
     },
 )
@@ -403,32 +319,89 @@
     "TagResourceInputRequestTypeDef",
     {
         "Resource": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateContainerOutputTypeDef = TypedDict(
+    "CreateContainerOutputTypeDef",
+    {
+        "Container": ContainerTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeContainerOutputTypeDef = TypedDict(
+    "DescribeContainerOutputTypeDef",
+    {
+        "Container": ContainerTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerPolicyOutputTypeDef = TypedDict(
+    "GetContainerPolicyOutputTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCorsPolicyOutputTypeDef = TypedDict(
+    "GetCorsPolicyOutputTypeDef",
+    {
+        "CorsPolicy": List[CorsRuleOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLifecyclePolicyOutputTypeDef = TypedDict(
+    "GetLifecyclePolicyOutputTypeDef",
+    {
+        "LifecyclePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContainersOutputTypeDef = TypedDict(
+    "ListContainersOutputTypeDef",
+    {
+        "Containers": List[ContainerTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListContainersInputListContainersPaginateTypeDef = TypedDict(
+    "ListContainersInputListContainersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 _RequiredMetricPolicyOutputTypeDef = TypedDict(
     "_RequiredMetricPolicyOutputTypeDef",
     {
         "ContainerLevelMetrics": ContainerLevelMetricsType,
     },
 )
 _OptionalMetricPolicyOutputTypeDef = TypedDict(
     "_OptionalMetricPolicyOutputTypeDef",
     {
-        "MetricPolicyRules": List[MetricPolicyRuleOutputTypeDef],
+        "MetricPolicyRules": List[MetricPolicyRuleTypeDef],
     },
     total=False,
 )
 
 class MetricPolicyOutputTypeDef(
     _RequiredMetricPolicyOutputTypeDef, _OptionalMetricPolicyOutputTypeDef
 ):
@@ -451,15 +424,15 @@
 class MetricPolicyTypeDef(_RequiredMetricPolicyTypeDef, _OptionalMetricPolicyTypeDef):
     pass
 
 GetMetricPolicyOutputTypeDef = TypedDict(
     "GetMetricPolicyOutputTypeDef",
     {
         "MetricPolicy": MetricPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetricPolicyInputRequestTypeDef = TypedDict(
     "PutMetricPolicyInputRequestTypeDef",
     {
         "ContainerName": str,
```

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/PKG-INFO` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mediastore
-Version: 1.28.12
-Summary: Type annotations for boto3.MediaStore 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mediastore.svg?color=blue)](https://pypi.org/project/mypy-boto3-mediastore)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mediastore)](https://pepy.tech/project/mypy-boto3-mediastore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaStore 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
+[boto3.MediaStore 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediastore.html#MediaStore)
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
 [mypy-boto3-mediastore docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mediastore/).
 
 See how it helps to find and fix potential bugs:
 
@@ -325,47 +325,45 @@
 
 ```python
 from mypy_boto3_mediastore.type_defs import (
     ContainerTypeDef,
     CorsRuleOutputTypeDef,
     CorsRuleTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteContainerInputRequestTypeDef,
     DeleteContainerPolicyInputRequestTypeDef,
     DeleteCorsPolicyInputRequestTypeDef,
     DeleteLifecyclePolicyInputRequestTypeDef,
     DeleteMetricPolicyInputRequestTypeDef,
     DescribeContainerInputRequestTypeDef,
     GetContainerPolicyInputRequestTypeDef,
-    GetContainerPolicyOutputTypeDef,
     GetCorsPolicyInputRequestTypeDef,
     GetLifecyclePolicyInputRequestTypeDef,
-    GetLifecyclePolicyOutputTypeDef,
     GetMetricPolicyInputRequestTypeDef,
-    ListContainersInputListContainersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListContainersInputRequestTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagOutputTypeDef,
-    MetricPolicyRuleOutputTypeDef,
     MetricPolicyRuleTypeDef,
-    PaginatorConfigTypeDef,
     PutContainerPolicyInputRequestTypeDef,
     PutLifecyclePolicyInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartAccessLoggingInputRequestTypeDef,
     StopAccessLoggingInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    CreateContainerOutputTypeDef,
-    DescribeContainerOutputTypeDef,
-    ListContainersOutputTypeDef,
-    GetCorsPolicyOutputTypeDef,
     PutCorsPolicyInputRequestTypeDef,
     CreateContainerInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateContainerOutputTypeDef,
+    DescribeContainerOutputTypeDef,
+    GetContainerPolicyOutputTypeDef,
+    GetCorsPolicyOutputTypeDef,
+    GetLifecyclePolicyOutputTypeDef,
+    ListContainersOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
+    ListContainersInputListContainersPaginateTypeDef,
     MetricPolicyOutputTypeDef,
     MetricPolicyTypeDef,
     GetMetricPolicyOutputTypeDef,
     PutMetricPolicyInputRequestTypeDef,
 )
```

### Comparing `mypy-boto3-mediastore-1.28.12/mypy_boto3_mediastore.egg-info/SOURCES.txt` & `mypy-boto3-mediastore-1.28.15/mypy_boto3_mediastore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mediastore-1.28.12/setup.py` & `mypy-boto3-mediastore-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mediastore",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mediastore"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MediaStore 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.MediaStore 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

