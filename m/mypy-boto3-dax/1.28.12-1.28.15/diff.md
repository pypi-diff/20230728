# Comparing `tmp/mypy-boto3-dax-1.28.12.tar.gz` & `tmp/mypy-boto3-dax-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dax-1.28.12.tar", last modified: Thu Jul 27 05:34:33 2023, max compression
+gzip compressed data, was "mypy-boto3-dax-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
```

## Comparing `mypy-boto3-dax-1.28.12.tar` & `mypy-boto3-dax-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14637 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/mypy_boto3_dax/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22558 2023-07-27 05:20:05.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22535 2023-07-27 05:20:05.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:33.000000 mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:33.720536 mypy-boto3-dax-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:20:04.000000 mypy-boto3-dax-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.768957 mypy-boto3-dax-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-07-28 20:42:37.768957 mypy-boto3-dax-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14615 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.764957 mypy-boto3-dax-1.28.15/mypy_boto3_dax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20424 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20389 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22331 2023-07-28 20:22:43.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22308 2023-07-28 20:22:43.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.768957 mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16086 2023-07-28 20:42:37.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:37.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:37.000000 mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.768957 mypy-boto3-dax-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:22:42.000000 mypy-boto3-dax-1.28.15/setup.py
```

### Comparing `mypy-boto3-dax-1.28.12/LICENSE` & `mypy-boto3-dax-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.12/PKG-INFO` & `mypy-boto3-dax-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dax
-Version: 1.28.12
-Summary: Type annotations for boto3.DAX 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DAX 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,59 +358,58 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
     SecurityGroupMembershipTypeDef,
     SSESpecificationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     ParameterGroupTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClustersRequestRequestTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     NodeTypeSpecificValueTypeDef,
-    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    DeleteParameterGroupResponseTypeDef,
+    DeleteSubnetGroupResponseTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DescribeEventsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
     CreateSubnetGroupResponseTypeDef,
```

### Comparing `mypy-boto3-dax-1.28.12/README.md` & `mypy-boto3-dax-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -326,59 +326,58 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
     SecurityGroupMembershipTypeDef,
     SSESpecificationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     ParameterGroupTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClustersRequestRequestTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     NodeTypeSpecificValueTypeDef,
-    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    DeleteParameterGroupResponseTypeDef,
+    DeleteSubnetGroupResponseTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DescribeEventsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
     CreateSubnetGroupResponseTypeDef,
