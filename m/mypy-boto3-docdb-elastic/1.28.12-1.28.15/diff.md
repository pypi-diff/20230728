# Comparing `tmp/mypy-boto3-docdb-elastic-1.28.12.tar.gz` & `tmp/mypy-boto3-docdb-elastic-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-docdb-elastic-1.28.12.tar", last modified: Thu Jul 27 05:34:35 2023, max compression
+gzip compressed data, was "mypy-boto3-docdb-elastic-1.28.15.tar", last modified: Fri Jul 28 20:42:40 2023, max compression
```

## Comparing `mypy-boto3-docdb-elastic-1.28.12.tar` & `mypy-boto3-docdb-elastic-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.692529 mypy-boto3-docdb-elastic-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-07-27 05:34:35.692529 mypy-boto3-docdb-elastic-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.684529 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10284 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.692529 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-07-27 05:34:35.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:35.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:35.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:35.000000 mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:35.692529 mypy-boto3-docdb-elastic-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 05:20:28.000000 mypy-boto3-docdb-elastic-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.652998 mypy-boto3-docdb-elastic-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:15.000000 mypy-boto3-docdb-elastic-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-07-28 20:42:40.652998 mypy-boto3-docdb-elastic-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-28 20:23:15.000000 mypy-boto3-docdb-elastic-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.644998 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-07-28 20:23:15.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-28 20:23:15.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-28 20:23:15.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-28 20:23:17.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-07-28 20:23:16.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8227 2023-07-28 20:23:17.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-28 20:23:17.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-07-28 20:23:17.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-07-28 20:23:17.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:15.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-07-28 20:23:17.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-07-28 20:23:17.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:15.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:40.652998 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14179 2023-07-28 20:42:40.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:42:40.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:40.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:40.000000 mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:40.652998 mypy-boto3-docdb-elastic-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-28 20:23:15.000000 mypy-boto3-docdb-elastic-1.28.15/setup.py
```

### Comparing `mypy-boto3-docdb-elastic-1.28.12/LICENSE` & `mypy-boto3-docdb-elastic-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.28.12/PKG-INFO` & `mypy-boto3-docdb-elastic-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb-elastic
-Version: 1.28.12
-Summary: Type annotations for boto3.DocDBElastic 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DocDBElastic 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb-elastic)](https://pepy.tech/project/mypy-boto3-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDBElastic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[boto3.DocDBElastic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [mypy-boto3-docdb-elastic docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,41 +329,41 @@
 ```python
 from mypy_boto3_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    ListClustersOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
     CreateClusterOutputTypeDef,
+    CreateClusterSnapshotOutputTypeDef,
     DeleteClusterOutputTypeDef,
+    DeleteClusterSnapshotOutputTypeDef,
     GetClusterOutputTypeDef,
+    GetClusterSnapshotOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
 def get_structure() -> ClusterInListTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-docdb-elastic-1.28.12/README.md` & `mypy-boto3-docdb-elastic-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb-elastic)](https://pepy.tech/project/mypy-boto3-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDBElastic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[boto3.DocDBElastic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [mypy-boto3-docdb-elastic docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,41 +297,41 @@
 ```python
 from mypy_boto3_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    ListClustersOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
     CreateClusterOutputTypeDef,
+    CreateClusterSnapshotOutputTypeDef,
     DeleteClusterOutputTypeDef,
+    DeleteClusterSnapshotOutputTypeDef,
     GetClusterOutputTypeDef,
+    GetClusterSnapshotOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
 def get_structure() -> ClusterInListTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/__init__.py` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/__init__.pyi` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/__main__.py` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DocDBElastic 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.DocDBElastic 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic\nOther"
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

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/client.py` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/client.pyi` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/literals.py` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/literals.pyi` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/paginator.py` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,28 +47,28 @@
 class ListClusterSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclustersnapshotspaginator)
     """
 
     def paginate(
-        self, *, clusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClusterSnapshotsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclustersnapshotspaginator)
         """
 
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclusterspaginator)
         """
```

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/paginator.pyi` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,27 +44,27 @@
 class ListClusterSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclustersnapshotspaginator)
     """
 
     def paginate(
-        self, *, clusterArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, clusterArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClusterSnapshotsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusterSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclustersnapshotspaginator)
         """
 
 class ListClustersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclusterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/paginators/#listclusterspaginator)
         """
