# Comparing `tmp/mypy-boto3-iotsecuretunneling-1.28.12.tar.gz` & `tmp/mypy-boto3-iotsecuretunneling-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iotsecuretunneling-1.28.12.tar", last modified: Thu Jul 27 05:34:50 2023, max compression
+gzip compressed data, was "mypy-boto3-iotsecuretunneling-1.28.15.tar", last modified: Fri Jul 28 20:43:01 2023, max compression
```

## Comparing `mypy-boto3-iotsecuretunneling-1.28.12.tar` & `mypy-boto3-iotsecuretunneling-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.492479 mypy-boto3-iotsecuretunneling-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-07-27 05:34:50.488479 mypy-boto3-iotsecuretunneling-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11659 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.484479 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:24:09.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:50.488479 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13190 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-27 05:34:50.000000 mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:50.492479 mypy-boto3-iotsecuretunneling-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-27 05:24:08.000000 mypy-boto3-iotsecuretunneling-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.525285 mypy-boto3-iotsecuretunneling-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-07-28 20:43:01.517285 mypy-boto3-iotsecuretunneling-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.517285 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7975 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8282 2023-07-28 20:28:32.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-28 20:28:32.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-07-28 20:28:32.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:01.517285 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13136 2023-07-28 20:43:01.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-28 20:43:01.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:01.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:01.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:01.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-28 20:43:01.000000 mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:01.525285 mypy-boto3-iotsecuretunneling-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-28 20:28:31.000000 mypy-boto3-iotsecuretunneling-1.28.15/setup.py
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/LICENSE` & `mypy-boto3-iotsecuretunneling-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/PKG-INFO` & `mypy-boto3-iotsecuretunneling-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsecuretunneling
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTSecureTunneling 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTSecureTunneling 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,31 +303,29 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
-    TagTypeDef,
     TimeoutConfigTypeDef,
+    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
-    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
-    TimeoutConfigOutputTypeDef,
-    UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListTunnelsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
 def get_structure() -> CloseTunnelRequestRequestTypeDef:
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/README.md` & `mypy-boto3-iotsecuretunneling-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,31 +271,29 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
-    TagTypeDef,
     TimeoutConfigTypeDef,
+    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
-    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
-    TimeoutConfigOutputTypeDef,
-    UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListTunnelsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
 def get_structure() -> CloseTunnelRequestRequestTypeDef:
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/__main__.py` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoTSecureTunneling 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoTSecureTunneling 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling\nOther"
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

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/client.py` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/client.pyi` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/literals.py` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/literals.pyi` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/type_defs.py` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,31 +23,29 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
-    "TagTypeDef",
     "TimeoutConfigTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
