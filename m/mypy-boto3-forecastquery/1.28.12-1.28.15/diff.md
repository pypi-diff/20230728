# Comparing `tmp/mypy-boto3-forecastquery-1.28.12.tar.gz` & `tmp/mypy-boto3-forecastquery-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-forecastquery-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
+gzip compressed data, was "mypy-boto3-forecastquery-1.28.15.tar", last modified: Fri Jul 28 20:42:50 2023, max compression
```

## Comparing `mypy-boto3-forecastquery-1.28.12.tar` & `mypy-boto3-forecastquery-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.568507 mypy-boto3-forecastquery-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-27 05:34:42.568507 mypy-boto3-forecastquery-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.568507 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.568507 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-27 05:34:42.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:42.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:42.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:42.000000 mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.568507 mypy-boto3-forecastquery-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-27 05:22:27.000000 mypy-boto3-forecastquery-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.105128 mypy-boto3-forecastquery-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-28 20:42:50.101128 mypy-boto3-forecastquery-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.093128 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7894 2023-07-28 20:26:07.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-28 20:26:07.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-28 20:26:07.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:50.101128 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12389 2023-07-28 20:42:49.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 20:42:49.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:49.000000 mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:50.105128 mypy-boto3-forecastquery-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-07-28 20:26:06.000000 mypy-boto3-forecastquery-1.28.15/setup.py
```

### Comparing `mypy-boto3-forecastquery-1.28.12/LICENSE` & `mypy-boto3-forecastquery-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecastquery-1.28.12/PKG-INFO` & `mypy-boto3-forecastquery-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecastquery
-Version: 1.28.12
-Summary: Type annotations for boto3.ForecastQueryService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ForecastQueryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecastquery.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecastquery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecastquery)](https://pepy.tech/project/mypy-boto3-forecastquery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastQueryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
+[boto3.ForecastQueryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
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
 [mypy-boto3-forecastquery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,16 +299,16 @@
 `mypy_boto3_forecastquery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecastquery.type_defs import (
     DataPointTypeDef,
     QueryForecastRequestRequestTypeDef,
-    QueryWhatIfForecastRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    QueryWhatIfForecastRequestRequestTypeDef,
     ForecastTypeDef,
     QueryForecastResponseTypeDef,
     QueryWhatIfForecastResponseTypeDef,
 )
 
 
 def get_structure() -> DataPointTypeDef:
```

### Comparing `mypy-boto3-forecastquery-1.28.12/README.md` & `mypy-boto3-forecastquery-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecastquery.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecastquery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecastquery)](https://pepy.tech/project/mypy-boto3-forecastquery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastQueryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
+[boto3.ForecastQueryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
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
 [mypy-boto3-forecastquery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,16 +267,16 @@
 `mypy_boto3_forecastquery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecastquery.type_defs import (
     DataPointTypeDef,
     QueryForecastRequestRequestTypeDef,
-    QueryWhatIfForecastRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    QueryWhatIfForecastRequestRequestTypeDef,
     ForecastTypeDef,
     QueryForecastResponseTypeDef,
     QueryWhatIfForecastResponseTypeDef,
 )
 
 
 def get_structure() -> DataPointTypeDef:
```

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/__main__.py` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ForecastQueryService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ForecastQueryService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService\nOther"
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

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/client.py` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/client.pyi` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/literals.py` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/literals.pyi` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/type_defs.py` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DataPointTypeDef",
     "QueryForecastRequestRequestTypeDef",
-    "QueryWhatIfForecastRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "QueryWhatIfForecastRequestRequestTypeDef",
     "ForecastTypeDef",
     "QueryForecastResponseTypeDef",
     "QueryWhatIfForecastResponseTypeDef",
 )
 
 DataPointTypeDef = TypedDict(
     "DataPointTypeDef",
@@ -59,14 +59,25 @@
 
 class QueryForecastRequestRequestTypeDef(
     _RequiredQueryForecastRequestRequestTypeDef, _OptionalQueryForecastRequestRequestTypeDef
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
 _RequiredQueryWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_RequiredQueryWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastArn": str,
         "Filters": Mapping[str, str],
     },
 )
@@ -84,41 +95,30 @@
 class QueryWhatIfForecastRequestRequestTypeDef(
     _RequiredQueryWhatIfForecastRequestRequestTypeDef,
     _OptionalQueryWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
 
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
 ForecastTypeDef = TypedDict(
     "ForecastTypeDef",
     {
         "Predictions": Dict[str, List[DataPointTypeDef]],
     },
     total=False,
 )
 
 QueryForecastResponseTypeDef = TypedDict(
     "QueryForecastResponseTypeDef",
     {
         "Forecast": ForecastTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryWhatIfForecastResponseTypeDef = TypedDict(
     "QueryWhatIfForecastResponseTypeDef",
     {
         "Forecast": ForecastTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery/type_defs.pyi` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DataPointTypeDef",
     "QueryForecastRequestRequestTypeDef",
-    "QueryWhatIfForecastRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "QueryWhatIfForecastRequestRequestTypeDef",
     "ForecastTypeDef",
     "QueryForecastResponseTypeDef",
     "QueryWhatIfForecastResponseTypeDef",
 )
 
 DataPointTypeDef = TypedDict(
     "DataPointTypeDef",
@@ -56,14 +56,25 @@
 )
 
 class QueryForecastRequestRequestTypeDef(
     _RequiredQueryForecastRequestRequestTypeDef, _OptionalQueryForecastRequestRequestTypeDef
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
 _RequiredQueryWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_RequiredQueryWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastArn": str,
         "Filters": Mapping[str, str],
     },
 )
@@ -79,41 +90,30 @@
 
 class QueryWhatIfForecastRequestRequestTypeDef(
     _RequiredQueryWhatIfForecastRequestRequestTypeDef,
     _OptionalQueryWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
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
 ForecastTypeDef = TypedDict(
     "ForecastTypeDef",
     {
         "Predictions": Dict[str, List[DataPointTypeDef]],
     },
     total=False,
 )
 
 QueryForecastResponseTypeDef = TypedDict(
     "QueryForecastResponseTypeDef",
     {
         "Forecast": ForecastTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryWhatIfForecastResponseTypeDef = TypedDict(
     "QueryWhatIfForecastResponseTypeDef",
     {
         "Forecast": ForecastTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/PKG-INFO` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-forecastquery
-Version: 1.28.12
-Summary: Type annotations for boto3.ForecastQueryService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ForecastQueryService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-forecastquery.svg?color=blue)](https://pypi.org/project/mypy-boto3-forecastquery)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-forecastquery)](https://pepy.tech/project/mypy-boto3-forecastquery)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ForecastQueryService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
+[boto3.ForecastQueryService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService)
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
 [mypy-boto3-forecastquery docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_forecastquery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,16 +299,16 @@
 `mypy_boto3_forecastquery.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_forecastquery.type_defs import (
     DataPointTypeDef,
     QueryForecastRequestRequestTypeDef,
-    QueryWhatIfForecastRequestRequestTypeDef,
     ResponseMetadataTypeDef,
+    QueryWhatIfForecastRequestRequestTypeDef,
     ForecastTypeDef,
     QueryForecastResponseTypeDef,
     QueryWhatIfForecastResponseTypeDef,
 )
 
 
 def get_structure() -> DataPointTypeDef:
```

### Comparing `mypy-boto3-forecastquery-1.28.12/mypy_boto3_forecastquery.egg-info/SOURCES.txt` & `mypy-boto3-forecastquery-1.28.15/mypy_boto3_forecastquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-forecastquery-1.28.12/setup.py` & `mypy-boto3-forecastquery-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-forecastquery",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_forecastquery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ForecastQueryService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ForecastQueryService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

