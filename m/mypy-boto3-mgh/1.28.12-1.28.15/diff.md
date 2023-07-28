# Comparing `tmp/mypy-boto3-mgh-1.28.12.tar.gz` & `tmp/mypy-boto3-mgh-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mgh-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
+gzip compressed data, was "mypy-boto3-mgh-1.28.15.tar", last modified: Fri Jul 28 20:43:18 2023, max compression
```

## Comparing `mypy-boto3-mgh-1.28.12.tar` & `mypy-boto3-mgh-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.868434 mypy-boto3-mgh-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-07-27 05:35:02.868434 mypy-boto3-mgh-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.864434 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6546 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19267 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19226 2023-07-27 05:26:34.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.868434 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15168 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:35:02.000000 mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.868434 mypy-boto3-mgh-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-27 05:26:33.000000 mypy-boto3-mgh-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.445517 mypy-boto3-mgh-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15038 2023-07-28 20:43:18.445517 mypy-boto3-mgh-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13558 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.429517 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17205 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17176 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-07-28 20:31:54.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17629 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:53.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.445517 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15038 2023-07-28 20:43:18.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:43:18.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:18.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:18.000000 mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:18.445517 mypy-boto3-mgh-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-28 20:31:52.000000 mypy-boto3-mgh-1.28.15/setup.py
```

### Comparing `mypy-boto3-mgh-1.28.12/LICENSE` & `mypy-boto3-mgh-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.12/PKG-INFO` & `mypy-boto3-mgh-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgh
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,52 +348,48 @@
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
-    CreatedArtifactOutputTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
-    DescribeApplicationStateResultTypeDef,
+    ResponseMetadataTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
-    DiscoveredResourceOutputTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
-    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
-    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
-    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
-    ResourceAttributeOutputTypeDef,
-    TaskOutputTypeDef,
-    NotifyApplicationStateRequestRequestTypeDef,
-    TaskTypeDef,
-    PaginatorConfigTypeDef,
     ResourceAttributeTypeDef,
-    ResponseMetadataTypeDef,
-    ListApplicationStatesResultTypeDef,
+    TaskTypeDef,
+    NotifyApplicationStateRequestRequestTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
+    DescribeApplicationStateResultTypeDef,
+    ListApplicationStatesResultTypeDef,
     ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
+    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
+    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
+    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
+    PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
-    PutResourceAttributesRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
 def get_structure() -> ApplicationStateTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mgh-1.28.12/README.md` & `mypy-boto3-mgh-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -316,52 +316,48 @@
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
-    CreatedArtifactOutputTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
-    DescribeApplicationStateResultTypeDef,
+    ResponseMetadataTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
-    DiscoveredResourceOutputTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
-    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
-    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
-    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
-    ResourceAttributeOutputTypeDef,
-    TaskOutputTypeDef,
-    NotifyApplicationStateRequestRequestTypeDef,
-    TaskTypeDef,
-    PaginatorConfigTypeDef,
     ResourceAttributeTypeDef,
-    ResponseMetadataTypeDef,
-    ListApplicationStatesResultTypeDef,
+    TaskTypeDef,
+    NotifyApplicationStateRequestRequestTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
+    DescribeApplicationStateResultTypeDef,
+    ListApplicationStatesResultTypeDef,
     ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
+    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
+    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
+    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
+    PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
-    PutResourceAttributesRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
 def get_structure() -> ApplicationStateTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__init__.py` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__init__.pyi` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/__main__.py` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MigrationHub 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MigrationHub 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub\nOther"
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

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/client.py` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/client.pyi` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/literals.py` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/literals.pyi` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/paginator.py` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -44,102 +44,92 @@
     "ListApplicationStatesPaginator",
     "ListCreatedArtifactsPaginator",
     "ListDiscoveredResourcesPaginator",
     "ListMigrationTasksPaginator",
     "ListProgressUpdateStreamsPaginator",
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
 class ListApplicationStatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listapplicationstatespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ApplicationIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listapplicationstatespaginator)
         """
 
-
 class ListCreatedArtifactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listcreatedartifactspaginator)
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCreatedArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listcreatedartifactspaginator)
         """
 
-
 class ListDiscoveredResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listdiscoveredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDiscoveredResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listdiscoveredresourcespaginator)
         """
 
-
 class ListMigrationTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listmigrationtaskspaginator)
     """
 
     def paginate(
-        self, *, ResourceName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMigrationTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listmigrationtaskspaginator)
         """
 
-
 class ListProgressUpdateStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listprogressupdatestreamspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProgressUpdateStreamsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listprogressupdatestreamspaginator)
         """
```

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/paginator.pyi` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,95 +44,99 @@
     "ListApplicationStatesPaginator",
     "ListCreatedArtifactsPaginator",
     "ListDiscoveredResourcesPaginator",
     "ListMigrationTasksPaginator",
     "ListProgressUpdateStreamsPaginator",
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
 class ListApplicationStatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listapplicationstatespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ApplicationIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApplicationIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListApplicationStatesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListApplicationStates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listapplicationstatespaginator)
         """
 
+
 class ListCreatedArtifactsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listcreatedartifactspaginator)
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCreatedArtifactsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListCreatedArtifacts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listcreatedartifactspaginator)
         """
 
