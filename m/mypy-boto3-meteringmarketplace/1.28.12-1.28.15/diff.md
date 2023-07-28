# Comparing `tmp/mypy-boto3-meteringmarketplace-1.28.12.tar.gz` & `tmp/mypy-boto3-meteringmarketplace-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-meteringmarketplace-1.28.12.tar", last modified: Thu Jul 27 05:35:02 2023, max compression
+gzip compressed data, was "mypy-boto3-meteringmarketplace-1.28.15.tar", last modified: Fri Jul 28 20:43:18 2023, max compression
```

## Comparing `mypy-boto3-meteringmarketplace-1.28.12.tar` & `mypy-boto3-meteringmarketplace-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.704435 mypy-boto3-meteringmarketplace-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-27 05:35:02.700435 mypy-boto3-meteringmarketplace-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.696435 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:35:02.700435 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12939 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-27 05:35:02.000000 mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:35:02.704435 mypy-boto3-meteringmarketplace-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-27 05:26:33.000000 mypy-boto3-meteringmarketplace-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.353516 mypy-boto3-meteringmarketplace-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-07-28 20:43:18.349516 mypy-boto3-meteringmarketplace-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11382 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.337516 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:18.349516 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12917 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-28 20:43:18.000000 mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:18.353516 mypy-boto3-meteringmarketplace-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-28 20:31:52.000000 mypy-boto3-meteringmarketplace-1.28.15/setup.py
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/LICENSE` & `mypy-boto3-meteringmarketplace-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.28.12
-Summary: Type annotations for boto3.MarketplaceMetering 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,34 +298,33 @@
 ### Typed dictionaries
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
-    MeterUsageResultTypeDef,
+    ResponseMetadataTypeDef,
     RegisterUsageRequestRequestTypeDef,
-    RegisterUsageResultTypeDef,
     ResolveCustomerRequestRequestTypeDef,
-    ResolveCustomerResultTypeDef,
-    ResponseMetadataTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
+    MeterUsageResultTypeDef,
+    RegisterUsageResultTypeDef,
+    ResolveCustomerResultTypeDef,
     UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
     UsageRecordOutputTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
     UsageRecordResultTypeDef,
     BatchMeterUsageRequestRequestTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
-def get_structure() -> MeterUsageResultTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/README.md` & `mypy-boto3-meteringmarketplace-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,34 +266,33 @@
 ### Typed dictionaries
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
-    MeterUsageResultTypeDef,
+    ResponseMetadataTypeDef,
     RegisterUsageRequestRequestTypeDef,
-    RegisterUsageResultTypeDef,
     ResolveCustomerRequestRequestTypeDef,
-    ResolveCustomerResultTypeDef,
-    ResponseMetadataTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
+    MeterUsageResultTypeDef,
+    RegisterUsageResultTypeDef,
+    ResolveCustomerResultTypeDef,
     UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
     UsageRecordOutputTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
     UsageRecordResultTypeDef,
     BatchMeterUsageRequestRequestTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
-def get_structure() -> MeterUsageResultTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/__main__.py` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MarketplaceMetering 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.MarketplaceMetering 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering\nOther"
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

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/client.py` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/client.pyi` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/literals.py` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/literals.pyi` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/type_defs.py` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for meteringmarketplace service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_meteringmarketplace.type_defs import MeterUsageResultTypeDef
+    from mypy_boto3_meteringmarketplace.type_defs import ResponseMetadataTypeDef
 
-    data: MeterUsageResultTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import UsageRecordResultStatusType
@@ -20,37 +20,39 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "MeterUsageResultTypeDef",
+    "ResponseMetadataTypeDef",
     "RegisterUsageRequestRequestTypeDef",
-    "RegisterUsageResultTypeDef",
     "ResolveCustomerRequestRequestTypeDef",
-    "ResolveCustomerResultTypeDef",
-    "ResponseMetadataTypeDef",
-    "TagOutputTypeDef",
     "TagTypeDef",
