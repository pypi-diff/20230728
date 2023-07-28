# Comparing `tmp/mypy-boto3-backupstorage-1.28.12.tar.gz` & `tmp/mypy-boto3-backupstorage-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-backupstorage-1.28.12.tar", last modified: Thu Jul 27 05:34:21 2023, max compression
+gzip compressed data, was "mypy-boto3-backupstorage-1.28.15.tar", last modified: Fri Jul 28 20:42:22 2023, max compression
```

## Comparing `mypy-boto3-backupstorage-1.28.12.tar` & `mypy-boto3-backupstorage-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:21.884569 mypy-boto3-backupstorage-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-27 05:34:21.884569 mypy-boto3-backupstorage-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:21.880569 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-27 05:17:56.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8459 2023-07-27 05:17:56.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-27 05:17:56.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:21.884569 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:21.000000 mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:21.884569 mypy-boto3-backupstorage-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:17:55.000000 mypy-boto3-backupstorage-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.248736 mypy-boto3-backupstorage-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-28 20:42:22.244736 mypy-boto3-backupstorage-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.244736 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9870 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:20:08.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:22.244736 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-07-28 20:42:22.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 20:42:22.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:22.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:22.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:22.000000 mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:22.248736 mypy-boto3-backupstorage-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:20:07.000000 mypy-boto3-backupstorage-1.28.15/setup.py
```

### Comparing `mypy-boto3-backupstorage-1.28.12/LICENSE` & `mypy-boto3-backupstorage-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.12/PKG-INFO` & `mypy-boto3-backupstorage-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backupstorage
-Version: 1.28.12
-Summary: Type annotations for boto3.BackupStorage 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.BackupStorage 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,32 +301,32 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
-    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
-    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
     ListObjectsInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
     PutChunkInputRequestTypeDef,
-    PutChunkOutputTypeDef,
     PutObjectInputRequestTypeDef,
-    PutObjectOutputTypeDef,
-    ResponseMetadataTypeDef,
     StartObjectInputRequestTypeDef,
-    StartObjectOutputTypeDef,
-    ListObjectsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChunkOutputTypeDef,
+    GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    NotifyObjectCompleteOutputTypeDef,
+    PutChunkOutputTypeDef,
+    PutObjectOutputTypeDef,
+    StartObjectOutputTypeDef,
 )
 
 
 def get_structure() -> BackupObjectTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-backupstorage-1.28.12/README.md` & `mypy-boto3-backupstorage-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,32 +269,32 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
-    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
-    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
     ListObjectsInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
     PutChunkInputRequestTypeDef,
-    PutChunkOutputTypeDef,
     PutObjectInputRequestTypeDef,
-    PutObjectOutputTypeDef,
-    ResponseMetadataTypeDef,
     StartObjectInputRequestTypeDef,
-    StartObjectOutputTypeDef,
-    ListObjectsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChunkOutputTypeDef,
+    GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    NotifyObjectCompleteOutputTypeDef,
+    PutChunkOutputTypeDef,
+    PutObjectOutputTypeDef,
+    StartObjectOutputTypeDef,
 )
 
 
 def get_structure() -> BackupObjectTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/__main__.py` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.BackupStorage 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.BackupStorage 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage\nOther"
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

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/client.py` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/client.pyi` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/literals.py` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/literals.pyi` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/type_defs.py` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,32 +27,32 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BackupObjectTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
-    "GetChunkOutputTypeDef",
     "GetObjectMetadataInputRequestTypeDef",
-    "GetObjectMetadataOutputTypeDef",
     "ListChunksInputRequestTypeDef",
     "ListObjectsInputRequestTypeDef",
     "NotifyObjectCompleteInputRequestTypeDef",
-    "NotifyObjectCompleteOutputTypeDef",
     "PutChunkInputRequestTypeDef",
-    "PutChunkOutputTypeDef",
     "PutObjectInputRequestTypeDef",
-    "PutObjectOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "StartObjectInputRequestTypeDef",
-    "StartObjectOutputTypeDef",
-    "ListObjectsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetChunkOutputTypeDef",
+    "GetObjectMetadataOutputTypeDef",
     "ListChunksOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "NotifyObjectCompleteOutputTypeDef",
