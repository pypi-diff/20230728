# Comparing `tmp/mypy-boto3-privatenetworks-1.28.12.tar.gz` & `tmp/mypy-boto3-privatenetworks-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-privatenetworks-1.28.12.tar", last modified: Thu Jul 27 11:49:24 2023, max compression
+gzip compressed data, was "mypy-boto3-privatenetworks-1.28.15.tar", last modified: Fri Jul 28 20:43:30 2023, max compression
```

## Comparing `mypy-boto3-privatenetworks-1.28.12.tar` & `mypy-boto3-privatenetworks-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15452 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21342 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-07-27 11:41:44.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31478 2023-07-27 11:41:45.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31419 2023-07-27 11:41:44.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16965 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-27 11:49:24.000000 mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:24.957163 mypy-boto3-privatenetworks-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-27 11:41:43.000000 mypy-boto3-privatenetworks-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.393681 mypy-boto3-privatenetworks-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-07-28 20:43:30.385681 mypy-boto3-privatenetworks-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15325 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.385681 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21342 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21304 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10068 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7016 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    29836 2023-07-28 20:33:39.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29781 2023-07-28 20:33:38.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:30.385681 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16838 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-28 20:43:30.000000 mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:30.393681 mypy-boto3-privatenetworks-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-28 20:33:37.000000 mypy-boto3-privatenetworks-1.28.15/setup.py
```

### Comparing `mypy-boto3-privatenetworks-1.28.12/LICENSE` & `mypy-boto3-privatenetworks-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/PKG-INFO` & `mypy-boto3-privatenetworks-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.28.12
-Summary: Type annotations for boto3.Private5G 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,16 +359,14 @@
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
     CommitmentConfigurationTypeDef,
-    AddressOutputTypeDef,
-    CommitmentConfigurationOutputTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
@@ -379,32 +377,30 @@
     PaginatorConfigTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
     ListNetworksRequestRequestTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    NameValuePairOutputTypeDef,
     NameValuePairTypeDef,
-    PositionOutputTypeDef,
     TrackingInformationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
     ReturnInformationTypeDef,
+    ActivateNetworkSiteRequestRequestTypeDef,
     CommitmentInformationTypeDef,
     OrderedResourceDefinitionTypeDef,
+    StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
```

### Comparing `mypy-boto3-privatenetworks-1.28.12/README.md` & `mypy-boto3-privatenetworks-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -327,16 +327,14 @@
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
     CommitmentConfigurationTypeDef,
-    AddressOutputTypeDef,
-    CommitmentConfigurationOutputTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
@@ -347,32 +345,30 @@
     PaginatorConfigTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
     ListNetworksRequestRequestTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    NameValuePairOutputTypeDef,
     NameValuePairTypeDef,
-    PositionOutputTypeDef,
     TrackingInformationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
     ReturnInformationTypeDef,
+    ActivateNetworkSiteRequestRequestTypeDef,
     CommitmentInformationTypeDef,
     OrderedResourceDefinitionTypeDef,