```

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/__init__.py` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/__init__.pyi` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/__main__.py` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DAX 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.DAX 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX\nOther"
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

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/client.py` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/client.pyi` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/literals.py` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/literals.pyi` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/paginator.py` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,138 +54,129 @@
     "DescribeEventsPaginator",
     "DescribeParameterGroupsPaginator",
     "DescribeParametersPaginator",
     "DescribeSubnetGroupsPaginator",
     "ListTagsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeclusterspaginator)
     """
 
     def paginate(
-        self, *, ClusterNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeclusterspaginator)
         """
 
-
 class DescribeDefaultParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDefaultParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describedefaultparameterspaginator)
         """
 
-
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeeventspaginator)
     """
 
     def paginate(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeeventspaginator)
         """
 
-
 class DescribeParameterGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         ParameterGroupNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeParameterGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparametergroupspaginator)
         """
 
-
 class DescribeParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparameterspaginator)
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparameterspaginator)
         """
 
-
 class DescribeSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describesubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         SubnetGroupNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describesubnetgroupspaginator)
         """
 
-
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#listtagspaginator)
         """
```

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/paginator.pyi` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,129 +54,138 @@
     "DescribeEventsPaginator",
     "DescribeParameterGroupsPaginator",
     "DescribeParametersPaginator",
     "DescribeSubnetGroupsPaginator",
     "ListTagsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeclusterspaginator)
     """
 
     def paginate(
-        self, *, ClusterNames: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterNames: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeclusterspaginator)
         """
 
+
 class DescribeDefaultParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describedefaultparameterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDefaultParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeDefaultParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describedefaultparameterspaginator)
         """
 
+
 class DescribeEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeeventspaginator)
     """
 
     def paginate(
         self,
         *,
         SourceName: str = ...,
         SourceType: SourceTypeType = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Duration: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeeventspaginator)
         """
 
+
 class DescribeParameterGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparametergroupspaginator)
     """
 
     def paginate(
         self,
         *,
         ParameterGroupNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeParameterGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameterGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparametergroupspaginator)
         """
 
+
 class DescribeParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparameterspaginator)
     """
 
     def paginate(
         self,
         *,
         ParameterGroupName: str,
         Source: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeParametersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describeparameterspaginator)
         """
 
+
 class DescribeSubnetGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describesubnetgroupspaginator)
     """
 
     def paginate(
         self,
         *,
         SubnetGroupNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeSubnetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.DescribeSubnetGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#describesubnetgroupspaginator)
         """
 
+
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX.Paginator.ListTags.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/paginators/#listtagspaginator)
         """
```

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/type_defs.py` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -25,68 +25,66 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "ParameterGroupStatusTypeDef",
     "SSEDescriptionTypeDef",
     "SecurityGroupMembershipTypeDef",
     "SSESpecificationTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateParameterGroupRequestRequestTypeDef",
     "ParameterGroupTypeDef",
     "CreateSubnetGroupRequestRequestTypeDef",
     "DecreaseReplicationFactorRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteParameterGroupRequestRequestTypeDef",
-    "DeleteParameterGroupResponseTypeDef",
     "DeleteSubnetGroupRequestRequestTypeDef",
-    "DeleteSubnetGroupResponseTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClustersRequestRequestTypeDef",
-    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
     "DescribeDefaultParametersRequestRequestTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "EventTypeDef",
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
-    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "IncreaseReplicationFactorRequestRequestTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "NodeTypeSpecificValueTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RebootNodeRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SubnetTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateSubnetGroupRequestRequestTypeDef",
     "NodeTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "DeleteParameterGroupResponseTypeDef",
+    "DeleteSubnetGroupResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "TagResourceResponseTypeDef",
+    "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
+    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "DescribeEventsResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "TagResourceResponseTypeDef",
-    "UntagResourceResponseTypeDef",
     "ParameterTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "SubnetGroupTypeDef",
     "ClusterTypeDef",
     "DescribeDefaultParametersResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "CreateSubnetGroupResponseTypeDef",
@@ -159,36 +157,45 @@
     {
         "Key": str,
         "Value": str,
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
 _RequiredCreateParameterGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalCreateParameterGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateParameterGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateParameterGroupRequestRequestTypeDef(
     _RequiredCreateParameterGroupRequestRequestTypeDef,
     _OptionalCreateParameterGroupRequestRequestTypeDef,
 ):
     pass
 
-
 ParameterGroupTypeDef = TypedDict(
     "ParameterGroupTypeDef",
     {
         "ParameterGroupName": str,
         "Description": str,
     },
     total=False,
@@ -205,21 +212,19 @@
     "_OptionalCreateSubnetGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateSubnetGroupRequestRequestTypeDef(
     _RequiredCreateSubnetGroupRequestRequestTypeDef, _OptionalCreateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDecreaseReplicationFactorRequestRequestTypeDef = TypedDict(
     "_RequiredDecreaseReplicationFactorRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NewReplicationFactor": int,
     },
 )
@@ -228,108 +233,70 @@
     {
         "AvailabilityZones": Sequence[str],
         "NodeIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
-
 class DecreaseReplicationFactorRequestRequestTypeDef(
     _RequiredDecreaseReplicationFactorRequestRequestTypeDef,
     _OptionalDecreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteClusterRequestRequestTypeDef = TypedDict(
     "DeleteClusterRequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 
 DeleteParameterGroupRequestRequestTypeDef = TypedDict(
     "DeleteParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 
-DeleteParameterGroupResponseTypeDef = TypedDict(
-    "DeleteParameterGroupResponseTypeDef",
-    {
-        "DeletionMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSubnetGroupRequestRequestTypeDef = TypedDict(
     "DeleteSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 
-DeleteSubnetGroupResponseTypeDef = TypedDict(
-    "DeleteSubnetGroupResponseTypeDef",
-    {
-        "DeletionMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "ClusterNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = TypedDict(
-    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDefaultParametersRequestRequestTypeDef = TypedDict(
     "DescribeDefaultParametersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -347,56 +314,24 @@
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
     },
     total=False,
 )
 
-DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeParameterGroupsRequestRequestTypeDef = TypedDict(
     "DescribeParameterGroupsRequestRequestTypeDef",
     {
         "ParameterGroupNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeParametersRequestDescribeParametersPaginateTypeDef(
-    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
-    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeParametersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeParametersRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeParametersRequestRequestTypeDef = TypedDict(
@@ -405,31 +340,20 @@
         "Source": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class DescribeParametersRequestRequestTypeDef(
     _RequiredDescribeParametersRequestRequestTypeDef,
     _OptionalDescribeParametersRequestRequestTypeDef,
 ):
     pass
 
-
-DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
-    {
-        "SubnetGroupNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeSubnetGroupsRequestRequestTypeDef = TypedDict(
     "DescribeSubnetGroupsRequestRequestTypeDef",
     {
         "SubnetGroupNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
@@ -447,92 +371,48 @@
     "_OptionalIncreaseReplicationFactorRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
     },
     total=False,
 )
 
-
 class IncreaseReplicationFactorRequestRequestTypeDef(
     _RequiredIncreaseReplicationFactorRequestRequestTypeDef,
     _OptionalIncreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceName": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
     "_OptionalListTagsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 NodeTypeSpecificValueTypeDef = TypedDict(
     "NodeTypeSpecificValueTypeDef",
     {
         "NodeType": str,
         "Value": str,
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
 ParameterNameValueTypeDef = TypedDict(
     "ParameterNameValueTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
@@ -542,25 +422,14 @@
     "RebootNodeRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NodeId": str,
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
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": str,
     },
     total=False,
@@ -589,21 +458,19 @@
         "NotificationTopicStatus": str,
         "ParameterGroupName": str,
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 _OptionalUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
@@ -611,21 +478,19 @@
     {
         "Description": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateSubnetGroupRequestRequestTypeDef(
     _RequiredUpdateSubnetGroupRequestRequestTypeDef, _OptionalUpdateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NodeId": str,
         "Endpoint": EndpointTypeDef,
         "NodeCreateTime": datetime,
         "AvailabilityZone": str,
@@ -657,85 +522,187 @@
         "Tags": Sequence[TagTypeDef],
         "SSESpecification": SSESpecificationTypeDef,
         "ClusterEndpointEncryptionType": ClusterEndpointEncryptionTypeType,
     },
     total=False,
 )
 
-
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DeleteParameterGroupResponseTypeDef = TypedDict(
+    "DeleteParameterGroupResponseTypeDef",
+    {
+        "DeletionMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSubnetGroupResponseTypeDef = TypedDict(
+    "DeleteSubnetGroupResponseTypeDef",
+    {
+        "DeletionMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceResponseTypeDef = TypedDict(
+    "TagResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UntagResourceResponseTypeDef = TypedDict(
+    "UntagResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeParameterGroupsResponseTypeDef = TypedDict(
     "DescribeParameterGroupsResponseTypeDef",
     {
         "NextToken": str,
         "ParameterGroups": List[ParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateParameterGroupResponseTypeDef = TypedDict(
     "UpdateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeEventsResponseTypeDef = TypedDict(
-    "DescribeEventsResponseTypeDef",
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     {
-        "NextToken": str,
-        "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
+DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = TypedDict(
+    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-TagResourceResponseTypeDef = TypedDict(
-    "TagResourceResponseTypeDef",
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-UntagResourceResponseTypeDef = TypedDict(
-    "UntagResourceResponseTypeDef",
+DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ParameterGroupNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeParametersRequestDescribeParametersPaginateTypeDef(
+    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
+    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
+):
+    pass
+
+DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
+    {
+        "SubnetGroupNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceName": str,
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+DescribeEventsResponseTypeDef = TypedDict(
+    "DescribeEventsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Events": List[EventTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": str,
@@ -797,101 +764,101 @@
 )
 
 DescribeDefaultParametersResponseTypeDef = TypedDict(
     "DescribeDefaultParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeParametersResponseTypeDef = TypedDict(
     "DescribeParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSubnetGroupResponseTypeDef = TypedDict(
     "CreateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeSubnetGroupsResponseTypeDef",
     {
         "NextToken": str,
         "SubnetGroups": List[SubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSubnetGroupResponseTypeDef = TypedDict(
     "UpdateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseReplicationFactorResponseTypeDef = TypedDict(
     "DecreaseReplicationFactorResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "NextToken": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseReplicationFactorResponseTypeDef = TypedDict(
     "IncreaseReplicationFactorResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootNodeResponseTypeDef = TypedDict(
     "RebootNodeResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax/type_defs.pyi` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,67 +25,67 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "EndpointTypeDef",
     "NotificationConfigurationTypeDef",
     "ParameterGroupStatusTypeDef",
     "SSEDescriptionTypeDef",
     "SecurityGroupMembershipTypeDef",
     "SSESpecificationTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateParameterGroupRequestRequestTypeDef",
     "ParameterGroupTypeDef",
     "CreateSubnetGroupRequestRequestTypeDef",
     "DecreaseReplicationFactorRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteParameterGroupRequestRequestTypeDef",
