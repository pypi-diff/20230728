# Comparing `tmp/mypy-boto3-resource-explorer-2-1.28.12.tar.gz` & `tmp/mypy-boto3-resource-explorer-2-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-resource-explorer-2-1.28.12.tar", last modified: Thu Jul 27 11:49:30 2023, max compression
+gzip compressed data, was "mypy-boto3-resource-explorer-2-1.28.15.tar", last modified: Fri Jul 28 20:43:34 2023, max compression
```

## Comparing `mypy-boto3-resource-explorer-2-1.28.12.tar` & `mypy-boto3-resource-explorer-2-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.317213 mypy-boto3-resource-explorer-2-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-07-27 11:49:30.317213 mypy-boto3-resource-explorer-2-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13779 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.313213 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-07-27 11:44:39.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13357 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:30.317213 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 11:49:30.000000 mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:30.317213 mypy-boto3-resource-explorer-2-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-27 11:44:38.000000 mypy-boto3-resource-explorer-2-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.985731 mypy-boto3-resource-explorer-2-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15245 2023-07-28 20:43:33.985731 mypy-boto3-resource-explorer-2-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13713 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.977730 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17102 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-07-28 20:36:55.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8721 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-28 20:36:59.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13041 2023-07-28 20:36:55.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.985731 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15245 2023-07-28 20:43:33.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-28 20:43:33.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:43:33.000000 mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:33.985731 mypy-boto3-resource-explorer-2-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-07-28 20:36:54.000000 mypy-boto3-resource-explorer-2-1.28.15/setup.py
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/LICENSE` & `mypy-boto3-resource-explorer-2-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/PKG-INFO` & `mypy-boto3-resource-explorer-2-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-explorer-2
-Version: 1.28.12
-Summary: Type annotations for boto3.ResourceExplorer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ResourceExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-explorer-2)](https://pepy.tech/project/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,25 +345,23 @@
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
     DeleteViewInputRequestTypeDef,
     GetViewInputRequestTypeDef,
-    IncludedPropertyOutputTypeDef,
     IndexTypeDef,
     PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListViewsInputRequestTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    SearchFilterOutputTypeDef,
     SearchInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
     AssociateDefaultViewOutputTypeDef,
     CreateIndexOutputTypeDef,
     DeleteIndexOutputTypeDef,
@@ -372,27 +370,27 @@
     GetDefaultViewOutputTypeDef,
     GetIndexOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
+    ViewTypeDef,
     ListIndexesOutputTypeDef,
     ListIndexesInputListIndexesPaginateTypeDef,
     ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListViewsInputListViewsPaginateTypeDef,
     SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
-    ViewTypeDef,
-    SearchOutputTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
+    SearchOutputTypeDef,
 )
 
 
 def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/README.md` & `mypy-boto3-resource-explorer-2-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-explorer-2)](https://pepy.tech/project/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -313,25 +313,23 @@
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
     DeleteViewInputRequestTypeDef,
     GetViewInputRequestTypeDef,
-    IncludedPropertyOutputTypeDef,
     IndexTypeDef,
     PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListViewsInputRequestTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    SearchFilterOutputTypeDef,
     SearchInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
     AssociateDefaultViewOutputTypeDef,
     CreateIndexOutputTypeDef,
     DeleteIndexOutputTypeDef,
@@ -340,27 +338,27 @@
     GetDefaultViewOutputTypeDef,
     GetIndexOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
+    ViewTypeDef,
     ListIndexesOutputTypeDef,
     ListIndexesInputListIndexesPaginateTypeDef,
     ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListViewsInputListViewsPaginateTypeDef,
     SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
-    ViewTypeDef,
-    SearchOutputTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
+    SearchOutputTypeDef,
 )
 
 
 def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__init__.py` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__init__.pyi` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/__main__.py` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ResourceExplorer 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ResourceExplorer 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer\nOther"
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

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/client.py` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/client.pyi` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/literals.py` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/literals.pyi` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/paginator.py` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/paginator.pyi` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/type_defs.py` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,25 +30,23 @@
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
     "IncludedPropertyTypeDef",
     "SearchFilterTypeDef",
     "DeleteIndexInputRequestTypeDef",
     "DeleteViewInputRequestTypeDef",
     "GetViewInputRequestTypeDef",
