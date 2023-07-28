# Comparing `tmp/mypy-boto3-ivs-realtime-1.28.12.tar.gz` & `tmp/mypy-boto3-ivs-realtime-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ivs-realtime-1.28.12.tar", last modified: Thu Jul 27 05:34:51 2023, max compression
+gzip compressed data, was "mypy-boto3-ivs-realtime-1.28.15.tar", last modified: Fri Jul 28 20:43:02 2023, max compression
```

## Comparing `mypy-boto3-ivs-realtime-1.28.12.tar` & `mypy-boto3-ivs-realtime-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.544475 mypy-boto3-ivs-realtime-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:24.000000 mypy-boto3-ivs-realtime-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-27 05:34:51.544475 mypy-boto3-ivs-realtime-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-07-27 05:24:24.000000 mypy-boto3-ivs-realtime-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.544475 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-27 05:24:24.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-27 05:24:24.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-27 05:24:25.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-27 05:24:25.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-27 05:24:25.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-07-27 05:24:25.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-27 05:24:25.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:25.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12193 2023-07-27 05:24:25.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-07-27 05:24:25.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:24.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:51.544475 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-27 05:34:51.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-27 05:34:51.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:51.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:51.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-27 05:34:51.000000 mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:51.544475 mypy-boto3-ivs-realtime-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 05:24:24.000000 mypy-boto3-ivs-realtime-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.665301 mypy-boto3-ivs-realtime-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-28 20:43:02.665301 mypy-boto3-ivs-realtime-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.665301 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12057 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12171 2023-07-28 20:28:55.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12154 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:02.665301 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13446 2023-07-28 20:43:02.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-28 20:43:02.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:02.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:02.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-28 20:43:02.000000 mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:02.665301 mypy-boto3-ivs-realtime-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:28:54.000000 mypy-boto3-ivs-realtime-1.28.15/setup.py
```

### Comparing `mypy-boto3-ivs-realtime-1.28.12/LICENSE` & `mypy-boto3-ivs-realtime-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.28.12/PKG-INFO` & `mypy-boto3-ivs-realtime-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs-realtime
-Version: 1.28.12
-Summary: Type annotations for boto3.ivsrealtime 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ivsrealtime 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs-realtime)](https://pepy.tech/project/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.ivsrealtime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
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
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,14 +302,15 @@
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import (
     CreateParticipantTokenRequestRequestTypeDef,
     ParticipantTokenTypeDef,
+    ResponseMetadataTypeDef,
     ParticipantTokenConfigurationTypeDef,
     StageTypeDef,
     DeleteStageRequestRequestTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     EventTypeDef,
     GetParticipantRequestRequestTypeDef,
     ParticipantTypeDef,
@@ -320,20 +321,19 @@
     ListParticipantsRequestRequestTypeDef,
     ParticipantSummaryTypeDef,
     ListStageSessionsRequestRequestTypeDef,
     StageSessionSummaryTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     CreateParticipantTokenResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     UpdateStageResponseTypeDef,
     ListParticipantEventsResponseTypeDef,
     GetParticipantResponseTypeDef,
     GetStageSessionResponseTypeDef,
```

### Comparing `mypy-boto3-ivs-realtime-1.28.12/README.md` & `mypy-boto3-ivs-realtime-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs-realtime)](https://pepy.tech/project/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.ivsrealtime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
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
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,14 +270,15 @@
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import (
     CreateParticipantTokenRequestRequestTypeDef,
     ParticipantTokenTypeDef,
+    ResponseMetadataTypeDef,
     ParticipantTokenConfigurationTypeDef,
     StageTypeDef,
     DeleteStageRequestRequestTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     EventTypeDef,
     GetParticipantRequestRequestTypeDef,
     ParticipantTypeDef,
@@ -288,20 +289,19 @@
     ListParticipantsRequestRequestTypeDef,
     ParticipantSummaryTypeDef,
     ListStageSessionsRequestRequestTypeDef,
     StageSessionSummaryTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     CreateParticipantTokenResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     UpdateStageResponseTypeDef,
     ListParticipantEventsResponseTypeDef,
     GetParticipantResponseTypeDef,
     GetStageSessionResponseTypeDef,
```

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/__main__.py` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ivsrealtime 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.ivsrealtime 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime\nOther"
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

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/client.py` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/client.pyi` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/literals.py` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/literals.pyi` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/type_defs.py` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateParticipantTokenRequestRequestTypeDef",
     "ParticipantTokenTypeDef",
+    "ResponseMetadataTypeDef",
     "ParticipantTokenConfigurationTypeDef",
     "StageTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
     "EventTypeDef",
     "GetParticipantRequestRequestTypeDef",
     "ParticipantTypeDef",
@@ -44,20 +45,19 @@
     "ListParticipantsRequestRequestTypeDef",
     "ParticipantSummaryTypeDef",
     "ListStageSessionsRequestRequestTypeDef",
     "StageSessionSummaryTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "CreateParticipantTokenResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "UpdateStageResponseTypeDef",
     "ListParticipantEventsResponseTypeDef",
     "GetParticipantResponseTypeDef",
     "GetStageSessionResponseTypeDef",
@@ -101,14 +101,25 @@
         "participantId": str,
         "token": str,
         "userId": str,
     },
     total=False,
 )
 
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
 ParticipantTokenConfigurationTypeDef = TypedDict(
     "ParticipantTokenConfigurationTypeDef",
     {
         "attributes": Mapping[str, str],
         "capabilities": Sequence[ParticipantTokenCapabilityType],
         "duration": int,
         "userId": str,
@@ -354,33 +365,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -414,15 +406,23 @@
     pass
 
 
 CreateParticipantTokenResponseTypeDef = TypedDict(
     "CreateParticipantTokenResponseTypeDef",
     {
         "participantToken": ParticipantTokenTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStageRequestRequestTypeDef = TypedDict(
     "CreateStageRequestRequestTypeDef",
     {
         "name": str,
@@ -433,78 +433,78 @@
 )
 
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
         "participantTokens": List[ParticipantTokenTypeDef],
         "stage": StageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
         "stage": StageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStageResponseTypeDef = TypedDict(
     "UpdateStageResponseTypeDef",
     {
         "stage": StageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListParticipantEventsResponseTypeDef = TypedDict(
     "ListParticipantEventsResponseTypeDef",
     {
         "events": List[EventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParticipantResponseTypeDef = TypedDict(
     "GetParticipantResponseTypeDef",
     {
         "participant": ParticipantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageSessionResponseTypeDef = TypedDict(
     "GetStageSessionResponseTypeDef",
     {
         "stageSession": StageSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListParticipantsResponseTypeDef = TypedDict(
     "ListParticipantsResponseTypeDef",
     {
         "nextToken": str,
         "participants": List[ParticipantSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStageSessionsResponseTypeDef = TypedDict(
     "ListStageSessionsResponseTypeDef",
     {
         "nextToken": str,
         "stageSessions": List[StageSessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStagesResponseTypeDef = TypedDict(
     "ListStagesResponseTypeDef",
     {
         "nextToken": str,
         "stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime/type_defs.pyi` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateParticipantTokenRequestRequestTypeDef",
     "ParticipantTokenTypeDef",
+    "ResponseMetadataTypeDef",
     "ParticipantTokenConfigurationTypeDef",
     "StageTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
     "EventTypeDef",
     "GetParticipantRequestRequestTypeDef",
     "ParticipantTypeDef",
@@ -43,20 +44,19 @@
     "ListParticipantsRequestRequestTypeDef",
     "ParticipantSummaryTypeDef",
     "ListStageSessionsRequestRequestTypeDef",
     "StageSessionSummaryTypeDef",
     "ListStagesRequestRequestTypeDef",
     "StageSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "CreateParticipantTokenResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "UpdateStageResponseTypeDef",
     "ListParticipantEventsResponseTypeDef",
     "GetParticipantResponseTypeDef",
     "GetStageSessionResponseTypeDef",
@@ -98,14 +98,25 @@
         "participantId": str,
         "token": str,
         "userId": str,
     },
     total=False,
 )
 
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
 ParticipantTokenConfigurationTypeDef = TypedDict(
     "ParticipantTokenConfigurationTypeDef",
     {
         "attributes": Mapping[str, str],
         "capabilities": Sequence[ParticipantTokenCapabilityType],
         "duration": int,
         "userId": str,
@@ -339,33 +350,14 @@
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -397,15 +389,23 @@
 ):
     pass
 
 CreateParticipantTokenResponseTypeDef = TypedDict(
     "CreateParticipantTokenResponseTypeDef",
     {
         "participantToken": ParticipantTokenTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateStageRequestRequestTypeDef = TypedDict(
     "CreateStageRequestRequestTypeDef",
     {
         "name": str,
@@ -416,78 +416,78 @@
 )
 
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
         "participantTokens": List[ParticipantTokenTypeDef],
         "stage": StageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
         "stage": StageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateStageResponseTypeDef = TypedDict(
     "UpdateStageResponseTypeDef",
     {
         "stage": StageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListParticipantEventsResponseTypeDef = TypedDict(
     "ListParticipantEventsResponseTypeDef",
     {
         "events": List[EventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetParticipantResponseTypeDef = TypedDict(
     "GetParticipantResponseTypeDef",
     {
         "participant": ParticipantTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageSessionResponseTypeDef = TypedDict(
     "GetStageSessionResponseTypeDef",
     {
         "stageSession": StageSessionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListParticipantsResponseTypeDef = TypedDict(
     "ListParticipantsResponseTypeDef",
     {
         "nextToken": str,
         "participants": List[ParticipantSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStageSessionsResponseTypeDef = TypedDict(
     "ListStageSessionsResponseTypeDef",
     {
         "nextToken": str,
         "stageSessions": List[StageSessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStagesResponseTypeDef = TypedDict(
     "ListStagesResponseTypeDef",
     {
         "nextToken": str,
         "stages": List[StageSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/PKG-INFO` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ivs-realtime
-Version: 1.28.12
-Summary: Type annotations for boto3.ivsrealtime 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.ivsrealtime 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ivs-realtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-ivs-realtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ivs-realtime)](https://pepy.tech/project/mypy-boto3-ivs-realtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ivsrealtime 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
+[boto3.ivsrealtime 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ivs-realtime.html#ivsrealtime)
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
 [mypy-boto3-ivs-realtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ivs_realtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,14 +302,15 @@
 `mypy_boto3_ivs_realtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ivs_realtime.type_defs import (
     CreateParticipantTokenRequestRequestTypeDef,
     ParticipantTokenTypeDef,
+    ResponseMetadataTypeDef,
     ParticipantTokenConfigurationTypeDef,
     StageTypeDef,
     DeleteStageRequestRequestTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     EventTypeDef,
     GetParticipantRequestRequestTypeDef,
     ParticipantTypeDef,
@@ -320,20 +321,19 @@
     ListParticipantsRequestRequestTypeDef,
     ParticipantSummaryTypeDef,
     ListStageSessionsRequestRequestTypeDef,
     StageSessionSummaryTypeDef,
     ListStagesRequestRequestTypeDef,
     StageSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateStageRequestRequestTypeDef,
     CreateParticipantTokenResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     UpdateStageResponseTypeDef,
     ListParticipantEventsResponseTypeDef,
     GetParticipantResponseTypeDef,
     GetStageSessionResponseTypeDef,
```

### Comparing `mypy-boto3-ivs-realtime-1.28.12/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt` & `mypy-boto3-ivs-realtime-1.28.15/mypy_boto3_ivs_realtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ivs-realtime-1.28.12/setup.py` & `mypy-boto3-ivs-realtime-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ivs-realtime",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ivs_realtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ivsrealtime 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.ivsrealtime 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

