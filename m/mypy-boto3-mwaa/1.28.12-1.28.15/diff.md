# Comparing `tmp/mypy-boto3-mwaa-1.28.12.tar.gz` & `tmp/mypy-boto3-mwaa-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mwaa-1.28.12.tar", last modified: Thu Jul 27 05:35:04 2023, max compression
+gzip compressed data, was "mypy-boto3-mwaa-1.28.15.tar", last modified: Fri Jul 28 20:43:21 2023, max compression
```

## Comparing `mypy-boto3-mwaa-1.28.12.tar` & `mypy-boto3-mwaa-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.756427 mypy-boto3-mwaa-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-27 05:35:04.752427 mypy-boto3-mwaa-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.748427 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11877 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:04.752427 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-27 05:35:04.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-27 05:35:04.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:04.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:04.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-27 05:35:04.000000 mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:04.756427 mypy-boto3-mwaa-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-27 05:26:49.000000 mypy-boto3-mwaa-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11086 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11067 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9140 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9138 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11861 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:15.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-28 20:43:21.000000 mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:21.429558 mypy-boto3-mwaa-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-07-28 20:32:14.000000 mypy-boto3-mwaa-1.28.15/setup.py
```

### Comparing `mypy-boto3-mwaa-1.28.12/LICENSE` & `mypy-boto3-mwaa-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.12/PKG-INFO` & `mypy-boto3-mwaa-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.28.12
-Summary: Type annotations for boto3.MWAA 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,39 +324,39 @@
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    CreateCliTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
-    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
     NetworkConfigurationOutputTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
+    CreateCliTokenResponseTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     LastUpdateTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
```

### Comparing `mypy-boto3-mwaa-1.28.12/README.md` & `mypy-boto3-mwaa-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,39 +292,39 @@
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    CreateCliTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
-    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
     NetworkConfigurationOutputTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