-    "TimeoutConfigOutputTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ListTunnelsResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
 )
 
 _RequiredCloseTunnelRequestRequestTypeDef = TypedDict(
     "_RequiredCloseTunnelRequestRequestTypeDef",
@@ -82,14 +80,25 @@
 DescribeTunnelRequestRequestTypeDef = TypedDict(
     "DescribeTunnelRequestRequestTypeDef",
     {
         "tunnelId": str,
     },
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
 _RequiredDestinationConfigOutputTypeDef = TypedDict(
     "_RequiredDestinationConfigOutputTypeDef",
     {
         "services": List[str],
     },
 )
 _OptionalDestinationConfigOutputTypeDef = TypedDict(
@@ -131,16 +140,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 ListTunnelsRequestRequestTypeDef = TypedDict(
@@ -162,75 +171,48 @@
         "description": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 TimeoutConfigTypeDef = TypedDict(
     "TimeoutConfigTypeDef",
     {
         "maxLifetimeTimeoutMinutes": int,
     },
     total=False,
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
 OpenTunnelResponseTypeDef = TypedDict(
     "OpenTunnelResponseTypeDef",
     {
         "tunnelId": str,
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateTunnelAccessTokenResponseTypeDef = TypedDict(
     "RotateTunnelAccessTokenResponseTypeDef",
     {
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TimeoutConfigOutputTypeDef = TypedDict(
-    "TimeoutConfigOutputTypeDef",
-    {
-        "maxLifetimeTimeoutMinutes": int,
-    },
-    total=False,
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
@@ -252,36 +234,36 @@
 ):
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTunnelsResponseTypeDef = TypedDict(
-    "ListTunnelsResponseTypeDef",
-    {
-        "tunnelSummaries": List[TunnelSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+ListTunnelsResponseTypeDef = TypedDict(
+    "ListTunnelsResponseTypeDef",
+    {
+        "tunnelSummaries": List[TunnelSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 OpenTunnelRequestRequestTypeDef = TypedDict(
     "OpenTunnelRequestRequestTypeDef",
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
         "destinationConfig": DestinationConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
@@ -295,22 +277,22 @@
         "tunnelId": str,
         "tunnelArn": str,
         "status": TunnelStatusType,
         "sourceConnectionState": ConnectionStateTypeDef,
         "destinationConnectionState": ConnectionStateTypeDef,
         "description": str,
         "destinationConfig": DestinationConfigOutputTypeDef,
-        "timeoutConfig": TimeoutConfigOutputTypeDef,
-        "tags": List[TagOutputTypeDef],
+        "timeoutConfig": TimeoutConfigTypeDef,
+        "tags": List[TagTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
 DescribeTunnelResponseTypeDef = TypedDict(
     "DescribeTunnelResponseTypeDef",
     {
         "tunnel": TunnelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling/type_defs.pyi` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -22,31 +22,29 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
-    "TagTypeDef",
     "TimeoutConfigTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
-    "TimeoutConfigOutputTypeDef",
-    "UntagResourceRequestRequestTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "ListTunnelsResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
 )
 
 _RequiredCloseTunnelRequestRequestTypeDef = TypedDict(
     "_RequiredCloseTunnelRequestRequestTypeDef",
@@ -79,14 +77,25 @@
 DescribeTunnelRequestRequestTypeDef = TypedDict(
     "DescribeTunnelRequestRequestTypeDef",
     {
         "tunnelId": str,
     },
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
 _RequiredDestinationConfigOutputTypeDef = TypedDict(
     "_RequiredDestinationConfigOutputTypeDef",
     {
         "services": List[str],
     },
 )
 _OptionalDestinationConfigOutputTypeDef = TypedDict(
@@ -124,16 +133,16 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
 ListTunnelsRequestRequestTypeDef = TypedDict(
@@ -155,75 +164,48 @@
         "description": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 TimeoutConfigTypeDef = TypedDict(
     "TimeoutConfigTypeDef",
     {
         "maxLifetimeTimeoutMinutes": int,
     },
     total=False,
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
 OpenTunnelResponseTypeDef = TypedDict(
     "OpenTunnelResponseTypeDef",
     {
         "tunnelId": str,
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateTunnelAccessTokenResponseTypeDef = TypedDict(
     "RotateTunnelAccessTokenResponseTypeDef",
     {
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-TimeoutConfigOutputTypeDef = TypedDict(
-    "TimeoutConfigOutputTypeDef",
-    {
-        "maxLifetimeTimeoutMinutes": int,
-    },
-    total=False,
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
@@ -243,36 +225,36 @@
     _OptionalRotateTunnelAccessTokenRequestRequestTypeDef,
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTunnelsResponseTypeDef = TypedDict(
-    "ListTunnelsResponseTypeDef",
-    {
-        "tunnelSummaries": List[TunnelSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
+ListTunnelsResponseTypeDef = TypedDict(
+    "ListTunnelsResponseTypeDef",
+    {
+        "tunnelSummaries": List[TunnelSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 OpenTunnelRequestRequestTypeDef = TypedDict(
     "OpenTunnelRequestRequestTypeDef",
     {
         "description": str,
         "tags": Sequence[TagTypeDef],
         "destinationConfig": DestinationConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
@@ -286,22 +268,22 @@
         "tunnelId": str,
         "tunnelArn": str,
         "status": TunnelStatusType,
         "sourceConnectionState": ConnectionStateTypeDef,
         "destinationConnectionState": ConnectionStateTypeDef,
         "description": str,
         "destinationConfig": DestinationConfigOutputTypeDef,
-        "timeoutConfig": TimeoutConfigOutputTypeDef,
-        "tags": List[TagOutputTypeDef],
+        "timeoutConfig": TimeoutConfigTypeDef,
+        "tags": List[TagTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
 DescribeTunnelResponseTypeDef = TypedDict(
     "DescribeTunnelResponseTypeDef",
     {
         "tunnel": TunnelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iotsecuretunneling
-Version: 1.28.12
-Summary: Type annotations for boto3.IoTSecureTunneling 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoTSecureTunneling 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/mypy-boto3-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iotsecuretunneling)](https://pepy.tech/project/mypy-boto3-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoTSecureTunneling 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
+[boto3.IoTSecureTunneling 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [mypy-boto3-iotsecuretunneling docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,31 +303,29 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
-    TagTypeDef,
     TimeoutConfigTypeDef,
+    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
-    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
-    TimeoutConfigOutputTypeDef,
-    UntagResourceRequestRequestTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
-    ListTunnelsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
 def get_structure() -> CloseTunnelRequestRequestTypeDef:
```

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt` & `mypy-boto3-iotsecuretunneling-1.28.15/mypy_boto3_iotsecuretunneling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iotsecuretunneling-1.28.12/setup.py` & `mypy-boto3-iotsecuretunneling-1.28.15/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iotsecuretunneling",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iotsecuretunneling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoTSecureTunneling 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IoTSecureTunneling 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