-    "DeleteParameterGroupResponseTypeDef",
     "DeleteSubnetGroupRequestRequestTypeDef",
-    "DeleteSubnetGroupResponseTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClustersRequestRequestTypeDef",
-    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
     "DescribeDefaultParametersRequestRequestTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "EventTypeDef",
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     "DescribeParameterGroupsRequestRequestTypeDef",
-    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     "DescribeSubnetGroupsRequestRequestTypeDef",
     "IncreaseReplicationFactorRequestRequestTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "NodeTypeSpecificValueTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterNameValueTypeDef",
     "RebootNodeRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SubnetTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterRequestRequestTypeDef",
     "UpdateSubnetGroupRequestRequestTypeDef",
     "NodeTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "DeleteParameterGroupResponseTypeDef",
+    "DeleteSubnetGroupResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "TagResourceResponseTypeDef",
+    "UntagResourceResponseTypeDef",
     "CreateParameterGroupResponseTypeDef",
     "DescribeParameterGroupsResponseTypeDef",
     "UpdateParameterGroupResponseTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
+    "DescribeParametersRequestDescribeParametersPaginateTypeDef",
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "DescribeEventsResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "TagResourceResponseTypeDef",
-    "UntagResourceResponseTypeDef",
     "ParameterTypeDef",
     "UpdateParameterGroupRequestRequestTypeDef",
     "SubnetGroupTypeDef",
     "ClusterTypeDef",
     "DescribeDefaultParametersResponseTypeDef",
     "DescribeParametersResponseTypeDef",
     "CreateSubnetGroupResponseTypeDef",
