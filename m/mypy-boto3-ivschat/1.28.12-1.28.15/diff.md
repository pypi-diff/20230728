# Comparing `tmp/mypy-boto3-ivschat-1.28.12.tar.gz` & `tmp/mypy-boto3-ivschat-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivschat-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
+gzip compressed data, was "mypy-boto3-ivschat-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
```

## Comparing `mypy-boto3-ivschat-1.28.12.tar` & `mypy-boto3-ivschat-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.752474 mypy-boto3-ivschat-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-07-27 05:34:51.744475 mypy-boto3-ivschat-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12232 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.736474 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-27 05:24:26.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15629 2023-07-27 05:24:26.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.744475 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13719 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:51.000000 mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.752474 mypy-boto3-ivschat-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:24:25.000000 mypy-boto3-ivschat-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.613300 mypy-boto3-ivschat-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-07-28 20:43:02.605300 mypy-boto3-ivschat-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11991 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.605300 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13477 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-07-28 20:28:56.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.605300 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13478 2023-07-28 20:43:02.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-28 20:43:02.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:43:02.000000 mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.613300 mypy-boto3-ivschat-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:28:55.000000 mypy-boto3-ivschat-1.28.15/setup.py
```

### Comparing `mypy-boto3-ivschat-1.28.12/LICENSE` & `mypy-boto3-ivschat-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.12/PKG-INFO` & `mypy-boto3-ivschat-1.28.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivschat
-Version: 1.28.12
-Summary: Type annotations for boto3.ivschat 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ivschat 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,61 +300,56 @@
 ### Typed dictionaries
 
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
-    CloudWatchLogsDestinationConfigurationOutputTypeDef,
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     MessageReviewHandlerTypeDef,
-    MessageReviewHandlerOutputTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
-    DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
-    FirehoseDestinationConfigurationOutputTypeDef,
-    S3DestinationConfigurationOutputTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateChatTokenResponseTypeDef,
+    DeleteMessageResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendEventResponseTypeDef,
     CreateRoomRequestRequestTypeDef,
-    UpdateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
+    UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
-    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     ListRoomsResponseTypeDef,
+    CreateLoggingConfigurationRequestRequestTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
+    UpdateLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsDestinationConfigurationOutputTypeDef:
+def get_structure() -> CloudWatchLogsDestinationConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivschat-1.28.12/README.md` & `mypy-boto3-ivschat-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -268,61 +268,56 @@
 ### Typed dictionaries
 
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
-    CloudWatchLogsDestinationConfigurationOutputTypeDef,
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     MessageReviewHandlerTypeDef,
-    MessageReviewHandlerOutputTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
-    DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
-    FirehoseDestinationConfigurationOutputTypeDef,
-    S3DestinationConfigurationOutputTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateChatTokenResponseTypeDef,
+    DeleteMessageResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendEventResponseTypeDef,
     CreateRoomRequestRequestTypeDef,
-    UpdateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
+    UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
-    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     ListRoomsResponseTypeDef,
+    CreateLoggingConfigurationRequestRequestTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
+    UpdateLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsDestinationConfigurationOutputTypeDef:
+def get_structure() -> CloudWatchLogsDestinationConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/__main__.py` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ivschat 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.ivschat 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat\nOther"
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

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/client.py` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/client.pyi` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/literals.py` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/literals.pyi` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/type_defs.py` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ivschat service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ivschat.type_defs import CloudWatchLogsDestinationConfigurationOutputTypeDef
+    from mypy_boto3_ivschat.type_defs import CloudWatchLogsDestinationConfigurationTypeDef
 
-    data: CloudWatchLogsDestinationConfigurationOutputTypeDef = {...}
+    data: CloudWatchLogsDestinationConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ChatTokenCapabilityType, FallbackResultType, LoggingConfigurationStateType
@@ -24,66 +24,54 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "CloudWatchLogsDestinationConfigurationOutputTypeDef",
     "CloudWatchLogsDestinationConfigurationTypeDef",
     "CreateChatTokenRequestRequestTypeDef",
-    "CreateChatTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "MessageReviewHandlerTypeDef",
-    "MessageReviewHandlerOutputTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteMessageRequestRequestTypeDef",
-    "DeleteMessageResponseTypeDef",
     "DeleteRoomRequestRequestTypeDef",
-    "FirehoseDestinationConfigurationOutputTypeDef",
-    "S3DestinationConfigurationOutputTypeDef",
     "FirehoseDestinationConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "DisconnectUserRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
