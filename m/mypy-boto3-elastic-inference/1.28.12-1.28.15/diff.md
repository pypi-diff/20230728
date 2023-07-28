# Comparing `tmp/mypy-boto3-elastic-inference-1.28.12.tar.gz` & `tmp/mypy-boto3-elastic-inference-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-elastic-inference-1.28.12.tar", last modified: Thu Jul 27 05:34:38 2023, max compression
+gzip compressed data, was "mypy-boto3-elastic-inference-1.28.15.tar", last modified: Fri Jul 28 20:42:44 2023, max compression
```

## Comparing `mypy-boto3-elastic-inference-1.28.12.tar` & `mypy-boto3-elastic-inference-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.340521 mypy-boto3-elastic-inference-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-27 05:34:38.340521 mypy-boto3-elastic-inference-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.336521 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:38.340521 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:38.000000 mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:38.340521 mypy-boto3-elastic-inference-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-27 05:21:41.000000 mypy-boto3-elastic-inference-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8114 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13829 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:43.000000 mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:43.977044 mypy-boto3-elastic-inference-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-07-28 20:25:03.000000 mypy-boto3-elastic-inference-1.28.15/setup.py
```

### Comparing `mypy-boto3-elastic-inference-1.28.12/LICENSE` & `mypy-boto3-elastic-inference-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.12/PKG-INFO` & `mypy-boto3-elastic-inference-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastic-inference
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticInference 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticInference 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastic-inference)](https://pepy.tech/project/mypy-boto3-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticInference 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[boto3.ElasticInference 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,26 +327,26 @@
 
 ```python
 from mypy_boto3_elastic_inference.type_defs import (
     AcceleratorTypeOfferingTypeDef,
     KeyValuePairTypeDef,
     MemoryInfoTypeDef,
     DescribeAcceleratorOfferingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     ElasticInferenceAcceleratorHealthTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
     AcceleratorTypeTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
+    DescribeAcceleratorOfferingsResponseTypeDef,
+    ListTagsForResourceResultTypeDef,
     DescribeAcceleratorsRequestRequestTypeDef,
+    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
     ElasticInferenceAcceleratorTypeDef,
     DescribeAcceleratorTypesResponseTypeDef,
     DescribeAcceleratorsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorTypeOfferingTypeDef:
```

### Comparing `mypy-boto3-elastic-inference-1.28.12/README.md` & `mypy-boto3-elastic-inference-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastic-inference)](https://pepy.tech/project/mypy-boto3-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticInference 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[boto3.ElasticInference 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,26 +295,26 @@
 
 ```python
 from mypy_boto3_elastic_inference.type_defs import (
     AcceleratorTypeOfferingTypeDef,
     KeyValuePairTypeDef,
     MemoryInfoTypeDef,
     DescribeAcceleratorOfferingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     ElasticInferenceAcceleratorHealthTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
     AcceleratorTypeTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
+    DescribeAcceleratorOfferingsResponseTypeDef,
+    ListTagsForResourceResultTypeDef,
     DescribeAcceleratorsRequestRequestTypeDef,
+    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
     ElasticInferenceAcceleratorTypeDef,
     DescribeAcceleratorTypesResponseTypeDef,
     DescribeAcceleratorsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorTypeOfferingTypeDef:
```

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__init__.py` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__init__.pyi` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/__main__.py` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ElasticInference 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ElasticInference 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference\nOther"
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

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/client.py` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/client.pyi` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/literals.py` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/literals.pyi` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/paginator.py` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -23,35 +23,32 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import DescribeAcceleratorsResponseTypeDef, FilterTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("DescribeAcceleratorsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/paginators/#describeacceleratorspaginator)
     """
 
     def paginate(
         self,
         *,
         acceleratorIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/paginators/#describeacceleratorspaginator)
         """
```

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/paginator.pyi` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,32 +23,35 @@
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import DescribeAcceleratorsResponseTypeDef, FilterTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("DescribeAcceleratorsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/paginators/#describeacceleratorspaginator)
     """
 
     def paginate(
         self,
         *,
         acceleratorIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference.Paginator.DescribeAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/paginators/#describeacceleratorspaginator)
         """
```

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/type_defs.py` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 
 
 __all__ = (
     "AcceleratorTypeOfferingTypeDef",
     "KeyValuePairTypeDef",
     "MemoryInfoTypeDef",
     "DescribeAcceleratorOfferingsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ElasticInferenceAcceleratorHealthTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "DescribeAcceleratorOfferingsResponseTypeDef",
     "AcceleratorTypeTypeDef",
-    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+    "DescribeAcceleratorOfferingsResponseTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "DescribeAcceleratorsRequestRequestTypeDef",
+    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
     "ElasticInferenceAcceleratorTypeDef",
     "DescribeAcceleratorTypesResponseTypeDef",
     "DescribeAcceleratorsResponseTypeDef",
 )
 
 AcceleratorTypeOfferingTypeDef = TypedDict(
     "AcceleratorTypeOfferingTypeDef",
@@ -89,23 +89,44 @@
 class DescribeAcceleratorOfferingsRequestRequestTypeDef(
     _RequiredDescribeAcceleratorOfferingsRequestRequestTypeDef,
     _OptionalDescribeAcceleratorOfferingsRequestRequestTypeDef,
 ):
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
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ElasticInferenceAcceleratorHealthTypeDef = TypedDict(
     "ElasticInferenceAcceleratorHealthTypeDef",
     {
         "status": str,
     },
     total=False,
 )
@@ -113,43 +134,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
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
@@ -158,53 +150,61 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-DescribeAcceleratorOfferingsResponseTypeDef = TypedDict(
-    "DescribeAcceleratorOfferingsResponseTypeDef",
-    {
-        "acceleratorTypeOfferings": List[AcceleratorTypeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AcceleratorTypeTypeDef = TypedDict(
     "AcceleratorTypeTypeDef",
     {
         "acceleratorTypeName": str,
         "memoryInfo": MemoryInfoTypeDef,
         "throughputInfo": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef = TypedDict(
-    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+DescribeAcceleratorOfferingsResponseTypeDef = TypedDict(
+    "DescribeAcceleratorOfferingsResponseTypeDef",
     {
-        "acceleratorIds": Sequence[str],
-        "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "acceleratorTypeOfferings": List[AcceleratorTypeOfferingTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeAcceleratorsRequestRequestTypeDef = TypedDict(
     "DescribeAcceleratorsRequestRequestTypeDef",
     {
         "acceleratorIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef = TypedDict(
+    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+    {
+        "acceleratorIds": Sequence[str],
+        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ElasticInferenceAcceleratorTypeDef = TypedDict(
     "ElasticInferenceAcceleratorTypeDef",
     {
         "acceleratorHealth": ElasticInferenceAcceleratorHealthTypeDef,
         "acceleratorType": str,
         "acceleratorId": str,
         "availabilityZone": str,
@@ -213,19 +213,19 @@
     total=False,
 )
 
 DescribeAcceleratorTypesResponseTypeDef = TypedDict(
     "DescribeAcceleratorTypesResponseTypeDef",
     {
         "acceleratorTypes": List[AcceleratorTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAcceleratorsResponseTypeDef = TypedDict(
     "DescribeAcceleratorsResponseTypeDef",
     {
         "acceleratorSet": List[ElasticInferenceAcceleratorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference/type_defs.pyi` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -22,26 +22,26 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceleratorTypeOfferingTypeDef",
     "KeyValuePairTypeDef",
     "MemoryInfoTypeDef",
     "DescribeAcceleratorOfferingsRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "FilterTypeDef",
+    "PaginatorConfigTypeDef",
     "ElasticInferenceAcceleratorHealthTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "DescribeAcceleratorOfferingsResponseTypeDef",
     "AcceleratorTypeTypeDef",
-    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+    "DescribeAcceleratorOfferingsResponseTypeDef",
+    "ListTagsForResourceResultTypeDef",
     "DescribeAcceleratorsRequestRequestTypeDef",
+    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
     "ElasticInferenceAcceleratorTypeDef",
     "DescribeAcceleratorTypesResponseTypeDef",
     "DescribeAcceleratorsResponseTypeDef",
 )
 
 AcceleratorTypeOfferingTypeDef = TypedDict(
     "AcceleratorTypeOfferingTypeDef",
@@ -86,23 +86,44 @@
 
 class DescribeAcceleratorOfferingsRequestRequestTypeDef(
     _RequiredDescribeAcceleratorOfferingsRequestRequestTypeDef,
     _OptionalDescribeAcceleratorOfferingsRequestRequestTypeDef,
 ):
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
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "name": str,
         "values": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 ElasticInferenceAcceleratorHealthTypeDef = TypedDict(
     "ElasticInferenceAcceleratorHealthTypeDef",
     {
         "status": str,
     },
     total=False,
 )
@@ -110,43 +131,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
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
@@ -155,53 +147,61 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-DescribeAcceleratorOfferingsResponseTypeDef = TypedDict(
-    "DescribeAcceleratorOfferingsResponseTypeDef",
-    {
-        "acceleratorTypeOfferings": List[AcceleratorTypeOfferingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AcceleratorTypeTypeDef = TypedDict(
     "AcceleratorTypeTypeDef",
     {
         "acceleratorTypeName": str,
         "memoryInfo": MemoryInfoTypeDef,
         "throughputInfo": List[KeyValuePairTypeDef],
     },
     total=False,
 )
 
-DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef = TypedDict(
-    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+DescribeAcceleratorOfferingsResponseTypeDef = TypedDict(
+    "DescribeAcceleratorOfferingsResponseTypeDef",
     {
-        "acceleratorIds": Sequence[str],
-        "filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "acceleratorTypeOfferings": List[AcceleratorTypeOfferingTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeAcceleratorsRequestRequestTypeDef = TypedDict(
     "DescribeAcceleratorsRequestRequestTypeDef",
     {
         "acceleratorIds": Sequence[str],
         "filters": Sequence[FilterTypeDef],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef = TypedDict(
+    "DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef",
+    {
+        "acceleratorIds": Sequence[str],
+        "filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ElasticInferenceAcceleratorTypeDef = TypedDict(
     "ElasticInferenceAcceleratorTypeDef",
     {
         "acceleratorHealth": ElasticInferenceAcceleratorHealthTypeDef,
         "acceleratorType": str,
         "acceleratorId": str,
         "availabilityZone": str,
@@ -210,19 +210,19 @@
     total=False,
 )
 
 DescribeAcceleratorTypesResponseTypeDef = TypedDict(
     "DescribeAcceleratorTypesResponseTypeDef",
     {
         "acceleratorTypes": List[AcceleratorTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAcceleratorsResponseTypeDef = TypedDict(
     "DescribeAcceleratorsResponseTypeDef",
     {
         "acceleratorSet": List[ElasticInferenceAcceleratorTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/PKG-INFO` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-elastic-inference
-Version: 1.28.12
-Summary: Type annotations for boto3.ElasticInference 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ElasticInference 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-elastic-inference.svg?color=blue)](https://pypi.org/project/mypy-boto3-elastic-inference)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-elastic-inference)](https://pepy.tech/project/mypy-boto3-elastic-inference)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ElasticInference 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
+[boto3.ElasticInference 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference)
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
 [mypy-boto3-elastic-inference docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,26 +327,26 @@
 
 ```python
 from mypy_boto3_elastic_inference.type_defs import (
     AcceleratorTypeOfferingTypeDef,
     KeyValuePairTypeDef,
     MemoryInfoTypeDef,
     DescribeAcceleratorOfferingsRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     FilterTypeDef,
+    PaginatorConfigTypeDef,
     ElasticInferenceAcceleratorHealthTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
     AcceleratorTypeTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
+    DescribeAcceleratorOfferingsResponseTypeDef,
+    ListTagsForResourceResultTypeDef,
     DescribeAcceleratorsRequestRequestTypeDef,
+    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
     ElasticInferenceAcceleratorTypeDef,
     DescribeAcceleratorTypesResponseTypeDef,
     DescribeAcceleratorsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorTypeOfferingTypeDef:
```

### Comparing `mypy-boto3-elastic-inference-1.28.12/mypy_boto3_elastic_inference.egg-info/SOURCES.txt` & `mypy-boto3-elastic-inference-1.28.15/mypy_boto3_elastic_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-elastic-inference-1.28.12/setup.py` & `mypy-boto3-elastic-inference-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-elastic-inference",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_elastic_inference"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ElasticInference 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ElasticInference 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