+    CreateCliTokenResponseTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     LastUpdateTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
```

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/__init__.py` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/__init__.pyi` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/__main__.py` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MWAA 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.MWAA 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA\nOther"
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

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/client.py` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/client.pyi` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/literals.py` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/literals.pyi` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/paginator.py` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/paginator.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,13 +41,13 @@
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/paginator.pyi` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -38,13 +38,13 @@
 class ListEnvironmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEnvironmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA.Paginator.ListEnvironments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/paginators/#listenvironmentspaginator)
         """
```

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/type_defs.py` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,39 +27,39 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
-    "CreateCliTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "NetworkConfigurationTypeDef",
-    "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
-    "CreateWebLoginTokenResponseTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
     "NetworkConfigurationOutputTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "UpdateErrorTypeDef",
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
-    "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
     "StatisticSetTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateNetworkConfigurationInputTypeDef",
+    "CreateCliTokenResponseTypeDef",
+    "CreateEnvironmentOutputTypeDef",
+    "CreateWebLoginTokenResponseTypeDef",
+    "ListEnvironmentsOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
     "LastUpdateTypeDef",
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
     "EnvironmentTypeDef",
     "PublishMetricsInputRequestTypeDef",
@@ -69,56 +69,41 @@
 CreateCliTokenRequestRequestTypeDef = TypedDict(
     "CreateCliTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateCliTokenResponseTypeDef = TypedDict(
-    "CreateCliTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CliToken": str,
-        "WebServerHostname": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-CreateEnvironmentOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWebLoginTokenRequestRequestTypeDef = TypedDict(
     "CreateWebLoginTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateWebLoginTokenResponseTypeDef = TypedDict(
-    "CreateWebLoginTokenResponseTypeDef",
-    {
-        "WebServerHostname": str,
-        "WebToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEnvironmentInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -151,55 +136,40 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
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
 
 ListEnvironmentsInputRequestTypeDef = TypedDict(
     "ListEnvironmentsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentsOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputTypeDef",
-    {
-        "Environments": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModuleLoggingConfigurationInputTypeDef = TypedDict(
     "ModuleLoggingConfigurationInputTypeDef",
     {
         "Enabled": bool,
         "LogLevel": LoggingLevelType,
     },
 )
@@ -221,35 +191,14 @@
         "Minimum": float,
         "SampleCount": int,
         "Sum": float,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -265,33 +214,84 @@
 UpdateNetworkConfigurationInputTypeDef = TypedDict(
     "UpdateNetworkConfigurationInputTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
 )
 
+CreateCliTokenResponseTypeDef = TypedDict(
+    "CreateCliTokenResponseTypeDef",
+    {
+        "CliToken": str,
+        "WebServerHostname": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEnvironmentOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWebLoginTokenResponseTypeDef = TypedDict(
+    "CreateWebLoginTokenResponseTypeDef",
+    {
+        "WebServerHostname": str,
+        "WebToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnvironmentsOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputTypeDef",
+    {
+        "Environments": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateEnvironmentOutputTypeDef = TypedDict(
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
     },
     total=False,
 )
 
+ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 LoggingConfigurationInputTypeDef = TypedDict(
     "LoggingConfigurationInputTypeDef",
     {
         "DagProcessingLogs": ModuleLoggingConfigurationInputTypeDef,
         "SchedulerLogs": ModuleLoggingConfigurationInputTypeDef,
         "TaskLogs": ModuleLoggingConfigurationInputTypeDef,
         "WebserverLogs": ModuleLoggingConfigurationInputTypeDef,
@@ -458,10 +458,10 @@
     },
 )
 
 GetEnvironmentOutputTypeDef = TypedDict(
     "GetEnvironmentOutputTypeDef",
     {
         "Environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa/type_defs.pyi` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -26,39 +26,39 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateCliTokenRequestRequestTypeDef",
-    "CreateCliTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "NetworkConfigurationTypeDef",
-    "CreateEnvironmentOutputTypeDef",
     "CreateWebLoginTokenRequestRequestTypeDef",
-    "CreateWebLoginTokenResponseTypeDef",
     "DeleteEnvironmentInputRequestTypeDef",
     "DimensionTypeDef",
     "NetworkConfigurationOutputTypeDef",
     "GetEnvironmentInputRequestTypeDef",
     "UpdateErrorTypeDef",
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListEnvironmentsInputRequestTypeDef",
-    "ListEnvironmentsOutputTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ModuleLoggingConfigurationInputTypeDef",
     "ModuleLoggingConfigurationTypeDef",
     "StatisticSetTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateNetworkConfigurationInputTypeDef",
+    "CreateCliTokenResponseTypeDef",
+    "CreateEnvironmentOutputTypeDef",
+    "CreateWebLoginTokenResponseTypeDef",
+    "ListEnvironmentsOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "UpdateEnvironmentOutputTypeDef",
     "LastUpdateTypeDef",
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
     "LoggingConfigurationInputTypeDef",
     "LoggingConfigurationTypeDef",
     "MetricDatumTypeDef",
     "CreateEnvironmentInputRequestTypeDef",
     "UpdateEnvironmentInputRequestTypeDef",
     "EnvironmentTypeDef",
     "PublishMetricsInputRequestTypeDef",
@@ -68,56 +68,41 @@
 CreateCliTokenRequestRequestTypeDef = TypedDict(
     "CreateCliTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateCliTokenResponseTypeDef = TypedDict(
-    "CreateCliTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CliToken": str,
-        "WebServerHostname": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
-CreateEnvironmentOutputTypeDef = TypedDict(
-    "CreateEnvironmentOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateWebLoginTokenRequestRequestTypeDef = TypedDict(
     "CreateWebLoginTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-CreateWebLoginTokenResponseTypeDef = TypedDict(
-    "CreateWebLoginTokenResponseTypeDef",
-    {
-        "WebServerHostname": str,
-        "WebToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEnvironmentInputRequestTypeDef = TypedDict(
     "DeleteEnvironmentInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -150,55 +135,40 @@
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
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
 
 ListEnvironmentsInputRequestTypeDef = TypedDict(
     "ListEnvironmentsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListEnvironmentsOutputTypeDef = TypedDict(
-    "ListEnvironmentsOutputTypeDef",
-    {
-        "Environments": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ModuleLoggingConfigurationInputTypeDef = TypedDict(
     "ModuleLoggingConfigurationInputTypeDef",
     {
         "Enabled": bool,
         "LogLevel": LoggingLevelType,
     },
 )
@@ -220,35 +190,14 @@
         "Minimum": float,
         "SampleCount": int,
         "Sum": float,
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
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -264,33 +213,84 @@
 UpdateNetworkConfigurationInputTypeDef = TypedDict(
     "UpdateNetworkConfigurationInputTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
     },
 )
 
+CreateCliTokenResponseTypeDef = TypedDict(
+    "CreateCliTokenResponseTypeDef",
+    {
+        "CliToken": str,
+        "WebServerHostname": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEnvironmentOutputTypeDef = TypedDict(
+    "CreateEnvironmentOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWebLoginTokenResponseTypeDef = TypedDict(
+    "CreateWebLoginTokenResponseTypeDef",
+    {
+        "WebServerHostname": str,
+        "WebToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnvironmentsOutputTypeDef = TypedDict(
+    "ListEnvironmentsOutputTypeDef",
+    {
+        "Environments": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateEnvironmentOutputTypeDef = TypedDict(
     "UpdateEnvironmentOutputTypeDef",
     {
         "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LastUpdateTypeDef = TypedDict(
     "LastUpdateTypeDef",
     {
         "CreatedAt": datetime,
         "Error": UpdateErrorTypeDef,
         "Source": str,
         "Status": UpdateStatusType,
     },
     total=False,
 )
 
+ListEnvironmentsInputListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsInputListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 LoggingConfigurationInputTypeDef = TypedDict(
     "LoggingConfigurationInputTypeDef",
     {
         "DagProcessingLogs": ModuleLoggingConfigurationInputTypeDef,
         "SchedulerLogs": ModuleLoggingConfigurationInputTypeDef,
         "TaskLogs": ModuleLoggingConfigurationInputTypeDef,
         "WebserverLogs": ModuleLoggingConfigurationInputTypeDef,
@@ -451,10 +451,10 @@
     },
 )
 
 GetEnvironmentOutputTypeDef = TypedDict(
     "GetEnvironmentOutputTypeDef",
     {
         "Environment": EnvironmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/PKG-INFO` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.28.12
-Summary: Type annotations for boto3.MWAA 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
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
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
 
@@ -324,39 +324,39 @@
 
 `mypy_boto3_mwaa.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_mwaa.type_defs import (
     CreateCliTokenRequestRequestTypeDef,
-    CreateCliTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     NetworkConfigurationTypeDef,
-    CreateEnvironmentOutputTypeDef,
     CreateWebLoginTokenRequestRequestTypeDef,
-    CreateWebLoginTokenResponseTypeDef,
     DeleteEnvironmentInputRequestTypeDef,
     DimensionTypeDef,
     NetworkConfigurationOutputTypeDef,
     GetEnvironmentInputRequestTypeDef,
     UpdateErrorTypeDef,
-    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListEnvironmentsInputRequestTypeDef,
-    ListEnvironmentsOutputTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ModuleLoggingConfigurationInputTypeDef,
     ModuleLoggingConfigurationTypeDef,
     StatisticSetTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateNetworkConfigurationInputTypeDef,
+    CreateCliTokenResponseTypeDef,
+    CreateEnvironmentOutputTypeDef,
+    CreateWebLoginTokenResponseTypeDef,
+    ListEnvironmentsOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     LastUpdateTypeDef,
+    ListEnvironmentsInputListEnvironmentsPaginateTypeDef,
     LoggingConfigurationInputTypeDef,
     LoggingConfigurationTypeDef,
     MetricDatumTypeDef,
     CreateEnvironmentInputRequestTypeDef,
     UpdateEnvironmentInputRequestTypeDef,
     EnvironmentTypeDef,
     PublishMetricsInputRequestTypeDef,
```

### Comparing `mypy-boto3-mwaa-1.28.12/mypy_boto3_mwaa.egg-info/SOURCES.txt` & `mypy-boto3-mwaa-1.28.15/mypy_boto3_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.28.12/setup.py` & `mypy-boto3-mwaa-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mwaa",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MWAA 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MWAA 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