-    "IncludedPropertyOutputTypeDef",
     "IndexTypeDef",
     "PaginatorConfigTypeDef",
     "ListIndexesInputRequestTypeDef",
     "ListSupportedResourceTypesInputRequestTypeDef",
     "SupportedResourceTypeTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListViewsInputRequestTypeDef",
     "ResourceCountTypeDef",
     "ResourcePropertyTypeDef",
-    "SearchFilterOutputTypeDef",
     "SearchInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateIndexTypeInputRequestTypeDef",
     "AssociateDefaultViewOutputTypeDef",
     "CreateIndexOutputTypeDef",
     "DeleteIndexOutputTypeDef",
@@ -57,27 +55,27 @@
     "GetDefaultViewOutputTypeDef",
     "GetIndexOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListViewsOutputTypeDef",
     "UpdateIndexTypeOutputTypeDef",
     "CreateViewInputRequestTypeDef",
     "UpdateViewInputRequestTypeDef",
+    "ViewTypeDef",
     "ListIndexesOutputTypeDef",
     "ListIndexesInputListIndexesPaginateTypeDef",
     "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     "ListViewsInputListViewsPaginateTypeDef",
     "SearchInputSearchPaginateTypeDef",
     "ListSupportedResourceTypesOutputTypeDef",
     "ResourceTypeDef",
-    "ViewTypeDef",
-    "SearchOutputTypeDef",
     "BatchGetViewOutputTypeDef",
     "CreateViewOutputTypeDef",
     "GetViewOutputTypeDef",
     "UpdateViewOutputTypeDef",
+    "SearchOutputTypeDef",
 )
 
 AssociateDefaultViewInputRequestTypeDef = TypedDict(
     "AssociateDefaultViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
@@ -150,21 +148,14 @@
 GetViewInputRequestTypeDef = TypedDict(
     "GetViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-IncludedPropertyOutputTypeDef = TypedDict(
-    "IncludedPropertyOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 IndexTypeDef = TypedDict(
     "IndexTypeDef",
     {
         "Arn": str,
         "Region": str,
         "Type": IndexTypeType,
     },
@@ -241,21 +232,14 @@
         "Data": Dict[str, Any],
         "LastReportedAt": datetime,
         "Name": str,
     },
     total=False,
 )
 
