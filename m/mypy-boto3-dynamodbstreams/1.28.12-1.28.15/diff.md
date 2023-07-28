# Comparing `tmp/mypy-boto3-dynamodbstreams-1.28.12.tar.gz` & `tmp/mypy-boto3-dynamodbstreams-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dynamodbstreams-1.28.12.tar", last modified: Thu Jul 27 05:34:36 2023, max compression
+gzip compressed data, was "mypy-boto3-dynamodbstreams-1.28.15.tar", last modified: Fri Jul 28 20:42:41 2023, max compression
```

## Comparing `mypy-boto3-dynamodbstreams-1.28.12.tar` & `mypy-boto3-dynamodbstreams-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.256528 mypy-boto3-dynamodbstreams-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-27 05:34:36.256528 mypy-boto3-dynamodbstreams-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.256528 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:36.256528 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-27 05:34:36.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-27 05:34:36.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:36.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:36.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 05:34:36.000000 mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:36.256528 mypy-boto3-dynamodbstreams-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-27 05:20:42.000000 mypy-boto3-dynamodbstreams-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:41.053003 mypy-boto3-dynamodbstreams-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-28 20:42:41.041003 mypy-boto3-dynamodbstreams-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:41.041003 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5821 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8675 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:41.041003 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12821 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:42:40.000000 mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:41.053003 mypy-boto3-dynamodbstreams-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-28 20:23:36.000000 mypy-boto3-dynamodbstreams-1.28.15/setup.py
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/LICENSE` & `mypy-boto3-dynamodbstreams-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/PKG-INFO` & `mypy-boto3-dynamodbstreams-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodbstreams
-Version: 1.28.12
-Summary: Type annotations for boto3.DynamoDBStreams 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DynamoDBStreams 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodbstreams)](https://pepy.tech/project/mypy-boto3-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDBStreams 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[boto3.DynamoDBStreams 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,24 +304,24 @@
 `mypy_boto3_dynamodbstreams.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/README.md` & `mypy-boto3-dynamodbstreams-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodbstreams)](https://pepy.tech/project/mypy-boto3-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDBStreams 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[boto3.DynamoDBStreams 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -272,24 +272,24 @@
 `mypy_boto3_dynamodbstreams.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/__main__.py` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DynamoDBStreams 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.DynamoDBStreams 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams\nOther"
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

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/client.py` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/client.pyi` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/literals.py` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/literals.pyi` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/type_defs.py` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,24 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttributeValueTypeDef",
     "DescribeStreamInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRecordsInputRequestTypeDef",
     "GetShardIteratorInputRequestTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "IdentityTypeDef",
     "KeySchemaElementTypeDef",
     "ListStreamsInputRequestTypeDef",
     "StreamTypeDef",
     "StreamRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "RecordTypeDef",
     "ShardTypeDef",
     "GetRecordsOutputTypeDef",
     "StreamDescriptionTypeDef",
     "DescribeStreamOutputTypeDef",
 )
@@ -85,14 +85,25 @@
 
 class DescribeStreamInputRequestTypeDef(
     _RequiredDescribeStreamInputRequestTypeDef, _OptionalDescribeStreamInputRequestTypeDef
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
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -129,22 +140,14 @@
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
 
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "PrincipalId": str,
         "Type": str,
     },
     total=False,
@@ -188,40 +191,37 @@
         "SequenceNumber": str,
         "SizeBytes": int,
         "StreamViewType": StreamViewTypeType,
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
 SequenceNumberRangeTypeDef = TypedDict(
     "SequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
         "EndingSequenceNumber": str,
     },
     total=False,
 )
 
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "Streams": List[StreamTypeDef],
         "LastEvaluatedStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "eventID": str,
@@ -246,15 +246,15 @@
 )
 
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamDescriptionTypeDef = TypedDict(
     "StreamDescriptionTypeDef",
     {
         "StreamArn": str,
@@ -270,10 +270,10 @@
     total=False,
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams/type_defs.pyi` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -27,24 +27,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttributeValueTypeDef",
     "DescribeStreamInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRecordsInputRequestTypeDef",
     "GetShardIteratorInputRequestTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "IdentityTypeDef",
     "KeySchemaElementTypeDef",
     "ListStreamsInputRequestTypeDef",
     "StreamTypeDef",
     "StreamRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "RecordTypeDef",
     "ShardTypeDef",
     "GetRecordsOutputTypeDef",
     "StreamDescriptionTypeDef",
     "DescribeStreamOutputTypeDef",
 )
@@ -82,14 +82,25 @@
 )
 
 class DescribeStreamInputRequestTypeDef(
     _RequiredDescribeStreamInputRequestTypeDef, _OptionalDescribeStreamInputRequestTypeDef
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
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -122,22 +133,14 @@
 )
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "PrincipalId": str,
         "Type": str,
     },
     total=False,
@@ -181,40 +184,37 @@
         "SequenceNumber": str,
         "SizeBytes": int,
         "StreamViewType": StreamViewTypeType,
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
 SequenceNumberRangeTypeDef = TypedDict(
     "SequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
         "EndingSequenceNumber": str,
     },
     total=False,
 )
 
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "Streams": List[StreamTypeDef],
         "LastEvaluatedStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "eventID": str,
@@ -239,15 +239,15 @@
 )
 
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamDescriptionTypeDef = TypedDict(
     "StreamDescriptionTypeDef",
     {
         "StreamArn": str,
@@ -263,10 +263,10 @@
     total=False,
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dynamodbstreams
-Version: 1.28.12
-Summary: Type annotations for boto3.DynamoDBStreams 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DynamoDBStreams 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dynamodbstreams.svg?color=blue)](https://pypi.org/project/mypy-boto3-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dynamodbstreams)](https://pepy.tech/project/mypy-boto3-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DynamoDBStreams 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
+[boto3.DynamoDBStreams 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [mypy-boto3-dynamodbstreams docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -304,24 +304,24 @@
 `mypy_boto3_dynamodbstreams.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
```

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt` & `mypy-boto3-dynamodbstreams-1.28.15/mypy_boto3_dynamodbstreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dynamodbstreams-1.28.12/setup.py` & `mypy-boto3-dynamodbstreams-1.28.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dynamodbstreams",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_dynamodbstreams"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DynamoDBStreams 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.DynamoDBStreams 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