+    "MeterUsageResultTypeDef",
+    "RegisterUsageResultTypeDef",
+    "ResolveCustomerResultTypeDef",
     "UsageAllocationOutputTypeDef",
     "UsageAllocationTypeDef",
     "UsageRecordOutputTypeDef",
     "MeterUsageRequestRequestTypeDef",
     "UsageRecordTypeDef",
     "UsageRecordResultTypeDef",
     "BatchMeterUsageRequestRequestTypeDef",
     "BatchMeterUsageResultTypeDef",
 )
 
-MeterUsageResultTypeDef = TypedDict(
-    "MeterUsageResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "MeteringRecordId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredRegisterUsageRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterUsageRequestRequestTypeDef",
     {
         "ProductCode": str,
@@ -68,77 +70,66 @@
 
 class RegisterUsageRequestRequestTypeDef(
     _RequiredRegisterUsageRequestRequestTypeDef, _OptionalRegisterUsageRequestRequestTypeDef
 ):
     pass
 
 
-RegisterUsageResultTypeDef = TypedDict(
-    "RegisterUsageResultTypeDef",
-    {
-        "PublicKeyRotationTimestamp": datetime,
-        "Signature": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResolveCustomerRequestRequestTypeDef = TypedDict(
     "ResolveCustomerRequestRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
-ResolveCustomerResultTypeDef = TypedDict(
-    "ResolveCustomerResultTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "CustomerIdentifier": str,
-        "ProductCode": str,
-        "CustomerAWSAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+MeterUsageResultTypeDef = TypedDict(
+    "MeterUsageResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MeteringRecordId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+RegisterUsageResultTypeDef = TypedDict(
+    "RegisterUsageResultTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "PublicKeyRotationTimestamp": datetime,
+        "Signature": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ResolveCustomerResultTypeDef = TypedDict(
+    "ResolveCustomerResultTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "CustomerIdentifier": str,
+        "ProductCode": str,
+        "CustomerAWSAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUsageAllocationOutputTypeDef = TypedDict(
     "_RequiredUsageAllocationOutputTypeDef",
     {
         "AllocatedUsageQuantity": int,
     },
 )
 _OptionalUsageAllocationOutputTypeDef = TypedDict(
     "_OptionalUsageAllocationOutputTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 
 class UsageAllocationOutputTypeDef(
     _RequiredUsageAllocationOutputTypeDef, _OptionalUsageAllocationOutputTypeDef
@@ -255,10 +246,10 @@
 )
 
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
         "UnprocessedRecords": List[UsageRecordOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace/type_defs.pyi` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,54 +2,56 @@
 Type annotations for meteringmarketplace service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_meteringmarketplace.type_defs import MeterUsageResultTypeDef
+    from mypy_boto3_meteringmarketplace.type_defs import ResponseMetadataTypeDef
 
-    data: MeterUsageResultTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import UsageRecordResultStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "MeterUsageResultTypeDef",
+    "ResponseMetadataTypeDef",
     "RegisterUsageRequestRequestTypeDef",
-    "RegisterUsageResultTypeDef",
     "ResolveCustomerRequestRequestTypeDef",
-    "ResolveCustomerResultTypeDef",
-    "ResponseMetadataTypeDef",
-    "TagOutputTypeDef",
     "TagTypeDef",
+    "MeterUsageResultTypeDef",
+    "RegisterUsageResultTypeDef",
+    "ResolveCustomerResultTypeDef",
     "UsageAllocationOutputTypeDef",
     "UsageAllocationTypeDef",
     "UsageRecordOutputTypeDef",
     "MeterUsageRequestRequestTypeDef",
     "UsageRecordTypeDef",
     "UsageRecordResultTypeDef",
     "BatchMeterUsageRequestRequestTypeDef",
     "BatchMeterUsageResultTypeDef",
 )
 
-MeterUsageResultTypeDef = TypedDict(
-    "MeterUsageResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "MeteringRecordId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredRegisterUsageRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterUsageRequestRequestTypeDef",
     {
         "ProductCode": str,
@@ -65,77 +67,66 @@
 )
 
 class RegisterUsageRequestRequestTypeDef(
     _RequiredRegisterUsageRequestRequestTypeDef, _OptionalRegisterUsageRequestRequestTypeDef
 ):
     pass
 
-RegisterUsageResultTypeDef = TypedDict(
-    "RegisterUsageResultTypeDef",
-    {
-        "PublicKeyRotationTimestamp": datetime,
-        "Signature": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ResolveCustomerRequestRequestTypeDef = TypedDict(
     "ResolveCustomerRequestRequestTypeDef",
     {
         "RegistrationToken": str,
     },
 )
 
-ResolveCustomerResultTypeDef = TypedDict(
-    "ResolveCustomerResultTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
-        "CustomerIdentifier": str,
-        "ProductCode": str,
-        "CustomerAWSAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Key": str,
+        "Value": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+MeterUsageResultTypeDef = TypedDict(
+    "MeterUsageResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "MeteringRecordId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+RegisterUsageResultTypeDef = TypedDict(
+    "RegisterUsageResultTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "PublicKeyRotationTimestamp": datetime,
+        "Signature": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
+ResolveCustomerResultTypeDef = TypedDict(
+    "ResolveCustomerResultTypeDef",
     {
-        "Key": str,
-        "Value": str,
+        "CustomerIdentifier": str,
+        "ProductCode": str,
+        "CustomerAWSAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUsageAllocationOutputTypeDef = TypedDict(
     "_RequiredUsageAllocationOutputTypeDef",
     {
         "AllocatedUsageQuantity": int,
     },
 )
 _OptionalUsageAllocationOutputTypeDef = TypedDict(
     "_OptionalUsageAllocationOutputTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 class UsageAllocationOutputTypeDef(
     _RequiredUsageAllocationOutputTypeDef, _OptionalUsageAllocationOutputTypeDef
 ):
@@ -242,10 +233,10 @@
 )
 
 BatchMeterUsageResultTypeDef = TypedDict(
     "BatchMeterUsageResultTypeDef",
     {
         "Results": List[UsageRecordResultTypeDef],
         "UnprocessedRecords": List[UsageRecordOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-meteringmarketplace
-Version: 1.28.12
-Summary: Type annotations for boto3.MarketplaceMetering 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-meteringmarketplace.svg?color=blue)](https://pypi.org/project/mypy-boto3-meteringmarketplace)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-meteringmarketplace)](https://pepy.tech/project/mypy-boto3-meteringmarketplace)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MarketplaceMetering 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
+[boto3.MarketplaceMetering 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/meteringmarketplace.html#MarketplaceMetering)
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
 [mypy-boto3-meteringmarketplace docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_meteringmarketplace/).
 
 See how it helps to find and fix potential bugs:
 
@@ -298,34 +298,33 @@
 ### Typed dictionaries
 
 `mypy_boto3_meteringmarketplace.type_defs` module contains structures and
 shapes assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_meteringmarketplace.type_defs import (
-    MeterUsageResultTypeDef,
+    ResponseMetadataTypeDef,
     RegisterUsageRequestRequestTypeDef,
-    RegisterUsageResultTypeDef,
     ResolveCustomerRequestRequestTypeDef,
-    ResolveCustomerResultTypeDef,
-    ResponseMetadataTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
+    MeterUsageResultTypeDef,
+    RegisterUsageResultTypeDef,
+    ResolveCustomerResultTypeDef,
     UsageAllocationOutputTypeDef,
     UsageAllocationTypeDef,
     UsageRecordOutputTypeDef,
     MeterUsageRequestRequestTypeDef,
     UsageRecordTypeDef,
     UsageRecordResultTypeDef,
     BatchMeterUsageRequestRequestTypeDef,
     BatchMeterUsageResultTypeDef,
 )
 
 
-def get_structure() -> MeterUsageResultTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt` & `mypy-boto3-meteringmarketplace-1.28.15/mypy_boto3_meteringmarketplace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-meteringmarketplace-1.28.12/setup.py` & `mypy-boto3-meteringmarketplace-1.28.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-meteringmarketplace",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_meteringmarketplace"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.MarketplaceMetering 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.MarketplaceMetering 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

