# Comparing `tmp/mypy-boto3-dlm-1.28.12.tar.gz` & `tmp/mypy-boto3-dlm-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-dlm-1.28.12.tar", last modified: Thu Jul 27 05:34:35 2023, max compression
+gzip compressed data, was "mypy-boto3-dlm-1.28.15.tar", last modified: Fri Jul 28 20:42:38 2023, max compression
```

## Comparing `mypy-boto3-dlm-1.28.12.tar` & `mypy-boto3-dlm-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.484530 mypy-boto3-dlm-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-27 05:34:35.480530 mypy-boto3-dlm-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12243 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.472530 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19704 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19675 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:18.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:35.480530 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13714 2023-07-27 05:34:35.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-27 05:34:35.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:35.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:35.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:35.000000 mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:35.484530 mypy-boto3-dlm-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:20:17.000000 mypy-boto3-dlm-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.156963 mypy-boto3-dlm-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-28 20:42:38.152963 mypy-boto3-dlm-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.152963 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9049 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16011 2023-07-28 20:23:03.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15988 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:38.152963 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:37.000000 mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:38.156963 mypy-boto3-dlm-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:23:02.000000 mypy-boto3-dlm-1.28.15/setup.py
```

### Comparing `mypy-boto3-dlm-1.28.12/LICENSE` & `mypy-boto3-dlm-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.12/PKG-INFO` & `mypy-boto3-dlm-1.28.15/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.28.12
-Summary: Type annotations for boto3.DLM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dlm)](https://pepy.tech/project/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,73 +305,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
-    RetentionArchiveTierOutputTypeDef,
     RetentionArchiveTierTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
-    CrossRegionCopyRetainRuleOutputTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
-    CrossRegionCopyDeprecateRuleOutputTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeprecateRuleOutputTypeDef,
     DeprecateRuleTypeDef,
     EventParametersOutputTypeDef,
     EventParametersTypeDef,
     FastRestoreRuleOutputTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
-    RetainRuleOutputTypeDef,
     RetainRuleTypeDef,
     ShareRuleOutputTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ArchiveRetainRuleOutputTypeDef,
     ArchiveRetainRuleTypeDef,
-    CrossRegionCopyActionOutputTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
-    CrossRegionCopyRuleOutputTypeDef,
     CrossRegionCopyRuleTypeDef,
     EventSourceOutputTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     ParametersOutputTypeDef,
     ParametersTypeDef,
-    ArchiveRuleOutputTypeDef,
     ArchiveRuleTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ScheduleOutputTypeDef,
     ScheduleTypeDef,
     PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
     LifecyclePolicyTypeDef,
     CreateLifecyclePolicyRequestRequestTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierOutputTypeDef:
+def get_structure() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dlm-1.28.12/README.md` & `mypy-boto3-dlm-1.28.15/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dlm)](https://pepy.tech/project/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -273,73 +273,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
-    RetentionArchiveTierOutputTypeDef,
     RetentionArchiveTierTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
-    CrossRegionCopyRetainRuleOutputTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
-    CrossRegionCopyDeprecateRuleOutputTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeprecateRuleOutputTypeDef,
     DeprecateRuleTypeDef,
     EventParametersOutputTypeDef,
     EventParametersTypeDef,
     FastRestoreRuleOutputTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
-    RetainRuleOutputTypeDef,
     RetainRuleTypeDef,
     ShareRuleOutputTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ArchiveRetainRuleOutputTypeDef,
     ArchiveRetainRuleTypeDef,
-    CrossRegionCopyActionOutputTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
-    CrossRegionCopyRuleOutputTypeDef,
     CrossRegionCopyRuleTypeDef,
     EventSourceOutputTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     ParametersOutputTypeDef,
     ParametersTypeDef,
-    ArchiveRuleOutputTypeDef,
     ArchiveRuleTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ScheduleOutputTypeDef,
     ScheduleTypeDef,
     PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
     LifecyclePolicyTypeDef,
     CreateLifecyclePolicyRequestRequestTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierOutputTypeDef:
+def get_structure() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/__main__.py` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DLM 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.DLM 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM\nOther"
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

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/client.py` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/client.pyi` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/literals.py` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/literals.pyi` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/type_defs.py` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/type_defs.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dlm service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dlm.type_defs import RetentionArchiveTierOutputTypeDef
+    from mypy_boto3_dlm.type_defs import RetentionArchiveTierTypeDef
 
-    data: RetentionArchiveTierOutputTypeDef = {...}
+    data: RetentionArchiveTierTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -32,96 +32,78 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "RetentionArchiveTierOutputTypeDef",
     "RetentionArchiveTierTypeDef",
-    "CreateLifecyclePolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateRuleOutputTypeDef",
     "CreateRuleTypeDef",
-    "CrossRegionCopyRetainRuleOutputTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "CrossRegionCopyRetainRuleTypeDef",
     "EncryptionConfigurationTypeDef",
-    "CrossRegionCopyDeprecateRuleOutputTypeDef",
     "CrossRegionCopyDeprecateRuleTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
-    "DeprecateRuleOutputTypeDef",
     "DeprecateRuleTypeDef",
     "EventParametersOutputTypeDef",
     "EventParametersTypeDef",
     "FastRestoreRuleOutputTypeDef",
     "FastRestoreRuleTypeDef",
     "GetLifecyclePoliciesRequestRequestTypeDef",
     "LifecyclePolicySummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "TagOutputTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
-    "RetainRuleOutputTypeDef",
     "RetainRuleTypeDef",
     "ShareRuleOutputTypeDef",
     "ShareRuleTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ArchiveRetainRuleOutputTypeDef",
     "ArchiveRetainRuleTypeDef",
-    "CrossRegionCopyActionOutputTypeDef",
+    "CreateLifecyclePolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CrossRegionCopyActionTypeDef",
-    "CrossRegionCopyRuleOutputTypeDef",
     "CrossRegionCopyRuleTypeDef",
     "EventSourceOutputTypeDef",
     "EventSourceTypeDef",
     "GetLifecyclePoliciesResponseTypeDef",
     "ParametersOutputTypeDef",
     "ParametersTypeDef",
-    "ArchiveRuleOutputTypeDef",
     "ArchiveRuleTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
     "ScheduleOutputTypeDef",
     "ScheduleTypeDef",
     "PolicyDetailsOutputTypeDef",
     "PolicyDetailsTypeDef",
     "LifecyclePolicyTypeDef",
     "CreateLifecyclePolicyRequestRequestTypeDef",
     "UpdateLifecyclePolicyRequestRequestTypeDef",
     "GetLifecyclePolicyResponseTypeDef",
 )
 