-SearchFilterOutputTypeDef = TypedDict(
-    "SearchFilterOutputTypeDef",
-    {
-        "FilterString": str,
-    },
-)
-
 _RequiredSearchInputRequestTypeDef = TypedDict(
     "_RequiredSearchInputRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalSearchInputRequestTypeDef = TypedDict(
@@ -448,14 +432,27 @@
 
 class UpdateViewInputRequestTypeDef(
     _RequiredUpdateViewInputRequestTypeDef, _OptionalUpdateViewInputRequestTypeDef
 ):
     pass
 
 
+ViewTypeDef = TypedDict(
+    "ViewTypeDef",
+    {
+        "Filters": SearchFilterTypeDef,
+        "IncludedProperties": List[IncludedPropertyTypeDef],
+        "LastUpdatedAt": datetime,
+        "Owner": str,
+        "Scope": str,
+        "ViewArn": str,
+    },
+    total=False,
+)
+
 ListIndexesOutputTypeDef = TypedDict(
     "ListIndexesOutputTypeDef",
     {
         "Indexes": List[IndexTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -528,38 +525,14 @@
         "Region": str,
         "ResourceType": str,
         "Service": str,
     },
     total=False,
 )
 
-ViewTypeDef = TypedDict(
-    "ViewTypeDef",
-    {
-        "Filters": SearchFilterOutputTypeDef,
-        "IncludedProperties": List[IncludedPropertyOutputTypeDef],
-        "LastUpdatedAt": datetime,
-        "Owner": str,
-        "Scope": str,
-        "ViewArn": str,
-    },
-    total=False,
-)
-
-SearchOutputTypeDef = TypedDict(
-    "SearchOutputTypeDef",
-    {
-        "Count": ResourceCountTypeDef,
-        "NextToken": str,
-        "Resources": List[ResourceTypeDef],
-        "ViewArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetViewOutputTypeDef = TypedDict(
     "BatchGetViewOutputTypeDef",
     {
         "Errors": List[BatchGetViewErrorTypeDef],
         "Views": List[ViewTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -585,7 +558,18 @@
 UpdateViewOutputTypeDef = TypedDict(
     "UpdateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+SearchOutputTypeDef = TypedDict(
+    "SearchOutputTypeDef",
+    {
+        "Count": ResourceCountTypeDef,
+        "NextToken": str,
+        "Resources": List[ResourceTypeDef],
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2/type_defs.pyi` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,23 @@
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
     "IncludedPropertyTypeDef",
     "SearchFilterTypeDef",
     "DeleteIndexInputRequestTypeDef",
     "DeleteViewInputRequestTypeDef",
     "GetViewInputRequestTypeDef",
-    "IncludedPropertyOutputTypeDef",
     "IndexTypeDef",
     "PaginatorConfigTypeDef",
     "ListIndexesInputRequestTypeDef",
     "ListSupportedResourceTypesInputRequestTypeDef",
     "SupportedResourceTypeTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListViewsInputRequestTypeDef",
     "ResourceCountTypeDef",
     "ResourcePropertyTypeDef",
-    "SearchFilterOutputTypeDef",
     "SearchInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateIndexTypeInputRequestTypeDef",
     "AssociateDefaultViewOutputTypeDef",
     "CreateIndexOutputTypeDef",
     "DeleteIndexOutputTypeDef",
@@ -56,27 +54,27 @@
     "GetDefaultViewOutputTypeDef",
     "GetIndexOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "ListViewsOutputTypeDef",
     "UpdateIndexTypeOutputTypeDef",
     "CreateViewInputRequestTypeDef",
     "UpdateViewInputRequestTypeDef",
+    "ViewTypeDef",
     "ListIndexesOutputTypeDef",
     "ListIndexesInputListIndexesPaginateTypeDef",
     "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     "ListViewsInputListViewsPaginateTypeDef",
     "SearchInputSearchPaginateTypeDef",
     "ListSupportedResourceTypesOutputTypeDef",
     "ResourceTypeDef",
-    "ViewTypeDef",
-    "SearchOutputTypeDef",
     "BatchGetViewOutputTypeDef",
     "CreateViewOutputTypeDef",
     "GetViewOutputTypeDef",
     "UpdateViewOutputTypeDef",
+    "SearchOutputTypeDef",
 )
 
 AssociateDefaultViewInputRequestTypeDef = TypedDict(
     "AssociateDefaultViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
@@ -149,21 +147,14 @@
 GetViewInputRequestTypeDef = TypedDict(
     "GetViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-IncludedPropertyOutputTypeDef = TypedDict(
-    "IncludedPropertyOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 IndexTypeDef = TypedDict(
     "IndexTypeDef",
     {
         "Arn": str,
         "Region": str,
         "Type": IndexTypeType,
     },
@@ -240,21 +231,14 @@
         "Data": Dict[str, Any],
         "LastReportedAt": datetime,
         "Name": str,
     },
     total=False,
 )
 
-SearchFilterOutputTypeDef = TypedDict(
-    "SearchFilterOutputTypeDef",
-    {
-        "FilterString": str,
-    },
-)
-
 _RequiredSearchInputRequestTypeDef = TypedDict(
     "_RequiredSearchInputRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalSearchInputRequestTypeDef = TypedDict(
@@ -439,14 +423,27 @@
 )
 
 class UpdateViewInputRequestTypeDef(
     _RequiredUpdateViewInputRequestTypeDef, _OptionalUpdateViewInputRequestTypeDef
 ):
     pass
 
+ViewTypeDef = TypedDict(
+    "ViewTypeDef",
+    {
+        "Filters": SearchFilterTypeDef,
+        "IncludedProperties": List[IncludedPropertyTypeDef],
+        "LastUpdatedAt": datetime,
+        "Owner": str,
+        "Scope": str,
+        "ViewArn": str,
+    },
+    total=False,
+)
+
 ListIndexesOutputTypeDef = TypedDict(
     "ListIndexesOutputTypeDef",
     {
         "Indexes": List[IndexTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -517,38 +514,14 @@
         "Region": str,
         "ResourceType": str,
         "Service": str,
     },
     total=False,
 )
 
-ViewTypeDef = TypedDict(
-    "ViewTypeDef",
-    {
-        "Filters": SearchFilterOutputTypeDef,
-        "IncludedProperties": List[IncludedPropertyOutputTypeDef],
-        "LastUpdatedAt": datetime,
-        "Owner": str,
-        "Scope": str,
-        "ViewArn": str,
-    },
-    total=False,
-)
-
-SearchOutputTypeDef = TypedDict(
-    "SearchOutputTypeDef",
-    {
-        "Count": ResourceCountTypeDef,
-        "NextToken": str,
-        "Resources": List[ResourceTypeDef],
-        "ViewArn": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchGetViewOutputTypeDef = TypedDict(
     "BatchGetViewOutputTypeDef",
     {
         "Errors": List[BatchGetViewErrorTypeDef],
         "Views": List[ViewTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -574,7 +547,18 @@
 UpdateViewOutputTypeDef = TypedDict(
     "UpdateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+SearchOutputTypeDef = TypedDict(
+    "SearchOutputTypeDef",
+    {
+        "Count": ResourceCountTypeDef,
+        "NextToken": str,
+        "Resources": List[ResourceTypeDef],
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-resource-explorer-2
-Version: 1.28.12
-Summary: Type annotations for boto3.ResourceExplorer 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ResourceExplorer 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-resource-explorer-2.svg?color=blue)](https://pypi.org/project/mypy-boto3-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-resource-explorer-2)](https://pepy.tech/project/mypy-boto3-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ResourceExplorer 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
+[boto3.ResourceExplorer 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [mypy-boto3-resource-explorer-2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_resource_explorer_2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -345,25 +345,23 @@
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
     DeleteViewInputRequestTypeDef,
     GetViewInputRequestTypeDef,
-    IncludedPropertyOutputTypeDef,
     IndexTypeDef,
     PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListViewsInputRequestTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    SearchFilterOutputTypeDef,
     SearchInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
     AssociateDefaultViewOutputTypeDef,
     CreateIndexOutputTypeDef,
     DeleteIndexOutputTypeDef,
@@ -372,27 +370,27 @@
     GetDefaultViewOutputTypeDef,
     GetIndexOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
+    ViewTypeDef,
     ListIndexesOutputTypeDef,
     ListIndexesInputListIndexesPaginateTypeDef,
     ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListViewsInputListViewsPaginateTypeDef,
     SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
-    ViewTypeDef,
-    SearchOutputTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
+    SearchOutputTypeDef,
 )
 
 
 def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt` & `mypy-boto3-resource-explorer-2-1.28.15/mypy_boto3_resource_explorer_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-resource-explorer-2-1.28.12/setup.py` & `mypy-boto3-resource-explorer-2-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-resource-explorer-2",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_resource_explorer_2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ResourceExplorer 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ResourceExplorer 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

