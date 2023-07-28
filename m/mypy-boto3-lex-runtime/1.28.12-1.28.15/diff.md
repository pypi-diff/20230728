# Comparing `tmp/mypy-boto3-lex-runtime-1.28.12.tar.gz` & `tmp/mypy-boto3-lex-runtime-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lex-runtime-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
+gzip compressed data, was "mypy-boto3-lex-runtime-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
```

## Comparing `mypy-boto3-lex-runtime-1.28.12.tar` & `mypy-boto3-lex-runtime-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12988 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 05:34:55.000000 mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.740460 mypy-boto3-lex-runtime-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-27 05:25:01.000000 mypy-boto3-lex-runtime-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.537382 mypy-boto3-lex-runtime-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12940 2023-07-28 20:43:08.529381 mypy-boto3-lex-runtime-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.521381 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7229 2023-07-28 20:29:44.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-07-28 20:29:44.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8512 2023-07-28 20:29:44.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-07-28 20:29:44.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-28 20:29:44.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.529381 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12940 2023-07-28 20:43:08.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-28 20:43:08.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:08.000000 mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.537382 mypy-boto3-lex-runtime-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-28 20:29:43.000000 mypy-boto3-lex-runtime-1.28.15/setup.py
```

### Comparing `mypy-boto3-lex-runtime-1.28.12/LICENSE` & `mypy-boto3-lex-runtime-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.12/PKG-INFO` & `mypy-boto3-lex-runtime-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-runtime
-Version: 1.28.12
-Summary: Type annotations for boto3.LexRuntimeService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LexRuntimeService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,43 +302,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
-    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
     IntentSummaryTypeDef,
     PostContentRequestRequestTypeDef,
-    PostContentResponseTypeDef,
     SentimentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    ResponseMetadataTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
+    DeleteSessionResponseTypeDef,
+    PostContentResponseTypeDef,
+    PutSessionResponseTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveOutputTypeDef:
+def get_structure() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.12/README.md` & `mypy-boto3-lex-runtime-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,43 +270,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
-    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
     IntentSummaryTypeDef,
     PostContentRequestRequestTypeDef,
-    PostContentResponseTypeDef,
     SentimentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    ResponseMetadataTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
+    DeleteSessionResponseTypeDef,
+    PostContentResponseTypeDef,
+    PutSessionResponseTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveOutputTypeDef:
+def get_structure() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/__main__.py` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexRuntimeService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LexRuntimeService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/client.py` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/client.pyi` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/literals.py` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/literals.pyi` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/type_defs.py` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lex-runtime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveOutputTypeDef
+    from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveOutputTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -29,52 +29,41 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "ActiveContextTimeToLiveOutputTypeDef",
     "ActiveContextTimeToLiveTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "DeleteSessionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentSummaryOutputTypeDef",
     "IntentConfidenceTypeDef",
     "IntentSummaryTypeDef",
     "PostContentRequestRequestTypeDef",
-    "PostContentResponseTypeDef",
     "SentimentResponseTypeDef",
-    "PutSessionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
     "GenericAttachmentTypeDef",
+    "DeleteSessionResponseTypeDef",
+    "PostContentResponseTypeDef",
+    "PutSessionResponseTypeDef",
     "PredictedIntentTypeDef",
     "GetSessionResponseTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
     "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
-ActiveContextTimeToLiveOutputTypeDef = TypedDict(
-    "ActiveContextTimeToLiveOutputTypeDef",
-    {
-        "timeToLiveInSeconds": int,
-        "turnsToLive": int,
-    },
-    total=False,
-)
-
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
     total=False,
@@ -93,22 +82,22 @@
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "botName": str,
-        "botAlias": str,
-        "userId": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredDialogActionOutputTypeDef = TypedDict(
     "_RequiredDialogActionOutputTypeDef",
     {
         "type": DialogActionTypeType,
@@ -123,21 +112,19 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
-
 class DialogActionOutputTypeDef(
     _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
 ):
     pass
 
-
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
@@ -149,19 +136,17 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
-
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
-
 _RequiredGetSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -170,21 +155,19 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "checkpointLabelFilter": str,
     },
     total=False,
 )
 
