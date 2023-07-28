# Comparing `tmp/mypy-boto3-kinesis-video-signaling-1.28.12.tar.gz` & `tmp/mypy-boto3-kinesis-video-signaling-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-kinesis-video-signaling-1.28.12.tar", last modified: Thu Jul 27 05:34:53 2023, max compression
+gzip compressed data, was "mypy-boto3-kinesis-video-signaling-1.28.15.tar", last modified: Fri Jul 28 20:43:05 2023, max compression
```

## Comparing `mypy-boto3-kinesis-video-signaling-1.28.12.tar` & `mypy-boto3-kinesis-video-signaling-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.680467 mypy-boto3-kinesis-video-signaling-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-27 05:34:53.672468 mypy-boto3-kinesis-video-signaling-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.672468 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:53.672468 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-27 05:34:53.000000 mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:53.680467 mypy-boto3-kinesis-video-signaling-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-27 05:24:42.000000 mypy-boto3-kinesis-video-signaling-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.593341 mypy-boto3-kinesis-video-signaling-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-28 20:43:05.593341 mypy-boto3-kinesis-video-signaling-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.585341 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:05.593341 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12905 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-28 20:43:05.000000 mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:05.593341 mypy-boto3-kinesis-video-signaling-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-28 20:29:15.000000 mypy-boto3-kinesis-video-signaling-1.28.15/setup.py
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/LICENSE` & `mypy-boto3-kinesis-video-signaling-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/PKG-INFO` & `mypy-boto3-kinesis-video-signaling-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-signaling
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisVideoSignalingChannels 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisVideoSignalingChannels 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-signaling)](https://pepy.tech/project/mypy-boto3-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoSignalingChannels 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[boto3.KinesisVideoSignalingChannels 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
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
 [mypy-boto3-kinesis-video-signaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,16 +302,16 @@
 
 ```python
 from mypy_boto3_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
     IceServerTypeDef,
     ResponseMetadataTypeDef,
     SendAlexaOfferToMasterRequestRequestTypeDef,
-    SendAlexaOfferToMasterResponseTypeDef,
     GetIceServerConfigResponseTypeDef,
+    SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
 def get_structure() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/README.md` & `mypy-boto3-kinesis-video-signaling-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-signaling)](https://pepy.tech/project/mypy-boto3-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoSignalingChannels 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[boto3.KinesisVideoSignalingChannels 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
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
 [mypy-boto3-kinesis-video-signaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,16 +270,16 @@
 
 ```python
 from mypy_boto3_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
     IceServerTypeDef,
     ResponseMetadataTypeDef,
     SendAlexaOfferToMasterRequestRequestTypeDef,
-    SendAlexaOfferToMasterResponseTypeDef,
     GetIceServerConfigResponseTypeDef,
+    SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
 def get_structure() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/__init__.py` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/__init__.pyi` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/__main__.py` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.KinesisVideoSignalingChannels 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.KinesisVideoSignalingChannels 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels\nOther"
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

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/client.py` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/client.pyi` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/literals.py` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/literals.pyi` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/type_defs.py` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "GetIceServerConfigRequestRequestTypeDef",
     "IceServerTypeDef",
     "ResponseMetadataTypeDef",
     "SendAlexaOfferToMasterRequestRequestTypeDef",
-    "SendAlexaOfferToMasterResponseTypeDef",
     "GetIceServerConfigResponseTypeDef",
+    "SendAlexaOfferToMasterResponseTypeDef",
 )
 
 _RequiredGetIceServerConfigRequestRequestTypeDef = TypedDict(
     "_RequiredGetIceServerConfigRequestRequestTypeDef",
     {
         "ChannelARN": str,
     },
@@ -45,22 +44,20 @@
         "ClientId": str,
         "Service": Literal["TURN"],
         "Username": str,
     },
     total=False,
 )
 
-
 class GetIceServerConfigRequestRequestTypeDef(
     _RequiredGetIceServerConfigRequestRequestTypeDef,
     _OptionalGetIceServerConfigRequestRequestTypeDef,
 ):
     pass
 