```

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/type_defs.py` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -17,48 +17,47 @@
 from .literals import AuthType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ClusterInListTypeDef",
     "ClusterSnapshotInListTypeDef",
     "ClusterSnapshotTypeDef",
     "ClusterTypeDef",
     "CreateClusterInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateClusterSnapshotInputRequestTypeDef",
     "DeleteClusterInputRequestTypeDef",
     "DeleteClusterSnapshotInputRequestTypeDef",
     "GetClusterInputRequestTypeDef",
     "GetClusterSnapshotInputRequestTypeDef",
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListClusterSnapshotsInputRequestTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreClusterFromSnapshotInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterInputRequestTypeDef",
-    "ListClustersOutputTypeDef",
-    "ListClusterSnapshotsOutputTypeDef",
-    "CreateClusterSnapshotOutputTypeDef",
-    "DeleteClusterSnapshotOutputTypeDef",
-    "GetClusterSnapshotOutputTypeDef",
     "CreateClusterOutputTypeDef",
+    "CreateClusterSnapshotOutputTypeDef",
     "DeleteClusterOutputTypeDef",
+    "DeleteClusterSnapshotOutputTypeDef",
     "GetClusterOutputTypeDef",
+    "GetClusterSnapshotOutputTypeDef",
+    "ListClusterSnapshotsOutputTypeDef",
+    "ListClustersOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RestoreClusterFromSnapshotOutputTypeDef",
     "UpdateClusterOutputTypeDef",
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
 )
 
 ClusterInListTypeDef = TypedDict(
     "ClusterInListTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
@@ -132,20 +131,29 @@
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateClusterInputRequestTypeDef(
     _RequiredCreateClusterInputRequestTypeDef, _OptionalCreateClusterInputRequestTypeDef
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
 
 _RequiredCreateClusterSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotInputRequestTypeDef",
     {
         "clusterArn": str,
         "snapshotName": str,
     },
@@ -154,22 +162,20 @@
     "_OptionalCreateClusterSnapshotInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateClusterSnapshotInputRequestTypeDef(
     _RequiredCreateClusterSnapshotInputRequestTypeDef,
     _OptionalCreateClusterSnapshotInputRequestTypeDef,
 ):
     pass
 
-
 DeleteClusterInputRequestTypeDef = TypedDict(
     "DeleteClusterInputRequestTypeDef",
     {
         "clusterArn": str,
     },
 )
 
@@ -190,41 +196,34 @@
 GetClusterSnapshotInputRequestTypeDef = TypedDict(
     "GetClusterSnapshotInputRequestTypeDef",
     {
         "snapshotArn": str,
     },
 )
 
-ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "clusterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListClusterSnapshotsInputRequestTypeDef = TypedDict(
     "ListClusterSnapshotsInputRequestTypeDef",
     {
         "clusterArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -233,43 +232,14 @@
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
 _RequiredRestoreClusterFromSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredRestoreClusterFromSnapshotInputRequestTypeDef",
     {
         "clusterName": str,
         "snapshotArn": str,
     },
 )
@@ -280,22 +250,20 @@
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class RestoreClusterFromSnapshotInputRequestTypeDef(
     _RequiredRestoreClusterFromSnapshotInputRequestTypeDef,
     _OptionalRestoreClusterFromSnapshotInputRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -325,95 +293,118 @@
         "shardCount": int,
         "subnetIds": Sequence[str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-
 class UpdateClusterInputRequestTypeDef(
     _RequiredUpdateClusterInputRequestTypeDef, _OptionalUpdateClusterInputRequestTypeDef
 ):
     pass
 
-
-ListClustersOutputTypeDef = TypedDict(
-    "ListClustersOutputTypeDef",
+CreateClusterOutputTypeDef = TypedDict(
+    "CreateClusterOutputTypeDef",
     {
-        "clusters": List[ClusterInListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListClusterSnapshotsOutputTypeDef = TypedDict(
-    "ListClusterSnapshotsOutputTypeDef",
+CreateClusterSnapshotOutputTypeDef = TypedDict(
+    "CreateClusterSnapshotOutputTypeDef",
     {
-        "nextToken": str,
-        "snapshots": List[ClusterSnapshotInListTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "snapshot": ClusterSnapshotTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterSnapshotOutputTypeDef = TypedDict(
-    "CreateClusterSnapshotOutputTypeDef",
+DeleteClusterOutputTypeDef = TypedDict(
+    "DeleteClusterOutputTypeDef",
     {
-        "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterSnapshotOutputTypeDef = TypedDict(
     "DeleteClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetClusterOutputTypeDef = TypedDict(
+    "GetClusterOutputTypeDef",
+    {
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetClusterSnapshotOutputTypeDef = TypedDict(
     "GetClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterOutputTypeDef = TypedDict(
-    "CreateClusterOutputTypeDef",
+ListClusterSnapshotsOutputTypeDef = TypedDict(
+    "ListClusterSnapshotsOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "nextToken": str,
+        "snapshots": List[ClusterSnapshotInListTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteClusterOutputTypeDef = TypedDict(
-    "DeleteClusterOutputTypeDef",
+ListClustersOutputTypeDef = TypedDict(
+    "ListClustersOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "clusters": List[ClusterInListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetClusterOutputTypeDef = TypedDict(
-    "GetClusterOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreClusterFromSnapshotOutputTypeDef = TypedDict(
     "RestoreClusterFromSnapshotOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterOutputTypeDef = TypedDict(
     "UpdateClusterOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    {
+        "clusterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
```

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic/type_defs.pyi` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,47 +17,48 @@
 from .literals import AuthType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ClusterInListTypeDef",
     "ClusterSnapshotInListTypeDef",
     "ClusterSnapshotTypeDef",
     "ClusterTypeDef",
     "CreateClusterInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateClusterSnapshotInputRequestTypeDef",
     "DeleteClusterInputRequestTypeDef",
     "DeleteClusterSnapshotInputRequestTypeDef",
     "GetClusterInputRequestTypeDef",
     "GetClusterSnapshotInputRequestTypeDef",
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListClusterSnapshotsInputRequestTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreClusterFromSnapshotInputRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateClusterInputRequestTypeDef",
-    "ListClustersOutputTypeDef",
-    "ListClusterSnapshotsOutputTypeDef",
-    "CreateClusterSnapshotOutputTypeDef",
-    "DeleteClusterSnapshotOutputTypeDef",
-    "GetClusterSnapshotOutputTypeDef",
     "CreateClusterOutputTypeDef",
+    "CreateClusterSnapshotOutputTypeDef",
     "DeleteClusterOutputTypeDef",
+    "DeleteClusterSnapshotOutputTypeDef",
     "GetClusterOutputTypeDef",
+    "GetClusterSnapshotOutputTypeDef",
+    "ListClusterSnapshotsOutputTypeDef",
+    "ListClustersOutputTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "RestoreClusterFromSnapshotOutputTypeDef",
     "UpdateClusterOutputTypeDef",
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
 )
 
 ClusterInListTypeDef = TypedDict(
     "ClusterInListTypeDef",
     {
         "clusterArn": str,
         "clusterName": str,
@@ -131,19 +132,32 @@
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateClusterInputRequestTypeDef(
     _RequiredCreateClusterInputRequestTypeDef, _OptionalCreateClusterInputRequestTypeDef
 ):
     pass
 
+
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
 _RequiredCreateClusterSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredCreateClusterSnapshotInputRequestTypeDef",
     {
         "clusterArn": str,
         "snapshotName": str,
     },
 )
@@ -151,20 +165,22 @@
     "_OptionalCreateClusterSnapshotInputRequestTypeDef",
     {
         "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateClusterSnapshotInputRequestTypeDef(
     _RequiredCreateClusterSnapshotInputRequestTypeDef,
     _OptionalCreateClusterSnapshotInputRequestTypeDef,
 ):
     pass
 
+
 DeleteClusterInputRequestTypeDef = TypedDict(
     "DeleteClusterInputRequestTypeDef",
     {
         "clusterArn": str,
     },
 )
 
@@ -185,41 +201,34 @@
 GetClusterSnapshotInputRequestTypeDef = TypedDict(
     "GetClusterSnapshotInputRequestTypeDef",
     {
         "snapshotArn": str,
     },
 )
 
-ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
-    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "clusterArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListClusterSnapshotsInputRequestTypeDef = TypedDict(
     "ListClusterSnapshotsInputRequestTypeDef",
     {
         "clusterArn": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -228,43 +237,14 @@
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
 _RequiredRestoreClusterFromSnapshotInputRequestTypeDef = TypedDict(
     "_RequiredRestoreClusterFromSnapshotInputRequestTypeDef",
     {
         "clusterName": str,
         "snapshotArn": str,
     },
 )
@@ -275,20 +255,22 @@
         "subnetIds": Sequence[str],
         "tags": Mapping[str, str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class RestoreClusterFromSnapshotInputRequestTypeDef(
     _RequiredRestoreClusterFromSnapshotInputRequestTypeDef,
     _OptionalRestoreClusterFromSnapshotInputRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -318,93 +300,120 @@
         "shardCount": int,
         "subnetIds": Sequence[str],
         "vpcSecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
+
 class UpdateClusterInputRequestTypeDef(
     _RequiredUpdateClusterInputRequestTypeDef, _OptionalUpdateClusterInputRequestTypeDef
 ):
     pass
 
-ListClustersOutputTypeDef = TypedDict(
-    "ListClustersOutputTypeDef",
-    {
-        "clusters": List[ClusterInListTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-ListClusterSnapshotsOutputTypeDef = TypedDict(
-    "ListClusterSnapshotsOutputTypeDef",
+CreateClusterOutputTypeDef = TypedDict(
+    "CreateClusterOutputTypeDef",
     {
-        "nextToken": str,
-        "snapshots": List[ClusterSnapshotInListTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterSnapshotOutputTypeDef = TypedDict(
     "CreateClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteClusterOutputTypeDef = TypedDict(
+    "DeleteClusterOutputTypeDef",
+    {
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterSnapshotOutputTypeDef = TypedDict(
     "DeleteClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetClusterOutputTypeDef = TypedDict(
+    "GetClusterOutputTypeDef",
+    {
+        "cluster": ClusterTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetClusterSnapshotOutputTypeDef = TypedDict(
     "GetClusterSnapshotOutputTypeDef",
     {
         "snapshot": ClusterSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateClusterOutputTypeDef = TypedDict(
-    "CreateClusterOutputTypeDef",
+ListClusterSnapshotsOutputTypeDef = TypedDict(
+    "ListClusterSnapshotsOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "nextToken": str,
+        "snapshots": List[ClusterSnapshotInListTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DeleteClusterOutputTypeDef = TypedDict(
-    "DeleteClusterOutputTypeDef",
+ListClustersOutputTypeDef = TypedDict(
+    "ListClustersOutputTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "clusters": List[ClusterInListTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetClusterOutputTypeDef = TypedDict(
-    "GetClusterOutputTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreClusterFromSnapshotOutputTypeDef = TypedDict(
     "RestoreClusterFromSnapshotOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateClusterOutputTypeDef = TypedDict(
     "UpdateClusterOutputTypeDef",
     {
         "cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef = TypedDict(
+    "ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef",
+    {
+        "clusterArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
```

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/PKG-INFO` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-docdb-elastic
-Version: 1.28.12
-Summary: Type annotations for boto3.DocDBElastic 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DocDBElastic 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-docdb-elastic.svg?color=blue)](https://pypi.org/project/mypy-boto3-docdb-elastic)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-docdb-elastic)](https://pepy.tech/project/mypy-boto3-docdb-elastic)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DocDBElastic 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
+[boto3.DocDBElastic 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic)
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
 [mypy-boto3-docdb-elastic docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -329,41 +329,41 @@
 ```python
 from mypy_boto3_docdb_elastic.type_defs import (
     ClusterInListTypeDef,
     ClusterSnapshotInListTypeDef,
     ClusterSnapshotTypeDef,
     ClusterTypeDef,
     CreateClusterInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     CreateClusterSnapshotInputRequestTypeDef,
     DeleteClusterInputRequestTypeDef,
     DeleteClusterSnapshotInputRequestTypeDef,
     GetClusterInputRequestTypeDef,
     GetClusterSnapshotInputRequestTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreClusterFromSnapshotInputRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateClusterInputRequestTypeDef,
-    ListClustersOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
     CreateClusterOutputTypeDef,
+    CreateClusterSnapshotOutputTypeDef,
     DeleteClusterOutputTypeDef,
+    DeleteClusterSnapshotOutputTypeDef,
     GetClusterOutputTypeDef,
+    GetClusterSnapshotOutputTypeDef,
+    ListClusterSnapshotsOutputTypeDef,
+    ListClustersOutputTypeDef,
+    ListTagsForResourceResponseTypeDef,
     RestoreClusterFromSnapshotOutputTypeDef,
     UpdateClusterOutputTypeDef,
+    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
 )
 
 
 def get_structure() -> ClusterInListTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-docdb-elastic-1.28.12/mypy_boto3_docdb_elastic.egg-info/SOURCES.txt` & `mypy-boto3-docdb-elastic-1.28.15/mypy_boto3_docdb_elastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-docdb-elastic-1.28.12/setup.py` & `mypy-boto3-docdb-elastic-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-docdb-elastic",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_docdb_elastic"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DocDBElastic 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.DocDBElastic 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

