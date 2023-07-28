# Comparing `tmp/mypy-boto3-lexv2-runtime-1.28.12.tar.gz` & `tmp/mypy-boto3-lexv2-runtime-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lexv2-runtime-1.28.12.tar", last modified: Thu Jul 27 05:34:55 2023, max compression
+gzip compressed data, was "mypy-boto3-lexv2-runtime-1.28.15.tar", last modified: Fri Jul 28 20:43:08 2023, max compression
```

## Comparing `mypy-boto3-lexv2-runtime-1.28.12.tar` & `mypy-boto3-lexv2-runtime-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.916460 mypy-boto3-lexv2-runtime-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-27 05:34:55.916460 mypy-boto3-lexv2-runtime-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.908460 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16324 2023-07-27 05:25:18.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:55.916460 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:55.000000 mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:55.916460 mypy-boto3-lexv2-runtime-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-27 05:25:16.000000 mypy-boto3-lexv2-runtime-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.737384 mypy-boto3-lexv2-runtime-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-07-28 20:43:08.733384 mypy-boto3-lexv2-runtime-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11890 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.721384 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-07-28 20:30:05.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14675 2023-07-28 20:30:05.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:08.733384 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-07-28 20:43:08.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-07-28 20:43:08.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:08.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:08.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:43:08.000000 mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:08.737384 mypy-boto3-lexv2-runtime-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-28 20:30:04.000000 mypy-boto3-lexv2-runtime-1.28.15/setup.py
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/LICENSE` & `mypy-boto3-lexv2-runtime-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/PKG-INFO` & `mypy-boto3-lexv2-runtime-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-runtime
-Version: 1.28.12
-Summary: Type annotations for boto3.LexRuntimeV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LexRuntimeV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,62 +303,57 @@
 ### Typed dictionaries
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
-    ActiveContextOutputTypeDef,
-    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
-    ActiveContextTypeDef,
-    ButtonOutputTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
-    DialogActionOutputTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionTypeDef,
-    ElicitSubSlotOutputTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
-    GetSessionResponseTypeDef,
-    ImageResponseCardOutputTypeDef,
-    ImageResponseCardTypeDef,
     IntentOutputTypeDef,
     IntentTypeDef,
-    InterpretationTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    PutSessionRequestRequestTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    RecognizeTextResponseTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    RecognizeUtteranceResponseTypeDef,
     RecognizedBotMemberTypeDef,
-    ResponseMetadataTypeDef,
-    RuntimeHintDetailsOutputTypeDef,
-    RuntimeHintDetailsTypeDef,
-    RuntimeHintValueOutputTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
-    SentimentResponseTypeDef,
     SentimentScoreTypeDef,
-    SessionStateOutputTypeDef,
-    SessionStateTypeDef,
-    SlotOutputTypeDef,
-    SlotTypeDef,
     ValueOutputTypeDef,
     ValueTypeDef,
+    ActiveContextOutputTypeDef,
+    ActiveContextTypeDef,
+    ImageResponseCardOutputTypeDef,
+    ImageResponseCardTypeDef,
+    DeleteSessionResponseTypeDef,
+    PutSessionResponseTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
+    RuntimeHintDetailsTypeDef,
+    SentimentResponseTypeDef,
+    SlotOutputTypeDef,
+    SlotTypeDef,
+    SessionStateOutputTypeDef,
+    SessionStateTypeDef,
+    MessageOutputTypeDef,
+    MessageTypeDef,
+    InterpretationTypeDef,
+    RecognizeTextRequestRequestTypeDef,
+    PutSessionRequestRequestTypeDef,
+    GetSessionResponseTypeDef,
+    RecognizeTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextOutputTypeDef:
+def get_structure() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/README.md` & `mypy-boto3-lexv2-runtime-1.28.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,62 +271,57 @@
 ### Typed dictionaries
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
-    ActiveContextOutputTypeDef,
-    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
-    ActiveContextTypeDef,
-    ButtonOutputTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
-    DialogActionOutputTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionTypeDef,
-    ElicitSubSlotOutputTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
-    GetSessionResponseTypeDef,
-    ImageResponseCardOutputTypeDef,
-    ImageResponseCardTypeDef,
     IntentOutputTypeDef,
     IntentTypeDef,
-    InterpretationTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    PutSessionRequestRequestTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    RecognizeTextResponseTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    RecognizeUtteranceResponseTypeDef,
     RecognizedBotMemberTypeDef,
-    ResponseMetadataTypeDef,
-    RuntimeHintDetailsOutputTypeDef,
-    RuntimeHintDetailsTypeDef,
-    RuntimeHintValueOutputTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
-    SentimentResponseTypeDef,
     SentimentScoreTypeDef,
-    SessionStateOutputTypeDef,
-    SessionStateTypeDef,
-    SlotOutputTypeDef,
-    SlotTypeDef,
     ValueOutputTypeDef,
     ValueTypeDef,
+    ActiveContextOutputTypeDef,
+    ActiveContextTypeDef,
+    ImageResponseCardOutputTypeDef,
+    ImageResponseCardTypeDef,
+    DeleteSessionResponseTypeDef,
+    PutSessionResponseTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
+    RuntimeHintDetailsTypeDef,
+    SentimentResponseTypeDef,
+    SlotOutputTypeDef,
+    SlotTypeDef,
+    SessionStateOutputTypeDef,
+    SessionStateTypeDef,
+    MessageOutputTypeDef,
+    MessageTypeDef,
+    InterpretationTypeDef,
+    RecognizeTextRequestRequestTypeDef,
+    PutSessionRequestRequestTypeDef,
+    GetSessionResponseTypeDef,
+    RecognizeTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextOutputTypeDef:
+def get_structure() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/__main__.py` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.LexRuntimeV2 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.LexRuntimeV2 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2\nOther"
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

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/client.py` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,16 +121,16 @@
     def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: "SessionStateTypeDef",
-        messages: Sequence["MessageTypeDef"] = ...,
+        sessionState: SessionStateTypeDef,
+        messages: Sequence[MessageTypeDef] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
@@ -141,15 +141,15 @@
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: "SessionStateTypeDef" = ...,
+        sessionState: SessionStateTypeDef = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#recognize_text)
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/client.pyi` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,16 @@
     def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: "SessionStateTypeDef",
-        messages: Sequence["MessageTypeDef"] = ...,
+        sessionState: SessionStateTypeDef,
+        messages: Sequence[MessageTypeDef] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
@@ -131,15 +131,15 @@
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: "SessionStateTypeDef" = ...,
+        sessionState: SessionStateTypeDef = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/client/#recognize_text)
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/literals.py` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/literals.pyi` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/type_defs.py` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lexv2-runtime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lexv2_runtime.type_defs import ActiveContextOutputTypeDef
+    from mypy_boto3_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextOutputTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -27,104 +27,64 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "ActiveContextOutputTypeDef",
-    "ActiveContextTimeToLiveOutputTypeDef",
     "ActiveContextTimeToLiveTypeDef",
-    "ActiveContextTypeDef",
-    "ButtonOutputTypeDef",
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "DeleteSessionResponseTypeDef",
-    "DialogActionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
-    "ElicitSubSlotOutputTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "GetSessionResponseTypeDef",
-    "ImageResponseCardOutputTypeDef",
-    "ImageResponseCardTypeDef",
     "IntentOutputTypeDef",
     "IntentTypeDef",
