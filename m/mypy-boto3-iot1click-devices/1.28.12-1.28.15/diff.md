# Comparing `tmp/mypy-boto3-iot1click-devices-1.28.12.tar.gz` & `tmp/mypy-boto3-iot1click-devices-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot1click-devices-1.28.12.tar", last modified: Thu Jul 27 05:34:47 2023, max compression
+gzip compressed data, was "mypy-boto3-iot1click-devices-1.28.15.tar", last modified: Fri Jul 28 20:42:56 2023, max compression
```

## Comparing `mypy-boto3-iot1click-devices-1.28.12.tar` & `mypy-boto3-iot1click-devices-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.660489 mypy-boto3-iot1click-devices-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-27 05:34:47.660489 mypy-boto3-iot1click-devices-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12984 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.656489 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-27 05:23:56.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:55.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:47.660489 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14517 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:47.000000 mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:47.660489 mypy-boto3-iot1click-devices-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-27 05:23:54.000000 mypy-boto3-iot1click-devices-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.401215 mypy-boto3-iot1click-devices-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-28 20:42:56.397215 mypy-boto3-iot1click-devices-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12953 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.389215 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12625 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9702 2023-07-28 20:28:13.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:56.397215 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14486 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:56.000000 mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:56.401215 mypy-boto3-iot1click-devices-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-28 20:28:12.000000 mypy-boto3-iot1click-devices-1.28.15/setup.py
```

### Comparing `mypy-boto3-iot1click-devices-1.28.12/LICENSE` & `mypy-boto3-iot1click-devices-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.12/PKG-INFO` & `mypy-boto3-iot1click-devices-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-devices
-Version: 1.28.12
-Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,45 +322,44 @@
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
-    DeviceMethodOutputTypeDef,
     DeviceMethodTypeDef,
-    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
-    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iot1click-devices-1.28.12/README.md` & `mypy-boto3-iot1click-devices-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,45 +290,44 @@
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
-    DeviceMethodOutputTypeDef,
     DeviceMethodTypeDef,
-    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
-    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__init__.py` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__init__.pyi` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/__main__.py` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT1ClickDevicesService 1.28.12\nVersion:        "
-        " 1.28.12\nBuilder version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoT1ClickDevicesService 1.28.15\nVersion:        "
+        " 1.28.15\nBuilder version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService\nOther"
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

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/client.py` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/client.pyi` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/literals.py` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/literals.pyi` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/paginator.py` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,28 +53,28 @@
 
     def paginate(
         self,
         *,
         DeviceId: str,
         FromTimeStamp: Union[datetime, str],
         ToTimeStamp: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
 
 
 class ListDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, DeviceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeviceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdevicespaginator)
         """
```

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/paginator.pyi` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/paginator.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -50,27 +50,27 @@
 
     def paginate(
         self,
         *,
         DeviceId: str,
         FromTimeStamp: Union[datetime, str],
         ToTimeStamp: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDeviceEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDeviceEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdeviceeventspaginator)
         """
 
 class ListDevicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdevicespaginator)
     """
 
     def paginate(
-        self, *, DeviceType: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DeviceType: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService.Paginator.ListDevices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/paginators/#listdevicespaginator)
         """
```

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/type_defs.py` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,61 +19,62 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
-    "ClaimDevicesByClaimCodeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
-    "DeviceMethodOutputTypeDef",
     "DeviceMethodTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
-    "FinalizeDeviceClaimResponseTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
-    "InitiateDeviceClaimResponseTypeDef",
-    "InvokeDeviceMethodResponseTypeDef",
-    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeviceEventsRequestRequestTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnclaimDeviceRequestRequestTypeDef",
-    "UnclaimDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceStateRequestRequestTypeDef",
+    "ClaimDevicesByClaimCodeResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FinalizeDeviceClaimResponseTypeDef",
+    "InitiateDeviceClaimResponseTypeDef",
+    "InvokeDeviceMethodResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UnclaimDeviceResponseTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "DeviceEventTypeDef",
     "GetDeviceMethodsResponseTypeDef",
     "InvokeDeviceMethodRequestRequestTypeDef",
+    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDeviceEventsResponseTypeDef",
 )
 
 ClaimDevicesByClaimCodeRequestRequestTypeDef = TypedDict(
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     {
         "ClaimCode": str,
     },
 )
 
-ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
-    "ClaimDevicesByClaimCodeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ClaimCode": str,
-        "Total": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -100,39 +101,23 @@
         "Attributes": Dict[str, Any],
         "DeviceId": str,
         "Type": str,
     },
     total=False,
 )
 