@@ -158,34 +158,47 @@
     {
         "Key": str,
         "Value": str,
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
 _RequiredCreateParameterGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalCreateParameterGroupRequestRequestTypeDef = TypedDict(
     "_OptionalCreateParameterGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateParameterGroupRequestRequestTypeDef(
     _RequiredCreateParameterGroupRequestRequestTypeDef,
     _OptionalCreateParameterGroupRequestRequestTypeDef,
 ):
     pass
 
+
 ParameterGroupTypeDef = TypedDict(
     "ParameterGroupTypeDef",
     {
         "ParameterGroupName": str,
         "Description": str,
     },
     total=False,
@@ -202,19 +215,21 @@
     "_OptionalCreateSubnetGroupRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateSubnetGroupRequestRequestTypeDef(
     _RequiredCreateSubnetGroupRequestRequestTypeDef, _OptionalCreateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDecreaseReplicationFactorRequestRequestTypeDef = TypedDict(
     "_RequiredDecreaseReplicationFactorRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NewReplicationFactor": int,
     },
 )
@@ -223,106 +238,72 @@
     {
         "AvailabilityZones": Sequence[str],
         "NodeIdsToRemove": Sequence[str],
     },
     total=False,
 )
 
+
 class DecreaseReplicationFactorRequestRequestTypeDef(
     _RequiredDecreaseReplicationFactorRequestRequestTypeDef,
     _OptionalDecreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteClusterRequestRequestTypeDef = TypedDict(
     "DeleteClusterRequestRequestTypeDef",
     {
         "ClusterName": str,
     },
 )
 
 DeleteParameterGroupRequestRequestTypeDef = TypedDict(
     "DeleteParameterGroupRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 
-DeleteParameterGroupResponseTypeDef = TypedDict(
-    "DeleteParameterGroupResponseTypeDef",
-    {
-        "DeletionMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteSubnetGroupRequestRequestTypeDef = TypedDict(
     "DeleteSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 
-DeleteSubnetGroupResponseTypeDef = TypedDict(
-    "DeleteSubnetGroupResponseTypeDef",
-    {
-        "DeletionMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "ClusterNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = TypedDict(
-    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDefaultParametersRequestRequestTypeDef = TypedDict(
     "DescribeDefaultParametersRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "SourceName": str,
-        "SourceType": SourceTypeType,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Duration": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEventsRequestRequestTypeDef = TypedDict(
     "DescribeEventsRequestRequestTypeDef",
     {
         "SourceName": str,
         "SourceType": SourceTypeType,
         "StartTime": Union[datetime, str],
         "EndTime": Union[datetime, str],
@@ -340,54 +321,24 @@
         "SourceType": SourceTypeType,
         "Message": str,
         "Date": datetime,
     },
     total=False,
 )
 
-DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
-    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
-    {
-        "ParameterGroupNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeParameterGroupsRequestRequestTypeDef = TypedDict(
     "DescribeParameterGroupsRequestRequestTypeDef",
     {
         "ParameterGroupNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
-    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
-    {
-        "Source": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeParametersRequestDescribeParametersPaginateTypeDef(
-    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
-    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeParametersRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeParametersRequestRequestTypeDef",
     {
         "ParameterGroupName": str,
     },
 )
 _OptionalDescribeParametersRequestRequestTypeDef = TypedDict(
@@ -396,28 +347,21 @@
         "Source": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class DescribeParametersRequestRequestTypeDef(
     _RequiredDescribeParametersRequestRequestTypeDef,
     _OptionalDescribeParametersRequestRequestTypeDef,
 ):
     pass
 
-DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
-    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
-    {
-        "SubnetGroupNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 DescribeSubnetGroupsRequestRequestTypeDef = TypedDict(
     "DescribeSubnetGroupsRequestRequestTypeDef",
     {
         "SubnetGroupNames": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
@@ -436,38 +380,21 @@
     "_OptionalIncreaseReplicationFactorRequestRequestTypeDef",
     {
         "AvailabilityZones": Sequence[str],
     },
     total=False,
 )
 
+
 class IncreaseReplicationFactorRequestRequestTypeDef(
     _RequiredIncreaseReplicationFactorRequestRequestTypeDef,
     _OptionalIncreaseReplicationFactorRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceName": str,
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
 
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceName": str,
     },
 )
@@ -475,47 +402,30 @@
     "_OptionalListTagsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
 
 NodeTypeSpecificValueTypeDef = TypedDict(
     "NodeTypeSpecificValueTypeDef",
     {
         "NodeType": str,
         "Value": str,
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
 ParameterNameValueTypeDef = TypedDict(
     "ParameterNameValueTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
     },
     total=False,
@@ -525,25 +435,14 @@
     "RebootNodeRequestRequestTypeDef",
     {
         "ClusterName": str,
         "NodeId": str,
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
 SubnetTypeDef = TypedDict(
     "SubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": str,
     },
     total=False,
@@ -572,19 +471,21 @@
         "NotificationTopicStatus": str,
         "ParameterGroupName": str,
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateClusterRequestRequestTypeDef(
     _RequiredUpdateClusterRequestRequestTypeDef, _OptionalUpdateClusterRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSubnetGroupRequestRequestTypeDef",
     {
         "SubnetGroupName": str,
     },
 )
 _OptionalUpdateSubnetGroupRequestRequestTypeDef = TypedDict(
@@ -592,19 +493,21 @@
     {
         "Description": str,
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateSubnetGroupRequestRequestTypeDef(
     _RequiredUpdateSubnetGroupRequestRequestTypeDef, _OptionalUpdateSubnetGroupRequestRequestTypeDef
 ):
     pass
 
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NodeId": str,
         "Endpoint": EndpointTypeDef,
         "NodeCreateTime": datetime,
         "AvailabilityZone": str,
@@ -636,83 +539,193 @@
         "Tags": Sequence[TagTypeDef],
         "SSESpecification": SSESpecificationTypeDef,
         "ClusterEndpointEncryptionType": ClusterEndpointEncryptionTypeType,
     },
     total=False,
 )
 
+
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceName": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DeleteParameterGroupResponseTypeDef = TypedDict(
+    "DeleteParameterGroupResponseTypeDef",
+    {
+        "DeletionMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSubnetGroupResponseTypeDef = TypedDict(
+    "DeleteSubnetGroupResponseTypeDef",
+    {
+        "DeletionMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceResponseTypeDef = TypedDict(
+    "TagResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UntagResourceResponseTypeDef = TypedDict(
+    "UntagResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateParameterGroupResponseTypeDef = TypedDict(
     "CreateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeParameterGroupsResponseTypeDef = TypedDict(
     "DescribeParameterGroupsResponseTypeDef",
     {
         "NextToken": str,
         "ParameterGroups": List[ParameterGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateParameterGroupResponseTypeDef = TypedDict(
     "UpdateParameterGroupResponseTypeDef",
     {
         "ParameterGroup": ParameterGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeEventsResponseTypeDef = TypedDict(
-    "DescribeEventsResponseTypeDef",
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     {
-        "NextToken": str,
-        "Events": List[EventTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClusterNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
+DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef = TypedDict(
+    "DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "SourceName": str,
+        "SourceType": SourceTypeType,
+        "StartTime": Union[datetime, str],
+        "EndTime": Union[datetime, str],
+        "Duration": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-TagResourceResponseTypeDef = TypedDict(
-    "TagResourceResponseTypeDef",
+DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef = TypedDict(
+    "DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ParameterGroupNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-UntagResourceResponseTypeDef = TypedDict(
-    "UntagResourceResponseTypeDef",
+_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "ParameterGroupName": str,
+    },
+)
+_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef = TypedDict(
+    "_OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef",
+    {
+        "Source": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeParametersRequestDescribeParametersPaginateTypeDef(
+    _RequiredDescribeParametersRequestDescribeParametersPaginateTypeDef,
+    _OptionalDescribeParametersRequestDescribeParametersPaginateTypeDef,
+):
+    pass
+
+
+DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef = TypedDict(
+    "DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SubnetGroupNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceName": str,
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
+
+DescribeEventsResponseTypeDef = TypedDict(
+    "DescribeEventsResponseTypeDef",
+    {
+        "NextToken": str,
+        "Events": List[EventTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParameterTypeDef = TypedDict(
     "ParameterTypeDef",
     {
         "ParameterName": str,
@@ -774,101 +787,101 @@
 )
 
 DescribeDefaultParametersResponseTypeDef = TypedDict(
     "DescribeDefaultParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeParametersResponseTypeDef = TypedDict(
     "DescribeParametersResponseTypeDef",
     {
         "NextToken": str,
         "Parameters": List[ParameterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSubnetGroupResponseTypeDef = TypedDict(
     "CreateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSubnetGroupsResponseTypeDef = TypedDict(
     "DescribeSubnetGroupsResponseTypeDef",
     {
         "NextToken": str,
         "SubnetGroups": List[SubnetGroupTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSubnetGroupResponseTypeDef = TypedDict(
     "UpdateSubnetGroupResponseTypeDef",
     {
         "SubnetGroup": SubnetGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DecreaseReplicationFactorResponseTypeDef = TypedDict(
     "DecreaseReplicationFactorResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "NextToken": str,
         "Clusters": List[ClusterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IncreaseReplicationFactorResponseTypeDef = TypedDict(
     "IncreaseReplicationFactorResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootNodeResponseTypeDef = TypedDict(
     "RebootNodeResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterResponseTypeDef = TypedDict(
     "UpdateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/PKG-INFO` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dax
-Version: 1.28.12
-Summary: Type annotations for boto3.DAX 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DAX 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dax.svg?color=blue)](https://pypi.org/project/mypy-boto3-dax)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dax)](https://pepy.tech/project/mypy-boto3-dax)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DAX 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
+[boto3.DAX 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dax.html#DAX)
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
 [mypy-boto3-dax docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dax/).
 
 See how it helps to find and fix potential bugs:
 
@@ -358,59 +358,58 @@
     EndpointTypeDef,
     NotificationConfigurationTypeDef,
     ParameterGroupStatusTypeDef,
     SSEDescriptionTypeDef,
     SecurityGroupMembershipTypeDef,
     SSESpecificationTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     CreateParameterGroupRequestRequestTypeDef,
     ParameterGroupTypeDef,
     CreateSubnetGroupRequestRequestTypeDef,
     DecreaseReplicationFactorRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteParameterGroupRequestRequestTypeDef,
-    DeleteParameterGroupResponseTypeDef,
     DeleteSubnetGroupRequestRequestTypeDef,
-    DeleteSubnetGroupResponseTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClustersRequestRequestTypeDef,
-    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
     DescribeDefaultParametersRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     EventTypeDef,
-    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
     DescribeParameterGroupsRequestRequestTypeDef,
-    DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
-    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
     DescribeSubnetGroupsRequestRequestTypeDef,
     IncreaseReplicationFactorRequestRequestTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     NodeTypeSpecificValueTypeDef,
-    PaginatorConfigTypeDef,
     ParameterNameValueTypeDef,
     RebootNodeRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SubnetTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterRequestRequestTypeDef,
     UpdateSubnetGroupRequestRequestTypeDef,
     NodeTypeDef,
     CreateClusterRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    DeleteParameterGroupResponseTypeDef,
+    DeleteSubnetGroupResponseTypeDef,
+    ListTagsResponseTypeDef,
+    TagResourceResponseTypeDef,
+    UntagResourceResponseTypeDef,
     CreateParameterGroupResponseTypeDef,
     DescribeParameterGroupsResponseTypeDef,
     UpdateParameterGroupResponseTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    DescribeDefaultParametersRequestDescribeDefaultParametersPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeParameterGroupsRequestDescribeParameterGroupsPaginateTypeDef,
+    DescribeParametersRequestDescribeParametersPaginateTypeDef,
+    DescribeSubnetGroupsRequestDescribeSubnetGroupsPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DescribeEventsResponseTypeDef,
-    ListTagsResponseTypeDef,
-    TagResourceResponseTypeDef,
-    UntagResourceResponseTypeDef,
     ParameterTypeDef,
     UpdateParameterGroupRequestRequestTypeDef,
     SubnetGroupTypeDef,
     ClusterTypeDef,
     DescribeDefaultParametersResponseTypeDef,
     DescribeParametersResponseTypeDef,
     CreateSubnetGroupResponseTypeDef,
```

### Comparing `mypy-boto3-dax-1.28.12/mypy_boto3_dax.egg-info/SOURCES.txt` & `mypy-boto3-dax-1.28.15/mypy_boto3_dax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dax-1.28.12/setup.py` & `mypy-boto3-dax-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dax",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_dax"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DAX 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.DAX 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

