# Comparing `tmp/mypy-boto3-kinesis-video-media-1.28.12.tar.gz` & `tmp/mypy-boto3-kinesis-video-media-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-video-media-1.28.12.tar", last modified: Thu Jul 27 05:34:53 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-video-media-1.28.15.tar", last modified: Fri Jul 28 20:43:05 2023, max compression
```

## Comparing `mypy-boto3-kinesis-video-media-1.28.12.tar` & `mypy-boto3-kinesis-video-media-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.652468 mypy-boto3-kinesis-video-media-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-27 05:34:53.644468 mypy-boto3-kinesis-video-media-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.644468 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.644468 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:53.652468 mypy-boto3-kinesis-video-media-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-27 05:24:41.000000 mypy-boto3-kinesis-video-media-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.553341 mypy-boto3-kinesis-video-media-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-media-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-28 20:43:05.549340 mypy-boto3-kinesis-video-media-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-media-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.549340 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8212 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.549340 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12518 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:05.553341 mypy-boto3-kinesis-video-media-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-07-28 20:29:14.000000 mypy-boto3-kinesis-video-media-1.28.15/setup.py
```

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/LICENSE` & `mypy-boto3-kinesis-video-media-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/PKG-INFO` & `mypy-boto3-kinesis-video-media-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-media
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisVideoMedia 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisVideoMedia 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoMedia 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
+[boto3.KinesisVideoMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
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
 [mypy-boto3-kinesis-video-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,17 +299,17 @@
 
 `mypy_boto3_kinesis_video_media.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_media.type_defs import (
     StartSelectorTypeDef,
-    GetMediaOutputTypeDef,
     ResponseMetadataTypeDef,
     GetMediaInputRequestTypeDef,
+    GetMediaOutputTypeDef,
 )
 
 
 def get_structure() -> StartSelectorTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/README.md` & `mypy-boto3-kinesis-video-media-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoMedia 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
+[boto3.KinesisVideoMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
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
 [mypy-boto3-kinesis-video-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,17 +267,17 @@
 
 `mypy_boto3_kinesis_video_media.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_media.type_defs import (
     StartSelectorTypeDef,
-    GetMediaOutputTypeDef,
     ResponseMetadataTypeDef,
     GetMediaInputRequestTypeDef,
+    GetMediaOutputTypeDef,
 )
 
 
 def get_structure() -> StartSelectorTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/__main__.py` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideoMedia 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.KinesisVideoMedia 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia\nOther"
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

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/client.py` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/client.pyi` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/literals.py` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/literals.pyi` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/type_defs.py` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,17 +23,17 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "StartSelectorTypeDef",
-    "GetMediaOutputTypeDef",
     "ResponseMetadataTypeDef",
     "GetMediaInputRequestTypeDef",
+    "GetMediaOutputTypeDef",
 )
 
 _RequiredStartSelectorTypeDef = TypedDict(
     "_RequiredStartSelectorTypeDef",
     {
         "StartSelectorType": StartSelectorTypeType,
     },
@@ -49,23 +49,14 @@
 )
 
 
 class StartSelectorTypeDef(_RequiredStartSelectorTypeDef, _OptionalStartSelectorTypeDef):
     pass
 
 
-GetMediaOutputTypeDef = TypedDict(
-    "GetMediaOutputTypeDef",
-    {
-        "ContentType": str,
-        "Payload": StreamingBody,
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
@@ -89,7 +80,17 @@
 )
 
 
 class GetMediaInputRequestTypeDef(
     _RequiredGetMediaInputRequestTypeDef, _OptionalGetMediaInputRequestTypeDef
 ):
     pass
+
+
+GetMediaOutputTypeDef = TypedDict(
+    "GetMediaOutputTypeDef",
+    {
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media/type_defs.pyi` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "StartSelectorTypeDef",
-    "GetMediaOutputTypeDef",
     "ResponseMetadataTypeDef",
     "GetMediaInputRequestTypeDef",
+    "GetMediaOutputTypeDef",
 )
 
 _RequiredStartSelectorTypeDef = TypedDict(
     "_RequiredStartSelectorTypeDef",
     {
         "StartSelectorType": StartSelectorTypeType,
     },
@@ -46,23 +46,14 @@
     },
     total=False,
 )
 
 class StartSelectorTypeDef(_RequiredStartSelectorTypeDef, _OptionalStartSelectorTypeDef):
     pass
 
-GetMediaOutputTypeDef = TypedDict(
-    "GetMediaOutputTypeDef",
-    {
-        "ContentType": str,
-        "Payload": StreamingBody,
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
@@ -85,7 +76,16 @@
     total=False,
 )
 
 class GetMediaInputRequestTypeDef(
     _RequiredGetMediaInputRequestTypeDef, _OptionalGetMediaInputRequestTypeDef
 ):
     pass
+
+GetMediaOutputTypeDef = TypedDict(
+    "GetMediaOutputTypeDef",
+    {
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/PKG-INFO` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-media
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisVideoMedia 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisVideoMedia 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-media.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-media)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-media)](https://pepy.tech/project/mypy-boto3-kinesis-video-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoMedia 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
+[boto3.KinesisVideoMedia 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-media.html#KinesisVideoMedia)
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
 [mypy-boto3-kinesis-video-media docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_media/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,17 +299,17 @@
 
 `mypy_boto3_kinesis_video_media.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_kinesis_video_media.type_defs import (
     StartSelectorTypeDef,
-    GetMediaOutputTypeDef,
     ResponseMetadataTypeDef,
     GetMediaInputRequestTypeDef,
+    GetMediaOutputTypeDef,
 )
 
 
 def get_structure() -> StartSelectorTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/mypy_boto3_kinesis_video_media.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-video-media-1.28.15/mypy_boto3_kinesis_video_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-media-1.28.12/setup.py` & `mypy-boto3-kinesis-video-media-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis-video-media",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kinesis_video_media"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideoMedia 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.KinesisVideoMedia 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