-    "InterpretationTypeDef",
-    "MessageOutputTypeDef",
-    "MessageTypeDef",
-    "PutSessionRequestRequestTypeDef",
-    "PutSessionResponseTypeDef",
-    "RecognizeTextRequestRequestTypeDef",
-    "RecognizeTextResponseTypeDef",
-    "RecognizeUtteranceRequestRequestTypeDef",
-    "RecognizeUtteranceResponseTypeDef",
     "RecognizedBotMemberTypeDef",
-    "ResponseMetadataTypeDef",
-    "RuntimeHintDetailsOutputTypeDef",
-    "RuntimeHintDetailsTypeDef",
-    "RuntimeHintValueOutputTypeDef",
+    "RecognizeUtteranceRequestRequestTypeDef",
     "RuntimeHintValueTypeDef",
     "RuntimeHintsOutputTypeDef",
     "RuntimeHintsTypeDef",
-    "SentimentResponseTypeDef",
     "SentimentScoreTypeDef",
-    "SessionStateOutputTypeDef",
-    "SessionStateTypeDef",
-    "SlotOutputTypeDef",
-    "SlotTypeDef",
     "ValueOutputTypeDef",
     "ValueTypeDef",
-)
-
-ActiveContextOutputTypeDef = TypedDict(
     "ActiveContextOutputTypeDef",
-    {
-        "name": str,
-        "timeToLive": "ActiveContextTimeToLiveOutputTypeDef",
-        "contextAttributes": Dict[str, str],
-    },
-)
-
-ActiveContextTimeToLiveOutputTypeDef = TypedDict(
-    "ActiveContextTimeToLiveOutputTypeDef",
-    {
-        "timeToLiveInSeconds": int,
-        "turnsToLive": int,
-    },
+    "ActiveContextTypeDef",
+    "ImageResponseCardOutputTypeDef",
+    "ImageResponseCardTypeDef",
+    "DeleteSessionResponseTypeDef",
+    "PutSessionResponseTypeDef",
+    "RecognizeUtteranceResponseTypeDef",
+    "RuntimeHintDetailsOutputTypeDef",
+    "RuntimeHintDetailsTypeDef",
+    "SentimentResponseTypeDef",
+    "SlotOutputTypeDef",
+    "SlotTypeDef",
+    "SessionStateOutputTypeDef",
+    "SessionStateTypeDef",
+    "MessageOutputTypeDef",
+    "MessageTypeDef",
+    "InterpretationTypeDef",
+    "RecognizeTextRequestRequestTypeDef",
+    "PutSessionRequestRequestTypeDef",
+    "GetSessionResponseTypeDef",
+    "RecognizeTextResponseTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
-ActiveContextTypeDef = TypedDict(
-    "ActiveContextTypeDef",
-    {
-        "name": str,
-        "timeToLive": "ActiveContextTimeToLiveTypeDef",
-        "contextAttributes": Mapping[str, str],
-    },
-)
-
-ButtonOutputTypeDef = TypedDict(
-    "ButtonOutputTypeDef",
-    {
-        "text": str,
-        "value": str,
-    },
-)
-
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -143,48 +103,25 @@
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDialogActionOutputTypeDef = TypedDict(
-    "_RequiredDialogActionOutputTypeDef",
-    {
-        "type": DialogActionTypeType,
-    },
-)
-_OptionalDialogActionOutputTypeDef = TypedDict(
-    "_OptionalDialogActionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "slotToElicit": str,
-        "slotElicitationStyle": StyleTypeType,
-        "subSlotToElicit": "ElicitSubSlotOutputTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-
-class DialogActionOutputTypeDef(
-    _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
-):
-    pass
-
-
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
@@ -193,126 +130,44 @@
         "slotToElicit": str,
         "slotElicitationStyle": StyleTypeType,
         "subSlotToElicit": "ElicitSubSlotTypeDef",
     },
     total=False,
 )
 
-
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
-
-_RequiredElicitSubSlotOutputTypeDef = TypedDict(
-    "_RequiredElicitSubSlotOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalElicitSubSlotOutputTypeDef = TypedDict(
-    "_OptionalElicitSubSlotOutputTypeDef",
-    {
-        "subSlotToElicit": Dict[str, Any],
-    },
-    total=False,
-)
-
-
-class ElicitSubSlotOutputTypeDef(
-    _RequiredElicitSubSlotOutputTypeDef, _OptionalElicitSubSlotOutputTypeDef
-):
-    pass
-
-
 _RequiredElicitSubSlotTypeDef = TypedDict(
     "_RequiredElicitSubSlotTypeDef",
     {
         "name": str,
     },
 )
 _OptionalElicitSubSlotTypeDef = TypedDict(
     "_OptionalElicitSubSlotTypeDef",
     {
         "subSlotToElicit": Dict[str, Any],
     },
     total=False,
 )
 
-
 class ElicitSubSlotTypeDef(_RequiredElicitSubSlotTypeDef, _OptionalElicitSubSlotTypeDef):
     pass
 
-
 GetSessionRequestRequestTypeDef = TypedDict(
     "GetSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "sessionId": str,
-        "messages": List["MessageOutputTypeDef"],
-        "interpretations": List["InterpretationTypeDef"],
-        "sessionState": "SessionStateOutputTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredImageResponseCardOutputTypeDef = TypedDict(
-    "_RequiredImageResponseCardOutputTypeDef",
-    {
-        "title": str,
-    },
-)
-_OptionalImageResponseCardOutputTypeDef = TypedDict(
-    "_OptionalImageResponseCardOutputTypeDef",
-    {
-        "subtitle": str,
-        "imageUrl": str,
-        "buttons": List["ButtonOutputTypeDef"],
-    },
-    total=False,
-)
-
-
-class ImageResponseCardOutputTypeDef(
-    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
-):
-    pass
-
-
-_RequiredImageResponseCardTypeDef = TypedDict(
-    "_RequiredImageResponseCardTypeDef",
-    {
-        "title": str,
-    },
-)
-_OptionalImageResponseCardTypeDef = TypedDict(
-    "_OptionalImageResponseCardTypeDef",
-    {
-        "subtitle": str,
-        "imageUrl": str,
-        "buttons": Sequence["ButtonTypeDef"],
-    },
-    total=False,
-)
-
-
-class ImageResponseCardTypeDef(
-    _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
-):
-    pass
-
-
 _RequiredIntentOutputTypeDef = TypedDict(
     "_RequiredIntentOutputTypeDef",
     {
         "name": str,
     },
 )
 _OptionalIntentOutputTypeDef = TypedDict(
@@ -321,19 +176,17 @@
         "slots": Dict[str, "SlotOutputTypeDef"],
         "state": IntentStateType,
         "confirmationState": ConfirmationStateType,
     },
     total=False,
 )
 
-
 class IntentOutputTypeDef(_RequiredIntentOutputTypeDef, _OptionalIntentOutputTypeDef):
     pass
 
-
 _RequiredIntentTypeDef = TypedDict(
     "_RequiredIntentTypeDef",
     {
         "name": str,
     },
 )
 _OptionalIntentTypeDef = TypedDict(
@@ -342,373 +195,420 @@
         "slots": Mapping[str, "SlotTypeDef"],
         "state": IntentStateType,
         "confirmationState": ConfirmationStateType,
     },
     total=False,
 )
 