-DeviceMethodOutputTypeDef = TypedDict(
-    "DeviceMethodOutputTypeDef",
-    {
-        "DeviceType": str,
-        "MethodName": str,
-    },
-    total=False,
-)
-
 DeviceMethodTypeDef = TypedDict(
     "DeviceMethodTypeDef",
     {
         "DeviceType": str,
         "MethodName": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
     "_RequiredFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 _OptionalFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
@@ -147,76 +132,38 @@
 class FinalizeDeviceClaimRequestRequestTypeDef(
     _RequiredFinalizeDeviceClaimRequestRequestTypeDef,
     _OptionalFinalizeDeviceClaimRequestRequestTypeDef,
 ):
     pass
 
 
-FinalizeDeviceClaimResponseTypeDef = TypedDict(
-    "FinalizeDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDeviceMethodsRequestRequestTypeDef = TypedDict(
     "GetDeviceMethodsRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
 InitiateDeviceClaimRequestRequestTypeDef = TypedDict(
     "InitiateDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-InitiateDeviceClaimResponseTypeDef = TypedDict(
-    "InitiateDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InvokeDeviceMethodResponseTypeDef = TypedDict(
-    "InvokeDeviceMethodResponseTypeDef",
-    {
-        "DeviceMethodResponse": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
-    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceEventsRequestRequestTypeDef",
     {
         "DeviceId": str,
         "FromTimeStamp": Union[datetime, str],
         "ToTimeStamp": Union[datetime, str],
     },
@@ -233,23 +180,14 @@
 
 class ListDeviceEventsRequestRequestTypeDef(
     _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
 ):
     pass
 
 
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "DeviceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "DeviceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -259,43 +197,14 @@
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
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
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
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -303,22 +212,14 @@
 UnclaimDeviceRequestRequestTypeDef = TypedDict(
     "UnclaimDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-UnclaimDeviceResponseTypeDef = TypedDict(
-    "UnclaimDeviceResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -340,28 +241,84 @@
 
 class UpdateDeviceStateRequestRequestTypeDef(
     _RequiredUpdateDeviceStateRequestRequestTypeDef, _OptionalUpdateDeviceStateRequestRequestTypeDef
 ):
     pass
 
 
+ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
+    "ClaimDevicesByClaimCodeResponseTypeDef",
+    {
+        "ClaimCode": str,
+        "Total": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FinalizeDeviceClaimResponseTypeDef = TypedDict(
+    "FinalizeDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateDeviceClaimResponseTypeDef = TypedDict(
+    "InitiateDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeDeviceMethodResponseTypeDef = TypedDict(
+    "InvokeDeviceMethodResponseTypeDef",
+    {
+        "DeviceMethodResponse": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnclaimDeviceResponseTypeDef = TypedDict(
+    "UnclaimDeviceResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceDescription": DeviceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceEventTypeDef = TypedDict(
     "DeviceEventTypeDef",
     {
         "Device": DeviceTypeDef,
@@ -369,16 +326,16 @@
     },
     total=False,
 )
 
 GetDeviceMethodsResponseTypeDef = TypedDict(
     "GetDeviceMethodsResponseTypeDef",
     {
-        "DeviceMethods": List[DeviceMethodOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeviceMethods": List[DeviceMethodTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInvokeDeviceMethodRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeDeviceMethodRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -397,15 +354,48 @@
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "FromTimeStamp": Union[datetime, str],
+        "ToTimeStamp": Union[datetime, str],
+    },
+)
+_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
+    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+):
+    pass
+
+
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "DeviceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices/type_defs.pyi` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices/type_defs.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -18,61 +18,62 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
-    "ClaimDevicesByClaimCodeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DescribeDeviceRequestRequestTypeDef",
     "DeviceDescriptionTypeDef",
     "DeviceTypeDef",
-    "DeviceMethodOutputTypeDef",
     "DeviceMethodTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FinalizeDeviceClaimRequestRequestTypeDef",
-    "FinalizeDeviceClaimResponseTypeDef",
     "GetDeviceMethodsRequestRequestTypeDef",
     "InitiateDeviceClaimRequestRequestTypeDef",
-    "InitiateDeviceClaimResponseTypeDef",
-    "InvokeDeviceMethodResponseTypeDef",
-    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDeviceEventsRequestRequestTypeDef",
-    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDevicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UnclaimDeviceRequestRequestTypeDef",
-    "UnclaimDeviceResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDeviceStateRequestRequestTypeDef",
+    "ClaimDevicesByClaimCodeResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FinalizeDeviceClaimResponseTypeDef",
+    "InitiateDeviceClaimResponseTypeDef",
+    "InvokeDeviceMethodResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UnclaimDeviceResponseTypeDef",
     "DescribeDeviceResponseTypeDef",
     "ListDevicesResponseTypeDef",
     "DeviceEventTypeDef",
     "GetDeviceMethodsResponseTypeDef",
     "InvokeDeviceMethodRequestRequestTypeDef",
+    "ListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    "ListDevicesRequestListDevicesPaginateTypeDef",
     "ListDeviceEventsResponseTypeDef",
 )
 
 ClaimDevicesByClaimCodeRequestRequestTypeDef = TypedDict(
     "ClaimDevicesByClaimCodeRequestRequestTypeDef",
     {
         "ClaimCode": str,
     },
 )
 
-ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
-    "ClaimDevicesByClaimCodeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ClaimCode": str,
-        "Total": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 DescribeDeviceRequestRequestTypeDef = TypedDict(
     "DescribeDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -99,39 +100,23 @@
         "Attributes": Dict[str, Any],
         "DeviceId": str,
         "Type": str,
     },
     total=False,
 )
 
-DeviceMethodOutputTypeDef = TypedDict(
-    "DeviceMethodOutputTypeDef",
-    {
-        "DeviceType": str,
-        "MethodName": str,
-    },
-    total=False,
-)
-
 DeviceMethodTypeDef = TypedDict(
     "DeviceMethodTypeDef",
     {
         "DeviceType": str,
         "MethodName": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
     "_RequiredFinalizeDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 _OptionalFinalizeDeviceClaimRequestRequestTypeDef = TypedDict(
@@ -144,74 +129,38 @@
 
 class FinalizeDeviceClaimRequestRequestTypeDef(
     _RequiredFinalizeDeviceClaimRequestRequestTypeDef,
     _OptionalFinalizeDeviceClaimRequestRequestTypeDef,
 ):
     pass
 
-FinalizeDeviceClaimResponseTypeDef = TypedDict(
-    "FinalizeDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDeviceMethodsRequestRequestTypeDef = TypedDict(
     "GetDeviceMethodsRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
 InitiateDeviceClaimRequestRequestTypeDef = TypedDict(
     "InitiateDeviceClaimRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-InitiateDeviceClaimResponseTypeDef = TypedDict(
-    "InitiateDeviceClaimResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-InvokeDeviceMethodResponseTypeDef = TypedDict(
-    "InvokeDeviceMethodResponseTypeDef",
-    {
-        "DeviceMethodResponse": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "FromTimeStamp": Union[datetime, str],
-        "ToTimeStamp": Union[datetime, str],
-    },
-)
-_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
-    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
-    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredListDeviceEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListDeviceEventsRequestRequestTypeDef",
     {
         "DeviceId": str,
         "FromTimeStamp": Union[datetime, str],
         "ToTimeStamp": Union[datetime, str],
     },
@@ -226,23 +175,14 @@
 )
 
 class ListDeviceEventsRequestRequestTypeDef(
     _RequiredListDeviceEventsRequestRequestTypeDef, _OptionalListDeviceEventsRequestRequestTypeDef
 ):
     pass
 
-ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
-    "ListDevicesRequestListDevicesPaginateTypeDef",
-    {
-        "DeviceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDevicesRequestRequestTypeDef = TypedDict(
     "ListDevicesRequestRequestTypeDef",
     {
         "DeviceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
@@ -252,43 +192,14 @@
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
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
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
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -296,22 +207,14 @@
 UnclaimDeviceRequestRequestTypeDef = TypedDict(
     "UnclaimDeviceRequestRequestTypeDef",
     {
         "DeviceId": str,
     },
 )
 
-UnclaimDeviceResponseTypeDef = TypedDict(
-    "UnclaimDeviceResponseTypeDef",
-    {
-        "State": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -331,28 +234,84 @@
 )
 
 class UpdateDeviceStateRequestRequestTypeDef(
     _RequiredUpdateDeviceStateRequestRequestTypeDef, _OptionalUpdateDeviceStateRequestRequestTypeDef
 ):
     pass
 
+ClaimDevicesByClaimCodeResponseTypeDef = TypedDict(
+    "ClaimDevicesByClaimCodeResponseTypeDef",
+    {
+        "ClaimCode": str,
+        "Total": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FinalizeDeviceClaimResponseTypeDef = TypedDict(
+    "FinalizeDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitiateDeviceClaimResponseTypeDef = TypedDict(
+    "InitiateDeviceClaimResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeDeviceMethodResponseTypeDef = TypedDict(
+    "InvokeDeviceMethodResponseTypeDef",
+    {
+        "DeviceMethodResponse": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UnclaimDeviceResponseTypeDef = TypedDict(
+    "UnclaimDeviceResponseTypeDef",
+    {
+        "State": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeDeviceResponseTypeDef = TypedDict(
     "DescribeDeviceResponseTypeDef",
     {
         "DeviceDescription": DeviceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeviceEventTypeDef = TypedDict(
     "DeviceEventTypeDef",
     {
         "Device": DeviceTypeDef,
@@ -360,16 +319,16 @@
     },
     total=False,
 )
 
 GetDeviceMethodsResponseTypeDef = TypedDict(
     "GetDeviceMethodsResponseTypeDef",
     {
-        "DeviceMethods": List[DeviceMethodOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DeviceMethods": List[DeviceMethodTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInvokeDeviceMethodRequestRequestTypeDef = TypedDict(
     "_RequiredInvokeDeviceMethodRequestRequestTypeDef",
     {
         "DeviceId": str,
@@ -386,15 +345,46 @@
 
 class InvokeDeviceMethodRequestRequestTypeDef(
     _RequiredInvokeDeviceMethodRequestRequestTypeDef,
     _OptionalInvokeDeviceMethodRequestRequestTypeDef,
 ):
     pass
 
+_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "FromTimeStamp": Union[datetime, str],
+        "ToTimeStamp": Union[datetime, str],
+    },
+)
+_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef = TypedDict(
+    "_OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDeviceEventsRequestListDeviceEventsPaginateTypeDef(
+    _RequiredListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    _OptionalListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+):
+    pass
+
+ListDevicesRequestListDevicesPaginateTypeDef = TypedDict(
+    "ListDevicesRequestListDevicesPaginateTypeDef",
+    {
+        "DeviceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListDeviceEventsResponseTypeDef = TypedDict(
     "ListDeviceEventsResponseTypeDef",
     {
         "Events": List[DeviceEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/PKG-INFO` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot1click-devices
-Version: 1.28.12
-Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoT1ClickDevicesService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot1click-devices.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot1click-devices)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot1click-devices)](https://pepy.tech/project/mypy-boto3-iot1click-devices)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT1ClickDevicesService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
+[boto3.IoT1ClickDevicesService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-devices.html#IoT1ClickDevicesService)
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
 [mypy-boto3-iot1click-devices docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot1click_devices/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,45 +322,44 @@
 
 `mypy_boto3_iot1click_devices.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot1click_devices.type_defs import (
     ClaimDevicesByClaimCodeRequestRequestTypeDef,
-    ClaimDevicesByClaimCodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     DescribeDeviceRequestRequestTypeDef,
     DeviceDescriptionTypeDef,
     DeviceTypeDef,
-    DeviceMethodOutputTypeDef,
     DeviceMethodTypeDef,
-    EmptyResponseMetadataTypeDef,
     FinalizeDeviceClaimRequestRequestTypeDef,
-    FinalizeDeviceClaimResponseTypeDef,
     GetDeviceMethodsRequestRequestTypeDef,
     InitiateDeviceClaimRequestRequestTypeDef,
-    InitiateDeviceClaimResponseTypeDef,
-    InvokeDeviceMethodResponseTypeDef,
-    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDeviceEventsRequestRequestTypeDef,
-    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDevicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UnclaimDeviceRequestRequestTypeDef,
-    UnclaimDeviceResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDeviceStateRequestRequestTypeDef,
+    ClaimDevicesByClaimCodeResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FinalizeDeviceClaimResponseTypeDef,
+    InitiateDeviceClaimResponseTypeDef,
+    InvokeDeviceMethodResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UnclaimDeviceResponseTypeDef,
     DescribeDeviceResponseTypeDef,
     ListDevicesResponseTypeDef,
     DeviceEventTypeDef,
     GetDeviceMethodsResponseTypeDef,
     InvokeDeviceMethodRequestRequestTypeDef,
+    ListDeviceEventsRequestListDeviceEventsPaginateTypeDef,
+    ListDevicesRequestListDevicesPaginateTypeDef,
     ListDeviceEventsResponseTypeDef,
 )
 
 
 def get_structure() -> ClaimDevicesByClaimCodeRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-iot1click-devices-1.28.12/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt` & `mypy-boto3-iot1click-devices-1.28.15/mypy_boto3_iot1click_devices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot1click-devices-1.28.12/setup.py` & `mypy-boto3-iot1click-devices-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot1click-devices",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iot1click_devices"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT1ClickDevicesService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IoT1ClickDevicesService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

