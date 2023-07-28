# Comparing `tmp/mypy-boto3-appconfigdata-1.28.12.tar.gz` & `tmp/mypy-boto3-appconfigdata-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appconfigdata-1.28.12.tar", last modified: Thu Jul 27 05:34:16 2023, max compression
+gzip compressed data, was "mypy-boto3-appconfigdata-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-appconfigdata-1.28.12.tar` & `mypy-boto3-appconfigdata-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.416583 mypy-boto3-appconfigdata-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-07-27 05:34:16.412583 mypy-boto3-appconfigdata-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.412583 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:16.412583 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-07-27 05:34:16.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:16.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:16.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:16.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:16.000000 mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:16.416583 mypy-boto3-appconfigdata-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:17:17.000000 mypy-boto3-appconfigdata-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.204654 mypy-boto3-appconfigdata-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-07-28 20:42:16.200654 mypy-boto3-appconfigdata-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10822 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.200654 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8183 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.200654 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12333 2023-07-28 20:42:15.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 20:42:16.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:15.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:15.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:15.000000 mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.204654 mypy-boto3-appconfigdata-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:19:14.000000 mypy-boto3-appconfigdata-1.28.15/setup.py
```

### Comparing `mypy-boto3-appconfigdata-1.28.12/LICENSE` & `mypy-boto3-appconfigdata-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.12/PKG-INFO` & `mypy-boto3-appconfigdata-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfigdata
-Version: 1.28.12
-Summary: Type annotations for boto3.AppConfigData 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppConfigData 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfigdata.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfigdata)](https://pepy.tech/project/mypy-boto3-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfigData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[boto3.AppConfigData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [mypy-boto3-appconfigdata docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,17 +297,17 @@
 
 `mypy_boto3_appconfigdata.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
+    GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
 def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-appconfigdata-1.28.12/README.md` & `mypy-boto3-appconfigdata-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfigdata.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfigdata)](https://pepy.tech/project/mypy-boto3-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfigData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[boto3.AppConfigData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [mypy-boto3-appconfigdata docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,17 +265,17 @@
 
 `mypy_boto3_appconfigdata.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
+    GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
 def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/__main__.py` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppConfigData 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.AppConfigData 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData\nOther"
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

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/client.py` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/client.pyi` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/literals.py` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/literals.pyi` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/type_defs.py` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,39 +20,27 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "GetLatestConfigurationRequestRequestTypeDef",
-    "GetLatestConfigurationResponseTypeDef",
     "ResponseMetadataTypeDef",
     "StartConfigurationSessionRequestRequestTypeDef",
+    "GetLatestConfigurationResponseTypeDef",
     "StartConfigurationSessionResponseTypeDef",
 )
 
 GetLatestConfigurationRequestRequestTypeDef = TypedDict(
     "GetLatestConfigurationRequestRequestTypeDef",
     {
         "ConfigurationToken": str,
     },
 )
 
-GetLatestConfigurationResponseTypeDef = TypedDict(
-    "GetLatestConfigurationResponseTypeDef",
-    {
-        "NextPollConfigurationToken": str,
-        "NextPollIntervalInSeconds": int,
-        "ContentType": str,
-        "Configuration": StreamingBody,
-        "VersionLabel": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -80,14 +68,26 @@
 class StartConfigurationSessionRequestRequestTypeDef(
     _RequiredStartConfigurationSessionRequestRequestTypeDef,
     _OptionalStartConfigurationSessionRequestRequestTypeDef,
 ):
     pass
 
 
+GetLatestConfigurationResponseTypeDef = TypedDict(
+    "GetLatestConfigurationResponseTypeDef",
+    {
+        "NextPollConfigurationToken": str,
+        "NextPollIntervalInSeconds": int,
+        "ContentType": str,
+        "Configuration": StreamingBody,
+        "VersionLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartConfigurationSessionResponseTypeDef = TypedDict(
     "StartConfigurationSessionResponseTypeDef",
     {
         "InitialConfigurationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata/type_defs.pyi` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,39 +19,27 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "GetLatestConfigurationRequestRequestTypeDef",
-    "GetLatestConfigurationResponseTypeDef",
     "ResponseMetadataTypeDef",
     "StartConfigurationSessionRequestRequestTypeDef",
+    "GetLatestConfigurationResponseTypeDef",
     "StartConfigurationSessionResponseTypeDef",
 )
 
 GetLatestConfigurationRequestRequestTypeDef = TypedDict(
     "GetLatestConfigurationRequestRequestTypeDef",
     {
         "ConfigurationToken": str,
     },
 )
 
-GetLatestConfigurationResponseTypeDef = TypedDict(
-    "GetLatestConfigurationResponseTypeDef",
-    {
-        "NextPollConfigurationToken": str,
-        "NextPollIntervalInSeconds": int,
-        "ContentType": str,
-        "Configuration": StreamingBody,
-        "VersionLabel": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -77,14 +65,26 @@
 
 class StartConfigurationSessionRequestRequestTypeDef(
     _RequiredStartConfigurationSessionRequestRequestTypeDef,
     _OptionalStartConfigurationSessionRequestRequestTypeDef,
 ):
     pass
 
+GetLatestConfigurationResponseTypeDef = TypedDict(
+    "GetLatestConfigurationResponseTypeDef",
+    {
+        "NextPollConfigurationToken": str,
+        "NextPollIntervalInSeconds": int,
+        "ContentType": str,
+        "Configuration": StreamingBody,
+        "VersionLabel": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 StartConfigurationSessionResponseTypeDef = TypedDict(
     "StartConfigurationSessionResponseTypeDef",
     {
         "InitialConfigurationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/PKG-INFO` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appconfigdata
-Version: 1.28.12
-Summary: Type annotations for boto3.AppConfigData 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppConfigData 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appconfigdata.svg?color=blue)](https://pypi.org/project/mypy-boto3-appconfigdata)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appconfigdata)](https://pepy.tech/project/mypy-boto3-appconfigdata)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppConfigData 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
+[boto3.AppConfigData 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData)
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
 [mypy-boto3-appconfigdata docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appconfigdata/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,17 +297,17 @@
 
 `mypy_boto3_appconfigdata.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appconfigdata.type_defs import (
     GetLatestConfigurationRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
     ResponseMetadataTypeDef,
     StartConfigurationSessionRequestRequestTypeDef,
+    GetLatestConfigurationResponseTypeDef,
     StartConfigurationSessionResponseTypeDef,
 )
 
 
 def get_structure() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-appconfigdata-1.28.12/mypy_boto3_appconfigdata.egg-info/SOURCES.txt` & `mypy-boto3-appconfigdata-1.28.15/mypy_boto3_appconfigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appconfigdata-1.28.12/setup.py` & `mypy-boto3-appconfigdata-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appconfigdata",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_appconfigdata"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppConfigData 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AppConfigData 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