+    "PutChunkOutputTypeDef",
+    "PutObjectOutputTypeDef",
+    "StartObjectOutputTypeDef",
 )
 
 _RequiredBackupObjectTypeDef = TypedDict(
     "_RequiredBackupObjectTypeDef",
     {
         "Name": str,
         "ObjectChecksum": str,
@@ -89,60 +89,41 @@
     "DeleteObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
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
 
 GetChunkInputRequestTypeDef = TypedDict(
     "GetChunkInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ChunkToken": str,
     },
 )
 
-GetChunkOutputTypeDef = TypedDict(
-    "GetChunkOutputTypeDef",
-    {
-        "Data": StreamingBody,
-        "Length": int,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetObjectMetadataInputRequestTypeDef = TypedDict(
     "GetObjectMetadataInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
 
-GetObjectMetadataOutputTypeDef = TypedDict(
-    "GetObjectMetadataOutputTypeDef",
-    {
-        "MetadataString": str,
-        "MetadataBlob": StreamingBody,
-        "MetadataBlobLength": int,
-        "MetadataBlobChecksum": str,
-        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListChunksInputRequestTypeDef = TypedDict(
     "_RequiredListChunksInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
@@ -213,45 +194,27 @@
 class NotifyObjectCompleteInputRequestTypeDef(
     _RequiredNotifyObjectCompleteInputRequestTypeDef,
     _OptionalNotifyObjectCompleteInputRequestTypeDef,
 ):
     pass
 
 
-NotifyObjectCompleteOutputTypeDef = TypedDict(
-    "NotifyObjectCompleteOutputTypeDef",
-    {
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutChunkInputRequestTypeDef = TypedDict(
     "PutChunkInputRequestTypeDef",
     {
         "BackupJobId": str,
         "UploadId": str,
         "ChunkIndex": int,
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 
-PutChunkOutputTypeDef = TypedDict(
-    "PutChunkOutputTypeDef",
-    {
-        "ChunkChecksum": str,
-        "ChunkChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutObjectInputRequestTypeDef = TypedDict(
     "_RequiredPutObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
@@ -273,36 +236,14 @@
 
 class PutObjectInputRequestTypeDef(
     _RequiredPutObjectInputRequestTypeDef, _OptionalPutObjectInputRequestTypeDef
 ):
     pass
 
 
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
-    {
-        "InlineChunkChecksum": str,
-        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
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
 _RequiredStartObjectInputRequestTypeDef = TypedDict(
     "_RequiredStartObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
@@ -317,32 +258,91 @@
 
 class StartObjectInputRequestTypeDef(
     _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
 ):
     pass
 
 
-StartObjectOutputTypeDef = TypedDict(
-    "StartObjectOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "UploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListObjectsOutputTypeDef = TypedDict(
-    "ListObjectsOutputTypeDef",
+GetChunkOutputTypeDef = TypedDict(
+    "GetChunkOutputTypeDef",
     {
-        "ObjectList": List[BackupObjectTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Data": StreamingBody,
+        "Length": int,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectMetadataOutputTypeDef = TypedDict(
+    "GetObjectMetadataOutputTypeDef",
+    {
+        "MetadataString": str,
+        "MetadataBlob": StreamingBody,
+        "MetadataBlobLength": int,
+        "MetadataBlobChecksum": str,
+        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChunksOutputTypeDef = TypedDict(
     "ListChunksOutputTypeDef",
     {
         "ChunkList": List[ChunkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectsOutputTypeDef = TypedDict(
+    "ListObjectsOutputTypeDef",
+    {
+        "ObjectList": List[BackupObjectTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+NotifyObjectCompleteOutputTypeDef = TypedDict(
+    "NotifyObjectCompleteOutputTypeDef",
+    {
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutChunkOutputTypeDef = TypedDict(
+    "PutChunkOutputTypeDef",
+    {
+        "ChunkChecksum": str,
+        "ChunkChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "InlineChunkChecksum": str,
+        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartObjectOutputTypeDef = TypedDict(
+    "StartObjectOutputTypeDef",
+    {
+        "UploadId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage/type_defs.pyi` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,32 +26,32 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BackupObjectTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
-    "GetChunkOutputTypeDef",
     "GetObjectMetadataInputRequestTypeDef",
-    "GetObjectMetadataOutputTypeDef",
     "ListChunksInputRequestTypeDef",
     "ListObjectsInputRequestTypeDef",
     "NotifyObjectCompleteInputRequestTypeDef",
-    "NotifyObjectCompleteOutputTypeDef",
     "PutChunkInputRequestTypeDef",
-    "PutChunkOutputTypeDef",
     "PutObjectInputRequestTypeDef",
-    "PutObjectOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "StartObjectInputRequestTypeDef",
-    "StartObjectOutputTypeDef",
-    "ListObjectsOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetChunkOutputTypeDef",
+    "GetObjectMetadataOutputTypeDef",
     "ListChunksOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "NotifyObjectCompleteOutputTypeDef",
+    "PutChunkOutputTypeDef",
+    "PutObjectOutputTypeDef",
+    "StartObjectOutputTypeDef",
 )
 
 _RequiredBackupObjectTypeDef = TypedDict(
     "_RequiredBackupObjectTypeDef",
     {
         "Name": str,
         "ObjectChecksum": str,
@@ -86,60 +86,41 @@
     "DeleteObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
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
 
 GetChunkInputRequestTypeDef = TypedDict(
     "GetChunkInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ChunkToken": str,
     },
 )
 
-GetChunkOutputTypeDef = TypedDict(
-    "GetChunkOutputTypeDef",
-    {
-        "Data": StreamingBody,
-        "Length": int,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetObjectMetadataInputRequestTypeDef = TypedDict(
     "GetObjectMetadataInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
 
-GetObjectMetadataOutputTypeDef = TypedDict(
-    "GetObjectMetadataOutputTypeDef",
-    {
-        "MetadataString": str,
-        "MetadataBlob": StreamingBody,
-        "MetadataBlobLength": int,
-        "MetadataBlobChecksum": str,
-        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListChunksInputRequestTypeDef = TypedDict(
     "_RequiredListChunksInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
@@ -204,45 +185,27 @@
 
 class NotifyObjectCompleteInputRequestTypeDef(
     _RequiredNotifyObjectCompleteInputRequestTypeDef,
     _OptionalNotifyObjectCompleteInputRequestTypeDef,
 ):
     pass
 
-NotifyObjectCompleteOutputTypeDef = TypedDict(
-    "NotifyObjectCompleteOutputTypeDef",
-    {
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutChunkInputRequestTypeDef = TypedDict(
     "PutChunkInputRequestTypeDef",
     {
         "BackupJobId": str,
         "UploadId": str,
         "ChunkIndex": int,
         "Data": Union[str, bytes, IO[Any], StreamingBody],
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 
-PutChunkOutputTypeDef = TypedDict(
-    "PutChunkOutputTypeDef",
-    {
-        "ChunkChecksum": str,
-        "ChunkChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutObjectInputRequestTypeDef = TypedDict(
     "_RequiredPutObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
@@ -262,36 +225,14 @@
 )
 
 class PutObjectInputRequestTypeDef(
     _RequiredPutObjectInputRequestTypeDef, _OptionalPutObjectInputRequestTypeDef
 ):
     pass
 
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
-    {
-        "InlineChunkChecksum": str,
-        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
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
 _RequiredStartObjectInputRequestTypeDef = TypedDict(
     "_RequiredStartObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
@@ -304,32 +245,91 @@
 )
 
 class StartObjectInputRequestTypeDef(
     _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
 ):
     pass
 
-StartObjectOutputTypeDef = TypedDict(
-    "StartObjectOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "UploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListObjectsOutputTypeDef = TypedDict(
-    "ListObjectsOutputTypeDef",
+GetChunkOutputTypeDef = TypedDict(
+    "GetChunkOutputTypeDef",
     {
-        "ObjectList": List[BackupObjectTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Data": StreamingBody,
+        "Length": int,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetObjectMetadataOutputTypeDef = TypedDict(
+    "GetObjectMetadataOutputTypeDef",
+    {
+        "MetadataString": str,
+        "MetadataBlob": StreamingBody,
+        "MetadataBlobLength": int,
+        "MetadataBlobChecksum": str,
+        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChunksOutputTypeDef = TypedDict(
     "ListChunksOutputTypeDef",
     {
         "ChunkList": List[ChunkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListObjectsOutputTypeDef = TypedDict(
+    "ListObjectsOutputTypeDef",
+    {
+        "ObjectList": List[BackupObjectTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+NotifyObjectCompleteOutputTypeDef = TypedDict(
+    "NotifyObjectCompleteOutputTypeDef",
+    {
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutChunkOutputTypeDef = TypedDict(
+    "PutChunkOutputTypeDef",
+    {
+        "ChunkChecksum": str,
+        "ChunkChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "InlineChunkChecksum": str,
+        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartObjectOutputTypeDef = TypedDict(
+    "StartObjectOutputTypeDef",
+    {
+        "UploadId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/PKG-INFO` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-backupstorage
-Version: 1.28.12
-Summary: Type annotations for boto3.BackupStorage 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.BackupStorage 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-backupstorage.svg?color=blue)](https://pypi.org/project/mypy-boto3-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-backupstorage)](https://pepy.tech/project/mypy-boto3-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.BackupStorage 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
+[boto3.BackupStorage 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [mypy-boto3-backupstorage docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,32 +301,32 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_backupstorage.type_defs import (
     BackupObjectTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
-    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
-    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
     ListObjectsInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
     PutChunkInputRequestTypeDef,
-    PutChunkOutputTypeDef,
     PutObjectInputRequestTypeDef,
-    PutObjectOutputTypeDef,
-    ResponseMetadataTypeDef,
     StartObjectInputRequestTypeDef,
-    StartObjectOutputTypeDef,
-    ListObjectsOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChunkOutputTypeDef,
+    GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    NotifyObjectCompleteOutputTypeDef,
+    PutChunkOutputTypeDef,
+    PutObjectOutputTypeDef,
+    StartObjectOutputTypeDef,
 )
 
 
 def get_structure() -> BackupObjectTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-backupstorage-1.28.12/mypy_boto3_backupstorage.egg-info/SOURCES.txt` & `mypy-boto3-backupstorage-1.28.15/mypy_boto3_backupstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-backupstorage-1.28.12/setup.py` & `mypy-boto3-backupstorage-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-backupstorage",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_backupstorage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.BackupStorage 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.BackupStorage 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