-
 class IntentTypeDef(_RequiredIntentTypeDef, _OptionalIntentTypeDef):
     pass
 
-
-InterpretationTypeDef = TypedDict(
-    "InterpretationTypeDef",
+_RequiredRecognizedBotMemberTypeDef = TypedDict(
+    "_RequiredRecognizedBotMemberTypeDef",
     {
-        "nluConfidence": "ConfidenceScoreTypeDef",
-        "sentimentResponse": "SentimentResponseTypeDef",
-        "intent": "IntentOutputTypeDef",
+        "botId": str,
+    },
+)
+_OptionalRecognizedBotMemberTypeDef = TypedDict(
+    "_OptionalRecognizedBotMemberTypeDef",
+    {
+        "botName": str,
     },
     total=False,
 )
 
-_RequiredMessageOutputTypeDef = TypedDict(
-    "_RequiredMessageOutputTypeDef",
+class RecognizedBotMemberTypeDef(
+    _RequiredRecognizedBotMemberTypeDef, _OptionalRecognizedBotMemberTypeDef
+):
+    pass
+
+_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
     {
-        "contentType": MessageContentTypeType,
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "requestContentType": str,
     },
 )
-_OptionalMessageOutputTypeDef = TypedDict(
-    "_OptionalMessageOutputTypeDef",
+_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
     {
-        "content": str,
-        "imageResponseCard": "ImageResponseCardOutputTypeDef",
+        "sessionState": str,
+        "requestAttributes": str,
+        "responseContentType": str,
+        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-
-class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+class RecognizeUtteranceRequestRequestTypeDef(
+    _RequiredRecognizeUtteranceRequestRequestTypeDef,
+    _OptionalRecognizeUtteranceRequestRequestTypeDef,
+):
     pass
 
+RuntimeHintValueTypeDef = TypedDict(
+    "RuntimeHintValueTypeDef",
+    {
+        "phrase": str,
+    },
+)
 
-_RequiredMessageTypeDef = TypedDict(
-    "_RequiredMessageTypeDef",
+RuntimeHintsOutputTypeDef = TypedDict(
+    "RuntimeHintsOutputTypeDef",
     {
-        "contentType": MessageContentTypeType,
+        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsOutputTypeDef"]],
     },
+    total=False,
 )
-_OptionalMessageTypeDef = TypedDict(
-    "_OptionalMessageTypeDef",
+
+RuntimeHintsTypeDef = TypedDict(
+    "RuntimeHintsTypeDef",
     {
-        "content": str,
-        "imageResponseCard": "ImageResponseCardTypeDef",
+        "slotHints": Mapping[str, Mapping[str, "RuntimeHintDetailsTypeDef"]],
+    },
+    total=False,
+)
+
+SentimentScoreTypeDef = TypedDict(
+    "SentimentScoreTypeDef",
+    {
+        "positive": float,
+        "negative": float,
+        "neutral": float,
+        "mixed": float,
     },
     total=False,
 )
 
+_RequiredValueOutputTypeDef = TypedDict(
+    "_RequiredValueOutputTypeDef",
+    {
+        "interpretedValue": str,
+    },
+)
+_OptionalValueOutputTypeDef = TypedDict(
+    "_OptionalValueOutputTypeDef",
+    {
+        "originalValue": str,
+        "resolvedValues": List[str],
+    },
+    total=False,
+)
 
-class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
+class ValueOutputTypeDef(_RequiredValueOutputTypeDef, _OptionalValueOutputTypeDef):
     pass
 
-
-_RequiredPutSessionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSessionRequestRequestTypeDef",
+_RequiredValueTypeDef = TypedDict(
+    "_RequiredValueTypeDef",
     {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "sessionState": "SessionStateTypeDef",
+        "interpretedValue": str,
     },
 )
-_OptionalPutSessionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSessionRequestRequestTypeDef",
+_OptionalValueTypeDef = TypedDict(
+    "_OptionalValueTypeDef",
     {
-        "messages": Sequence["MessageTypeDef"],
-        "requestAttributes": Mapping[str, str],
-        "responseContentType": str,
+        "originalValue": str,
+        "resolvedValues": Sequence[str],
     },
     total=False,
 )
 
-
-class PutSessionRequestRequestTypeDef(
-    _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
-):
+class ValueTypeDef(_RequiredValueTypeDef, _OptionalValueTypeDef):
     pass
 
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "contextAttributes": Dict[str, str],
+    },
+)
 
-PutSessionResponseTypeDef = TypedDict(
-    "PutSessionResponseTypeDef",
+ActiveContextTypeDef = TypedDict(
+    "ActiveContextTypeDef",
     {
-        "contentType": str,
-        "messages": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "audioStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "contextAttributes": Mapping[str, str],
     },
 )
 
-_RequiredRecognizeTextRequestRequestTypeDef = TypedDict(
-    "_RequiredRecognizeTextRequestRequestTypeDef",
+_RequiredImageResponseCardOutputTypeDef = TypedDict(
+    "_RequiredImageResponseCardOutputTypeDef",
     {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "text": str,
+        "title": str,
     },
 )
-_OptionalRecognizeTextRequestRequestTypeDef = TypedDict(
-    "_OptionalRecognizeTextRequestRequestTypeDef",
+_OptionalImageResponseCardOutputTypeDef = TypedDict(
+    "_OptionalImageResponseCardOutputTypeDef",
     {
-        "sessionState": "SessionStateTypeDef",
-        "requestAttributes": Mapping[str, str],
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
     },
     total=False,
 )
 
-
-class RecognizeTextRequestRequestTypeDef(
-    _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
+class ImageResponseCardOutputTypeDef(
+    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
 ):
     pass
 
-
-RecognizeTextResponseTypeDef = TypedDict(
-    "RecognizeTextResponseTypeDef",
+_RequiredImageResponseCardTypeDef = TypedDict(
+    "_RequiredImageResponseCardTypeDef",
     {
-        "messages": List["MessageOutputTypeDef"],
-        "sessionState": "SessionStateOutputTypeDef",
-        "interpretations": List["InterpretationTypeDef"],
-        "requestAttributes": Dict[str, str],
-        "sessionId": str,
-        "recognizedBotMember": "RecognizedBotMemberTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "title": str,
     },
 )
+_OptionalImageResponseCardTypeDef = TypedDict(
+    "_OptionalImageResponseCardTypeDef",
+    {
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": Sequence[ButtonTypeDef],
+    },
+    total=False,
+)
 
-_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
+class ImageResponseCardTypeDef(
+    _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
+):
+    pass
+
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
-        "requestContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
+
+PutSessionResponseTypeDef = TypedDict(
+    "PutSessionResponseTypeDef",
     {
+        "contentType": str,
+        "messages": str,
         "sessionState": str,
         "requestAttributes": str,
-        "responseContentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
+        "sessionId": str,
+        "audioStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class RecognizeUtteranceRequestRequestTypeDef(
-    _RequiredRecognizeUtteranceRequestRequestTypeDef,
-    _OptionalRecognizeUtteranceRequestRequestTypeDef,
-):
-    pass
-
-
 RecognizeUtteranceResponseTypeDef = TypedDict(
     "RecognizeUtteranceResponseTypeDef",
     {
         "inputMode": str,
         "contentType": str,
         "messages": str,
         "interpretations": str,
         "sessionState": str,
         "requestAttributes": str,
         "sessionId": str,
         "inputTranscript": str,
         "audioStream": StreamingBody,
         "recognizedBotMember": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredRecognizedBotMemberTypeDef = TypedDict(
-    "_RequiredRecognizedBotMemberTypeDef",
-    {
-        "botId": str,
-    },
-)
-_OptionalRecognizedBotMemberTypeDef = TypedDict(
-    "_OptionalRecognizedBotMemberTypeDef",
-    {
-        "botName": str,
-    },
-    total=False,
-)
-
-
-class RecognizedBotMemberTypeDef(
-    _RequiredRecognizedBotMemberTypeDef, _OptionalRecognizedBotMemberTypeDef
-):
-    pass
-
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuntimeHintDetailsOutputTypeDef = TypedDict(
     "RuntimeHintDetailsOutputTypeDef",
     {
-        "runtimeHintValues": List["RuntimeHintValueOutputTypeDef"],
+        "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
 RuntimeHintDetailsTypeDef = TypedDict(
     "RuntimeHintDetailsTypeDef",
     {
-        "runtimeHintValues": Sequence["RuntimeHintValueTypeDef"],
+        "runtimeHintValues": Sequence[RuntimeHintValueTypeDef],
         "subSlotHints": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
-RuntimeHintValueOutputTypeDef = TypedDict(
-    "RuntimeHintValueOutputTypeDef",
+SentimentResponseTypeDef = TypedDict(
+    "SentimentResponseTypeDef",
     {
-        "phrase": str,
+        "sentiment": SentimentTypeType,
+        "sentimentScore": SentimentScoreTypeDef,
     },
+    total=False,
 )
 
-RuntimeHintValueTypeDef = TypedDict(
-    "RuntimeHintValueTypeDef",
+SlotOutputTypeDef = TypedDict(
+    "SlotOutputTypeDef",
     {
-        "phrase": str,
+        "value": ValueOutputTypeDef,
+        "shape": ShapeType,
+        "values": List[Dict[str, Any]],
+        "subSlots": Dict[str, Dict[str, Any]],
     },
+    total=False,
 )
 
-RuntimeHintsOutputTypeDef = TypedDict(
-    "RuntimeHintsOutputTypeDef",
+SlotTypeDef = TypedDict(
+    "SlotTypeDef",
     {
-        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsOutputTypeDef"]],
+        "value": ValueTypeDef,
+        "shape": ShapeType,
+        "values": Sequence[Dict[str, Any]],
+        "subSlots": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
-RuntimeHintsTypeDef = TypedDict(
-    "RuntimeHintsTypeDef",
+SessionStateOutputTypeDef = TypedDict(
+    "SessionStateOutputTypeDef",
     {
-        "slotHints": Mapping[str, Mapping[str, "RuntimeHintDetailsTypeDef"]],
+        "dialogAction": DialogActionTypeDef,
+        "intent": IntentOutputTypeDef,
+        "activeContexts": List[ActiveContextOutputTypeDef],
+        "sessionAttributes": Dict[str, str],
+        "originatingRequestId": str,
+        "runtimeHints": RuntimeHintsOutputTypeDef,
     },
     total=False,
 )
 
-SentimentResponseTypeDef = TypedDict(
-    "SentimentResponseTypeDef",
+SessionStateTypeDef = TypedDict(
+    "SessionStateTypeDef",
     {
-        "sentiment": SentimentTypeType,
-        "sentimentScore": "SentimentScoreTypeDef",
+        "dialogAction": DialogActionTypeDef,
+        "intent": IntentTypeDef,
+        "activeContexts": Sequence[ActiveContextTypeDef],
+        "sessionAttributes": Mapping[str, str],
+        "originatingRequestId": str,
+        "runtimeHints": RuntimeHintsTypeDef,
     },
     total=False,
 )
 
-SentimentScoreTypeDef = TypedDict(
-    "SentimentScoreTypeDef",
+_RequiredMessageOutputTypeDef = TypedDict(
+    "_RequiredMessageOutputTypeDef",
     {
-        "positive": float,
-        "negative": float,
-        "neutral": float,
-        "mixed": float,
+        "contentType": MessageContentTypeType,
     },
-    total=False,
 )
-
-SessionStateOutputTypeDef = TypedDict(
-    "SessionStateOutputTypeDef",
+_OptionalMessageOutputTypeDef = TypedDict(
+    "_OptionalMessageOutputTypeDef",
     {
-        "dialogAction": "DialogActionOutputTypeDef",
-        "intent": "IntentOutputTypeDef",
-        "activeContexts": List["ActiveContextOutputTypeDef"],
-        "sessionAttributes": Dict[str, str],
-        "originatingRequestId": str,
-        "runtimeHints": "RuntimeHintsOutputTypeDef",
+        "content": str,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
     },
     total=False,
 )
 
-SessionStateTypeDef = TypedDict(
-    "SessionStateTypeDef",
+class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+    pass
+
+_RequiredMessageTypeDef = TypedDict(
+    "_RequiredMessageTypeDef",
     {
-        "dialogAction": "DialogActionTypeDef",
-        "intent": "IntentTypeDef",
-        "activeContexts": Sequence["ActiveContextTypeDef"],
-        "sessionAttributes": Mapping[str, str],
-        "originatingRequestId": str,
-        "runtimeHints": "RuntimeHintsTypeDef",
+        "contentType": MessageContentTypeType,
     },
-    total=False,
 )
-
-SlotOutputTypeDef = TypedDict(
-    "SlotOutputTypeDef",
+_OptionalMessageTypeDef = TypedDict(
+    "_OptionalMessageTypeDef",
     {
-        "value": "ValueOutputTypeDef",
-        "shape": ShapeType,
-        "values": List[Dict[str, Any]],
-        "subSlots": Dict[str, Dict[str, Any]],
+        "content": str,
+        "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
-SlotTypeDef = TypedDict(
-    "SlotTypeDef",
+class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
+    pass
+
+InterpretationTypeDef = TypedDict(
+    "InterpretationTypeDef",
     {
-        "value": "ValueTypeDef",
-        "shape": ShapeType,
-        "values": Sequence[Dict[str, Any]],
-        "subSlots": Mapping[str, Dict[str, Any]],
+        "nluConfidence": ConfidenceScoreTypeDef,
+        "sentimentResponse": SentimentResponseTypeDef,
+        "intent": IntentOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredValueOutputTypeDef = TypedDict(
-    "_RequiredValueOutputTypeDef",
+_RequiredRecognizeTextRequestRequestTypeDef = TypedDict(
+    "_RequiredRecognizeTextRequestRequestTypeDef",
     {
-        "interpretedValue": str,
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "text": str,
     },
 )
-_OptionalValueOutputTypeDef = TypedDict(
-    "_OptionalValueOutputTypeDef",
+_OptionalRecognizeTextRequestRequestTypeDef = TypedDict(
+    "_OptionalRecognizeTextRequestRequestTypeDef",
     {
-        "originalValue": str,
-        "resolvedValues": List[str],
+        "sessionState": SessionStateTypeDef,
+        "requestAttributes": Mapping[str, str],
     },
     total=False,
 )
 
-
-class ValueOutputTypeDef(_RequiredValueOutputTypeDef, _OptionalValueOutputTypeDef):
+class RecognizeTextRequestRequestTypeDef(
+    _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
+):
     pass
 
-
-_RequiredValueTypeDef = TypedDict(
-    "_RequiredValueTypeDef",
+_RequiredPutSessionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSessionRequestRequestTypeDef",
     {
-        "interpretedValue": str,
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "sessionState": SessionStateTypeDef,
     },
 )
-_OptionalValueTypeDef = TypedDict(
-    "_OptionalValueTypeDef",
+_OptionalPutSessionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSessionRequestRequestTypeDef",
     {
-        "originalValue": str,
-        "resolvedValues": Sequence[str],
+        "messages": Sequence[MessageTypeDef],
+        "requestAttributes": Mapping[str, str],
+        "responseContentType": str,
     },
     total=False,
 )
 
-
-class ValueTypeDef(_RequiredValueTypeDef, _OptionalValueTypeDef):
+class PutSessionRequestRequestTypeDef(
+    _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
+):
     pass
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "sessionId": str,
+        "messages": List[MessageOutputTypeDef],
+        "interpretations": List[InterpretationTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecognizeTextResponseTypeDef = TypedDict(
+    "RecognizeTextResponseTypeDef",
+    {
+        "messages": List[MessageOutputTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "interpretations": List[InterpretationTypeDef],
+        "requestAttributes": Dict[str, str],
+        "sessionId": str,
+        "recognizedBotMember": RecognizedBotMemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime/type_defs.pyi` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for lexv2-runtime service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_lexv2_runtime.type_defs import ActiveContextOutputTypeDef
+    from mypy_boto3_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextOutputTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = {...}
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
 
@@ -27,103 +27,65 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "ActiveContextOutputTypeDef",
-    "ActiveContextTimeToLiveOutputTypeDef",
     "ActiveContextTimeToLiveTypeDef",
-    "ActiveContextTypeDef",
-    "ButtonOutputTypeDef",
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "DeleteSessionResponseTypeDef",
-    "DialogActionOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
-    "ElicitSubSlotOutputTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "GetSessionResponseTypeDef",
-    "ImageResponseCardOutputTypeDef",
-    "ImageResponseCardTypeDef",
     "IntentOutputTypeDef",
     "IntentTypeDef",
-    "InterpretationTypeDef",
-    "MessageOutputTypeDef",
-    "MessageTypeDef",
-    "PutSessionRequestRequestTypeDef",
-    "PutSessionResponseTypeDef",
-    "RecognizeTextRequestRequestTypeDef",
-    "RecognizeTextResponseTypeDef",
-    "RecognizeUtteranceRequestRequestTypeDef",
-    "RecognizeUtteranceResponseTypeDef",
     "RecognizedBotMemberTypeDef",
-    "ResponseMetadataTypeDef",
-    "RuntimeHintDetailsOutputTypeDef",
-    "RuntimeHintDetailsTypeDef",
-    "RuntimeHintValueOutputTypeDef",
+    "RecognizeUtteranceRequestRequestTypeDef",
     "RuntimeHintValueTypeDef",
     "RuntimeHintsOutputTypeDef",
     "RuntimeHintsTypeDef",
-    "SentimentResponseTypeDef",
     "SentimentScoreTypeDef",
-    "SessionStateOutputTypeDef",
-    "SessionStateTypeDef",
-    "SlotOutputTypeDef",
-    "SlotTypeDef",
     "ValueOutputTypeDef",
     "ValueTypeDef",
-)
-
-ActiveContextOutputTypeDef = TypedDict(
     "ActiveContextOutputTypeDef",
-    {
-        "name": str,
-        "timeToLive": "ActiveContextTimeToLiveOutputTypeDef",
-        "contextAttributes": Dict[str, str],
-    },
-)
-
-ActiveContextTimeToLiveOutputTypeDef = TypedDict(
-    "ActiveContextTimeToLiveOutputTypeDef",
-    {
-        "timeToLiveInSeconds": int,
-        "turnsToLive": int,
-    },
+    "ActiveContextTypeDef",
+    "ImageResponseCardOutputTypeDef",
+    "ImageResponseCardTypeDef",
+    "DeleteSessionResponseTypeDef",
+    "PutSessionResponseTypeDef",
+    "RecognizeUtteranceResponseTypeDef",
+    "RuntimeHintDetailsOutputTypeDef",
+    "RuntimeHintDetailsTypeDef",
+    "SentimentResponseTypeDef",
+    "SlotOutputTypeDef",
+    "SlotTypeDef",
+    "SessionStateOutputTypeDef",
+    "SessionStateTypeDef",
+    "MessageOutputTypeDef",
+    "MessageTypeDef",
+    "InterpretationTypeDef",
+    "RecognizeTextRequestRequestTypeDef",
+    "PutSessionRequestRequestTypeDef",
+    "GetSessionResponseTypeDef",
+    "RecognizeTextResponseTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
-ActiveContextTypeDef = TypedDict(
-    "ActiveContextTypeDef",
-    {
-        "name": str,
-        "timeToLive": "ActiveContextTimeToLiveTypeDef",
-        "contextAttributes": Mapping[str, str],
-    },
-)
-
-ButtonOutputTypeDef = TypedDict(
-    "ButtonOutputTypeDef",
-    {
-        "text": str,
-        "value": str,
-    },
-)
-
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -142,46 +104,25 @@
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDialogActionOutputTypeDef = TypedDict(
-    "_RequiredDialogActionOutputTypeDef",
-    {
-        "type": DialogActionTypeType,
-    },
-)
-_OptionalDialogActionOutputTypeDef = TypedDict(
-    "_OptionalDialogActionOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "slotToElicit": str,
-        "slotElicitationStyle": StyleTypeType,
-        "subSlotToElicit": "ElicitSubSlotOutputTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-class DialogActionOutputTypeDef(
-    _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
-):
-    pass
-
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
@@ -190,35 +131,18 @@
         "slotToElicit": str,
         "slotElicitationStyle": StyleTypeType,
         "subSlotToElicit": "ElicitSubSlotTypeDef",
     },
     total=False,
 )
 
+
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
-_RequiredElicitSubSlotOutputTypeDef = TypedDict(
-    "_RequiredElicitSubSlotOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalElicitSubSlotOutputTypeDef = TypedDict(
-    "_OptionalElicitSubSlotOutputTypeDef",
-    {
-        "subSlotToElicit": Dict[str, Any],
-    },
-    total=False,
-)
-
-class ElicitSubSlotOutputTypeDef(
-    _RequiredElicitSubSlotOutputTypeDef, _OptionalElicitSubSlotOutputTypeDef
-):
-    pass
 
 _RequiredElicitSubSlotTypeDef = TypedDict(
     "_RequiredElicitSubSlotTypeDef",
     {
         "name": str,
     },
 )
@@ -226,457 +150,494 @@
     "_OptionalElicitSubSlotTypeDef",
     {
         "subSlotToElicit": Dict[str, Any],
     },
     total=False,
 )
 
+
 class ElicitSubSlotTypeDef(_RequiredElicitSubSlotTypeDef, _OptionalElicitSubSlotTypeDef):
     pass
 
+
 GetSessionRequestRequestTypeDef = TypedDict(
     "GetSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
+_RequiredIntentOutputTypeDef = TypedDict(
+    "_RequiredIntentOutputTypeDef",
     {
-        "sessionId": str,
-        "messages": List["MessageOutputTypeDef"],
-        "interpretations": List["InterpretationTypeDef"],
-        "sessionState": "SessionStateOutputTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "name": str,
     },
 )
+_OptionalIntentOutputTypeDef = TypedDict(
+    "_OptionalIntentOutputTypeDef",
+    {
+        "slots": Dict[str, "SlotOutputTypeDef"],
+        "state": IntentStateType,
+        "confirmationState": ConfirmationStateType,
+    },
+    total=False,
+)
 
-_RequiredImageResponseCardOutputTypeDef = TypedDict(
-    "_RequiredImageResponseCardOutputTypeDef",
+
+class IntentOutputTypeDef(_RequiredIntentOutputTypeDef, _OptionalIntentOutputTypeDef):
+    pass
+
+
+_RequiredIntentTypeDef = TypedDict(
+    "_RequiredIntentTypeDef",
     {
-        "title": str,
+        "name": str,
     },
 )
-_OptionalImageResponseCardOutputTypeDef = TypedDict(
-    "_OptionalImageResponseCardOutputTypeDef",
+_OptionalIntentTypeDef = TypedDict(
+    "_OptionalIntentTypeDef",
     {
-        "subtitle": str,
-        "imageUrl": str,
-        "buttons": List["ButtonOutputTypeDef"],
+        "slots": Mapping[str, "SlotTypeDef"],
+        "state": IntentStateType,
+        "confirmationState": ConfirmationStateType,
     },
     total=False,
 )
 
-class ImageResponseCardOutputTypeDef(
-    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
-):
+
+class IntentTypeDef(_RequiredIntentTypeDef, _OptionalIntentTypeDef):
     pass
 
-_RequiredImageResponseCardTypeDef = TypedDict(
-    "_RequiredImageResponseCardTypeDef",
+
+_RequiredRecognizedBotMemberTypeDef = TypedDict(
+    "_RequiredRecognizedBotMemberTypeDef",
     {
-        "title": str,
+        "botId": str,
     },
 )
-_OptionalImageResponseCardTypeDef = TypedDict(
-    "_OptionalImageResponseCardTypeDef",
+_OptionalRecognizedBotMemberTypeDef = TypedDict(
+    "_OptionalRecognizedBotMemberTypeDef",
     {
-        "subtitle": str,
-        "imageUrl": str,
-        "buttons": Sequence["ButtonTypeDef"],
+        "botName": str,
     },
     total=False,
 )
 
-class ImageResponseCardTypeDef(
-    _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
+
+class RecognizedBotMemberTypeDef(
+    _RequiredRecognizedBotMemberTypeDef, _OptionalRecognizedBotMemberTypeDef
 ):
     pass
 
-_RequiredIntentOutputTypeDef = TypedDict(
-    "_RequiredIntentOutputTypeDef",
+
+_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
     {
-        "name": str,
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "requestContentType": str,
     },
 )
-_OptionalIntentOutputTypeDef = TypedDict(
-    "_OptionalIntentOutputTypeDef",
+_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
     {
-        "slots": Dict[str, "SlotOutputTypeDef"],
-        "state": IntentStateType,
-        "confirmationState": ConfirmationStateType,
+        "sessionState": str,
+        "requestAttributes": str,
+        "responseContentType": str,
+        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-class IntentOutputTypeDef(_RequiredIntentOutputTypeDef, _OptionalIntentOutputTypeDef):
+
+class RecognizeUtteranceRequestRequestTypeDef(
+    _RequiredRecognizeUtteranceRequestRequestTypeDef,
+    _OptionalRecognizeUtteranceRequestRequestTypeDef,
+):
     pass
 
-_RequiredIntentTypeDef = TypedDict(
-    "_RequiredIntentTypeDef",
+
+RuntimeHintValueTypeDef = TypedDict(
+    "RuntimeHintValueTypeDef",
     {
-        "name": str,
+        "phrase": str,
     },
 )
-_OptionalIntentTypeDef = TypedDict(
-    "_OptionalIntentTypeDef",
+
+RuntimeHintsOutputTypeDef = TypedDict(
+    "RuntimeHintsOutputTypeDef",
     {
-        "slots": Mapping[str, "SlotTypeDef"],
-        "state": IntentStateType,
-        "confirmationState": ConfirmationStateType,
+        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsOutputTypeDef"]],
     },
     total=False,
 )
 
-class IntentTypeDef(_RequiredIntentTypeDef, _OptionalIntentTypeDef):
-    pass
+RuntimeHintsTypeDef = TypedDict(
+    "RuntimeHintsTypeDef",
+    {
+        "slotHints": Mapping[str, Mapping[str, "RuntimeHintDetailsTypeDef"]],
+    },
+    total=False,
+)
 
-InterpretationTypeDef = TypedDict(
-    "InterpretationTypeDef",
+SentimentScoreTypeDef = TypedDict(
+    "SentimentScoreTypeDef",
     {
-        "nluConfidence": "ConfidenceScoreTypeDef",
-        "sentimentResponse": "SentimentResponseTypeDef",
-        "intent": "IntentOutputTypeDef",
+        "positive": float,
+        "negative": float,
+        "neutral": float,
+        "mixed": float,
     },
     total=False,
 )
 
-_RequiredMessageOutputTypeDef = TypedDict(
-    "_RequiredMessageOutputTypeDef",
+_RequiredValueOutputTypeDef = TypedDict(
+    "_RequiredValueOutputTypeDef",
     {
-        "contentType": MessageContentTypeType,
+        "interpretedValue": str,
     },
 )
-_OptionalMessageOutputTypeDef = TypedDict(
-    "_OptionalMessageOutputTypeDef",
+_OptionalValueOutputTypeDef = TypedDict(
+    "_OptionalValueOutputTypeDef",
     {
-        "content": str,
-        "imageResponseCard": "ImageResponseCardOutputTypeDef",
+        "originalValue": str,
+        "resolvedValues": List[str],
     },
     total=False,
 )
 
-class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+
+class ValueOutputTypeDef(_RequiredValueOutputTypeDef, _OptionalValueOutputTypeDef):
     pass
 
-_RequiredMessageTypeDef = TypedDict(
-    "_RequiredMessageTypeDef",
+
+_RequiredValueTypeDef = TypedDict(
+    "_RequiredValueTypeDef",
     {
-        "contentType": MessageContentTypeType,
+        "interpretedValue": str,
     },
 )
-_OptionalMessageTypeDef = TypedDict(
-    "_OptionalMessageTypeDef",
+_OptionalValueTypeDef = TypedDict(
+    "_OptionalValueTypeDef",
     {
-        "content": str,
-        "imageResponseCard": "ImageResponseCardTypeDef",
+        "originalValue": str,
+        "resolvedValues": Sequence[str],
     },
     total=False,
 )
 
-class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
+
+class ValueTypeDef(_RequiredValueTypeDef, _OptionalValueTypeDef):
     pass
 
-_RequiredPutSessionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSessionRequestRequestTypeDef",
+
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
     {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "sessionState": "SessionStateTypeDef",
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "contextAttributes": Dict[str, str],
     },
 )
-_OptionalPutSessionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSessionRequestRequestTypeDef",
+
+ActiveContextTypeDef = TypedDict(
+    "ActiveContextTypeDef",
     {
-        "messages": Sequence["MessageTypeDef"],
-        "requestAttributes": Mapping[str, str],
-        "responseContentType": str,
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "contextAttributes": Mapping[str, str],
+    },
+)
+
+_RequiredImageResponseCardOutputTypeDef = TypedDict(
+    "_RequiredImageResponseCardOutputTypeDef",
+    {
+        "title": str,
+    },
+)
+_OptionalImageResponseCardOutputTypeDef = TypedDict(
+    "_OptionalImageResponseCardOutputTypeDef",
+    {
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
     },
     total=False,
 )
 
-class PutSessionRequestRequestTypeDef(
-    _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
+
+class ImageResponseCardOutputTypeDef(
+    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
 ):
     pass
 
-PutSessionResponseTypeDef = TypedDict(
-    "PutSessionResponseTypeDef",
-    {
-        "contentType": str,
-        "messages": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "audioStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-_RequiredRecognizeTextRequestRequestTypeDef = TypedDict(
-    "_RequiredRecognizeTextRequestRequestTypeDef",
+_RequiredImageResponseCardTypeDef = TypedDict(
+    "_RequiredImageResponseCardTypeDef",
     {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "text": str,
+        "title": str,
     },
 )
-_OptionalRecognizeTextRequestRequestTypeDef = TypedDict(
-    "_OptionalRecognizeTextRequestRequestTypeDef",
+_OptionalImageResponseCardTypeDef = TypedDict(
+    "_OptionalImageResponseCardTypeDef",
     {
-        "sessionState": "SessionStateTypeDef",
-        "requestAttributes": Mapping[str, str],
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": Sequence[ButtonTypeDef],
     },
     total=False,
 )
 
-class RecognizeTextRequestRequestTypeDef(
-    _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
+
+class ImageResponseCardTypeDef(
+    _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
-RecognizeTextResponseTypeDef = TypedDict(
-    "RecognizeTextResponseTypeDef",
-    {
-        "messages": List["MessageOutputTypeDef"],
-        "sessionState": "SessionStateOutputTypeDef",
-        "interpretations": List["InterpretationTypeDef"],
-        "requestAttributes": Dict[str, str],
-        "sessionId": str,
-        "recognizedBotMember": "RecognizedBotMemberTypeDef",
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
-        "requestContentType": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
+
+PutSessionResponseTypeDef = TypedDict(
+    "PutSessionResponseTypeDef",
     {
+        "contentType": str,
+        "messages": str,
         "sessionState": str,
         "requestAttributes": str,
-        "responseContentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
+        "sessionId": str,
+        "audioStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class RecognizeUtteranceRequestRequestTypeDef(
-    _RequiredRecognizeUtteranceRequestRequestTypeDef,
-    _OptionalRecognizeUtteranceRequestRequestTypeDef,
-):
-    pass
-
 RecognizeUtteranceResponseTypeDef = TypedDict(
     "RecognizeUtteranceResponseTypeDef",
     {
         "inputMode": str,
         "contentType": str,
         "messages": str,
         "interpretations": str,
         "sessionState": str,
         "requestAttributes": str,
         "sessionId": str,
         "inputTranscript": str,
         "audioStream": StreamingBody,
         "recognizedBotMember": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredRecognizedBotMemberTypeDef = TypedDict(
-    "_RequiredRecognizedBotMemberTypeDef",
-    {
-        "botId": str,
-    },
-)
-_OptionalRecognizedBotMemberTypeDef = TypedDict(
-    "_OptionalRecognizedBotMemberTypeDef",
-    {
-        "botName": str,
-    },
-    total=False,
-)
-
-class RecognizedBotMemberTypeDef(
-    _RequiredRecognizedBotMemberTypeDef, _OptionalRecognizedBotMemberTypeDef
-):
-    pass
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuntimeHintDetailsOutputTypeDef = TypedDict(
     "RuntimeHintDetailsOutputTypeDef",
     {
-        "runtimeHintValues": List["RuntimeHintValueOutputTypeDef"],
+        "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
 RuntimeHintDetailsTypeDef = TypedDict(
     "RuntimeHintDetailsTypeDef",
     {
-        "runtimeHintValues": Sequence["RuntimeHintValueTypeDef"],
+        "runtimeHintValues": Sequence[RuntimeHintValueTypeDef],
         "subSlotHints": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
-RuntimeHintValueOutputTypeDef = TypedDict(
-    "RuntimeHintValueOutputTypeDef",
+SentimentResponseTypeDef = TypedDict(
+    "SentimentResponseTypeDef",
     {
-        "phrase": str,
+        "sentiment": SentimentTypeType,
+        "sentimentScore": SentimentScoreTypeDef,
     },
+    total=False,
 )
 
-RuntimeHintValueTypeDef = TypedDict(
-    "RuntimeHintValueTypeDef",
+SlotOutputTypeDef = TypedDict(
+    "SlotOutputTypeDef",
     {
-        "phrase": str,
+        "value": ValueOutputTypeDef,
+        "shape": ShapeType,
+        "values": List[Dict[str, Any]],
+        "subSlots": Dict[str, Dict[str, Any]],
     },
+    total=False,
 )
 
-RuntimeHintsOutputTypeDef = TypedDict(
-    "RuntimeHintsOutputTypeDef",
+SlotTypeDef = TypedDict(
+    "SlotTypeDef",
     {
-        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsOutputTypeDef"]],
+        "value": ValueTypeDef,
+        "shape": ShapeType,
+        "values": Sequence[Dict[str, Any]],
+        "subSlots": Mapping[str, Dict[str, Any]],
     },
     total=False,
 )
 
-RuntimeHintsTypeDef = TypedDict(
-    "RuntimeHintsTypeDef",
+SessionStateOutputTypeDef = TypedDict(
+    "SessionStateOutputTypeDef",
     {
-        "slotHints": Mapping[str, Mapping[str, "RuntimeHintDetailsTypeDef"]],
+        "dialogAction": DialogActionTypeDef,
+        "intent": IntentOutputTypeDef,
+        "activeContexts": List[ActiveContextOutputTypeDef],
+        "sessionAttributes": Dict[str, str],
+        "originatingRequestId": str,
+        "runtimeHints": RuntimeHintsOutputTypeDef,
     },
     total=False,
 )
 
-SentimentResponseTypeDef = TypedDict(
-    "SentimentResponseTypeDef",
+SessionStateTypeDef = TypedDict(
+    "SessionStateTypeDef",
     {
-        "sentiment": SentimentTypeType,
-        "sentimentScore": "SentimentScoreTypeDef",
+        "dialogAction": DialogActionTypeDef,
+        "intent": IntentTypeDef,
+        "activeContexts": Sequence[ActiveContextTypeDef],
+        "sessionAttributes": Mapping[str, str],
+        "originatingRequestId": str,
+        "runtimeHints": RuntimeHintsTypeDef,
     },
     total=False,
 )
 
-SentimentScoreTypeDef = TypedDict(
-    "SentimentScoreTypeDef",
+_RequiredMessageOutputTypeDef = TypedDict(
+    "_RequiredMessageOutputTypeDef",
     {
-        "positive": float,
-        "negative": float,
-        "neutral": float,
-        "mixed": float,
+        "contentType": MessageContentTypeType,
     },
-    total=False,
 )
-
-SessionStateOutputTypeDef = TypedDict(
-    "SessionStateOutputTypeDef",
+_OptionalMessageOutputTypeDef = TypedDict(
+    "_OptionalMessageOutputTypeDef",
     {
-        "dialogAction": "DialogActionOutputTypeDef",
-        "intent": "IntentOutputTypeDef",
-        "activeContexts": List["ActiveContextOutputTypeDef"],
-        "sessionAttributes": Dict[str, str],
-        "originatingRequestId": str,
-        "runtimeHints": "RuntimeHintsOutputTypeDef",
+        "content": str,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
     },
     total=False,
 )
 
-SessionStateTypeDef = TypedDict(
-    "SessionStateTypeDef",
+
+class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+    pass
+
+
+_RequiredMessageTypeDef = TypedDict(
+    "_RequiredMessageTypeDef",
     {
-        "dialogAction": "DialogActionTypeDef",
-        "intent": "IntentTypeDef",
-        "activeContexts": Sequence["ActiveContextTypeDef"],
-        "sessionAttributes": Mapping[str, str],
-        "originatingRequestId": str,
-        "runtimeHints": "RuntimeHintsTypeDef",
+        "contentType": MessageContentTypeType,
     },
-    total=False,
 )
-
-SlotOutputTypeDef = TypedDict(
-    "SlotOutputTypeDef",
+_OptionalMessageTypeDef = TypedDict(
+    "_OptionalMessageTypeDef",
     {
-        "value": "ValueOutputTypeDef",
-        "shape": ShapeType,
-        "values": List[Dict[str, Any]],
-        "subSlots": Dict[str, Dict[str, Any]],
+        "content": str,
+        "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
-SlotTypeDef = TypedDict(
-    "SlotTypeDef",
+
+class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
+    pass
+
+
+InterpretationTypeDef = TypedDict(
+    "InterpretationTypeDef",
     {
-        "value": "ValueTypeDef",
-        "shape": ShapeType,
-        "values": Sequence[Dict[str, Any]],
-        "subSlots": Mapping[str, Dict[str, Any]],
+        "nluConfidence": ConfidenceScoreTypeDef,
+        "sentimentResponse": SentimentResponseTypeDef,
+        "intent": IntentOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredValueOutputTypeDef = TypedDict(
-    "_RequiredValueOutputTypeDef",
+_RequiredRecognizeTextRequestRequestTypeDef = TypedDict(
+    "_RequiredRecognizeTextRequestRequestTypeDef",
     {
-        "interpretedValue": str,
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "text": str,
     },
 )
-_OptionalValueOutputTypeDef = TypedDict(
-    "_OptionalValueOutputTypeDef",
+_OptionalRecognizeTextRequestRequestTypeDef = TypedDict(
+    "_OptionalRecognizeTextRequestRequestTypeDef",
     {
-        "originalValue": str,
-        "resolvedValues": List[str],
+        "sessionState": SessionStateTypeDef,
+        "requestAttributes": Mapping[str, str],
     },
     total=False,
 )
 
-class ValueOutputTypeDef(_RequiredValueOutputTypeDef, _OptionalValueOutputTypeDef):
+
+class RecognizeTextRequestRequestTypeDef(
+    _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
+):
     pass
 
-_RequiredValueTypeDef = TypedDict(
-    "_RequiredValueTypeDef",
+
+_RequiredPutSessionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSessionRequestRequestTypeDef",
     {
-        "interpretedValue": str,
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "sessionState": SessionStateTypeDef,
     },
 )
-_OptionalValueTypeDef = TypedDict(
-    "_OptionalValueTypeDef",
+_OptionalPutSessionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSessionRequestRequestTypeDef",
     {
-        "originalValue": str,
-        "resolvedValues": Sequence[str],
+        "messages": Sequence[MessageTypeDef],
+        "requestAttributes": Mapping[str, str],
+        "responseContentType": str,
     },
     total=False,
 )
 
-class ValueTypeDef(_RequiredValueTypeDef, _OptionalValueTypeDef):
+
+class PutSessionRequestRequestTypeDef(
+    _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
+):
     pass
+
+
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "sessionId": str,
+        "messages": List[MessageOutputTypeDef],
+        "interpretations": List[InterpretationTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecognizeTextResponseTypeDef = TypedDict(
+    "RecognizeTextResponseTypeDef",
+    {
+        "messages": List[MessageOutputTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "interpretations": List[InterpretationTypeDef],
+        "requestAttributes": Dict[str, str],
+        "sessionId": str,
+        "recognizedBotMember": RecognizedBotMemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lexv2-runtime
-Version: 1.28.12
-Summary: Type annotations for boto3.LexRuntimeV2 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.LexRuntimeV2 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lexv2-runtime.svg?color=blue)](https://pypi.org/project/mypy-boto3-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lexv2-runtime)](https://pepy.tech/project/mypy-boto3-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.LexRuntimeV2 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
+[boto3.LexRuntimeV2 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [mypy-boto3-lexv2-runtime docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lexv2_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,62 +303,57 @@
 ### Typed dictionaries
 
 `mypy_boto3_lexv2_runtime.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lexv2_runtime.type_defs import (
-    ActiveContextOutputTypeDef,
-    ActiveContextTimeToLiveOutputTypeDef,
     ActiveContextTimeToLiveTypeDef,
-    ActiveContextTypeDef,
-    ButtonOutputTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
-    DialogActionOutputTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionTypeDef,
-    ElicitSubSlotOutputTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
-    GetSessionResponseTypeDef,
-    ImageResponseCardOutputTypeDef,
-    ImageResponseCardTypeDef,
     IntentOutputTypeDef,
     IntentTypeDef,
-    InterpretationTypeDef,
-    MessageOutputTypeDef,
-    MessageTypeDef,
-    PutSessionRequestRequestTypeDef,
-    PutSessionResponseTypeDef,
-    RecognizeTextRequestRequestTypeDef,
-    RecognizeTextResponseTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    RecognizeUtteranceResponseTypeDef,
     RecognizedBotMemberTypeDef,
-    ResponseMetadataTypeDef,
-    RuntimeHintDetailsOutputTypeDef,
-    RuntimeHintDetailsTypeDef,
-    RuntimeHintValueOutputTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
     RuntimeHintValueTypeDef,
     RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
-    SentimentResponseTypeDef,
     SentimentScoreTypeDef,
-    SessionStateOutputTypeDef,
-    SessionStateTypeDef,
-    SlotOutputTypeDef,
-    SlotTypeDef,
     ValueOutputTypeDef,
     ValueTypeDef,
+    ActiveContextOutputTypeDef,
+    ActiveContextTypeDef,
+    ImageResponseCardOutputTypeDef,
+    ImageResponseCardTypeDef,
+    DeleteSessionResponseTypeDef,
+    PutSessionResponseTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
+    RuntimeHintDetailsTypeDef,
+    SentimentResponseTypeDef,
+    SlotOutputTypeDef,
+    SlotTypeDef,
+    SessionStateOutputTypeDef,
+    SessionStateTypeDef,
+    MessageOutputTypeDef,
+    MessageTypeDef,
+    InterpretationTypeDef,
+    RecognizeTextRequestRequestTypeDef,
+    PutSessionRequestRequestTypeDef,
+    GetSessionResponseTypeDef,
+    RecognizeTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextOutputTypeDef:
+def get_structure() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt` & `mypy-boto3-lexv2-runtime-1.28.15/mypy_boto3_lexv2_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lexv2-runtime-1.28.12/setup.py` & `mypy-boto3-lexv2-runtime-1.28.15/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lexv2-runtime",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_lexv2_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.LexRuntimeV2 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.LexRuntimeV2 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