-    "SendEventResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateChatTokenResponseTypeDef",
+    "DeleteMessageResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SendEventResponseTypeDef",
     "CreateRoomRequestRequestTypeDef",
-    "UpdateRoomRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "RoomSummaryTypeDef",
+    "UpdateRoomRequestRequestTypeDef",
     "UpdateRoomResponseTypeDef",
-    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "ListRoomsResponseTypeDef",
+    "CreateLoggingConfigurationRequestRequestTypeDef",
     "CreateLoggingConfigurationResponseTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "LoggingConfigurationSummaryTypeDef",
-    "UpdateLoggingConfigurationResponseTypeDef",
-    "CreateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
+    "UpdateLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
 )
 
-CloudWatchLogsDestinationConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchLogsDestinationConfigurationOutputTypeDef",
-    {
-        "logGroupName": str,
-    },
-)
-
 CloudWatchLogsDestinationConfigurationTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigurationTypeDef",
     {
         "logGroupName": str,
     },
 )
 
@@ -107,42 +95,34 @@
 
 class CreateChatTokenRequestRequestTypeDef(
     _RequiredCreateChatTokenRequestRequestTypeDef, _OptionalCreateChatTokenRequestRequestTypeDef
 ):
     pass
 
 
-CreateChatTokenResponseTypeDef = TypedDict(
-    "CreateChatTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "sessionExpirationTime": datetime,
-        "token": str,
-        "tokenExpirationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 MessageReviewHandlerTypeDef = TypedDict(
     "MessageReviewHandlerTypeDef",
     {
         "fallbackResult": FallbackResultType,
         "uri": str,
     },
     total=False,
 )
 
-MessageReviewHandlerOutputTypeDef = TypedDict(
-    "MessageReviewHandlerOutputTypeDef",
-    {
-        "fallbackResult": FallbackResultType,
-        "uri": str,
-    },
-    total=False,
-)
-
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -164,43 +144,21 @@
 
 class DeleteMessageRequestRequestTypeDef(
     _RequiredDeleteMessageRequestRequestTypeDef, _OptionalDeleteMessageRequestRequestTypeDef
 ):
     pass
 
 
-DeleteMessageResponseTypeDef = TypedDict(
-    "DeleteMessageResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRoomRequestRequestTypeDef = TypedDict(
     "DeleteRoomRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
-FirehoseDestinationConfigurationOutputTypeDef = TypedDict(
-    "FirehoseDestinationConfigurationOutputTypeDef",
-    {
-        "deliveryStreamName": str,
-    },
-)
-
-S3DestinationConfigurationOutputTypeDef = TypedDict(
-    "S3DestinationConfigurationOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-
 FirehoseDestinationConfigurationTypeDef = TypedDict(
     "FirehoseDestinationConfigurationTypeDef",
     {
         "deliveryStreamName": str,
     },
 )
 
@@ -229,21 +187,14 @@
 
 class DisconnectUserRequestRequestTypeDef(
     _RequiredDisconnectUserRequestRequestTypeDef, _OptionalDisconnectUserRequestRequestTypeDef
 ):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -278,33 +229,14 @@
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
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
         "eventName": str,
         "roomIdentifier": str,
     },
 )