-
 IceServerTypeDef = TypedDict(
     "IceServerTypeDef",
     {
         "Uris": List[str],
         "Username": str,
         "Password": str,
         "Ttl": int,
@@ -84,22 +81,22 @@
     {
         "ChannelARN": str,
         "SenderClientId": str,
         "MessagePayload": str,
     },
 )
 
-SendAlexaOfferToMasterResponseTypeDef = TypedDict(
-    "SendAlexaOfferToMasterResponseTypeDef",
+GetIceServerConfigResponseTypeDef = TypedDict(
+    "GetIceServerConfigResponseTypeDef",
     {
-        "Answer": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IceServerList": List[IceServerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetIceServerConfigResponseTypeDef = TypedDict(
-    "GetIceServerConfigResponseTypeDef",
+SendAlexaOfferToMasterResponseTypeDef = TypedDict(
+    "SendAlexaOfferToMasterResponseTypeDef",
     {
-        "IceServerList": List[IceServerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Answer": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling/type_defs.pyi` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,21 +19,22 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "GetIceServerConfigRequestRequestTypeDef",
     "IceServerTypeDef",
     "ResponseMetadataTypeDef",
     "SendAlexaOfferToMasterRequestRequestTypeDef",
-    "SendAlexaOfferToMasterResponseTypeDef",
     "GetIceServerConfigResponseTypeDef",
+    "SendAlexaOfferToMasterResponseTypeDef",
 )
 
 _RequiredGetIceServerConfigRequestRequestTypeDef = TypedDict(
     "_RequiredGetIceServerConfigRequestRequestTypeDef",
     {
         "ChannelARN": str,
     },
@@ -44,20 +45,22 @@
         "ClientId": str,
         "Service": Literal["TURN"],
         "Username": str,
     },
     total=False,
 )
 
+
 class GetIceServerConfigRequestRequestTypeDef(
     _RequiredGetIceServerConfigRequestRequestTypeDef,
     _OptionalGetIceServerConfigRequestRequestTypeDef,
 ):
     pass
 
+
 IceServerTypeDef = TypedDict(
     "IceServerTypeDef",
     {
         "Uris": List[str],
         "Username": str,
         "Password": str,
         "Ttl": int,
@@ -81,22 +84,22 @@
     {
         "ChannelARN": str,
         "SenderClientId": str,
         "MessagePayload": str,
     },
 )
 
-SendAlexaOfferToMasterResponseTypeDef = TypedDict(
-    "SendAlexaOfferToMasterResponseTypeDef",
+GetIceServerConfigResponseTypeDef = TypedDict(
+    "GetIceServerConfigResponseTypeDef",
     {
-        "Answer": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "IceServerList": List[IceServerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetIceServerConfigResponseTypeDef = TypedDict(
-    "GetIceServerConfigResponseTypeDef",
+SendAlexaOfferToMasterResponseTypeDef = TypedDict(
+    "SendAlexaOfferToMasterResponseTypeDef",
     {
-        "IceServerList": List[IceServerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Answer": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/PKG-INFO` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kinesis-video-signaling
-Version: 1.28.12
-Summary: Type annotations for boto3.KinesisVideoSignalingChannels 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.KinesisVideoSignalingChannels 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kinesis-video-signaling.svg?color=blue)](https://pypi.org/project/mypy-boto3-kinesis-video-signaling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kinesis-video-signaling)](https://pepy.tech/project/mypy-boto3-kinesis-video-signaling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.KinesisVideoSignalingChannels 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
+[boto3.KinesisVideoSignalingChannels 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels)
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
 [mypy-boto3-kinesis-video-signaling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kinesis_video_signaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,16 +302,16 @@
 
 ```python
 from mypy_boto3_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
     IceServerTypeDef,
     ResponseMetadataTypeDef,
     SendAlexaOfferToMasterRequestRequestTypeDef,
-    SendAlexaOfferToMasterResponseTypeDef,
     GetIceServerConfigResponseTypeDef,
+    SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
 def get_structure() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/mypy_boto3_kinesis_video_signaling.egg-info/SOURCES.txt` & `mypy-boto3-kinesis-video-signaling-1.28.15/mypy_boto3_kinesis_video_signaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-kinesis-video-signaling-1.28.12/setup.py` & `mypy-boto3-kinesis-video-signaling-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kinesis-video-signaling",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_kinesis_video_signaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.KinesisVideoSignalingChannels 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.KinesisVideoSignalingChannels 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