-RetentionArchiveTierOutputTypeDef = TypedDict(
-    "RetentionArchiveTierOutputTypeDef",
-    {
-        "Count": int,
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
 RetentionArchiveTierTypeDef = TypedDict(
     "RetentionArchiveTierTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
 )
 
-CreateLifecyclePolicyResponseTypeDef = TypedDict(
-    "CreateLifecyclePolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PolicyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateRuleOutputTypeDef = TypedDict(
     "CreateRuleOutputTypeDef",
     {
         "Location": LocationValuesType,
@@ -141,44 +123,14 @@
         "IntervalUnit": Literal["HOURS"],
         "Times": Sequence[str],
         "CronExpression": str,
     },
     total=False,
 )
 
-CrossRegionCopyRetainRuleOutputTypeDef = TypedDict(
-    "CrossRegionCopyRetainRuleOutputTypeDef",
-    {
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
-_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigurationOutputTypeDef",
-    {
-        "Encrypted": bool,
-    },
-)
-_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigurationOutputTypeDef",
-    {
-        "CmkArn": str,
-    },
-    total=False,
-)
-
-
-class EncryptionConfigurationOutputTypeDef(
-    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
-):
-    pass
-
-
 CrossRegionCopyRetainRuleTypeDef = TypedDict(
     "CrossRegionCopyRetainRuleTypeDef",
     {
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
@@ -201,23 +153,14 @@
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
 
-CrossRegionCopyDeprecateRuleOutputTypeDef = TypedDict(
-    "CrossRegionCopyDeprecateRuleOutputTypeDef",
-    {
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
 CrossRegionCopyDeprecateRuleTypeDef = TypedDict(
     "CrossRegionCopyDeprecateRuleTypeDef",
     {
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
@@ -226,24 +169,14 @@
 DeleteLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "DeleteLifecyclePolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
-DeprecateRuleOutputTypeDef = TypedDict(
-    "DeprecateRuleOutputTypeDef",
-    {
-        "Count": int,
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
 DeprecateRuleTypeDef = TypedDict(
     "DeprecateRuleTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
@@ -346,59 +279,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
-RetainRuleOutputTypeDef = TypedDict(
-    "RetainRuleOutputTypeDef",
-    {
-        "Count": int,
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
 RetainRuleTypeDef = TypedDict(
     "RetainRuleTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
@@ -457,50 +353,37 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ArchiveRetainRuleOutputTypeDef = TypedDict(
-    "ArchiveRetainRuleOutputTypeDef",
-    {
-        "RetentionArchiveTier": RetentionArchiveTierOutputTypeDef,
-    },
-)
-
 ArchiveRetainRuleTypeDef = TypedDict(
     "ArchiveRetainRuleTypeDef",
     {
         "RetentionArchiveTier": RetentionArchiveTierTypeDef,
     },
 )
 
-_RequiredCrossRegionCopyActionOutputTypeDef = TypedDict(
-    "_RequiredCrossRegionCopyActionOutputTypeDef",
+CreateLifecyclePolicyResponseTypeDef = TypedDict(
+    "CreateLifecyclePolicyResponseTypeDef",
     {
-        "Target": str,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "PolicyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCrossRegionCopyActionOutputTypeDef = TypedDict(
-    "_OptionalCrossRegionCopyActionOutputTypeDef",
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "RetainRule": CrossRegionCopyRetainRuleOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CrossRegionCopyActionOutputTypeDef(
-    _RequiredCrossRegionCopyActionOutputTypeDef, _OptionalCrossRegionCopyActionOutputTypeDef
-):
-    pass
-
-
 _RequiredCrossRegionCopyActionTypeDef = TypedDict(
     "_RequiredCrossRegionCopyActionTypeDef",
     {
         "Target": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
@@ -515,40 +398,14 @@
 
 class CrossRegionCopyActionTypeDef(
     _RequiredCrossRegionCopyActionTypeDef, _OptionalCrossRegionCopyActionTypeDef
 ):
     pass
 
 
-_RequiredCrossRegionCopyRuleOutputTypeDef = TypedDict(
-    "_RequiredCrossRegionCopyRuleOutputTypeDef",
-    {
-        "Encrypted": bool,
-    },
-)
-_OptionalCrossRegionCopyRuleOutputTypeDef = TypedDict(
-    "_OptionalCrossRegionCopyRuleOutputTypeDef",
-    {
-        "TargetRegion": str,
-        "Target": str,
-        "CmkArn": str,
-        "CopyTags": bool,
-        "RetainRule": CrossRegionCopyRetainRuleOutputTypeDef,
-        "DeprecateRule": CrossRegionCopyDeprecateRuleOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CrossRegionCopyRuleOutputTypeDef(
-    _RequiredCrossRegionCopyRuleOutputTypeDef, _OptionalCrossRegionCopyRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredCrossRegionCopyRuleTypeDef = TypedDict(
     "_RequiredCrossRegionCopyRuleTypeDef",
     {
         "Encrypted": bool,
     },
 )
 _OptionalCrossRegionCopyRuleTypeDef = TypedDict(
@@ -611,57 +468,50 @@
     pass
 
 
 GetLifecyclePoliciesResponseTypeDef = TypedDict(
     "GetLifecyclePoliciesResponseTypeDef",
     {
         "Policies": List[LifecyclePolicySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParametersOutputTypeDef = TypedDict(
     "ParametersOutputTypeDef",
     {
         "ExcludeBootVolume": bool,
         "NoReboot": bool,
-        "ExcludeDataVolumeTags": List[TagOutputTypeDef],
+        "ExcludeDataVolumeTags": List[TagTypeDef],
     },
     total=False,
 )
 
 ParametersTypeDef = TypedDict(
     "ParametersTypeDef",
     {
         "ExcludeBootVolume": bool,
         "NoReboot": bool,
         "ExcludeDataVolumeTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-ArchiveRuleOutputTypeDef = TypedDict(
-    "ArchiveRuleOutputTypeDef",
-    {
-        "RetainRule": ArchiveRetainRuleOutputTypeDef,
-    },
-)
-
 ArchiveRuleTypeDef = TypedDict(
     "ArchiveRuleTypeDef",
     {
         "RetainRule": ArchiveRetainRuleTypeDef,
     },
 )
 
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
         "Name": str,
-        "CrossRegionCopy": List[CrossRegionCopyActionOutputTypeDef],
+        "CrossRegionCopy": List[CrossRegionCopyActionTypeDef],
     },
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "Name": str,
@@ -670,23 +520,23 @@
 )
 
 ScheduleOutputTypeDef = TypedDict(
     "ScheduleOutputTypeDef",
     {
         "Name": str,
         "CopyTags": bool,
-        "TagsToAdd": List[TagOutputTypeDef],
-        "VariableTags": List[TagOutputTypeDef],
+        "TagsToAdd": List[TagTypeDef],
+        "VariableTags": List[TagTypeDef],
         "CreateRule": CreateRuleOutputTypeDef,
-        "RetainRule": RetainRuleOutputTypeDef,
+        "RetainRule": RetainRuleTypeDef,
         "FastRestoreRule": FastRestoreRuleOutputTypeDef,
-        "CrossRegionCopyRules": List[CrossRegionCopyRuleOutputTypeDef],
+        "CrossRegionCopyRules": List[CrossRegionCopyRuleTypeDef],
         "ShareRules": List[ShareRuleOutputTypeDef],
-        "DeprecateRule": DeprecateRuleOutputTypeDef,
-        "ArchiveRule": ArchiveRuleOutputTypeDef,
+        "DeprecateRule": DeprecateRuleTypeDef,
+        "ArchiveRule": ArchiveRuleTypeDef,
     },
     total=False,
 )
 
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
@@ -707,15 +557,15 @@
 
 PolicyDetailsOutputTypeDef = TypedDict(
     "PolicyDetailsOutputTypeDef",
     {
         "PolicyType": PolicyTypeValuesType,
         "ResourceTypes": List[ResourceTypeValuesType],
         "ResourceLocations": List[ResourceLocationValuesType],
-        "TargetTags": List[TagOutputTypeDef],
+        "TargetTags": List[TagTypeDef],
         "Schedules": List[ScheduleOutputTypeDef],
         "Parameters": ParametersOutputTypeDef,
         "EventSource": EventSourceOutputTypeDef,
         "Actions": List[ActionOutputTypeDef],
     },
     total=False,
 )
@@ -802,10 +652,10 @@
     pass
 
 
 GetLifecyclePolicyResponseTypeDef = TypedDict(
     "GetLifecyclePolicyResponseTypeDef",
     {
         "Policy": LifecyclePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm/type_defs.pyi` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for dlm service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_dlm.type_defs import RetentionArchiveTierOutputTypeDef
+    from mypy_boto3_dlm.type_defs import RetentionArchiveTierTypeDef
 
-    data: RetentionArchiveTierOutputTypeDef = {...}
+    data: RetentionArchiveTierTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -31,96 +31,78 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "RetentionArchiveTierOutputTypeDef",
     "RetentionArchiveTierTypeDef",
-    "CreateLifecyclePolicyResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateRuleOutputTypeDef",
     "CreateRuleTypeDef",
-    "CrossRegionCopyRetainRuleOutputTypeDef",
-    "EncryptionConfigurationOutputTypeDef",
     "CrossRegionCopyRetainRuleTypeDef",
     "EncryptionConfigurationTypeDef",
-    "CrossRegionCopyDeprecateRuleOutputTypeDef",
     "CrossRegionCopyDeprecateRuleTypeDef",
     "DeleteLifecyclePolicyRequestRequestTypeDef",
-    "DeprecateRuleOutputTypeDef",
     "DeprecateRuleTypeDef",
     "EventParametersOutputTypeDef",
     "EventParametersTypeDef",
     "FastRestoreRuleOutputTypeDef",
     "FastRestoreRuleTypeDef",
     "GetLifecyclePoliciesRequestRequestTypeDef",
     "LifecyclePolicySummaryTypeDef",
     "GetLifecyclePolicyRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "TagOutputTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
-    "RetainRuleOutputTypeDef",
     "RetainRuleTypeDef",
     "ShareRuleOutputTypeDef",
     "ShareRuleTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "ArchiveRetainRuleOutputTypeDef",
     "ArchiveRetainRuleTypeDef",
-    "CrossRegionCopyActionOutputTypeDef",
+    "CreateLifecyclePolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CrossRegionCopyActionTypeDef",
-    "CrossRegionCopyRuleOutputTypeDef",
     "CrossRegionCopyRuleTypeDef",
     "EventSourceOutputTypeDef",
     "EventSourceTypeDef",
     "GetLifecyclePoliciesResponseTypeDef",
     "ParametersOutputTypeDef",
     "ParametersTypeDef",
-    "ArchiveRuleOutputTypeDef",
     "ArchiveRuleTypeDef",
     "ActionOutputTypeDef",
     "ActionTypeDef",
     "ScheduleOutputTypeDef",
     "ScheduleTypeDef",
     "PolicyDetailsOutputTypeDef",
     "PolicyDetailsTypeDef",
     "LifecyclePolicyTypeDef",
     "CreateLifecyclePolicyRequestRequestTypeDef",
     "UpdateLifecyclePolicyRequestRequestTypeDef",
     "GetLifecyclePolicyResponseTypeDef",
 )
 
-RetentionArchiveTierOutputTypeDef = TypedDict(
-    "RetentionArchiveTierOutputTypeDef",
-    {
-        "Count": int,
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
 RetentionArchiveTierTypeDef = TypedDict(
     "RetentionArchiveTierTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
 )
 
-CreateLifecyclePolicyResponseTypeDef = TypedDict(
-    "CreateLifecyclePolicyResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "PolicyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateRuleOutputTypeDef = TypedDict(
     "CreateRuleOutputTypeDef",
     {
         "Location": LocationValuesType,
@@ -140,42 +122,14 @@
         "IntervalUnit": Literal["HOURS"],
         "Times": Sequence[str],
         "CronExpression": str,
     },
     total=False,
 )
 
-CrossRegionCopyRetainRuleOutputTypeDef = TypedDict(
-    "CrossRegionCopyRetainRuleOutputTypeDef",
-    {
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
-_RequiredEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEncryptionConfigurationOutputTypeDef",
-    {
-        "Encrypted": bool,
-    },
-)
-_OptionalEncryptionConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEncryptionConfigurationOutputTypeDef",
-    {
-        "CmkArn": str,
-    },
-    total=False,
-)
-
-class EncryptionConfigurationOutputTypeDef(
-    _RequiredEncryptionConfigurationOutputTypeDef, _OptionalEncryptionConfigurationOutputTypeDef
-):
-    pass
-
 CrossRegionCopyRetainRuleTypeDef = TypedDict(
     "CrossRegionCopyRetainRuleTypeDef",
     {
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
@@ -196,23 +150,14 @@
 )
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
-CrossRegionCopyDeprecateRuleOutputTypeDef = TypedDict(
-    "CrossRegionCopyDeprecateRuleOutputTypeDef",
-    {
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
 CrossRegionCopyDeprecateRuleTypeDef = TypedDict(
     "CrossRegionCopyDeprecateRuleTypeDef",
     {
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
     total=False,
@@ -221,24 +166,14 @@
 DeleteLifecyclePolicyRequestRequestTypeDef = TypedDict(
     "DeleteLifecyclePolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
-DeprecateRuleOutputTypeDef = TypedDict(
-    "DeprecateRuleOutputTypeDef",
-    {
-        "Count": int,
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
 DeprecateRuleTypeDef = TypedDict(
     "DeprecateRuleTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
@@ -337,59 +272,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
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
-RetainRuleOutputTypeDef = TypedDict(
-    "RetainRuleOutputTypeDef",
-    {
-        "Count": int,
-        "Interval": int,
-        "IntervalUnit": RetentionIntervalUnitValuesType,
-    },
-    total=False,
-)
-
 RetainRuleTypeDef = TypedDict(
     "RetainRuleTypeDef",
     {
         "Count": int,
         "Interval": int,
         "IntervalUnit": RetentionIntervalUnitValuesType,
     },
@@ -444,48 +342,37 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-ArchiveRetainRuleOutputTypeDef = TypedDict(
-    "ArchiveRetainRuleOutputTypeDef",
-    {
-        "RetentionArchiveTier": RetentionArchiveTierOutputTypeDef,
-    },
-)
-
 ArchiveRetainRuleTypeDef = TypedDict(
     "ArchiveRetainRuleTypeDef",
     {
         "RetentionArchiveTier": RetentionArchiveTierTypeDef,
     },
 )
 
-_RequiredCrossRegionCopyActionOutputTypeDef = TypedDict(
-    "_RequiredCrossRegionCopyActionOutputTypeDef",
+CreateLifecyclePolicyResponseTypeDef = TypedDict(
+    "CreateLifecyclePolicyResponseTypeDef",
     {
-        "Target": str,
-        "EncryptionConfiguration": EncryptionConfigurationOutputTypeDef,
+        "PolicyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCrossRegionCopyActionOutputTypeDef = TypedDict(
-    "_OptionalCrossRegionCopyActionOutputTypeDef",
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "RetainRule": CrossRegionCopyRetainRuleOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CrossRegionCopyActionOutputTypeDef(
-    _RequiredCrossRegionCopyActionOutputTypeDef, _OptionalCrossRegionCopyActionOutputTypeDef
-):
-    pass
-
 _RequiredCrossRegionCopyActionTypeDef = TypedDict(
     "_RequiredCrossRegionCopyActionTypeDef",
     {
         "Target": str,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
 )
@@ -498,38 +385,14 @@
 )
 
 class CrossRegionCopyActionTypeDef(
     _RequiredCrossRegionCopyActionTypeDef, _OptionalCrossRegionCopyActionTypeDef
 ):
     pass
 
-_RequiredCrossRegionCopyRuleOutputTypeDef = TypedDict(
-    "_RequiredCrossRegionCopyRuleOutputTypeDef",
-    {
-        "Encrypted": bool,
-    },
-)
-_OptionalCrossRegionCopyRuleOutputTypeDef = TypedDict(
-    "_OptionalCrossRegionCopyRuleOutputTypeDef",
-    {
-        "TargetRegion": str,
-        "Target": str,
-        "CmkArn": str,
-        "CopyTags": bool,
-        "RetainRule": CrossRegionCopyRetainRuleOutputTypeDef,
-        "DeprecateRule": CrossRegionCopyDeprecateRuleOutputTypeDef,
-    },
-    total=False,
-)
-
-class CrossRegionCopyRuleOutputTypeDef(
-    _RequiredCrossRegionCopyRuleOutputTypeDef, _OptionalCrossRegionCopyRuleOutputTypeDef
-):
-    pass
-
 _RequiredCrossRegionCopyRuleTypeDef = TypedDict(
     "_RequiredCrossRegionCopyRuleTypeDef",
     {
         "Encrypted": bool,
     },
 )
 _OptionalCrossRegionCopyRuleTypeDef = TypedDict(
@@ -586,57 +449,50 @@
 class EventSourceTypeDef(_RequiredEventSourceTypeDef, _OptionalEventSourceTypeDef):
     pass
 
 GetLifecyclePoliciesResponseTypeDef = TypedDict(
     "GetLifecyclePoliciesResponseTypeDef",
     {
         "Policies": List[LifecyclePolicySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ParametersOutputTypeDef = TypedDict(
     "ParametersOutputTypeDef",
     {
         "ExcludeBootVolume": bool,
         "NoReboot": bool,
-        "ExcludeDataVolumeTags": List[TagOutputTypeDef],
+        "ExcludeDataVolumeTags": List[TagTypeDef],
     },
     total=False,
 )
 
 ParametersTypeDef = TypedDict(
     "ParametersTypeDef",
     {
         "ExcludeBootVolume": bool,
         "NoReboot": bool,
         "ExcludeDataVolumeTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-ArchiveRuleOutputTypeDef = TypedDict(
-    "ArchiveRuleOutputTypeDef",
-    {
-        "RetainRule": ArchiveRetainRuleOutputTypeDef,
-    },
-)
-
 ArchiveRuleTypeDef = TypedDict(
     "ArchiveRuleTypeDef",
     {
         "RetainRule": ArchiveRetainRuleTypeDef,
     },
 )
 
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
         "Name": str,
-        "CrossRegionCopy": List[CrossRegionCopyActionOutputTypeDef],
+        "CrossRegionCopy": List[CrossRegionCopyActionTypeDef],
     },
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "Name": str,
@@ -645,23 +501,23 @@
 )
 
 ScheduleOutputTypeDef = TypedDict(
     "ScheduleOutputTypeDef",
     {
         "Name": str,
         "CopyTags": bool,
-        "TagsToAdd": List[TagOutputTypeDef],
-        "VariableTags": List[TagOutputTypeDef],
+        "TagsToAdd": List[TagTypeDef],
+        "VariableTags": List[TagTypeDef],
         "CreateRule": CreateRuleOutputTypeDef,
-        "RetainRule": RetainRuleOutputTypeDef,
+        "RetainRule": RetainRuleTypeDef,
         "FastRestoreRule": FastRestoreRuleOutputTypeDef,
-        "CrossRegionCopyRules": List[CrossRegionCopyRuleOutputTypeDef],
+        "CrossRegionCopyRules": List[CrossRegionCopyRuleTypeDef],
         "ShareRules": List[ShareRuleOutputTypeDef],
-        "DeprecateRule": DeprecateRuleOutputTypeDef,
-        "ArchiveRule": ArchiveRuleOutputTypeDef,
+        "DeprecateRule": DeprecateRuleTypeDef,
+        "ArchiveRule": ArchiveRuleTypeDef,
     },
     total=False,
 )
 
 ScheduleTypeDef = TypedDict(
     "ScheduleTypeDef",
     {
@@ -682,15 +538,15 @@
 
 PolicyDetailsOutputTypeDef = TypedDict(
     "PolicyDetailsOutputTypeDef",
     {
         "PolicyType": PolicyTypeValuesType,
         "ResourceTypes": List[ResourceTypeValuesType],
         "ResourceLocations": List[ResourceLocationValuesType],
-        "TargetTags": List[TagOutputTypeDef],
+        "TargetTags": List[TagTypeDef],
         "Schedules": List[ScheduleOutputTypeDef],
         "Parameters": ParametersOutputTypeDef,
         "EventSource": EventSourceOutputTypeDef,
         "Actions": List[ActionOutputTypeDef],
     },
     total=False,
 )
@@ -773,10 +629,10 @@
 ):
     pass
 
 GetLifecyclePolicyResponseTypeDef = TypedDict(
     "GetLifecyclePolicyResponseTypeDef",
     {
         "Policy": LifecyclePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/PKG-INFO` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-dlm
-Version: 1.28.12
-Summary: Type annotations for boto3.DLM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-dlm.svg?color=blue)](https://pypi.org/project/mypy-boto3-dlm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-dlm)](https://pepy.tech/project/mypy-boto3-dlm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DLM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
+[boto3.DLM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dlm.html#DLM)
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
 [mypy-boto3-dlm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_dlm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -305,73 +305,62 @@
 ### Typed dictionaries
 
 `mypy_boto3_dlm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_dlm.type_defs import (
-    RetentionArchiveTierOutputTypeDef,
     RetentionArchiveTierTypeDef,
-    CreateLifecyclePolicyResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRuleOutputTypeDef,
     CreateRuleTypeDef,
-    CrossRegionCopyRetainRuleOutputTypeDef,
-    EncryptionConfigurationOutputTypeDef,
     CrossRegionCopyRetainRuleTypeDef,
     EncryptionConfigurationTypeDef,
-    CrossRegionCopyDeprecateRuleOutputTypeDef,
     CrossRegionCopyDeprecateRuleTypeDef,
     DeleteLifecyclePolicyRequestRequestTypeDef,
-    DeprecateRuleOutputTypeDef,
     DeprecateRuleTypeDef,
     EventParametersOutputTypeDef,
     EventParametersTypeDef,
     FastRestoreRuleOutputTypeDef,
     FastRestoreRuleTypeDef,
     GetLifecyclePoliciesRequestRequestTypeDef,
     LifecyclePolicySummaryTypeDef,
     GetLifecyclePolicyRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
-    RetainRuleOutputTypeDef,
     RetainRuleTypeDef,
     ShareRuleOutputTypeDef,
     ShareRuleTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    ArchiveRetainRuleOutputTypeDef,
     ArchiveRetainRuleTypeDef,
-    CrossRegionCopyActionOutputTypeDef,
+    CreateLifecyclePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CrossRegionCopyActionTypeDef,
-    CrossRegionCopyRuleOutputTypeDef,
     CrossRegionCopyRuleTypeDef,
     EventSourceOutputTypeDef,
     EventSourceTypeDef,
     GetLifecyclePoliciesResponseTypeDef,
     ParametersOutputTypeDef,
     ParametersTypeDef,
-    ArchiveRuleOutputTypeDef,
     ArchiveRuleTypeDef,
     ActionOutputTypeDef,
     ActionTypeDef,
     ScheduleOutputTypeDef,
     ScheduleTypeDef,
     PolicyDetailsOutputTypeDef,
     PolicyDetailsTypeDef,
     LifecyclePolicyTypeDef,
     CreateLifecyclePolicyRequestRequestTypeDef,
     UpdateLifecyclePolicyRequestRequestTypeDef,
     GetLifecyclePolicyResponseTypeDef,
 )
 
 
-def get_structure() -> RetentionArchiveTierOutputTypeDef:
+def get_structure() -> RetentionArchiveTierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-dlm-1.28.12/mypy_boto3_dlm.egg-info/SOURCES.txt` & `mypy-boto3-dlm-1.28.15/mypy_boto3_dlm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-dlm-1.28.12/setup.py` & `mypy-boto3-dlm-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-dlm",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_dlm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DLM 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.DLM 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

