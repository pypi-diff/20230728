# Comparing `tmp/mypy-boto3-cloud9-1.28.12.tar.gz` & `tmp/mypy-boto3-cloud9-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cloud9-1.28.12.tar", last modified: Thu Jul 27 05:34:24 2023, max compression
+gzip compressed data, was "mypy-boto3-cloud9-1.28.15.tar", last modified: Fri Jul 28 20:42:25 2023, max compression
```

## Comparing `mypy-boto3-cloud9-1.28.12.tar` & `mypy-boto3-cloud9-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.860563 mypy-boto3-cloud9-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-07-27 05:34:24.860563 mypy-boto3-cloud9-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.856563 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9861 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:24.860563 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14157 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-27 05:34:24.000000 mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:24.860563 mypy-boto3-cloud9-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-27 05:18:25.000000 mypy-boto3-cloud9-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.328779 mypy-boto3-cloud9-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:48.000000 mypy-boto3-cloud9-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-28 20:42:25.328779 mypy-boto3-cloud9-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12652 2023-07-28 20:20:48.000000 mypy-boto3-cloud9-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.328779 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-28 20:20:48.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-28 20:20:48.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-28 20:20:48.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-07-28 20:20:49.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-28 20:20:49.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-07-28 20:20:50.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-07-28 20:20:50.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-07-28 20:20:49.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-28 20:20:49.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:48.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-07-28 20:20:50.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-07-28 20:20:50.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:48.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:25.328779 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-28 20:42:25.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-07-28 20:42:25.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:25.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:25.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 20:42:25.000000 mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:25.328779 mypy-boto3-cloud9-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-28 20:20:48.000000 mypy-boto3-cloud9-1.28.15/setup.py
```

### Comparing `mypy-boto3-cloud9-1.28.12/LICENSE` & `mypy-boto3-cloud9-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.12/PKG-INFO` & `mypy-boto3-cloud9-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloud9
-Version: 1.28.12
-Summary: Type annotations for boto3.Cloud9 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Cloud9 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloud9)](https://pepy.tech/project/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,42 +334,41 @@
 
 `mypy_boto3_cloud9.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloud9.type_defs import (
     TagTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
+    ListEnvironmentsResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloud9-1.28.12/README.md` & `mypy-boto3-cloud9-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloud9)](https://pepy.tech/project/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,42 +302,41 @@
 
 `mypy_boto3_cloud9.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloud9.type_defs import (
     TagTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
+    ListEnvironmentsResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__init__.py` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__init__.pyi` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/__main__.py` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Cloud9 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Cloud9 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9\nOther"
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

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/client.py` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/client.pyi` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/literals.py` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/literals.pyi` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/paginator.py` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,51 +30,47 @@
     DescribeEnvironmentMembershipsResultTypeDef,
     ListEnvironmentsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeEnvironmentMembershipsPaginator", "ListEnvironmentsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeEnvironmentMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#describeenvironmentmembershipspaginator)
     """
 
     def paginate(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEnvironmentMembershipsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#describeenvironmentmembershipspaginator)
         """
 
-
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnvironmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/paginator.pyi` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,47 +30,51 @@
     DescribeEnvironmentMembershipsResultTypeDef,
     ListEnvironmentsResultTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("DescribeEnvironmentMembershipsPaginator", "ListEnvironmentsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeEnvironmentMembershipsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#describeenvironmentmembershipspaginator)
     """
 
     def paginate(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEnvironmentMembershipsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#describeenvironmentmembershipspaginator)
         """
 
+
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnvironmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/type_defs.py` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,58 +30,60 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "CreateEnvironmentEC2ResultTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     "DescribeEnvironmentStatusRequestRequestTypeDef",
-    "DescribeEnvironmentStatusResultTypeDef",
     "DescribeEnvironmentsRequestRequestTypeDef",
     "EnvironmentLifecycleTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
-    "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEnvironmentMembershipRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentEC2RequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateEnvironmentEC2ResultTypeDef",
+    "DescribeEnvironmentStatusResultTypeDef",
+    "ListEnvironmentsResultTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateEnvironmentMembershipResultTypeDef",
     "DescribeEnvironmentMembershipsResultTypeDef",
     "UpdateEnvironmentMembershipResultTypeDef",
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "EnvironmentTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DescribeEnvironmentsResultTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateEnvironmentEC2ResultTypeDef = TypedDict(
-    "CreateEnvironmentEC2ResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "environmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -125,21 +127,20 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "userArn": str,
-        "environmentId": str,
-        "permissions": Sequence[PermissionsType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEnvironmentMembershipsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     {
@@ -155,23 +156,14 @@
 DescribeEnvironmentStatusRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentStatusRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-DescribeEnvironmentStatusResultTypeDef = TypedDict(
-    "DescribeEnvironmentStatusResultTypeDef",
-    {
-        "status": EnvironmentStatusType,
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentsRequestRequestTypeDef",
     {
         "environmentIds": Sequence[str],
     },
 )
 
@@ -181,76 +173,30 @@
         "status": EnvironmentLifecycleStatusType,
         "reason": str,
         "failureResource": str,
     },
     total=False,
 )
 
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListEnvironmentsResultTypeDef = TypedDict(
-    "ListEnvironmentsResultTypeDef",
-    {
-        "nextToken": str,
-        "environmentIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -322,37 +268,90 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateEnvironmentEC2ResultTypeDef = TypedDict(
+    "CreateEnvironmentEC2ResultTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentStatusResultTypeDef = TypedDict(
+    "DescribeEnvironmentStatusResultTypeDef",
+    {
+        "status": EnvironmentStatusType,
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnvironmentsResultTypeDef = TypedDict(
+    "ListEnvironmentsResultTypeDef",
+    {
+        "nextToken": str,
+        "environmentIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateEnvironmentMembershipResultTypeDef = TypedDict(
     "CreateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentMembershipsResultTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsResultTypeDef",
     {
         "memberships": List[EnvironmentMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEnvironmentMembershipResultTypeDef = TypedDict(
     "UpdateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    {
+        "userArn": str,
+        "environmentId": str,
+        "permissions": Sequence[PermissionsType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 _RequiredEnvironmentTypeDef = TypedDict(
     "_RequiredEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "arn": str,
@@ -373,22 +372,14 @@
 )
 
 
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEnvironmentsResultTypeDef = TypedDict(
     "DescribeEnvironmentsResultTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9/type_defs.pyi` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,58 +29,60 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "CreateEnvironmentEC2ResultTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     "DescribeEnvironmentStatusRequestRequestTypeDef",
-    "DescribeEnvironmentStatusResultTypeDef",
     "DescribeEnvironmentsRequestRequestTypeDef",
     "EnvironmentLifecycleTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
-    "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEnvironmentMembershipRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentEC2RequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateEnvironmentEC2ResultTypeDef",
+    "DescribeEnvironmentStatusResultTypeDef",
+    "ListEnvironmentsResultTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateEnvironmentMembershipResultTypeDef",
     "DescribeEnvironmentMembershipsResultTypeDef",
     "UpdateEnvironmentMembershipResultTypeDef",
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "EnvironmentTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "DescribeEnvironmentsResultTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateEnvironmentEC2ResultTypeDef = TypedDict(
-    "CreateEnvironmentEC2ResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "environmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -122,21 +124,20 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "userArn": str,
-        "environmentId": str,
-        "permissions": Sequence[PermissionsType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEnvironmentMembershipsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     {
@@ -152,23 +153,14 @@
 DescribeEnvironmentStatusRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentStatusRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-DescribeEnvironmentStatusResultTypeDef = TypedDict(
-    "DescribeEnvironmentStatusResultTypeDef",
-    {
-        "status": EnvironmentStatusType,
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentsRequestRequestTypeDef",
     {
         "environmentIds": Sequence[str],
     },
 )
 
@@ -178,76 +170,30 @@
         "status": EnvironmentLifecycleStatusType,
         "reason": str,
         "failureResource": str,
     },
     total=False,
 )
 
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListEnvironmentsResultTypeDef = TypedDict(
-    "ListEnvironmentsResultTypeDef",
-    {
-        "nextToken": str,
-        "environmentIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -315,37 +261,90 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateEnvironmentEC2ResultTypeDef = TypedDict(
+    "CreateEnvironmentEC2ResultTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentStatusResultTypeDef = TypedDict(
+    "DescribeEnvironmentStatusResultTypeDef",
+    {
+        "status": EnvironmentStatusType,
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnvironmentsResultTypeDef = TypedDict(
+    "ListEnvironmentsResultTypeDef",
+    {
+        "nextToken": str,
+        "environmentIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateEnvironmentMembershipResultTypeDef = TypedDict(
     "CreateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentMembershipsResultTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsResultTypeDef",
     {
         "memberships": List[EnvironmentMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEnvironmentMembershipResultTypeDef = TypedDict(
     "UpdateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    {
+        "userArn": str,
+        "environmentId": str,
+        "permissions": Sequence[PermissionsType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 _RequiredEnvironmentTypeDef = TypedDict(
     "_RequiredEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "arn": str,
@@ -364,22 +363,14 @@
     },
     total=False,
 )
 
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEnvironmentsResultTypeDef = TypedDict(
     "DescribeEnvironmentsResultTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/PKG-INFO` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cloud9
-Version: 1.28.12
-Summary: Type annotations for boto3.Cloud9 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Cloud9 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cloud9.svg?color=blue)](https://pypi.org/project/mypy-boto3-cloud9)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-cloud9)](https://pepy.tech/project/mypy-boto3-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Cloud9 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
+[boto3.Cloud9 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [mypy-boto3-cloud9 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -334,42 +334,41 @@
 
 `mypy_boto3_cloud9.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_cloud9.type_defs import (
     TagTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
+    ListEnvironmentsResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
-    ListTagsForResourceResponseTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
 def get_structure() -> TagTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-cloud9-1.28.12/mypy_boto3_cloud9.egg-info/SOURCES.txt` & `mypy-boto3-cloud9-1.28.15/mypy_boto3_cloud9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cloud9-1.28.12/setup.py` & `mypy-boto3-cloud9-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cloud9",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_cloud9"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Cloud9 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.Cloud9 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