-
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredIntentSummaryOutputTypeDef = TypedDict(
     "_RequiredIntentSummaryOutputTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
 _OptionalIntentSummaryOutputTypeDef = TypedDict(
@@ -196,21 +179,19 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
-
 class IntentSummaryOutputTypeDef(
     _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
 ):
     pass
 
-
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
@@ -230,19 +211,17 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
-
 class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
-
 _RequiredPostContentRequestRequestTypeDef = TypedDict(
     "_RequiredPostContentRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "contentType": str,
@@ -256,20 +235,68 @@
         "requestAttributes": str,
         "accept": str,
         "activeContexts": str,
     },
     total=False,
 )
 
-
 class PostContentRequestRequestTypeDef(
     _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
 ):
     pass
 
+SentimentResponseTypeDef = TypedDict(
+    "SentimentResponseTypeDef",
+    {
+        "sentimentLabel": str,
+        "sentimentScore": str,
+    },
+    total=False,
+)
+
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Dict[str, str],
+    },
+)
+
+ActiveContextTypeDef = TypedDict(
+    "ActiveContextTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Mapping[str, str],
+    },
+)
+
+GenericAttachmentTypeDef = TypedDict(
+    "GenericAttachmentTypeDef",
+    {
+        "title": str,
+        "subTitle": str,
+        "attachmentLinkUrl": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+        "userId": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 PostContentResponseTypeDef = TypedDict(
     "PostContentResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "nluIntentConfidence": str,
@@ -284,27 +311,18 @@
         "slotToElicit": str,
         "inputTranscript": str,
         "encodedInputTranscript": str,
         "audioStream": StreamingBody,
         "botVersion": str,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SentimentResponseTypeDef = TypedDict(
-    "SentimentResponseTypeDef",
-    {
-        "sentimentLabel": str,
-        "sentimentScore": str,
-    },
-    total=False,
-)
-
 PutSessionResponseTypeDef = TypedDict(
     "PutSessionResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "slots": str,
         "sessionAttributes": str,
@@ -312,59 +330,18 @@
         "encodedMessage": str,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
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
-ActiveContextOutputTypeDef = TypedDict(
-    "ActiveContextOutputTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveOutputTypeDef,
-        "parameters": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ActiveContextTypeDef = TypedDict(
-    "ActiveContextTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Mapping[str, str],
-    },
-)
-
-GenericAttachmentTypeDef = TypedDict(
-    "GenericAttachmentTypeDef",
-    {
-        "title": str,
-        "subTitle": str,
-        "attachmentLinkUrl": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
@@ -375,15 +352,15 @@
     "GetSessionResponseTypeDef",
     {
         "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
         "dialogAction": DialogActionOutputTypeDef,
         "activeContexts": List[ActiveContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
@@ -398,21 +375,19 @@
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
         "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
-
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -425,21 +400,19 @@
         "recentIntentSummaryView": Sequence[IntentSummaryTypeDef],
         "accept": str,
         "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
-
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
-
 ResponseCardTypeDef = TypedDict(
     "ResponseCardTypeDef",
     {
         "version": str,
         "contentType": Literal["application/vnd.amazonaws.card.generic"],
         "genericAttachments": List[GenericAttachmentTypeDef],
     },
@@ -459,10 +432,10 @@
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
         "activeContexts": List[ActiveContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime/type_defs.pyi` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lex-runtime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveOutputTypeDef
+    from mypy_boto3_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveOutputTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -29,51 +29,42 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "ActiveContextTimeToLiveOutputTypeDef",
     "ActiveContextTimeToLiveTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "DeleteSessionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
     "IntentSummaryOutputTypeDef",
     "IntentConfidenceTypeDef",
     "IntentSummaryTypeDef",
     "PostContentRequestRequestTypeDef",
-    "PostContentResponseTypeDef",
     "SentimentResponseTypeDef",
-    "PutSessionResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
     "GenericAttachmentTypeDef",
+    "DeleteSessionResponseTypeDef",
+    "PostContentResponseTypeDef",
+    "PutSessionResponseTypeDef",
     "PredictedIntentTypeDef",
     "GetSessionResponseTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
     "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
-ActiveContextTimeToLiveOutputTypeDef = TypedDict(
-    "ActiveContextTimeToLiveOutputTypeDef",
-    {
-        "timeToLiveInSeconds": int,
-        "turnsToLive": int,
-    },
-    total=False,
-)
-
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
     total=False,
@@ -92,22 +83,22 @@
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "botName": str,
-        "botAlias": str,
-        "userId": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredDialogActionOutputTypeDef = TypedDict(
     "_RequiredDialogActionOutputTypeDef",
     {
         "type": DialogActionTypeType,
@@ -122,19 +113,21 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
+
 class DialogActionOutputTypeDef(
     _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
 ):
     pass
 
+
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
@@ -146,17 +139,19 @@
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
+
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
+
 _RequiredGetSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -165,19 +160,21 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "checkpointLabelFilter": str,
     },
     total=False,
 )
 
+
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredIntentSummaryOutputTypeDef = TypedDict(
     "_RequiredIntentSummaryOutputTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
 _OptionalIntentSummaryOutputTypeDef = TypedDict(
@@ -189,19 +186,21 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
+
 class IntentSummaryOutputTypeDef(
     _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
 ):
     pass
 
+
 IntentConfidenceTypeDef = TypedDict(
     "IntentConfidenceTypeDef",
     {
         "score": float,
     },
     total=False,
 )
@@ -221,17 +220,19 @@
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
+
 class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
+
 _RequiredPostContentRequestRequestTypeDef = TypedDict(
     "_RequiredPostContentRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "contentType": str,
@@ -245,19 +246,71 @@
         "requestAttributes": str,
         "accept": str,
         "activeContexts": str,
     },
     total=False,
 )
 
+
 class PostContentRequestRequestTypeDef(
     _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
 ):
     pass
 
+
+SentimentResponseTypeDef = TypedDict(
+    "SentimentResponseTypeDef",
+    {
+        "sentimentLabel": str,
+        "sentimentScore": str,
+    },
+    total=False,
+)
+
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Dict[str, str],
+    },
+)
+
+ActiveContextTypeDef = TypedDict(
+    "ActiveContextTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Mapping[str, str],
+    },
+)
+
+GenericAttachmentTypeDef = TypedDict(
+    "GenericAttachmentTypeDef",
+    {
+        "title": str,
+        "subTitle": str,
+        "attachmentLinkUrl": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+        "userId": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PostContentResponseTypeDef = TypedDict(
     "PostContentResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "nluIntentConfidence": str,
         "alternativeIntents": str,
@@ -271,27 +324,18 @@
         "slotToElicit": str,
         "inputTranscript": str,
         "encodedInputTranscript": str,
         "audioStream": StreamingBody,
         "botVersion": str,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SentimentResponseTypeDef = TypedDict(
-    "SentimentResponseTypeDef",
-    {
-        "sentimentLabel": str,
-        "sentimentScore": str,
-    },
-    total=False,
-)
-
 PutSessionResponseTypeDef = TypedDict(
     "PutSessionResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "slots": str,
         "sessionAttributes": str,
@@ -299,59 +343,18 @@
         "encodedMessage": str,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
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
-ActiveContextOutputTypeDef = TypedDict(
-    "ActiveContextOutputTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveOutputTypeDef,
-        "parameters": Dict[str, str],
-    },
-)
-
-ActiveContextTypeDef = TypedDict(
-    "ActiveContextTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Mapping[str, str],
-    },
-)
-
-GenericAttachmentTypeDef = TypedDict(
-    "GenericAttachmentTypeDef",
-    {
-        "title": str,
-        "subTitle": str,
-        "attachmentLinkUrl": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
@@ -362,15 +365,15 @@
     "GetSessionResponseTypeDef",
     {
         "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
         "dialogAction": DialogActionOutputTypeDef,
         "activeContexts": List[ActiveContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
@@ -385,19 +388,21 @@
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
         "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
+
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -410,19 +415,21 @@
         "recentIntentSummaryView": Sequence[IntentSummaryTypeDef],
         "accept": str,
         "activeContexts": Sequence[ActiveContextTypeDef],
     },
     total=False,
 )
 
+
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
+
 ResponseCardTypeDef = TypedDict(
     "ResponseCardTypeDef",
     {
         "version": str,
         "contentType": Literal["application/vnd.amazonaws.card.generic"],
         "genericAttachments": List[GenericAttachmentTypeDef],
     },
@@ -442,10 +449,10 @@
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
         "activeContexts": List[ActiveContextOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/PKG-INFO` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lex-runtime
-Version: 1.28.12
-Summary: Type annotations for boto3.LexRuntimeService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LexRuntimeService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lex-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lex-runtime)](https://pepy.tech/project/mypy-boto3-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
+[boto3.LexRuntimeService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [mypy-boto3-lex-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lex_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -302,43 +302,42 @@
 ### Typed dictionaries
 
 `mypy_boto3_lex_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lex_runtime.type_defs import (
-    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
     IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
     IntentSummaryTypeDef,
     PostContentRequestRequestTypeDef,
-    PostContentResponseTypeDef,
     SentimentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    ResponseMetadataTypeDef,
     ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
     GenericAttachmentTypeDef,
+    DeleteSessionResponseTypeDef,
+    PostContentResponseTypeDef,
+    PutSessionResponseTypeDef,
     PredictedIntentTypeDef,
     GetSessionResponseTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
     ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveOutputTypeDef:
+def get_structure() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lex-runtime-1.28.12/mypy_boto3_lex_runtime.egg-info/SOURCES.txt` & `mypy-boto3-lex-runtime-1.28.15/mypy_boto3_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lex-runtime-1.28.12/setup.py` & `mypy-boto3-lex-runtime-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lex-runtime",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexRuntimeService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.LexRuntimeService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