+    StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
```

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__init__.py` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__init__.pyi` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/__main__.py` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Private5G 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Private5G 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G\nOther"
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

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/client.py` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/client.pyi` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/literals.py` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/literals.pyi` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/paginator.py` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/paginator.pyi` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/type_defs.py` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,16 +44,14 @@
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
     "CommitmentConfigurationTypeDef",
-    "AddressOutputTypeDef",
-    "CommitmentConfigurationOutputTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
@@ -64,32 +62,30 @@
     "PaginatorConfigTypeDef",
     "ListDeviceIdentifiersRequestRequestTypeDef",
     "ListNetworkResourcesRequestRequestTypeDef",
     "ListNetworkSitesRequestRequestTypeDef",
     "ListNetworksRequestRequestTypeDef",
     "ListOrdersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "NameValuePairOutputTypeDef",
     "NameValuePairTypeDef",
-    "PositionOutputTypeDef",
     "TrackingInformationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateNetworkSiteRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ActivateNetworkSiteRequestRequestTypeDef",
-    "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ReturnInformationTypeDef",
+    "ActivateNetworkSiteRequestRequestTypeDef",
     "CommitmentInformationTypeDef",
     "OrderedResourceDefinitionTypeDef",
+    "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
     "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
@@ -208,50 +204,14 @@
     "CommitmentConfigurationTypeDef",
     {
         "automaticRenewal": bool,
         "commitmentLength": CommitmentLengthType,
     },
 )
 
-_RequiredAddressOutputTypeDef = TypedDict(
-    "_RequiredAddressOutputTypeDef",
-    {
-        "city": str,
-        "country": str,
-        "name": str,
-        "postalCode": str,
-        "stateOrProvince": str,
-        "street1": str,
-    },
-)
-_OptionalAddressOutputTypeDef = TypedDict(
-    "_OptionalAddressOutputTypeDef",
-    {
-        "company": str,
-        "emailAddress": str,
-        "phoneNumber": str,
-        "street2": str,
-        "street3": str,
-    },
-    total=False,
-)
-
-
-class AddressOutputTypeDef(_RequiredAddressOutputTypeDef, _OptionalAddressOutputTypeDef):
-    pass
-
-
-CommitmentConfigurationOutputTypeDef = TypedDict(
-    "CommitmentConfigurationOutputTypeDef",
-    {
-        "automaticRenewal": bool,
-        "commitmentLength": CommitmentLengthType,
-    },
-)
-
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -522,35 +482,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredNameValuePairOutputTypeDef = TypedDict(
-    "_RequiredNameValuePairOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalNameValuePairOutputTypeDef = TypedDict(
-    "_OptionalNameValuePairOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class NameValuePairOutputTypeDef(
-    _RequiredNameValuePairOutputTypeDef, _OptionalNameValuePairOutputTypeDef
-):
-    pass
-
-
 _RequiredNameValuePairTypeDef = TypedDict(
     "_RequiredNameValuePairTypeDef",
     {
         "name": str,
     },
 )
 _OptionalNameValuePairTypeDef = TypedDict(
@@ -562,26 +501,14 @@
 )
 
 
 class NameValuePairTypeDef(_RequiredNameValuePairTypeDef, _OptionalNameValuePairTypeDef):
     pass
 
 
-PositionOutputTypeDef = TypedDict(
-    "PositionOutputTypeDef",
-    {
-        "elevation": float,
-        "elevationReference": ElevationReferenceType,
-        "elevationUnit": Literal["FEET"],
-        "latitude": float,
-        "longitude": float,
-    },
-    total=False,
-)
-
 TrackingInformationTypeDef = TypedDict(
     "TrackingInformationTypeDef",
     {
         "trackingNumber": str,
     },
     total=False,
 )
@@ -671,14 +598,25 @@
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
+    {
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+        "shippingLabel": str,
+    },
+    total=False,
+)
+
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
     },
 )
@@ -695,54 +633,18 @@
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
-    {
-        "networkResourceArn": str,
-        "updateType": UpdateTypeType,
-    },
-)
-_OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
-    {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-    },
-    total=False,
-)
-
-
-class StartNetworkResourceUpdateRequestRequestTypeDef(
-    _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
-    _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
-):
-    pass
-
-
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
-    {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressOutputTypeDef,
-        "shippingLabel": str,
-    },
-    total=False,
-)
-
 _RequiredCommitmentInformationTypeDef = TypedDict(
     "_RequiredCommitmentInformationTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationOutputTypeDef,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
 )
 _OptionalCommitmentInformationTypeDef = TypedDict(
     "_OptionalCommitmentInformationTypeDef",
     {
         "expiresOn": datetime,
         "startAt": datetime,
@@ -763,26 +665,51 @@
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalOrderedResourceDefinitionTypeDef = TypedDict(
     "_OptionalOrderedResourceDefinitionTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationOutputTypeDef,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
 
 class OrderedResourceDefinitionTypeDef(
     _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
 ):
     pass
 
 
+_RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
+    {
+        "networkResourceArn": str,
+        "updateType": UpdateTypeType,
+    },
+)
+_OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+    },
+    total=False,
+)
+
+
+class StartNetworkResourceUpdateRequestRequestTypeDef(
+    _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
+    _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
+):
+    pass
+
+
 _RequiredConfigureAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAccessPointRequestRequestTypeDef",
     {
         "accessPointArn": str,
     },
 )
 _OptionalConfigureAccessPointRequestRequestTypeDef = TypedDict(
@@ -947,15 +874,15 @@
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalNetworkResourceDefinitionOutputTypeDef = TypedDict(
     "_OptionalNetworkResourceDefinitionOutputTypeDef",
     {
-        "options": List[NameValuePairOutputTypeDef],
+        "options": List[NameValuePairTypeDef],
     },
     total=False,
 )
 
 
 class NetworkResourceDefinitionOutputTypeDef(
     _RequiredNetworkResourceDefinitionOutputTypeDef, _OptionalNetworkResourceDefinitionOutputTypeDef
@@ -984,25 +911,25 @@
 ):
     pass
 
 
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
-        "attributes": List[NameValuePairOutputTypeDef],
+        "attributes": List[NameValuePairTypeDef],
         "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
         "orderArn": str,
-        "position": PositionOutputTypeDef,
+        "position": PositionTypeDef,
         "returnInformation": ReturnInformationTypeDef,
         "serialNumber": str,
         "status": NetworkResourceStatusType,
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
@@ -1014,24 +941,24 @@
     {
         "acknowledgmentStatus": AcknowledgmentStatusType,
         "createdAt": datetime,
         "networkArn": str,
         "networkSiteArn": str,
         "orderArn": str,
         "orderedResources": List[OrderedResourceDefinitionTypeDef],
-        "shippingAddress": AddressOutputTypeDef,
+        "shippingAddress": AddressTypeDef,
         "trackingInformation": List[TrackingInformationTypeDef],
     },
     total=False,
 )
 
 SitePlanOutputTypeDef = TypedDict(
     "SitePlanOutputTypeDef",
     {
-        "options": List[NameValuePairOutputTypeDef],
+        "options": List[NameValuePairTypeDef],
         "resourceDefinitions": List[NetworkResourceDefinitionOutputTypeDef],
     },
     total=False,
 )
 
 SitePlanTypeDef = TypedDict(
     "SitePlanTypeDef",
```

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks/type_defs.pyi` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -43,16 +43,14 @@
 __all__ = (
     "AcknowledgeOrderReceiptRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ActivateDeviceIdentifierRequestRequestTypeDef",
     "DeviceIdentifierTypeDef",
     "AddressTypeDef",
     "CommitmentConfigurationTypeDef",
-    "AddressOutputTypeDef",
-    "CommitmentConfigurationOutputTypeDef",
     "PositionTypeDef",
     "CreateNetworkRequestRequestTypeDef",
     "NetworkTypeDef",
     "DeactivateDeviceIdentifierRequestRequestTypeDef",
     "DeleteNetworkRequestRequestTypeDef",
     "DeleteNetworkSiteRequestRequestTypeDef",
     "GetDeviceIdentifierRequestRequestTypeDef",
@@ -63,32 +61,30 @@
     "PaginatorConfigTypeDef",
     "ListDeviceIdentifiersRequestRequestTypeDef",
     "ListNetworkResourcesRequestRequestTypeDef",
     "ListNetworkSitesRequestRequestTypeDef",
     "ListNetworksRequestRequestTypeDef",
     "ListOrdersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "NameValuePairOutputTypeDef",
     "NameValuePairTypeDef",
-    "PositionOutputTypeDef",
     "TrackingInformationTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateNetworkSiteRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PingResponseTypeDef",
     "ActivateDeviceIdentifierResponseTypeDef",
     "DeactivateDeviceIdentifierResponseTypeDef",
     "GetDeviceIdentifierResponseTypeDef",
     "ListDeviceIdentifiersResponseTypeDef",
-    "ActivateNetworkSiteRequestRequestTypeDef",
-    "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ReturnInformationTypeDef",
+    "ActivateNetworkSiteRequestRequestTypeDef",
     "CommitmentInformationTypeDef",
     "OrderedResourceDefinitionTypeDef",
+    "StartNetworkResourceUpdateRequestRequestTypeDef",
     "ConfigureAccessPointRequestRequestTypeDef",
     "CreateNetworkResponseTypeDef",
     "DeleteNetworkResponseTypeDef",
     "GetNetworkResponseTypeDef",
     "ListNetworksResponseTypeDef",
     "ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef",
     "ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef",
@@ -203,48 +199,14 @@
     "CommitmentConfigurationTypeDef",
     {
         "automaticRenewal": bool,
         "commitmentLength": CommitmentLengthType,
     },
 )
 
-_RequiredAddressOutputTypeDef = TypedDict(
-    "_RequiredAddressOutputTypeDef",
-    {
-        "city": str,
-        "country": str,
-        "name": str,
-        "postalCode": str,
-        "stateOrProvince": str,
-        "street1": str,
-    },
-)
-_OptionalAddressOutputTypeDef = TypedDict(
-    "_OptionalAddressOutputTypeDef",
-    {
-        "company": str,
-        "emailAddress": str,
-        "phoneNumber": str,
-        "street2": str,
-        "street3": str,
-    },
-    total=False,
-)
-
-class AddressOutputTypeDef(_RequiredAddressOutputTypeDef, _OptionalAddressOutputTypeDef):
-    pass
-
-CommitmentConfigurationOutputTypeDef = TypedDict(
-    "CommitmentConfigurationOutputTypeDef",
-    {
-        "automaticRenewal": bool,
-        "commitmentLength": CommitmentLengthType,
-    },
-)
-
 PositionTypeDef = TypedDict(
     "PositionTypeDef",
     {
         "elevation": float,
         "elevationReference": ElevationReferenceType,
         "elevationUnit": Literal["FEET"],
         "latitude": float,
@@ -497,33 +459,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-_RequiredNameValuePairOutputTypeDef = TypedDict(
-    "_RequiredNameValuePairOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalNameValuePairOutputTypeDef = TypedDict(
-    "_OptionalNameValuePairOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class NameValuePairOutputTypeDef(
-    _RequiredNameValuePairOutputTypeDef, _OptionalNameValuePairOutputTypeDef
-):
-    pass
-
 _RequiredNameValuePairTypeDef = TypedDict(
     "_RequiredNameValuePairTypeDef",
     {
         "name": str,
     },
 )
 _OptionalNameValuePairTypeDef = TypedDict(
@@ -533,26 +476,14 @@
     },
     total=False,
 )
 
 class NameValuePairTypeDef(_RequiredNameValuePairTypeDef, _OptionalNameValuePairTypeDef):
     pass
 
-PositionOutputTypeDef = TypedDict(
-    "PositionOutputTypeDef",
-    {
-        "elevation": float,
-        "elevationReference": ElevationReferenceType,
-        "elevationUnit": Literal["FEET"],
-        "latitude": float,
-        "longitude": float,
-    },
-    total=False,
-)
-
 TrackingInformationTypeDef = TypedDict(
     "TrackingInformationTypeDef",
     {
         "trackingNumber": str,
     },
     total=False,
 )
@@ -640,14 +571,25 @@
     {
         "deviceIdentifiers": List[DeviceIdentifierTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ReturnInformationTypeDef = TypedDict(
+    "ReturnInformationTypeDef",
+    {
+        "replacementOrderArn": str,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+        "shippingLabel": str,
+    },
+    total=False,
+)
+
 _RequiredActivateNetworkSiteRequestRequestTypeDef = TypedDict(
     "_RequiredActivateNetworkSiteRequestRequestTypeDef",
     {
         "networkSiteArn": str,
         "shippingAddress": AddressTypeDef,
     },
 )
@@ -662,52 +604,18 @@
 
 class ActivateNetworkSiteRequestRequestTypeDef(
     _RequiredActivateNetworkSiteRequestRequestTypeDef,
     _OptionalActivateNetworkSiteRequestRequestTypeDef,
 ):
     pass
 
-_RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
-    "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
-    {
-        "networkResourceArn": str,
-        "updateType": UpdateTypeType,
-    },
-)
-_OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
-    "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
-    {
-        "commitmentConfiguration": CommitmentConfigurationTypeDef,
-        "returnReason": str,
-        "shippingAddress": AddressTypeDef,
-    },
-    total=False,
-)
-
-class StartNetworkResourceUpdateRequestRequestTypeDef(
-    _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
-    _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
-):
-    pass
-
-ReturnInformationTypeDef = TypedDict(
-    "ReturnInformationTypeDef",
-    {
-        "replacementOrderArn": str,
-        "returnReason": str,
-        "shippingAddress": AddressOutputTypeDef,
-        "shippingLabel": str,
-    },
-    total=False,
-)
-
 _RequiredCommitmentInformationTypeDef = TypedDict(
     "_RequiredCommitmentInformationTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationOutputTypeDef,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
 )
 _OptionalCommitmentInformationTypeDef = TypedDict(
     "_OptionalCommitmentInformationTypeDef",
     {
         "expiresOn": datetime,
         "startAt": datetime,
@@ -726,24 +634,47 @@
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalOrderedResourceDefinitionTypeDef = TypedDict(
     "_OptionalOrderedResourceDefinitionTypeDef",
     {
-        "commitmentConfiguration": CommitmentConfigurationOutputTypeDef,
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
     },
     total=False,
 )
 
 class OrderedResourceDefinitionTypeDef(
     _RequiredOrderedResourceDefinitionTypeDef, _OptionalOrderedResourceDefinitionTypeDef
 ):
     pass
 
+_RequiredStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
+    "_RequiredStartNetworkResourceUpdateRequestRequestTypeDef",
+    {
+        "networkResourceArn": str,
+        "updateType": UpdateTypeType,
+    },
+)
+_OptionalStartNetworkResourceUpdateRequestRequestTypeDef = TypedDict(
+    "_OptionalStartNetworkResourceUpdateRequestRequestTypeDef",
+    {
+        "commitmentConfiguration": CommitmentConfigurationTypeDef,
+        "returnReason": str,
+        "shippingAddress": AddressTypeDef,
+    },
+    total=False,
+)
+
+class StartNetworkResourceUpdateRequestRequestTypeDef(
+    _RequiredStartNetworkResourceUpdateRequestRequestTypeDef,
+    _OptionalStartNetworkResourceUpdateRequestRequestTypeDef,
+):
+    pass
+
 _RequiredConfigureAccessPointRequestRequestTypeDef = TypedDict(
     "_RequiredConfigureAccessPointRequestRequestTypeDef",
     {
         "accessPointArn": str,
     },
 )
 _OptionalConfigureAccessPointRequestRequestTypeDef = TypedDict(
@@ -898,15 +829,15 @@
         "count": int,
         "type": NetworkResourceDefinitionTypeType,
     },
 )
 _OptionalNetworkResourceDefinitionOutputTypeDef = TypedDict(
     "_OptionalNetworkResourceDefinitionOutputTypeDef",
     {
-        "options": List[NameValuePairOutputTypeDef],
+        "options": List[NameValuePairTypeDef],
     },
     total=False,
 )
 
 class NetworkResourceDefinitionOutputTypeDef(
     _RequiredNetworkResourceDefinitionOutputTypeDef, _OptionalNetworkResourceDefinitionOutputTypeDef
 ):
@@ -931,25 +862,25 @@
     _RequiredNetworkResourceDefinitionTypeDef, _OptionalNetworkResourceDefinitionTypeDef
 ):
     pass
 
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
-        "attributes": List[NameValuePairOutputTypeDef],
+        "attributes": List[NameValuePairTypeDef],
         "commitmentInformation": CommitmentInformationTypeDef,
         "createdAt": datetime,
         "description": str,
         "health": HealthStatusType,
         "model": str,
         "networkArn": str,
         "networkResourceArn": str,
         "networkSiteArn": str,
         "orderArn": str,
-        "position": PositionOutputTypeDef,
+        "position": PositionTypeDef,
         "returnInformation": ReturnInformationTypeDef,
         "serialNumber": str,
         "status": NetworkResourceStatusType,
         "statusReason": str,
         "type": Literal["RADIO_UNIT"],
         "vendor": str,
     },
@@ -961,24 +892,24 @@
     {
         "acknowledgmentStatus": AcknowledgmentStatusType,
         "createdAt": datetime,
         "networkArn": str,
         "networkSiteArn": str,
         "orderArn": str,
         "orderedResources": List[OrderedResourceDefinitionTypeDef],
-        "shippingAddress": AddressOutputTypeDef,
+        "shippingAddress": AddressTypeDef,
         "trackingInformation": List[TrackingInformationTypeDef],
     },
     total=False,
 )
 
 SitePlanOutputTypeDef = TypedDict(
     "SitePlanOutputTypeDef",
     {
-        "options": List[NameValuePairOutputTypeDef],
+        "options": List[NameValuePairTypeDef],
         "resourceDefinitions": List[NetworkResourceDefinitionOutputTypeDef],
     },
     total=False,
 )
 
 SitePlanTypeDef = TypedDict(
     "SitePlanTypeDef",
```

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/PKG-INFO` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-privatenetworks
-Version: 1.28.12
-Summary: Type annotations for boto3.Private5G 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-privatenetworks.svg?color=blue)](https://pypi.org/project/mypy-boto3-privatenetworks)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-privatenetworks)](https://pepy.tech/project/mypy-boto3-privatenetworks)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Private5G 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
+[boto3.Private5G 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/privatenetworks.html#Private5G)
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
 [mypy-boto3-privatenetworks docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_privatenetworks/).
 
 See how it helps to find and fix potential bugs:
 
@@ -359,16 +359,14 @@
 from mypy_boto3_privatenetworks.type_defs import (
     AcknowledgeOrderReceiptRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     ActivateDeviceIdentifierRequestRequestTypeDef,
     DeviceIdentifierTypeDef,
     AddressTypeDef,
     CommitmentConfigurationTypeDef,
-    AddressOutputTypeDef,
-    CommitmentConfigurationOutputTypeDef,
     PositionTypeDef,
     CreateNetworkRequestRequestTypeDef,
     NetworkTypeDef,
     DeactivateDeviceIdentifierRequestRequestTypeDef,
     DeleteNetworkRequestRequestTypeDef,
     DeleteNetworkSiteRequestRequestTypeDef,
     GetDeviceIdentifierRequestRequestTypeDef,
@@ -379,32 +377,30 @@
     PaginatorConfigTypeDef,
     ListDeviceIdentifiersRequestRequestTypeDef,
     ListNetworkResourcesRequestRequestTypeDef,
     ListNetworkSitesRequestRequestTypeDef,
     ListNetworksRequestRequestTypeDef,
     ListOrdersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    NameValuePairOutputTypeDef,
     NameValuePairTypeDef,
-    PositionOutputTypeDef,
     TrackingInformationTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateNetworkSiteRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     PingResponseTypeDef,
     ActivateDeviceIdentifierResponseTypeDef,
     DeactivateDeviceIdentifierResponseTypeDef,
     GetDeviceIdentifierResponseTypeDef,
     ListDeviceIdentifiersResponseTypeDef,
-    ActivateNetworkSiteRequestRequestTypeDef,
-    StartNetworkResourceUpdateRequestRequestTypeDef,
     ReturnInformationTypeDef,
+    ActivateNetworkSiteRequestRequestTypeDef,
     CommitmentInformationTypeDef,
     OrderedResourceDefinitionTypeDef,
+    StartNetworkResourceUpdateRequestRequestTypeDef,
     ConfigureAccessPointRequestRequestTypeDef,
     CreateNetworkResponseTypeDef,
     DeleteNetworkResponseTypeDef,
     GetNetworkResponseTypeDef,
     ListNetworksResponseTypeDef,
     ListDeviceIdentifiersRequestListDeviceIdentifiersPaginateTypeDef,
     ListNetworkResourcesRequestListNetworkResourcesPaginateTypeDef,
```

### Comparing `mypy-boto3-privatenetworks-1.28.12/mypy_boto3_privatenetworks.egg-info/SOURCES.txt` & `mypy-boto3-privatenetworks-1.28.15/mypy_boto3_privatenetworks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-privatenetworks-1.28.12/setup.py` & `mypy-boto3-privatenetworks-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-privatenetworks",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_privatenetworks"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Private5G 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Private5G 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