+
 class ListDiscoveredResourcesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listdiscoveredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         ProgressUpdateStream: str,
         MigrationTaskName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDiscoveredResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListDiscoveredResources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listdiscoveredresourcespaginator)
         """
 
+
 class ListMigrationTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listmigrationtaskspaginator)
     """
 
     def paginate(
-        self, *, ResourceName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMigrationTasksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListMigrationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listmigrationtaskspaginator)
         """
 
+
 class ListProgressUpdateStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listprogressupdatestreamspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProgressUpdateStreamsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub.Paginator.ListProgressUpdateStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/paginators/#listprogressupdatestreamspaginator)
         """
```

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/type_defs.py` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -18,58 +18,53 @@
 from .literals import ApplicationStatusType, ResourceAttributeTypeType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ApplicationStateTypeDef",
     "CreatedArtifactTypeDef",
     "DiscoveredResourceTypeDef",
     "CreateProgressUpdateStreamRequestRequestTypeDef",
-    "CreatedArtifactOutputTypeDef",
     "DeleteProgressUpdateStreamRequestRequestTypeDef",
     "DescribeApplicationStateRequestRequestTypeDef",
-    "DescribeApplicationStateResultTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeMigrationTaskRequestRequestTypeDef",
     "DisassociateCreatedArtifactRequestRequestTypeDef",
     "DisassociateDiscoveredResourceRequestRequestTypeDef",
-    "DiscoveredResourceOutputTypeDef",
     "ImportMigrationTaskRequestRequestTypeDef",
-    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationStatesRequestRequestTypeDef",
-    "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     "ListCreatedArtifactsRequestRequestTypeDef",
-    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
-    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     "ListMigrationTasksRequestRequestTypeDef",
     "MigrationTaskSummaryTypeDef",
-    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     "ProgressUpdateStreamSummaryTypeDef",
-    "ResourceAttributeOutputTypeDef",
-    "TaskOutputTypeDef",
-    "NotifyApplicationStateRequestRequestTypeDef",
-    "TaskTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceAttributeTypeDef",
-    "ResponseMetadataTypeDef",
-    "ListApplicationStatesResultTypeDef",
+    "TaskTypeDef",
+    "NotifyApplicationStateRequestRequestTypeDef",
     "AssociateCreatedArtifactRequestRequestTypeDef",
     "AssociateDiscoveredResourceRequestRequestTypeDef",
+    "DescribeApplicationStateResultTypeDef",
+    "ListApplicationStatesResultTypeDef",
     "ListCreatedArtifactsResultTypeDef",
     "ListDiscoveredResourcesResultTypeDef",
+    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
+    "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
+    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
+    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListMigrationTasksResultTypeDef",
     "ListProgressUpdateStreamsResultTypeDef",
+    "PutResourceAttributesRequestRequestTypeDef",
     "MigrationTaskTypeDef",
     "NotifyMigrationTaskStateRequestRequestTypeDef",