@@ -319,22 +251,14 @@
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
 
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -343,128 +267,159 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateRoomRequestRequestTypeDef = TypedDict(
-    "CreateRoomRequestRequestTypeDef",
+CreateChatTokenResponseTypeDef = TypedDict(
+    "CreateChatTokenResponseTypeDef",
     {
-        "loggingConfigurationIdentifiers": Sequence[str],
-        "maximumMessageLength": int,
-        "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
-        "name": str,
-        "tags": Mapping[str, str],
+        "sessionExpirationTime": datetime,
+        "token": str,
+        "tokenExpirationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredUpdateRoomRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRoomRequestRequestTypeDef",
+DeleteMessageResponseTypeDef = TypedDict(
+    "DeleteMessageResponseTypeDef",
     {
-        "identifier": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateRoomRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRoomRequestRequestTypeDef",
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRoomRequestRequestTypeDef = TypedDict(
+    "CreateRoomRequestRequestTypeDef",
     {
         "loggingConfigurationIdentifiers": Sequence[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
-class UpdateRoomRequestRequestTypeDef(
-    _RequiredUpdateRoomRequestRequestTypeDef, _OptionalUpdateRoomRequestRequestTypeDef
-):
-    pass
-
-
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RoomSummaryTypeDef = TypedDict(
     "RoomSummaryTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
-        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
     },
     total=False,
 )
 
+_RequiredUpdateRoomRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRoomRequestRequestTypeDef",
+    {
+        "identifier": str,
+    },
+)
+_OptionalUpdateRoomRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRoomRequestRequestTypeDef",
+    {
+        "loggingConfigurationIdentifiers": Sequence[str],
+        "maximumMessageLength": int,
+        "maximumMessageRatePerSecond": int,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "name": str,
+    },
+    total=False,
+)
+
+
+class UpdateRoomRequestRequestTypeDef(
+    _RequiredUpdateRoomRequestRequestTypeDef, _OptionalUpdateRoomRequestRequestTypeDef
+):
+    pass
+
+
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DestinationConfigurationOutputTypeDef = TypedDict(
-    "DestinationConfigurationOutputTypeDef",
-    {
-        "cloudWatchLogs": CloudWatchLogsDestinationConfigurationOutputTypeDef,
-        "firehose": FirehoseDestinationConfigurationOutputTypeDef,
-        "s3": S3DestinationConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsDestinationConfigurationTypeDef,
         "firehose": FirehoseDestinationConfigurationTypeDef,
         "s3": S3DestinationConfigurationTypeDef,
     },
@@ -472,101 +427,86 @@
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "nextToken": str,
         "rooms": List[RoomSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
+    {
+        "destinationConfiguration": DestinationConfigurationTypeDef,
+    },
+)
+_OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
+
+class CreateLoggingConfigurationRequestRequestTypeDef(
+    _RequiredCreateLoggingConfigurationRequestRequestTypeDef,
+    _OptionalCreateLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 CreateLoggingConfigurationResponseTypeDef = TypedDict(
     "CreateLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": Literal["ACTIVE"],
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingConfigurationSummaryTypeDef = TypedDict(
     "LoggingConfigurationSummaryTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
     },
     total=False,
 )
 
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
-    {
-        "arn": str,
-        "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
-        "id": str,
-        "name": str,
-        "state": Literal["ACTIVE"],
-        "tags": Dict[str, str],
-        "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateLoggingConfigurationRequestRequestTypeDef(
-    _RequiredCreateLoggingConfigurationRequestRequestTypeDef,
-    _OptionalCreateLoggingConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 _OptionalUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
@@ -582,15 +522,30 @@
 class UpdateLoggingConfigurationRequestRequestTypeDef(
     _RequiredUpdateLoggingConfigurationRequestRequestTypeDef,
     _OptionalUpdateLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
+    {
+        "arn": str,
+        "createTime": datetime,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "id": str,
+        "name": str,
+        "state": Literal["ACTIVE"],
+        "tags": Dict[str, str],
+        "updateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
         "loggingConfigurations": List[LoggingConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat/type_defs.pyi` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for ivschat service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_ivschat.type_defs import CloudWatchLogsDestinationConfigurationOutputTypeDef
+    from mypy_boto3_ivschat.type_defs import CloudWatchLogsDestinationConfigurationTypeDef
 
-    data: CloudWatchLogsDestinationConfigurationOutputTypeDef = {...}
+    data: CloudWatchLogsDestinationConfigurationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ChatTokenCapabilityType, FallbackResultType, LoggingConfigurationStateType
@@ -23,66 +23,54 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "CloudWatchLogsDestinationConfigurationOutputTypeDef",
     "CloudWatchLogsDestinationConfigurationTypeDef",
     "CreateChatTokenRequestRequestTypeDef",
-    "CreateChatTokenResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "MessageReviewHandlerTypeDef",
-    "MessageReviewHandlerOutputTypeDef",
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     "DeleteMessageRequestRequestTypeDef",
-    "DeleteMessageResponseTypeDef",
     "DeleteRoomRequestRequestTypeDef",
-    "FirehoseDestinationConfigurationOutputTypeDef",
-    "S3DestinationConfigurationOutputTypeDef",
     "FirehoseDestinationConfigurationTypeDef",
     "S3DestinationConfigurationTypeDef",
     "DisconnectUserRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "GetLoggingConfigurationRequestRequestTypeDef",
     "GetRoomRequestRequestTypeDef",
     "ListLoggingConfigurationsRequestRequestTypeDef",
     "ListRoomsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
-    "SendEventResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CreateChatTokenResponseTypeDef",
+    "DeleteMessageResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "SendEventResponseTypeDef",
     "CreateRoomRequestRequestTypeDef",
-    "UpdateRoomRequestRequestTypeDef",
     "CreateRoomResponseTypeDef",
     "GetRoomResponseTypeDef",
     "RoomSummaryTypeDef",
+    "UpdateRoomRequestRequestTypeDef",
     "UpdateRoomResponseTypeDef",
-    "DestinationConfigurationOutputTypeDef",
     "DestinationConfigurationTypeDef",
     "ListRoomsResponseTypeDef",
+    "CreateLoggingConfigurationRequestRequestTypeDef",
     "CreateLoggingConfigurationResponseTypeDef",
     "GetLoggingConfigurationResponseTypeDef",
     "LoggingConfigurationSummaryTypeDef",
-    "UpdateLoggingConfigurationResponseTypeDef",
-    "CreateLoggingConfigurationRequestRequestTypeDef",
     "UpdateLoggingConfigurationRequestRequestTypeDef",
+    "UpdateLoggingConfigurationResponseTypeDef",
     "ListLoggingConfigurationsResponseTypeDef",
 )
 
-CloudWatchLogsDestinationConfigurationOutputTypeDef = TypedDict(
-    "CloudWatchLogsDestinationConfigurationOutputTypeDef",
-    {
-        "logGroupName": str,
-    },
-)
-
 CloudWatchLogsDestinationConfigurationTypeDef = TypedDict(
     "CloudWatchLogsDestinationConfigurationTypeDef",
     {
         "logGroupName": str,
     },
 )
 
@@ -104,42 +92,34 @@
 )
 
 class CreateChatTokenRequestRequestTypeDef(
     _RequiredCreateChatTokenRequestRequestTypeDef, _OptionalCreateChatTokenRequestRequestTypeDef
 ):
     pass
 
-CreateChatTokenResponseTypeDef = TypedDict(
-    "CreateChatTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "sessionExpirationTime": datetime,
-        "token": str,
-        "tokenExpirationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 MessageReviewHandlerTypeDef = TypedDict(
     "MessageReviewHandlerTypeDef",
     {
         "fallbackResult": FallbackResultType,
         "uri": str,
     },
     total=False,
 )
 
-MessageReviewHandlerOutputTypeDef = TypedDict(
-    "MessageReviewHandlerOutputTypeDef",
-    {
-        "fallbackResult": FallbackResultType,
-        "uri": str,
-    },
-    total=False,
-)
-
 DeleteLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -159,43 +139,21 @@
 )
 
 class DeleteMessageRequestRequestTypeDef(
     _RequiredDeleteMessageRequestRequestTypeDef, _OptionalDeleteMessageRequestRequestTypeDef
 ):
     pass
 
-DeleteMessageResponseTypeDef = TypedDict(
-    "DeleteMessageResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRoomRequestRequestTypeDef = TypedDict(
     "DeleteRoomRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
-FirehoseDestinationConfigurationOutputTypeDef = TypedDict(
-    "FirehoseDestinationConfigurationOutputTypeDef",
-    {
-        "deliveryStreamName": str,
-    },
-)
-
-S3DestinationConfigurationOutputTypeDef = TypedDict(
-    "S3DestinationConfigurationOutputTypeDef",
-    {
-        "bucketName": str,
-    },
-)
-
 FirehoseDestinationConfigurationTypeDef = TypedDict(
     "FirehoseDestinationConfigurationTypeDef",
     {
         "deliveryStreamName": str,
     },
 )
 
@@ -222,21 +180,14 @@
 )
 
 class DisconnectUserRequestRequestTypeDef(
     _RequiredDisconnectUserRequestRequestTypeDef, _OptionalDisconnectUserRequestRequestTypeDef
 ):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "GetLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 
@@ -271,33 +222,14 @@
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
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
         "eventName": str,
         "roomIdentifier": str,
     },
 )
@@ -310,22 +242,14 @@
 )
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -334,124 +258,155 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-CreateRoomRequestRequestTypeDef = TypedDict(
-    "CreateRoomRequestRequestTypeDef",
+CreateChatTokenResponseTypeDef = TypedDict(
+    "CreateChatTokenResponseTypeDef",
     {
-        "loggingConfigurationIdentifiers": Sequence[str],
-        "maximumMessageLength": int,
-        "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerTypeDef,
-        "name": str,
-        "tags": Mapping[str, str],
+        "sessionExpirationTime": datetime,
+        "token": str,
+        "tokenExpirationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredUpdateRoomRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateRoomRequestRequestTypeDef",
+DeleteMessageResponseTypeDef = TypedDict(
+    "DeleteMessageResponseTypeDef",
     {
-        "identifier": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateRoomRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateRoomRequestRequestTypeDef",
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRoomRequestRequestTypeDef = TypedDict(
+    "CreateRoomRequestRequestTypeDef",
     {
         "loggingConfigurationIdentifiers": Sequence[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
         "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class UpdateRoomRequestRequestTypeDef(
-    _RequiredUpdateRoomRequestRequestTypeDef, _OptionalUpdateRoomRequestRequestTypeDef
-):
-    pass
-
 CreateRoomResponseTypeDef = TypedDict(
     "CreateRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoomResponseTypeDef = TypedDict(
     "GetRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RoomSummaryTypeDef = TypedDict(
     "RoomSummaryTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
-        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
     },
     total=False,
 )
 
+_RequiredUpdateRoomRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateRoomRequestRequestTypeDef",
+    {
+        "identifier": str,
+    },
+)
+_OptionalUpdateRoomRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateRoomRequestRequestTypeDef",
+    {
+        "loggingConfigurationIdentifiers": Sequence[str],
+        "maximumMessageLength": int,
+        "maximumMessageRatePerSecond": int,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
+        "name": str,
+    },
+    total=False,
+)
+
+class UpdateRoomRequestRequestTypeDef(
+    _RequiredUpdateRoomRequestRequestTypeDef, _OptionalUpdateRoomRequestRequestTypeDef
+):
+    pass
+
 UpdateRoomResponseTypeDef = TypedDict(
     "UpdateRoomResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
         "id": str,
         "loggingConfigurationIdentifiers": List[str],
         "maximumMessageLength": int,
         "maximumMessageRatePerSecond": int,
-        "messageReviewHandler": MessageReviewHandlerOutputTypeDef,
+        "messageReviewHandler": MessageReviewHandlerTypeDef,
         "name": str,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DestinationConfigurationOutputTypeDef = TypedDict(
-    "DestinationConfigurationOutputTypeDef",
-    {
-        "cloudWatchLogs": CloudWatchLogsDestinationConfigurationOutputTypeDef,
-        "firehose": FirehoseDestinationConfigurationOutputTypeDef,
-        "s3": S3DestinationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DestinationConfigurationTypeDef = TypedDict(
     "DestinationConfigurationTypeDef",
     {
         "cloudWatchLogs": CloudWatchLogsDestinationConfigurationTypeDef,
         "firehose": FirehoseDestinationConfigurationTypeDef,
@@ -461,99 +416,84 @@
 )
 
 ListRoomsResponseTypeDef = TypedDict(
     "ListRoomsResponseTypeDef",
     {
         "nextToken": str,
         "rooms": List[RoomSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
+    {
+        "destinationConfiguration": DestinationConfigurationTypeDef,
+    },
+)
+_OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
+    {
+        "name": str,
+        "tags": Mapping[str, str],
     },
+    total=False,
 )
 
+class CreateLoggingConfigurationRequestRequestTypeDef(
+    _RequiredCreateLoggingConfigurationRequestRequestTypeDef,
+    _OptionalCreateLoggingConfigurationRequestRequestTypeDef,
+):
+    pass
+
 CreateLoggingConfigurationResponseTypeDef = TypedDict(
     "CreateLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": Literal["ACTIVE"],
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoggingConfigurationResponseTypeDef = TypedDict(
     "GetLoggingConfigurationResponseTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoggingConfigurationSummaryTypeDef = TypedDict(
     "LoggingConfigurationSummaryTypeDef",
     {
         "arn": str,
         "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
         "id": str,
         "name": str,
         "state": LoggingConfigurationStateType,
         "tags": Dict[str, str],
         "updateTime": datetime,
     },
     total=False,
 )
 
-UpdateLoggingConfigurationResponseTypeDef = TypedDict(
-    "UpdateLoggingConfigurationResponseTypeDef",
-    {
-        "arn": str,
-        "createTime": datetime,
-        "destinationConfiguration": DestinationConfigurationOutputTypeDef,
-        "id": str,
-        "name": str,
-        "state": Literal["ACTIVE"],
-        "tags": Dict[str, str],
-        "updateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLoggingConfigurationRequestRequestTypeDef",
-    {
-        "destinationConfiguration": DestinationConfigurationTypeDef,
-    },
-)
-_OptionalCreateLoggingConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLoggingConfigurationRequestRequestTypeDef",
-    {
-        "name": str,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateLoggingConfigurationRequestRequestTypeDef(
-    _RequiredCreateLoggingConfigurationRequestRequestTypeDef,
-    _OptionalCreateLoggingConfigurationRequestRequestTypeDef,
-):
-    pass
-
 _RequiredUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLoggingConfigurationRequestRequestTypeDef",
     {
         "identifier": str,
     },
 )
 _OptionalUpdateLoggingConfigurationRequestRequestTypeDef = TypedDict(
@@ -567,15 +507,30 @@
 
 class UpdateLoggingConfigurationRequestRequestTypeDef(
     _RequiredUpdateLoggingConfigurationRequestRequestTypeDef,
     _OptionalUpdateLoggingConfigurationRequestRequestTypeDef,
 ):
     pass
 
+UpdateLoggingConfigurationResponseTypeDef = TypedDict(
+    "UpdateLoggingConfigurationResponseTypeDef",
+    {
+        "arn": str,
+        "createTime": datetime,
+        "destinationConfiguration": DestinationConfigurationTypeDef,
+        "id": str,
+        "name": str,
+        "state": Literal["ACTIVE"],
+        "tags": Dict[str, str],
+        "updateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListLoggingConfigurationsResponseTypeDef = TypedDict(
     "ListLoggingConfigurationsResponseTypeDef",
     {
         "loggingConfigurations": List[LoggingConfigurationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/PKG-INFO` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivschat
-Version: 1.28.12
-Summary: Type annotations for boto3.ivschat 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ivschat 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivschat.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivschat)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivschat)](https://pepy.tech/project/mypy-boto3-ivschat)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivschat 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
+[boto3.ivschat 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivschat.html#ivschat)
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
 [mypy-boto3-ivschat docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivschat/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,61 +300,56 @@
 ### Typed dictionaries
 
 `mypy_boto3_ivschat.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivschat.type_defs import (
-    CloudWatchLogsDestinationConfigurationOutputTypeDef,
     CloudWatchLogsDestinationConfigurationTypeDef,
     CreateChatTokenRequestRequestTypeDef,
-    CreateChatTokenResponseTypeDef,
+    ResponseMetadataTypeDef,
     MessageReviewHandlerTypeDef,
-    MessageReviewHandlerOutputTypeDef,
     DeleteLoggingConfigurationRequestRequestTypeDef,
     DeleteMessageRequestRequestTypeDef,
-    DeleteMessageResponseTypeDef,
     DeleteRoomRequestRequestTypeDef,
-    FirehoseDestinationConfigurationOutputTypeDef,
-    S3DestinationConfigurationOutputTypeDef,
     FirehoseDestinationConfigurationTypeDef,
     S3DestinationConfigurationTypeDef,
     DisconnectUserRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     GetLoggingConfigurationRequestRequestTypeDef,
     GetRoomRequestRequestTypeDef,
     ListLoggingConfigurationsRequestRequestTypeDef,
     ListRoomsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CreateChatTokenResponseTypeDef,
+    DeleteMessageResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    SendEventResponseTypeDef,
     CreateRoomRequestRequestTypeDef,
-    UpdateRoomRequestRequestTypeDef,
     CreateRoomResponseTypeDef,
     GetRoomResponseTypeDef,
     RoomSummaryTypeDef,
+    UpdateRoomRequestRequestTypeDef,
     UpdateRoomResponseTypeDef,
-    DestinationConfigurationOutputTypeDef,
     DestinationConfigurationTypeDef,
     ListRoomsResponseTypeDef,
+    CreateLoggingConfigurationRequestRequestTypeDef,
     CreateLoggingConfigurationResponseTypeDef,
     GetLoggingConfigurationResponseTypeDef,
     LoggingConfigurationSummaryTypeDef,
-    UpdateLoggingConfigurationResponseTypeDef,
-    CreateLoggingConfigurationRequestRequestTypeDef,
     UpdateLoggingConfigurationRequestRequestTypeDef,
+    UpdateLoggingConfigurationResponseTypeDef,
     ListLoggingConfigurationsResponseTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLogsDestinationConfigurationOutputTypeDef:
+def get_structure() -> CloudWatchLogsDestinationConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-ivschat-1.28.12/mypy_boto3_ivschat.egg-info/SOURCES.txt` & `mypy-boto3-ivschat-1.28.15/mypy_boto3_ivschat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivschat-1.28.12/setup.py` & `mypy-boto3-ivschat-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivschat",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ivschat"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ivschat 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ivschat 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

