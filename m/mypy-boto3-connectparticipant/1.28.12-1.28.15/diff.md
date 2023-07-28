# Comparing `tmp/mypy-boto3-connectparticipant-1.28.12.tar.gz` & `tmp/mypy-boto3-connectparticipant-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-connectparticipant-1.28.12.tar", last modified: Thu Jul 27 05:34:31 2023, max compression
+gzip compressed data, was "mypy-boto3-connectparticipant-1.28.15.tar", last modified: Fri Jul 28 20:42:34 2023, max compression
```

## Comparing `mypy-boto3-connectparticipant-1.28.12.tar` & `mypy-boto3-connectparticipant-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.732542 mypy-boto3-connectparticipant-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-07-27 05:34:31.732542 mypy-boto3-connectparticipant-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.728542 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:31.728542 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-07-27 05:34:31.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:31.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:31.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:31.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:31.000000 mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:31.732542 mypy-boto3-connectparticipant-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-27 05:19:49.000000 mypy-boto3-connectparticipant-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.732913 mypy-boto3-connectparticipant-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-07-28 20:42:34.728913 mypy-boto3-connectparticipant-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.724913 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8619 2023-07-28 20:22:21.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-07-28 20:22:22.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-07-28 20:22:21.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:34.728913 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-07-28 20:42:34.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 20:42:34.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:34.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:34.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 20:42:34.000000 mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:34.732913 mypy-boto3-connectparticipant-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 20:22:20.000000 mypy-boto3-connectparticipant-1.28.15/setup.py
```

### Comparing `mypy-boto3-connectparticipant-1.28.12/LICENSE` & `mypy-boto3-connectparticipant-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.28.12/PKG-INFO` & `mypy-boto3-connectparticipant-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectparticipant
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectParticipant 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConnectParticipant 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectparticipant)](https://pepy.tech/project/mypy-boto3-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectParticipant 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
+[boto3.ConnectParticipant 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [mypy-boto3-connectparticipant docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,27 +307,27 @@
 
 ```python
 from mypy_boto3_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
-    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
-    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    GetAttachmentResponseTypeDef,
+    SendEventResponseTypeDef,
+    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
```

### Comparing `mypy-boto3-connectparticipant-1.28.12/README.md` & `mypy-boto3-connectparticipant-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectparticipant)](https://pepy.tech/project/mypy-boto3-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectParticipant 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
+[boto3.ConnectParticipant 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [mypy-boto3-connectparticipant docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/).
 
 See how it helps to find and fix potential bugs:
 
@@ -275,27 +275,27 @@
 
 ```python
 from mypy_boto3_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
-    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
-    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    GetAttachmentResponseTypeDef,
+    SendEventResponseTypeDef,
+    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
```

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/__main__.py` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ConnectParticipant 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.ConnectParticipant 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant\nOther"
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

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/client.py` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/client.pyi` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/literals.py` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/literals.pyi` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/type_defs.py` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,27 @@
 
 
 __all__ = (
     "AttachmentItemTypeDef",
     "CompleteAttachmentUploadRequestRequestTypeDef",
     "ConnectionCredentialsTypeDef",
     "CreateParticipantConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "WebsocketTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
     "GetAttachmentRequestRequestTypeDef",
-    "GetAttachmentResponseTypeDef",
     "StartPositionTypeDef",
     "ReceiptTypeDef",
-    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
-    "SendEventResponseTypeDef",
     "SendMessageRequestRequestTypeDef",
-    "SendMessageResponseTypeDef",
     "StartAttachmentUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
+    "GetAttachmentResponseTypeDef",
+    "SendEventResponseTypeDef",
+    "SendMessageResponseTypeDef",
     "CreateParticipantConnectionResponseTypeDef",
     "GetTranscriptRequestRequestTypeDef",
     "MessageMetadataTypeDef",
     "StartAttachmentUploadResponseTypeDef",
     "ItemTypeDef",
     "GetTranscriptResponseTypeDef",
 )
@@ -103,14 +103,25 @@
 class CreateParticipantConnectionRequestRequestTypeDef(
     _RequiredCreateParticipantConnectionRequestRequestTypeDef,
     _OptionalCreateParticipantConnectionRequestRequestTypeDef,
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
 WebsocketTypeDef = TypedDict(
     "WebsocketTypeDef",
     {
         "Url": str,
         "ConnectionExpiry": str,
     },
     total=False,
@@ -142,23 +153,14 @@
     "GetAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
         "ConnectionToken": str,
     },
 )
 
-GetAttachmentResponseTypeDef = TypedDict(
-    "GetAttachmentResponseTypeDef",
-    {
-        "Url": str,
-        "UrlExpiry": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartPositionTypeDef = TypedDict(
     "StartPositionTypeDef",
     {
         "Id": str,
         "AbsoluteTime": str,
         "MostRecent": int,
     },
@@ -171,25 +173,14 @@
         "DeliveredTimestamp": str,
         "ReadTimestamp": str,
         "RecipientParticipantId": str,
     },
     total=False,
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
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
         "ContentType": str,
         "ConnectionToken": str,
     },
 )
@@ -205,23 +196,14 @@
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
 
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "ContentType": str,
         "Content": str,
         "ConnectionToken": str,
     },
@@ -237,23 +219,14 @@
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
 
-SendMessageResponseTypeDef = TypedDict(
-    "SendMessageResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartAttachmentUploadRequestRequestTypeDef = TypedDict(
     "StartAttachmentUploadRequestRequestTypeDef",
     {
         "ContentType": str,
         "AttachmentSizeInBytes": int,
         "AttachmentName": str,
         "ClientToken": str,
@@ -267,20 +240,47 @@
         "Url": str,
         "UrlExpiry": str,
         "HeadersToInclude": Dict[str, str],
     },
     total=False,
 )
 
+GetAttachmentResponseTypeDef = TypedDict(
+    "GetAttachmentResponseTypeDef",
+    {
+        "Url": str,
+        "UrlExpiry": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendMessageResponseTypeDef = TypedDict(
+    "SendMessageResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateParticipantConnectionResponseTypeDef = TypedDict(
     "CreateParticipantConnectionResponseTypeDef",
     {
         "Websocket": WebsocketTypeDef,
         "ConnectionCredentials": ConnectionCredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTranscriptRequestRequestTypeDef = TypedDict(
     "_RequiredGetTranscriptRequestRequestTypeDef",
     {
         "ConnectionToken": str,
@@ -316,15 +316,15 @@
 )
 
 StartAttachmentUploadResponseTypeDef = TypedDict(
     "StartAttachmentUploadResponseTypeDef",
     {
         "AttachmentId": str,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "AbsoluteTime": str,
@@ -345,10 +345,10 @@
 
 GetTranscriptResponseTypeDef = TypedDict(
     "GetTranscriptResponseTypeDef",
     {
         "InitialContactId": str,
         "Transcript": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant/type_defs.pyi` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -29,27 +29,27 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttachmentItemTypeDef",
     "CompleteAttachmentUploadRequestRequestTypeDef",
     "ConnectionCredentialsTypeDef",
     "CreateParticipantConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "WebsocketTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
     "GetAttachmentRequestRequestTypeDef",
-    "GetAttachmentResponseTypeDef",
     "StartPositionTypeDef",
     "ReceiptTypeDef",
-    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
-    "SendEventResponseTypeDef",
     "SendMessageRequestRequestTypeDef",
-    "SendMessageResponseTypeDef",
     "StartAttachmentUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
+    "GetAttachmentResponseTypeDef",
+    "SendEventResponseTypeDef",
+    "SendMessageResponseTypeDef",
     "CreateParticipantConnectionResponseTypeDef",
     "GetTranscriptRequestRequestTypeDef",
     "MessageMetadataTypeDef",
     "StartAttachmentUploadResponseTypeDef",
     "ItemTypeDef",
     "GetTranscriptResponseTypeDef",
 )
@@ -100,14 +100,25 @@
 
 class CreateParticipantConnectionRequestRequestTypeDef(
     _RequiredCreateParticipantConnectionRequestRequestTypeDef,
     _OptionalCreateParticipantConnectionRequestRequestTypeDef,
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
 WebsocketTypeDef = TypedDict(
     "WebsocketTypeDef",
     {
         "Url": str,
         "ConnectionExpiry": str,
     },
     total=False,
@@ -137,23 +148,14 @@
     "GetAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
         "ConnectionToken": str,
     },
 )
 
-GetAttachmentResponseTypeDef = TypedDict(
-    "GetAttachmentResponseTypeDef",
-    {
-        "Url": str,
-        "UrlExpiry": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartPositionTypeDef = TypedDict(
     "StartPositionTypeDef",
     {
         "Id": str,
         "AbsoluteTime": str,
         "MostRecent": int,
     },
@@ -166,25 +168,14 @@
         "DeliveredTimestamp": str,
         "ReadTimestamp": str,
         "RecipientParticipantId": str,
     },
     total=False,
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
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
         "ContentType": str,
         "ConnectionToken": str,
     },
 )
@@ -198,23 +189,14 @@
 )
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "ContentType": str,
         "Content": str,
         "ConnectionToken": str,
     },
@@ -228,23 +210,14 @@
 )
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
-SendMessageResponseTypeDef = TypedDict(
-    "SendMessageResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartAttachmentUploadRequestRequestTypeDef = TypedDict(
     "StartAttachmentUploadRequestRequestTypeDef",
     {
         "ContentType": str,
         "AttachmentSizeInBytes": int,
         "AttachmentName": str,
         "ClientToken": str,
@@ -258,20 +231,47 @@
         "Url": str,
         "UrlExpiry": str,
         "HeadersToInclude": Dict[str, str],
     },
     total=False,
 )
 
+GetAttachmentResponseTypeDef = TypedDict(
+    "GetAttachmentResponseTypeDef",
+    {
+        "Url": str,
+        "UrlExpiry": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendMessageResponseTypeDef = TypedDict(
+    "SendMessageResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateParticipantConnectionResponseTypeDef = TypedDict(
     "CreateParticipantConnectionResponseTypeDef",
     {
         "Websocket": WebsocketTypeDef,
         "ConnectionCredentials": ConnectionCredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTranscriptRequestRequestTypeDef = TypedDict(
     "_RequiredGetTranscriptRequestRequestTypeDef",
     {
         "ConnectionToken": str,
@@ -305,15 +305,15 @@
 )
 
 StartAttachmentUploadResponseTypeDef = TypedDict(
     "StartAttachmentUploadResponseTypeDef",
     {
         "AttachmentId": str,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "AbsoluteTime": str,
@@ -334,10 +334,10 @@
 
 GetTranscriptResponseTypeDef = TypedDict(
     "GetTranscriptResponseTypeDef",
     {
         "InitialContactId": str,
         "Transcript": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/PKG-INFO` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-connectparticipant
-Version: 1.28.12
-Summary: Type annotations for boto3.ConnectParticipant 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ConnectParticipant 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-connectparticipant.svg?color=blue)](https://pypi.org/project/mypy-boto3-connectparticipant)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-connectparticipant)](https://pepy.tech/project/mypy-boto3-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ConnectParticipant 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
+[boto3.ConnectParticipant 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [mypy-boto3-connectparticipant docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_connectparticipant/).
 
 See how it helps to find and fix potential bugs:
 
@@ -307,27 +307,27 @@
 
 ```python
 from mypy_boto3_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
-    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
-    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    GetAttachmentResponseTypeDef,
+    SendEventResponseTypeDef,
+    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
```

### Comparing `mypy-boto3-connectparticipant-1.28.12/mypy_boto3_connectparticipant.egg-info/SOURCES.txt` & `mypy-boto3-connectparticipant-1.28.15/mypy_boto3_connectparticipant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-connectparticipant-1.28.12/setup.py` & `mypy-boto3-connectparticipant-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-connectparticipant",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_connectparticipant"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ConnectParticipant 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.ConnectParticipant 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