-    "PutResourceAttributesRequestRequestTypeDef",
     "DescribeMigrationTaskResultTypeDef",
 )
 
 ApplicationStateTypeDef = TypedDict(
     "ApplicationStateTypeDef",
     {
         "ApplicationId": str,
@@ -89,118 +84,91 @@
     "_OptionalCreatedArtifactTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class CreatedArtifactTypeDef(_RequiredCreatedArtifactTypeDef, _OptionalCreatedArtifactTypeDef):
     pass
 
-
 _RequiredDiscoveredResourceTypeDef = TypedDict(
     "_RequiredDiscoveredResourceTypeDef",
     {
         "ConfigurationId": str,
     },
 )
 _OptionalDiscoveredResourceTypeDef = TypedDict(
     "_OptionalDiscoveredResourceTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class DiscoveredResourceTypeDef(
     _RequiredDiscoveredResourceTypeDef, _OptionalDiscoveredResourceTypeDef
 ):
     pass
 
-
 _RequiredCreateProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProgressUpdateStreamRequestRequestTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
 )
 _OptionalCreateProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_OptionalCreateProgressUpdateStreamRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class CreateProgressUpdateStreamRequestRequestTypeDef(
     _RequiredCreateProgressUpdateStreamRequestRequestTypeDef,
     _OptionalCreateProgressUpdateStreamRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredCreatedArtifactOutputTypeDef = TypedDict(
-    "_RequiredCreatedArtifactOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreatedArtifactOutputTypeDef = TypedDict(
-    "_OptionalCreatedArtifactOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class CreatedArtifactOutputTypeDef(
-    _RequiredCreatedArtifactOutputTypeDef, _OptionalCreatedArtifactOutputTypeDef
-):
-    pass
-
-
 _RequiredDeleteProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProgressUpdateStreamRequestRequestTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
 )
 _OptionalDeleteProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_OptionalDeleteProgressUpdateStreamRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class DeleteProgressUpdateStreamRequestRequestTypeDef(
     _RequiredDeleteProgressUpdateStreamRequestRequestTypeDef,
     _OptionalDeleteProgressUpdateStreamRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeApplicationStateRequestRequestTypeDef = TypedDict(
     "DescribeApplicationStateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-DescribeApplicationStateResultTypeDef = TypedDict(
-    "DescribeApplicationStateResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApplicationStatus": ApplicationStatusType,
-        "LastUpdatedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeMigrationTaskRequestRequestTypeDef = TypedDict(
     "DescribeMigrationTaskRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
@@ -220,22 +188,20 @@
     "_OptionalDisassociateCreatedArtifactRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class DisassociateCreatedArtifactRequestRequestTypeDef(
     _RequiredDisassociateCreatedArtifactRequestRequestTypeDef,
     _OptionalDisassociateCreatedArtifactRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredDisassociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateDiscoveredResourceRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "ConfigurationId": str,
     },
@@ -244,43 +210,20 @@
     "_OptionalDisassociateDiscoveredResourceRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class DisassociateDiscoveredResourceRequestRequestTypeDef(
     _RequiredDisassociateDiscoveredResourceRequestRequestTypeDef,
     _OptionalDisassociateDiscoveredResourceRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredDiscoveredResourceOutputTypeDef = TypedDict(
-    "_RequiredDiscoveredResourceOutputTypeDef",
-    {
-        "ConfigurationId": str,
-    },
-)
-_OptionalDiscoveredResourceOutputTypeDef = TypedDict(
-    "_OptionalDiscoveredResourceOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class DiscoveredResourceOutputTypeDef(
-    _RequiredDiscoveredResourceOutputTypeDef, _OptionalDiscoveredResourceOutputTypeDef
-):
-    pass
-
-
 _RequiredImportMigrationTaskRequestRequestTypeDef = TypedDict(
     "_RequiredImportMigrationTaskRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -288,64 +231,40 @@
     "_OptionalImportMigrationTaskRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class ImportMigrationTaskRequestRequestTypeDef(
     _RequiredImportMigrationTaskRequestRequestTypeDef,
     _OptionalImportMigrationTaskRequestRequestTypeDef,
 ):
     pass
 
-
-ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = TypedDict(
-    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ApplicationIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListApplicationStatesRequestRequestTypeDef = TypedDict(
     "ListApplicationStatesRequestRequestTypeDef",
     {
         "ApplicationIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-    },
-)
-_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef(
-    _RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    _OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCreatedArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListCreatedArtifactsRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -354,45 +273,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListCreatedArtifactsRequestRequestTypeDef(
     _RequiredListCreatedArtifactsRequestRequestTypeDef,
     _OptionalListCreatedArtifactsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-    },
-)
-_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
-    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -401,31 +295,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
-ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = TypedDict(
-    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMigrationTasksRequestRequestTypeDef = TypedDict(
     "ListMigrationTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResourceName": str,
     },
@@ -441,22 +324,14 @@
         "ProgressPercent": int,
         "StatusDetail": str,
         "UpdateDateTime": datetime,
     },
     total=False,
 )
 
-ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = TypedDict(
-    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProgressUpdateStreamsRequestRequestTypeDef = TypedDict(
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -466,42 +341,40 @@
     "ProgressUpdateStreamSummaryTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
     total=False,
 )
 
-ResourceAttributeOutputTypeDef = TypedDict(
-    "ResourceAttributeOutputTypeDef",
+ResourceAttributeTypeDef = TypedDict(
+    "ResourceAttributeTypeDef",
     {
         "Type": ResourceAttributeTypeType,
         "Value": str,
     },
 )
 
-_RequiredTaskOutputTypeDef = TypedDict(
-    "_RequiredTaskOutputTypeDef",
+_RequiredTaskTypeDef = TypedDict(
+    "_RequiredTaskTypeDef",
     {
         "Status": StatusType,
     },
 )
-_OptionalTaskOutputTypeDef = TypedDict(
-    "_OptionalTaskOutputTypeDef",
+_OptionalTaskTypeDef = TypedDict(
+    "_OptionalTaskTypeDef",
     {
         "StatusDetail": str,
         "ProgressPercent": int,
     },
     total=False,
 )
 
-
-class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
+class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
-
 _RequiredNotifyApplicationStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyApplicationStateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "Status": ApplicationStatusType,
     },
 )
@@ -510,172 +383,216 @@
     {
         "UpdateDateTime": Union[datetime, str],
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class NotifyApplicationStateRequestRequestTypeDef(
     _RequiredNotifyApplicationStateRequestRequestTypeDef,
     _OptionalNotifyApplicationStateRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredTaskTypeDef = TypedDict(
-    "_RequiredTaskTypeDef",
+_RequiredAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateCreatedArtifactRequestRequestTypeDef",
     {
-        "Status": StatusType,
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+        "CreatedArtifact": CreatedArtifactTypeDef,
     },
 )
-_OptionalTaskTypeDef = TypedDict(
-    "_OptionalTaskTypeDef",
+_OptionalAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateCreatedArtifactRequestRequestTypeDef",
     {
-        "StatusDetail": str,
-        "ProgressPercent": int,
+        "DryRun": bool,
     },
     total=False,
 )
 
-
-class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
+class AssociateCreatedArtifactRequestRequestTypeDef(
+    _RequiredAssociateCreatedArtifactRequestRequestTypeDef,
+    _OptionalAssociateCreatedArtifactRequestRequestTypeDef,
+):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateDiscoveredResourceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+        "DiscoveredResource": DiscoveredResourceTypeDef,
     },
-    total=False,
 )
-
-ResourceAttributeTypeDef = TypedDict(
-    "ResourceAttributeTypeDef",
+_OptionalAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateDiscoveredResourceRequestRequestTypeDef",
     {
-        "Type": ResourceAttributeTypeType,
-        "Value": str,
+        "DryRun": bool,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class AssociateDiscoveredResourceRequestRequestTypeDef(
+    _RequiredAssociateDiscoveredResourceRequestRequestTypeDef,
+    _OptionalAssociateDiscoveredResourceRequestRequestTypeDef,
+):
+    pass
+
+DescribeApplicationStateResultTypeDef = TypedDict(
+    "DescribeApplicationStateResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ApplicationStatus": ApplicationStatusType,
+        "LastUpdatedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationStatesResultTypeDef = TypedDict(
     "ListApplicationStatesResultTypeDef",
     {
         "ApplicationStateList": List[ApplicationStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateCreatedArtifactRequestRequestTypeDef",
+ListCreatedArtifactsResultTypeDef = TypedDict(
+    "ListCreatedArtifactsResultTypeDef",
+    {
+        "NextToken": str,
+        "CreatedArtifactList": List[CreatedArtifactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDiscoveredResourcesResultTypeDef = TypedDict(
+    "ListDiscoveredResourcesResultTypeDef",
+    {
+        "NextToken": str,
+        "DiscoveredResourceList": List[DiscoveredResourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = TypedDict(
+    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
+    {
+        "ApplicationIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
-        "CreatedArtifact": CreatedArtifactTypeDef,
     },
 )
-_OptionalAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateCreatedArtifactRequestRequestTypeDef",
+_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     {
-        "DryRun": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class AssociateCreatedArtifactRequestRequestTypeDef(
-    _RequiredAssociateCreatedArtifactRequestRequestTypeDef,
-    _OptionalAssociateCreatedArtifactRequestRequestTypeDef,
+class ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef(
+    _RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+    _OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
 ):
     pass
 
-
-_RequiredAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateDiscoveredResourceRequestRequestTypeDef",
+_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
-        "DiscoveredResource": DiscoveredResourceTypeDef,
     },
 )
-_OptionalAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateDiscoveredResourceRequestRequestTypeDef",
+_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     {
-        "DryRun": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class AssociateDiscoveredResourceRequestRequestTypeDef(
-    _RequiredAssociateDiscoveredResourceRequestRequestTypeDef,
-    _OptionalAssociateDiscoveredResourceRequestRequestTypeDef,
+class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
+    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
-
-ListCreatedArtifactsResultTypeDef = TypedDict(
-    "ListCreatedArtifactsResultTypeDef",
+ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = TypedDict(
+    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     {
-        "NextToken": str,
-        "CreatedArtifactList": List[CreatedArtifactOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListDiscoveredResourcesResultTypeDef = TypedDict(
-    "ListDiscoveredResourcesResultTypeDef",
+ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = TypedDict(
+    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     {
-        "NextToken": str,
-        "DiscoveredResourceList": List[DiscoveredResourceOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListMigrationTasksResultTypeDef = TypedDict(
     "ListMigrationTasksResultTypeDef",
     {
         "NextToken": str,
         "MigrationTaskSummaryList": List[MigrationTaskSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProgressUpdateStreamsResultTypeDef = TypedDict(
     "ListProgressUpdateStreamsResultTypeDef",
     {
         "ProgressUpdateStreamSummaryList": List[ProgressUpdateStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceAttributesRequestRequestTypeDef",
+    {
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+        "ResourceAttributeList": Sequence[ResourceAttributeTypeDef],
+    },
+)
+_OptionalPutResourceAttributesRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceAttributesRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class PutResourceAttributesRequestRequestTypeDef(
+    _RequiredPutResourceAttributesRequestRequestTypeDef,
+    _OptionalPutResourceAttributesRequestRequestTypeDef,
+):
+    pass
+
 MigrationTaskTypeDef = TypedDict(
     "MigrationTaskTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
-        "Task": TaskOutputTypeDef,
+        "Task": TaskTypeDef,
         "UpdateDateTime": datetime,
-        "ResourceAttributeList": List[ResourceAttributeOutputTypeDef],
+        "ResourceAttributeList": List[ResourceAttributeTypeDef],
     },
     total=False,
 )
 
 _RequiredNotifyMigrationTaskStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyMigrationTaskStateRequestRequestTypeDef",
     {
@@ -690,46 +607,20 @@
     "_OptionalNotifyMigrationTaskStateRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class NotifyMigrationTaskStateRequestRequestTypeDef(
     _RequiredNotifyMigrationTaskStateRequestRequestTypeDef,
     _OptionalNotifyMigrationTaskStateRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceAttributesRequestRequestTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-        "ResourceAttributeList": Sequence[ResourceAttributeTypeDef],
-    },
-)
-_OptionalPutResourceAttributesRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceAttributesRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class PutResourceAttributesRequestRequestTypeDef(
-    _RequiredPutResourceAttributesRequestRequestTypeDef,
-    _OptionalPutResourceAttributesRequestRequestTypeDef,
-):
-    pass
-
-
 DescribeMigrationTaskResultTypeDef = TypedDict(
     "DescribeMigrationTaskResultTypeDef",
     {
         "MigrationTask": MigrationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh/type_defs.pyi` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,57 +18,54 @@
 from .literals import ApplicationStatusType, ResourceAttributeTypeType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ApplicationStateTypeDef",
     "CreatedArtifactTypeDef",
     "DiscoveredResourceTypeDef",
     "CreateProgressUpdateStreamRequestRequestTypeDef",
-    "CreatedArtifactOutputTypeDef",
     "DeleteProgressUpdateStreamRequestRequestTypeDef",
     "DescribeApplicationStateRequestRequestTypeDef",
-    "DescribeApplicationStateResultTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeMigrationTaskRequestRequestTypeDef",
     "DisassociateCreatedArtifactRequestRequestTypeDef",
     "DisassociateDiscoveredResourceRequestRequestTypeDef",
-    "DiscoveredResourceOutputTypeDef",
     "ImportMigrationTaskRequestRequestTypeDef",
-    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApplicationStatesRequestRequestTypeDef",
-    "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     "ListCreatedArtifactsRequestRequestTypeDef",
-    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
-    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     "ListMigrationTasksRequestRequestTypeDef",
     "MigrationTaskSummaryTypeDef",
-    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     "ProgressUpdateStreamSummaryTypeDef",
-    "ResourceAttributeOutputTypeDef",
-    "TaskOutputTypeDef",
-    "NotifyApplicationStateRequestRequestTypeDef",
-    "TaskTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceAttributeTypeDef",
-    "ResponseMetadataTypeDef",
-    "ListApplicationStatesResultTypeDef",
+    "TaskTypeDef",
+    "NotifyApplicationStateRequestRequestTypeDef",
     "AssociateCreatedArtifactRequestRequestTypeDef",
     "AssociateDiscoveredResourceRequestRequestTypeDef",
+    "DescribeApplicationStateResultTypeDef",
+    "ListApplicationStatesResultTypeDef",
     "ListCreatedArtifactsResultTypeDef",
     "ListDiscoveredResourcesResultTypeDef",
+    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
+    "ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
+    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
+    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     "ListMigrationTasksResultTypeDef",
     "ListProgressUpdateStreamsResultTypeDef",
+    "PutResourceAttributesRequestRequestTypeDef",
     "MigrationTaskTypeDef",
     "NotifyMigrationTaskStateRequestRequestTypeDef",
-    "PutResourceAttributesRequestRequestTypeDef",
     "DescribeMigrationTaskResultTypeDef",
 )
 
 ApplicationStateTypeDef = TypedDict(
     "ApplicationStateTypeDef",
     {
         "ApplicationId": str,
@@ -88,74 +85,61 @@
     "_OptionalCreatedArtifactTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class CreatedArtifactTypeDef(_RequiredCreatedArtifactTypeDef, _OptionalCreatedArtifactTypeDef):
     pass
 
+
 _RequiredDiscoveredResourceTypeDef = TypedDict(
     "_RequiredDiscoveredResourceTypeDef",
     {
         "ConfigurationId": str,
     },
 )
 _OptionalDiscoveredResourceTypeDef = TypedDict(
     "_OptionalDiscoveredResourceTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class DiscoveredResourceTypeDef(
     _RequiredDiscoveredResourceTypeDef, _OptionalDiscoveredResourceTypeDef
 ):
     pass
 
+
 _RequiredCreateProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProgressUpdateStreamRequestRequestTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
 )
 _OptionalCreateProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_OptionalCreateProgressUpdateStreamRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class CreateProgressUpdateStreamRequestRequestTypeDef(
     _RequiredCreateProgressUpdateStreamRequestRequestTypeDef,
     _OptionalCreateProgressUpdateStreamRequestRequestTypeDef,
 ):
     pass
 
-_RequiredCreatedArtifactOutputTypeDef = TypedDict(
-    "_RequiredCreatedArtifactOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreatedArtifactOutputTypeDef = TypedDict(
-    "_OptionalCreatedArtifactOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class CreatedArtifactOutputTypeDef(
-    _RequiredCreatedArtifactOutputTypeDef, _OptionalCreatedArtifactOutputTypeDef
-):
-    pass
 
 _RequiredDeleteProgressUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteProgressUpdateStreamRequestRequestTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
 )
@@ -163,33 +147,37 @@
     "_OptionalDeleteProgressUpdateStreamRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class DeleteProgressUpdateStreamRequestRequestTypeDef(
     _RequiredDeleteProgressUpdateStreamRequestRequestTypeDef,
     _OptionalDeleteProgressUpdateStreamRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeApplicationStateRequestRequestTypeDef = TypedDict(
     "DescribeApplicationStateRequestRequestTypeDef",
     {
         "ApplicationId": str,
     },
 )
 
-DescribeApplicationStateResultTypeDef = TypedDict(
-    "DescribeApplicationStateResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApplicationStatus": ApplicationStatusType,
-        "LastUpdatedTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeMigrationTaskRequestRequestTypeDef = TypedDict(
     "DescribeMigrationTaskRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
@@ -209,20 +197,22 @@
     "_OptionalDisassociateCreatedArtifactRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class DisassociateCreatedArtifactRequestRequestTypeDef(
     _RequiredDisassociateCreatedArtifactRequestRequestTypeDef,
     _OptionalDisassociateCreatedArtifactRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredDisassociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateDiscoveredResourceRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
         "ConfigurationId": str,
     },
@@ -231,38 +221,21 @@
     "_OptionalDisassociateDiscoveredResourceRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class DisassociateDiscoveredResourceRequestRequestTypeDef(
     _RequiredDisassociateDiscoveredResourceRequestRequestTypeDef,
     _OptionalDisassociateDiscoveredResourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDiscoveredResourceOutputTypeDef = TypedDict(
-    "_RequiredDiscoveredResourceOutputTypeDef",
-    {
-        "ConfigurationId": str,
-    },
-)
-_OptionalDiscoveredResourceOutputTypeDef = TypedDict(
-    "_OptionalDiscoveredResourceOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class DiscoveredResourceOutputTypeDef(
-    _RequiredDiscoveredResourceOutputTypeDef, _OptionalDiscoveredResourceOutputTypeDef
-):
-    pass
 
 _RequiredImportMigrationTaskRequestRequestTypeDef = TypedDict(
     "_RequiredImportMigrationTaskRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
@@ -271,60 +244,42 @@
     "_OptionalImportMigrationTaskRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class ImportMigrationTaskRequestRequestTypeDef(
     _RequiredImportMigrationTaskRequestRequestTypeDef,
     _OptionalImportMigrationTaskRequestRequestTypeDef,
 ):
     pass
 
-ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = TypedDict(
-    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
+
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ApplicationIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListApplicationStatesRequestRequestTypeDef = TypedDict(
     "ListApplicationStatesRequestRequestTypeDef",
     {
         "ApplicationIds": Sequence[str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-    },
-)
-_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef(
-    _RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-    _OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
-):
-    pass
-
 _RequiredListCreatedArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListCreatedArtifactsRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
 )
@@ -333,40 +288,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListCreatedArtifactsRequestRequestTypeDef(
     _RequiredListCreatedArtifactsRequestRequestTypeDef,
     _OptionalListCreatedArtifactsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-    },
-)
-_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
-    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-):
-    pass
 
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
     },
@@ -376,28 +312,21 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = TypedDict(
-    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
-    {
-        "ResourceName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListMigrationTasksRequestRequestTypeDef = TypedDict(
     "ListMigrationTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "ResourceName": str,
@@ -414,22 +343,14 @@
         "ProgressPercent": int,
         "StatusDetail": str,
         "UpdateDateTime": datetime,
     },
     total=False,
 )
 
-ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = TypedDict(
-    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProgressUpdateStreamsRequestRequestTypeDef = TypedDict(
     "ListProgressUpdateStreamsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -439,40 +360,42 @@
     "ProgressUpdateStreamSummaryTypeDef",
     {
         "ProgressUpdateStreamName": str,
     },
     total=False,
 )
 
-ResourceAttributeOutputTypeDef = TypedDict(
-    "ResourceAttributeOutputTypeDef",
+ResourceAttributeTypeDef = TypedDict(
+    "ResourceAttributeTypeDef",
     {
         "Type": ResourceAttributeTypeType,
         "Value": str,
     },
 )
 
-_RequiredTaskOutputTypeDef = TypedDict(
-    "_RequiredTaskOutputTypeDef",
+_RequiredTaskTypeDef = TypedDict(
+    "_RequiredTaskTypeDef",
     {
         "Status": StatusType,
     },
 )
-_OptionalTaskOutputTypeDef = TypedDict(
-    "_OptionalTaskOutputTypeDef",
+_OptionalTaskTypeDef = TypedDict(
+    "_OptionalTaskTypeDef",
     {
         "StatusDetail": str,
         "ProgressPercent": int,
     },
     total=False,
 )
 
-class TaskOutputTypeDef(_RequiredTaskOutputTypeDef, _OptionalTaskOutputTypeDef):
+
+class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
     pass
 
+
 _RequiredNotifyApplicationStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyApplicationStateRequestRequestTypeDef",
     {
         "ApplicationId": str,
         "Status": ApplicationStatusType,
     },
 )
@@ -481,164 +404,228 @@
     {
         "UpdateDateTime": Union[datetime, str],
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class NotifyApplicationStateRequestRequestTypeDef(
     _RequiredNotifyApplicationStateRequestRequestTypeDef,
     _OptionalNotifyApplicationStateRequestRequestTypeDef,
 ):
     pass
 
-_RequiredTaskTypeDef = TypedDict(
-    "_RequiredTaskTypeDef",
+
+_RequiredAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateCreatedArtifactRequestRequestTypeDef",
     {
-        "Status": StatusType,
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+        "CreatedArtifact": CreatedArtifactTypeDef,
     },
 )
-_OptionalTaskTypeDef = TypedDict(
-    "_OptionalTaskTypeDef",
+_OptionalAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateCreatedArtifactRequestRequestTypeDef",
     {
-        "StatusDetail": str,
-        "ProgressPercent": int,
+        "DryRun": bool,
     },
     total=False,
 )
 
-class TaskTypeDef(_RequiredTaskTypeDef, _OptionalTaskTypeDef):
+
+class AssociateCreatedArtifactRequestRequestTypeDef(
+    _RequiredAssociateCreatedArtifactRequestRequestTypeDef,
+    _OptionalAssociateCreatedArtifactRequestRequestTypeDef,
+):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+
+_RequiredAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateDiscoveredResourceRequestRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+        "DiscoveredResource": DiscoveredResourceTypeDef,
     },
-    total=False,
 )
-
-ResourceAttributeTypeDef = TypedDict(
-    "ResourceAttributeTypeDef",
+_OptionalAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateDiscoveredResourceRequestRequestTypeDef",
     {
-        "Type": ResourceAttributeTypeType,
-        "Value": str,
+        "DryRun": bool,
     },
+    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class AssociateDiscoveredResourceRequestRequestTypeDef(
+    _RequiredAssociateDiscoveredResourceRequestRequestTypeDef,
+    _OptionalAssociateDiscoveredResourceRequestRequestTypeDef,
+):
+    pass
+
+
+DescribeApplicationStateResultTypeDef = TypedDict(
+    "DescribeApplicationStateResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ApplicationStatus": ApplicationStatusType,
+        "LastUpdatedTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationStatesResultTypeDef = TypedDict(
     "ListApplicationStatesResultTypeDef",
     {
         "ApplicationStateList": List[ApplicationStateTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateCreatedArtifactRequestRequestTypeDef",
+ListCreatedArtifactsResultTypeDef = TypedDict(
+    "ListCreatedArtifactsResultTypeDef",
+    {
+        "NextToken": str,
+        "CreatedArtifactList": List[CreatedArtifactTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDiscoveredResourcesResultTypeDef = TypedDict(
+    "ListDiscoveredResourcesResultTypeDef",
+    {
+        "NextToken": str,
+        "DiscoveredResourceList": List[DiscoveredResourceTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationStatesRequestListApplicationStatesPaginateTypeDef = TypedDict(
+    "ListApplicationStatesRequestListApplicationStatesPaginateTypeDef",
+    {
+        "ApplicationIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
-        "CreatedArtifact": CreatedArtifactTypeDef,
     },
 )
-_OptionalAssociateCreatedArtifactRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateCreatedArtifactRequestRequestTypeDef",
+_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef",
     {
-        "DryRun": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class AssociateCreatedArtifactRequestRequestTypeDef(
-    _RequiredAssociateCreatedArtifactRequestRequestTypeDef,
-    _OptionalAssociateCreatedArtifactRequestRequestTypeDef,
+
+class ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef(
+    _RequiredListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+    _OptionalListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
 ):
     pass
 
-_RequiredAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateDiscoveredResourceRequestRequestTypeDef",
+
+_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
-        "DiscoveredResource": DiscoveredResourceTypeDef,
     },
 )
-_OptionalAssociateDiscoveredResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateDiscoveredResourceRequestRequestTypeDef",
+_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     {
-        "DryRun": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class AssociateDiscoveredResourceRequestRequestTypeDef(
-    _RequiredAssociateDiscoveredResourceRequestRequestTypeDef,
-    _OptionalAssociateDiscoveredResourceRequestRequestTypeDef,
+
+class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
+    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
 ):
     pass
 
-ListCreatedArtifactsResultTypeDef = TypedDict(
-    "ListCreatedArtifactsResultTypeDef",
+
+ListMigrationTasksRequestListMigrationTasksPaginateTypeDef = TypedDict(
+    "ListMigrationTasksRequestListMigrationTasksPaginateTypeDef",
     {
-        "NextToken": str,
-        "CreatedArtifactList": List[CreatedArtifactOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListDiscoveredResourcesResultTypeDef = TypedDict(
-    "ListDiscoveredResourcesResultTypeDef",
+ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef = TypedDict(
+    "ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef",
     {
-        "NextToken": str,
-        "DiscoveredResourceList": List[DiscoveredResourceOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 ListMigrationTasksResultTypeDef = TypedDict(
     "ListMigrationTasksResultTypeDef",
     {
         "NextToken": str,
         "MigrationTaskSummaryList": List[MigrationTaskSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProgressUpdateStreamsResultTypeDef = TypedDict(
     "ListProgressUpdateStreamsResultTypeDef",
     {
         "ProgressUpdateStreamSummaryList": List[ProgressUpdateStreamSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceAttributesRequestRequestTypeDef",
+    {
+        "ProgressUpdateStream": str,
+        "MigrationTaskName": str,
+        "ResourceAttributeList": Sequence[ResourceAttributeTypeDef],
+    },
+)
+_OptionalPutResourceAttributesRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceAttributesRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class PutResourceAttributesRequestRequestTypeDef(
+    _RequiredPutResourceAttributesRequestRequestTypeDef,
+    _OptionalPutResourceAttributesRequestRequestTypeDef,
+):
+    pass
+
+
 MigrationTaskTypeDef = TypedDict(
     "MigrationTaskTypeDef",
     {
         "ProgressUpdateStream": str,
         "MigrationTaskName": str,
-        "Task": TaskOutputTypeDef,
+        "Task": TaskTypeDef,
         "UpdateDateTime": datetime,
-        "ResourceAttributeList": List[ResourceAttributeOutputTypeDef],
+        "ResourceAttributeList": List[ResourceAttributeTypeDef],
     },
     total=False,
 )
 
 _RequiredNotifyMigrationTaskStateRequestRequestTypeDef = TypedDict(
     "_RequiredNotifyMigrationTaskStateRequestRequestTypeDef",
     {
@@ -653,42 +640,22 @@
     "_OptionalNotifyMigrationTaskStateRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class NotifyMigrationTaskStateRequestRequestTypeDef(
     _RequiredNotifyMigrationTaskStateRequestRequestTypeDef,
     _OptionalNotifyMigrationTaskStateRequestRequestTypeDef,
 ):
     pass
 
-_RequiredPutResourceAttributesRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceAttributesRequestRequestTypeDef",
-    {
-        "ProgressUpdateStream": str,
-        "MigrationTaskName": str,
-        "ResourceAttributeList": Sequence[ResourceAttributeTypeDef],
-    },
-)
-_OptionalPutResourceAttributesRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceAttributesRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class PutResourceAttributesRequestRequestTypeDef(
-    _RequiredPutResourceAttributesRequestRequestTypeDef,
-    _OptionalPutResourceAttributesRequestRequestTypeDef,
-):
-    pass
 
 DescribeMigrationTaskResultTypeDef = TypedDict(
     "DescribeMigrationTaskResultTypeDef",
     {
         "MigrationTask": MigrationTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/PKG-INFO` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mgh
-Version: 1.28.12
-Summary: Type annotations for boto3.MigrationHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MigrationHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mgh.svg?color=blue)](https://pypi.org/project/mypy-boto3-mgh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mgh)](https://pepy.tech/project/mypy-boto3-mgh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MigrationHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
+[boto3.MigrationHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mgh.html#MigrationHub)
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
 [mypy-boto3-mgh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mgh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -348,52 +348,48 @@
 
 ```python
 from mypy_boto3_mgh.type_defs import (
     ApplicationStateTypeDef,
     CreatedArtifactTypeDef,
     DiscoveredResourceTypeDef,
     CreateProgressUpdateStreamRequestRequestTypeDef,
-    CreatedArtifactOutputTypeDef,
     DeleteProgressUpdateStreamRequestRequestTypeDef,
     DescribeApplicationStateRequestRequestTypeDef,
-    DescribeApplicationStateResultTypeDef,
+    ResponseMetadataTypeDef,
     DescribeMigrationTaskRequestRequestTypeDef,
     DisassociateCreatedArtifactRequestRequestTypeDef,
     DisassociateDiscoveredResourceRequestRequestTypeDef,
-    DiscoveredResourceOutputTypeDef,
     ImportMigrationTaskRequestRequestTypeDef,
-    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApplicationStatesRequestRequestTypeDef,
-    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
     ListCreatedArtifactsRequestRequestTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
     ListMigrationTasksRequestRequestTypeDef,
     MigrationTaskSummaryTypeDef,
-    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListProgressUpdateStreamsRequestRequestTypeDef,
     ProgressUpdateStreamSummaryTypeDef,
-    ResourceAttributeOutputTypeDef,
-    TaskOutputTypeDef,
-    NotifyApplicationStateRequestRequestTypeDef,
-    TaskTypeDef,
-    PaginatorConfigTypeDef,
     ResourceAttributeTypeDef,
-    ResponseMetadataTypeDef,
-    ListApplicationStatesResultTypeDef,
+    TaskTypeDef,
+    NotifyApplicationStateRequestRequestTypeDef,
     AssociateCreatedArtifactRequestRequestTypeDef,
     AssociateDiscoveredResourceRequestRequestTypeDef,
+    DescribeApplicationStateResultTypeDef,
+    ListApplicationStatesResultTypeDef,
     ListCreatedArtifactsResultTypeDef,
     ListDiscoveredResourcesResultTypeDef,
+    ListApplicationStatesRequestListApplicationStatesPaginateTypeDef,
+    ListCreatedArtifactsRequestListCreatedArtifactsPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListMigrationTasksRequestListMigrationTasksPaginateTypeDef,
+    ListProgressUpdateStreamsRequestListProgressUpdateStreamsPaginateTypeDef,
     ListMigrationTasksResultTypeDef,
     ListProgressUpdateStreamsResultTypeDef,
+    PutResourceAttributesRequestRequestTypeDef,
     MigrationTaskTypeDef,
     NotifyMigrationTaskStateRequestRequestTypeDef,
-    PutResourceAttributesRequestRequestTypeDef,
     DescribeMigrationTaskResultTypeDef,
 )
 
 
 def get_structure() -> ApplicationStateTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-mgh-1.28.12/mypy_boto3_mgh.egg-info/SOURCES.txt` & `mypy-boto3-mgh-1.28.15/mypy_boto3_mgh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mgh-1.28.12/setup.py` & `mypy-boto3-mgh-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mgh",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mgh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MigrationHub 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.MigrationHub 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

