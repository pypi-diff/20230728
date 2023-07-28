# Comparing `tmp/mypy-boto3-apigatewaymanagementapi-1.28.12.tar.gz` & `tmp/mypy-boto3-apigatewaymanagementapi-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-apigatewaymanagementapi-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
+gzip compressed data, was "mypy-boto3-apigatewaymanagementapi-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12.tar` & `mypy-boto3-apigatewaymanagementapi-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.360584 mypy-boto3-apigatewaymanagementapi-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-07-27 05:34:16.360584 mypy-boto3-apigatewaymanagementapi-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.360584 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:12.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.360584 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-07-27 05:34:16.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 05:34:16.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 05:34:16.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.360584 mypy-boto3-apigatewaymanagementapi-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-27 05:17:11.000000 mypy-boto3-apigatewaymanagementapi-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.220654 mypy-boto3-apigatewaymanagementapi-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-07-28 20:42:16.220654 mypy-boto3-apigatewaymanagementapi-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11305 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.216654 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-07-28 20:19:06.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-07-28 20:19:06.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-07-28 20:19:06.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-28 20:19:06.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-28 20:19:06.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.220654 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12856 2023-07-28 20:42:15.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 20:42:16.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:15.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 20:42:15.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.220654 mypy-boto3-apigatewaymanagementapi-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-07-28 20:19:05.000000 mypy-boto3-apigatewaymanagementapi-1.28.15/setup.py
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/LICENSE` & `mypy-boto3-apigatewaymanagementapi-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/PKG-INFO` & `mypy-boto3-apigatewaymanagementapi-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewaymanagementapi
-Version: 1.28.12
-Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewaymanagementapi)](https://pepy.tech/project/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [mypy-boto3-apigatewaymanagementapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,19 +297,19 @@
 
 `mypy_boto3_apigatewaymanagementapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewaymanagementapi.type_defs import (
     DeleteConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
 def get_structure() -> DeleteConnectionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/README.md` & `mypy-boto3-apigatewaymanagementapi-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewaymanagementapi)](https://pepy.tech/project/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [mypy-boto3-apigatewaymanagementapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,19 +265,19 @@
 
 `mypy_boto3_apigatewaymanagementapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewaymanagementapi.type_defs import (
     DeleteConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
 def get_structure() -> DeleteConnectionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/__main__.py` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ApiGatewayManagementApi 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ApiGatewayManagementApi 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi\nOther"
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

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/client.py` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/client.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/literals.py` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/literals.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/type_defs.py` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,33 +21,37 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteConnectionRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "IdentityTypeDef",
     "PostToConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetConnectionResponseTypeDef",
 )
 
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetConnectionRequestRequestTypeDef = TypedDict(
     "GetConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
@@ -66,27 +70,23 @@
     "PostToConnectionRequestRequestTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "ConnectionId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "ConnectedAt": datetime,
         "Identity": IdentityTypeDef,
         "LastActiveAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi/type_defs.pyi` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -20,33 +20,37 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteConnectionRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "IdentityTypeDef",
     "PostToConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetConnectionResponseTypeDef",
 )
 
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetConnectionRequestRequestTypeDef = TypedDict(
     "GetConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
@@ -65,27 +69,23 @@
     "PostToConnectionRequestRequestTypeDef",
     {
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "ConnectionId": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "ConnectedAt": datetime,
         "Identity": IdentityTypeDef,
         "LastActiveAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-apigatewaymanagementapi
-Version: 1.28.12
-Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ApiGatewayManagementApi 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/mypy-boto3-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-apigatewaymanagementapi)](https://pepy.tech/project/mypy-boto3-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ApiGatewayManagementApi 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
+[boto3.ApiGatewayManagementApi 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [mypy-boto3-apigatewaymanagementapi docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_apigatewaymanagementapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,19 +297,19 @@
 
 `mypy_boto3_apigatewaymanagementapi.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_apigatewaymanagementapi.type_defs import (
     DeleteConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
 def get_structure() -> DeleteConnectionRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt` & `mypy-boto3-apigatewaymanagementapi-1.28.15/mypy_boto3_apigatewaymanagementapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-apigatewaymanagementapi-1.28.12/setup.py` & `mypy-boto3-apigatewaymanagementapi-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-apigatewaymanagementapi",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_apigatewaymanagementapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ApiGatewayManagementApi 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ApiGatewayManagementApi 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

