# Comparing `tmp/mypy-boto3-globalaccelerator-1.28.12.tar.gz` & `tmp/mypy-boto3-globalaccelerator-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-globalaccelerator-1.28.12.tar", last modified: Thu Jul 27 05:34:44 2023, max compression
+gzip compressed data, was "mypy-boto3-globalaccelerator-1.28.15.tar", last modified: Fri Jul 28 20:42:52 2023, max compression
```

## Comparing `mypy-boto3-globalaccelerator-1.28.12.tar` & `mypy-boto3-globalaccelerator-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.156501 mypy-boto3-globalaccelerator-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20569 2023-07-27 05:34:44.148501 mypy-boto3-globalaccelerator-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19042 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.148501 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41373 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41309 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10634 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45263 2023-07-27 05:22:47.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45214 2023-07-27 05:22:47.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:44.148501 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20569 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-27 05:34:44.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-27 05:34:43.000000 mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:44.156501 mypy-boto3-globalaccelerator-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-27 05:22:45.000000 mypy-boto3-globalaccelerator-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.537162 mypy-boto3-globalaccelerator-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20488 2023-07-28 20:42:52.529162 mypy-boto3-globalaccelerator-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18961 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.521161 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41373 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41309 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-07-28 20:26:34.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10139 2023-07-28 20:26:34.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-07-28 20:26:34.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10608 2023-07-28 20:26:34.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44638 2023-07-28 20:26:35.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44589 2023-07-28 20:26:34.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:52.529162 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20488 2023-07-28 20:42:52.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-28 20:42:52.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:52.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:52.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-28 20:42:52.000000 mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:52.537162 mypy-boto3-globalaccelerator-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-28 20:26:33.000000 mypy-boto3-globalaccelerator-1.28.15/setup.py
```

### Comparing `mypy-boto3-globalaccelerator-1.28.12/LICENSE` & `mypy-boto3-globalaccelerator-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.12/PKG-INFO` & `mypy-boto3-globalaccelerator-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-globalaccelerator
-Version: 1.28.12
-Summary: Type annotations for boto3.GlobalAccelerator 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GlobalAccelerator 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-globalaccelerator)](https://pepy.tech/project/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,27 +368,27 @@
 ```python
 from mypy_boto3_globalaccelerator.type_defs import (
     AcceleratorAttributesTypeDef,
     AcceleratorEventTypeDef,
     IpSetTypeDef,
     CustomRoutingEndpointConfigurationTypeDef,
     CustomRoutingEndpointDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     EndpointConfigurationTypeDef,
     EndpointDescriptionTypeDef,
     AdvertiseByoipCidrRequestRequestTypeDef,
     AllowCustomRoutingTrafficRequestRequestTypeDef,
     ByoipCidrEventTypeDef,
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
     CustomRoutingDestinationConfigurationTypeDef,
     PortRangeTypeDef,
     PortOverrideTypeDef,
     CustomRoutingAcceleratorAttributesTypeDef,
     CustomRoutingDestinationDescriptionTypeDef,
-    PortRangeOutputTypeDef,
     DeleteAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingEndpointGroupRequestRequestTypeDef,
     DeleteCustomRoutingListenerRequestRequestTypeDef,
     DeleteEndpointGroupRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DenyCustomRoutingTrafficRequestRequestTypeDef,
@@ -398,105 +398,102 @@
     DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PortOverrideOutputTypeDef,
     EndpointIdentifierTypeDef,
-    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
-    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
-    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
     ListCustomRoutingEndpointGroupsRequestRequestTypeDef,
-    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
     ListCustomRoutingListenersRequestRequestTypeDef,
-    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
     ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
-    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
-    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorRequestRequestTypeDef,
     WithdrawByoipCidrRequestRequestTypeDef,
-    DescribeAcceleratorAttributesResponseTypeDef,
-    UpdateAcceleratorAttributesResponseTypeDef,
     AcceleratorTypeDef,
     CustomRoutingAcceleratorTypeDef,
     AddCustomRoutingEndpointsRequestRequestTypeDef,
     AddCustomRoutingEndpointsResponseTypeDef,
+    DescribeAcceleratorAttributesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    UpdateAcceleratorAttributesResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateCustomRoutingEndpointGroupRequestRequestTypeDef,
     CreateCustomRoutingListenerRequestRequestTypeDef,
     CreateListenerRequestRequestTypeDef,
+    CustomRoutingListenerTypeDef,
+    ListenerTypeDef,
     UpdateCustomRoutingListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateEndpointGroupRequestRequestTypeDef,
+    EndpointGroupTypeDef,
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
-    CustomRoutingListenerTypeDef,
-    ListenerTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
-    EndpointGroupTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
+    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
+    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
+    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
     UpdateCustomRoutingAcceleratorResponseTypeDef,
     AdvertiseByoipCidrResponseTypeDef,
     DeprovisionByoipCidrResponseTypeDef,
     ListByoipCidrsResponseTypeDef,
     ProvisionByoipCidrResponseTypeDef,
     WithdrawByoipCidrResponseTypeDef,
-    CreateCustomRoutingEndpointGroupResponseTypeDef,
-    DescribeCustomRoutingEndpointGroupResponseTypeDef,
-    ListCustomRoutingEndpointGroupsResponseTypeDef,
     CreateCustomRoutingListenerResponseTypeDef,
     DescribeCustomRoutingListenerResponseTypeDef,
     ListCustomRoutingListenersResponseTypeDef,
     UpdateCustomRoutingListenerResponseTypeDef,
     CreateListenerResponseTypeDef,
     DescribeListenerResponseTypeDef,
     ListListenersResponseTypeDef,
     UpdateListenerResponseTypeDef,
-    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
-    ListCustomRoutingPortMappingsResponseTypeDef,
     CreateEndpointGroupResponseTypeDef,
     DescribeEndpointGroupResponseTypeDef,
     ListEndpointGroupsResponseTypeDef,
     UpdateEndpointGroupResponseTypeDef,
+    CreateCustomRoutingEndpointGroupResponseTypeDef,
+    DescribeCustomRoutingEndpointGroupResponseTypeDef,
+    ListCustomRoutingEndpointGroupsResponseTypeDef,
+    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
+    ListCustomRoutingPortMappingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-globalaccelerator-1.28.12/README.md` & `mypy-boto3-globalaccelerator-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-globalaccelerator)](https://pepy.tech/project/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -336,27 +336,27 @@
 ```python
 from mypy_boto3_globalaccelerator.type_defs import (
     AcceleratorAttributesTypeDef,
     AcceleratorEventTypeDef,
     IpSetTypeDef,
     CustomRoutingEndpointConfigurationTypeDef,
     CustomRoutingEndpointDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     EndpointConfigurationTypeDef,
     EndpointDescriptionTypeDef,
     AdvertiseByoipCidrRequestRequestTypeDef,
     AllowCustomRoutingTrafficRequestRequestTypeDef,
     ByoipCidrEventTypeDef,
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
     CustomRoutingDestinationConfigurationTypeDef,
     PortRangeTypeDef,
     PortOverrideTypeDef,
     CustomRoutingAcceleratorAttributesTypeDef,
     CustomRoutingDestinationDescriptionTypeDef,
-    PortRangeOutputTypeDef,
     DeleteAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingEndpointGroupRequestRequestTypeDef,
     DeleteCustomRoutingListenerRequestRequestTypeDef,
     DeleteEndpointGroupRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DenyCustomRoutingTrafficRequestRequestTypeDef,
@@ -366,105 +366,102 @@
     DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PortOverrideOutputTypeDef,
     EndpointIdentifierTypeDef,
-    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
-    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
-    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
     ListCustomRoutingEndpointGroupsRequestRequestTypeDef,
-    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
     ListCustomRoutingListenersRequestRequestTypeDef,
-    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
     ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
-    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
-    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorRequestRequestTypeDef,
     WithdrawByoipCidrRequestRequestTypeDef,
-    DescribeAcceleratorAttributesResponseTypeDef,
-    UpdateAcceleratorAttributesResponseTypeDef,
     AcceleratorTypeDef,
     CustomRoutingAcceleratorTypeDef,
     AddCustomRoutingEndpointsRequestRequestTypeDef,
     AddCustomRoutingEndpointsResponseTypeDef,
+    DescribeAcceleratorAttributesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    UpdateAcceleratorAttributesResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateCustomRoutingEndpointGroupRequestRequestTypeDef,
     CreateCustomRoutingListenerRequestRequestTypeDef,
     CreateListenerRequestRequestTypeDef,
+    CustomRoutingListenerTypeDef,
+    ListenerTypeDef,
     UpdateCustomRoutingListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateEndpointGroupRequestRequestTypeDef,
+    EndpointGroupTypeDef,
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
-    CustomRoutingListenerTypeDef,
-    ListenerTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
-    EndpointGroupTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
+    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
+    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
+    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
     UpdateCustomRoutingAcceleratorResponseTypeDef,
     AdvertiseByoipCidrResponseTypeDef,
     DeprovisionByoipCidrResponseTypeDef,
     ListByoipCidrsResponseTypeDef,
     ProvisionByoipCidrResponseTypeDef,
     WithdrawByoipCidrResponseTypeDef,
-    CreateCustomRoutingEndpointGroupResponseTypeDef,
-    DescribeCustomRoutingEndpointGroupResponseTypeDef,
-    ListCustomRoutingEndpointGroupsResponseTypeDef,
     CreateCustomRoutingListenerResponseTypeDef,
     DescribeCustomRoutingListenerResponseTypeDef,
     ListCustomRoutingListenersResponseTypeDef,
     UpdateCustomRoutingListenerResponseTypeDef,
     CreateListenerResponseTypeDef,
     DescribeListenerResponseTypeDef,
     ListListenersResponseTypeDef,
     UpdateListenerResponseTypeDef,
-    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
-    ListCustomRoutingPortMappingsResponseTypeDef,
     CreateEndpointGroupResponseTypeDef,
     DescribeEndpointGroupResponseTypeDef,
     ListEndpointGroupsResponseTypeDef,
     UpdateEndpointGroupResponseTypeDef,
+    CreateCustomRoutingEndpointGroupResponseTypeDef,
+    DescribeCustomRoutingEndpointGroupResponseTypeDef,
+    ListCustomRoutingEndpointGroupsResponseTypeDef,
+    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
+    ListCustomRoutingPortMappingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__init__.py` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__init__.pyi` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/__main__.py` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GlobalAccelerator 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.GlobalAccelerator 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator\nOther"
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

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/client.py` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/client.pyi` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/literals.py` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/literals.pyi` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/paginator.py` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,60 +74,60 @@
 class ListAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listacceleratorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listacceleratorspaginator)
         """
 
 
 class ListByoipCidrsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listbyoipcidrspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListByoipCidrsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listbyoipcidrspaginator)
         """
 
 
 class ListCustomRoutingAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingacceleratorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomRoutingAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingacceleratorspaginator)
         """
 
 
 class ListCustomRoutingListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutinglistenerspaginator)
     """
 
     def paginate(
-        self, *, AcceleratorArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceleratorArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomRoutingListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutinglistenerspaginator)
         """
 
 
@@ -138,15 +138,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceleratorArn: str,
         EndpointGroupArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomRoutingPortMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingspaginator)
         """
 
 
@@ -157,43 +157,43 @@
     """
 
     def paginate(
         self,
         *,
         EndpointId: str,
         DestinationAddress: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomRoutingPortMappingsByDestinationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingsbydestinationpaginator)
         """
 
 
 class ListEndpointGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listendpointgroupspaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listendpointgroupspaginator)
         """
 
 
 class ListListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, AcceleratorArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceleratorArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listlistenerspaginator)
         """
```

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/paginator.pyi` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -71,57 +71,57 @@
 class ListAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listacceleratorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listacceleratorspaginator)
         """
 
 class ListByoipCidrsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listbyoipcidrspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListByoipCidrsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListByoipCidrs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listbyoipcidrspaginator)
         """
 
 class ListCustomRoutingAcceleratorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingacceleratorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomRoutingAcceleratorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingAccelerators.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingacceleratorspaginator)
         """
 
 class ListCustomRoutingListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutinglistenerspaginator)
     """
 
     def paginate(
-        self, *, AcceleratorArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceleratorArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomRoutingListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutinglistenerspaginator)
         """
 
 class ListCustomRoutingPortMappingsPaginator(Paginator):
@@ -131,15 +131,15 @@
     """
 
     def paginate(
         self,
         *,
         AcceleratorArn: str,
         EndpointGroupArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomRoutingPortMappingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingspaginator)
         """
 
 class ListCustomRoutingPortMappingsByDestinationPaginator(Paginator):
@@ -149,41 +149,41 @@
     """
 
     def paginate(
         self,
         *,
         EndpointId: str,
         DestinationAddress: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomRoutingPortMappingsByDestinationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListCustomRoutingPortMappingsByDestination.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listcustomroutingportmappingsbydestinationpaginator)
         """
 
 class ListEndpointGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listendpointgroupspaginator)
     """
 
     def paginate(
-        self, *, ListenerArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ListenerArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListEndpointGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListEndpointGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listendpointgroupspaginator)
         """
 
 class ListListenersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, AcceleratorArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, AcceleratorArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator.Paginator.ListListeners.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/paginators/#listlistenerspaginator)
         """
```

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/type_defs.py` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,27 +37,27 @@
 
 __all__ = (
     "AcceleratorAttributesTypeDef",
     "AcceleratorEventTypeDef",
     "IpSetTypeDef",
     "CustomRoutingEndpointConfigurationTypeDef",
     "CustomRoutingEndpointDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "EndpointConfigurationTypeDef",
     "EndpointDescriptionTypeDef",
     "AdvertiseByoipCidrRequestRequestTypeDef",
     "AllowCustomRoutingTrafficRequestRequestTypeDef",
     "ByoipCidrEventTypeDef",
     "CidrAuthorizationContextTypeDef",
     "TagTypeDef",
     "CustomRoutingDestinationConfigurationTypeDef",
     "PortRangeTypeDef",
     "PortOverrideTypeDef",
     "CustomRoutingAcceleratorAttributesTypeDef",
     "CustomRoutingDestinationDescriptionTypeDef",
-    "PortRangeOutputTypeDef",
     "DeleteAcceleratorRequestRequestTypeDef",
     "DeleteCustomRoutingAcceleratorRequestRequestTypeDef",
     "DeleteCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DeleteCustomRoutingListenerRequestRequestTypeDef",
     "DeleteEndpointGroupRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DenyCustomRoutingTrafficRequestRequestTypeDef",
@@ -67,105 +67,102 @@
     "DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorRequestRequestTypeDef",
     "DescribeCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingListenerRequestRequestTypeDef",
     "DescribeEndpointGroupRequestRequestTypeDef",
     "DescribeListenerRequestRequestTypeDef",
     "SocketAddressTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "PortOverrideOutputTypeDef",
     "EndpointIdentifierTypeDef",
-    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAcceleratorsRequestRequestTypeDef",
-    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
     "ListByoipCidrsRequestRequestTypeDef",
-    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
     "ListCustomRoutingEndpointGroupsRequestRequestTypeDef",
-    "ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
     "ListCustomRoutingListenersRequestRequestTypeDef",
-    "ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
     "ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef",
-    "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
     "ListCustomRoutingPortMappingsRequestRequestTypeDef",
-    "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
     "ListEndpointGroupsRequestRequestTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAcceleratorAttributesRequestRequestTypeDef",
     "UpdateAcceleratorRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorRequestRequestTypeDef",
     "WithdrawByoipCidrRequestRequestTypeDef",
-    "DescribeAcceleratorAttributesResponseTypeDef",
-    "UpdateAcceleratorAttributesResponseTypeDef",
     "AcceleratorTypeDef",
     "CustomRoutingAcceleratorTypeDef",
     "AddCustomRoutingEndpointsRequestRequestTypeDef",
     "AddCustomRoutingEndpointsResponseTypeDef",
+    "DescribeAcceleratorAttributesResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "UpdateAcceleratorAttributesResponseTypeDef",
     "AddEndpointsRequestRequestTypeDef",
     "AddEndpointsResponseTypeDef",
     "ByoipCidrTypeDef",
     "ProvisionByoipCidrRequestRequestTypeDef",
     "CreateAcceleratorRequestRequestTypeDef",
     "CreateCustomRoutingAcceleratorRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateCustomRoutingEndpointGroupRequestRequestTypeDef",
     "CreateCustomRoutingListenerRequestRequestTypeDef",
     "CreateListenerRequestRequestTypeDef",
+    "CustomRoutingListenerTypeDef",
+    "ListenerTypeDef",
     "UpdateCustomRoutingListenerRequestRequestTypeDef",
     "UpdateListenerRequestRequestTypeDef",
     "CreateEndpointGroupRequestRequestTypeDef",
+    "EndpointGroupTypeDef",
     "UpdateEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     "CustomRoutingEndpointGroupTypeDef",
-    "CustomRoutingListenerTypeDef",
-    "ListenerTypeDef",
     "DestinationPortMappingTypeDef",
     "PortMappingTypeDef",
-    "EndpointGroupTypeDef",
     "RemoveEndpointsRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
+    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
+    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
+    "ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    "ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+    "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
     "CreateAcceleratorResponseTypeDef",
     "DescribeAcceleratorResponseTypeDef",
     "ListAcceleratorsResponseTypeDef",
     "UpdateAcceleratorResponseTypeDef",
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     "ListCustomRoutingAcceleratorsResponseTypeDef",
     "UpdateCustomRoutingAcceleratorResponseTypeDef",
     "AdvertiseByoipCidrResponseTypeDef",
     "DeprovisionByoipCidrResponseTypeDef",
     "ListByoipCidrsResponseTypeDef",
     "ProvisionByoipCidrResponseTypeDef",
     "WithdrawByoipCidrResponseTypeDef",
-    "CreateCustomRoutingEndpointGroupResponseTypeDef",
-    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
-    "ListCustomRoutingEndpointGroupsResponseTypeDef",
     "CreateCustomRoutingListenerResponseTypeDef",
     "DescribeCustomRoutingListenerResponseTypeDef",
     "ListCustomRoutingListenersResponseTypeDef",
     "UpdateCustomRoutingListenerResponseTypeDef",
     "CreateListenerResponseTypeDef",
     "DescribeListenerResponseTypeDef",
     "ListListenersResponseTypeDef",
     "UpdateListenerResponseTypeDef",
-    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
-    "ListCustomRoutingPortMappingsResponseTypeDef",
     "CreateEndpointGroupResponseTypeDef",
     "DescribeEndpointGroupResponseTypeDef",
     "ListEndpointGroupsResponseTypeDef",
     "UpdateEndpointGroupResponseTypeDef",
+    "CreateCustomRoutingEndpointGroupResponseTypeDef",
+    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
+    "ListCustomRoutingEndpointGroupsResponseTypeDef",
+    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
+    "ListCustomRoutingPortMappingsResponseTypeDef",
 )
 
 AcceleratorAttributesTypeDef = TypedDict(
     "AcceleratorAttributesTypeDef",
     {
         "FlowLogsEnabled": bool,
         "FlowLogsS3Bucket": str,
@@ -205,14 +202,25 @@
     "CustomRoutingEndpointDescriptionTypeDef",
     {
         "EndpointId": str,
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
 EndpointConfigurationTypeDef = TypedDict(
     "EndpointConfigurationTypeDef",
     {
         "EndpointId": str,
         "Weight": int,
         "ClientIPPreservationEnabled": bool,
     },
@@ -331,23 +339,14 @@
         "FromPort": int,
         "ToPort": int,
         "Protocols": List[ProtocolType],
     },
     total=False,
 )
 
-PortRangeOutputTypeDef = TypedDict(
-    "PortRangeOutputTypeDef",
-    {
-        "FromPort": int,
-        "ToPort": int,
-    },
-    total=False,
-)
-
 DeleteAcceleratorRequestRequestTypeDef = TypedDict(
     "DeleteAcceleratorRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 
@@ -479,30 +478,14 @@
     {
         "IpAddress": str,
         "Port": int,
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
-PortOverrideOutputTypeDef = TypedDict(
-    "PortOverrideOutputTypeDef",
-    {
-        "ListenerPort": int,
-        "EndpointPort": int,
-    },
-    total=False,
-)
-
 _RequiredEndpointIdentifierTypeDef = TypedDict(
     "_RequiredEndpointIdentifierTypeDef",
     {
         "EndpointId": str,
     },
 )
 _OptionalEndpointIdentifierTypeDef = TypedDict(
@@ -516,56 +499,42 @@
 
 class EndpointIdentifierTypeDef(
     _RequiredEndpointIdentifierTypeDef, _OptionalEndpointIdentifierTypeDef
 ):
     pass
 
 
-ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = TypedDict(
-    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
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
 
 ListAcceleratorsRequestRequestTypeDef = TypedDict(
     "ListAcceleratorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = TypedDict(
-    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListByoipCidrsRequestRequestTypeDef = TypedDict(
     "ListByoipCidrsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = TypedDict(
-    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomRoutingAcceleratorsRequestRequestTypeDef = TypedDict(
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -590,36 +559,14 @@
 class ListCustomRoutingEndpointGroupsRequestRequestTypeDef(
     _RequiredListCustomRoutingEndpointGroupsRequestRequestTypeDef,
     _OptionalListCustomRoutingEndpointGroupsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
-    "_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    {
-        "AcceleratorArn": str,
-    },
-)
-_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
-    "_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef(
-    _RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-    _OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCustomRoutingListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingListenersRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListCustomRoutingListenersRequestRequestTypeDef = TypedDict(
@@ -635,37 +582,14 @@
 class ListCustomRoutingListenersRequestRequestTypeDef(
     _RequiredListCustomRoutingListenersRequestRequestTypeDef,
     _OptionalListCustomRoutingListenersRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
-    "_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    {
-        "EndpointId": str,
-        "DestinationAddress": str,
-    },
-)
-_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
-    "_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef(
-    _RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-    _OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef",
     {
         "EndpointId": str,
         "DestinationAddress": str,
     },
 )
@@ -682,41 +606,14 @@
 class ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef(
     _RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
     _OptionalListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-        {
-            "AcceleratorArn": str,
-        },
-    )
-)
-_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-        {
-            "EndpointGroupArn": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef(
-    _RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-    _OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCustomRoutingPortMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingPortMappingsRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListCustomRoutingPortMappingsRequestRequestTypeDef = TypedDict(
@@ -733,36 +630,14 @@
 class ListCustomRoutingPortMappingsRequestRequestTypeDef(
     _RequiredListCustomRoutingPortMappingsRequestRequestTypeDef,
     _OptionalListCustomRoutingPortMappingsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef(
-    _RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-    _OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEndpointGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListEndpointGroupsRequestRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalListEndpointGroupsRequestRequestTypeDef = TypedDict(
@@ -778,36 +653,14 @@
 class ListEndpointGroupsRequestRequestTypeDef(
     _RequiredListEndpointGroupsRequestRequestTypeDef,
     _OptionalListEndpointGroupsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "AcceleratorArn": str,
-    },
-)
-_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_OptionalListListenersRequestListListenersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListListenersRequestListListenersPaginateTypeDef(
-    _RequiredListListenersRequestListListenersPaginateTypeDef,
-    _OptionalListListenersRequestListListenersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListListenersRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -829,51 +682,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
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
 RemoveCustomRoutingEndpointsRequestRequestTypeDef = TypedDict(
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
     {
         "EndpointIds": Sequence[str],
         "EndpointGroupArn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -976,30 +800,14 @@
 WithdrawByoipCidrRequestRequestTypeDef = TypedDict(
     "WithdrawByoipCidrRequestRequestTypeDef",
     {
         "Cidr": str,
     },
 )
 
-DescribeAcceleratorAttributesResponseTypeDef = TypedDict(
-    "DescribeAcceleratorAttributesResponseTypeDef",
-    {
-        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAcceleratorAttributesResponseTypeDef = TypedDict(
-    "UpdateAcceleratorAttributesResponseTypeDef",
-    {
-        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AcceleratorTypeDef = TypedDict(
     "AcceleratorTypeDef",
     {
         "AcceleratorArn": str,
         "Name": str,
         "IpAddressType": IpAddressTypeType,
         "Enabled": bool,
@@ -1039,15 +847,38 @@
 )
 
 AddCustomRoutingEndpointsResponseTypeDef = TypedDict(
     "AddCustomRoutingEndpointsResponseTypeDef",
     {
         "EndpointDescriptions": List[CustomRoutingEndpointDescriptionTypeDef],
         "EndpointGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAcceleratorAttributesResponseTypeDef = TypedDict(
+    "DescribeAcceleratorAttributesResponseTypeDef",
+    {
+        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
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
+UpdateAcceleratorAttributesResponseTypeDef = TypedDict(
+    "UpdateAcceleratorAttributesResponseTypeDef",
+    {
+        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddEndpointsRequestRequestTypeDef = TypedDict(
     "AddEndpointsRequestRequestTypeDef",
     {
         "EndpointConfigurations": Sequence[EndpointConfigurationTypeDef],
@@ -1056,15 +887,15 @@
 )
 
 AddEndpointsResponseTypeDef = TypedDict(
     "AddEndpointsResponseTypeDef",
     {
         "EndpointDescriptions": List[EndpointDescriptionTypeDef],
         "EndpointGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ByoipCidrTypeDef = TypedDict(
     "ByoipCidrTypeDef",
     {
         "Cidr": str,
@@ -1129,14 +960,22 @@
 class CreateCustomRoutingAcceleratorRequestRequestTypeDef(
     _RequiredCreateCustomRoutingAcceleratorRequestRequestTypeDef,
     _OptionalCreateCustomRoutingAcceleratorRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1180,14 +1019,34 @@
 
 class CreateListenerRequestRequestTypeDef(
     _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
 ):
     pass
 
 
+CustomRoutingListenerTypeDef = TypedDict(
+    "CustomRoutingListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "PortRanges": List[PortRangeTypeDef],
+    },
+    total=False,
+)
+
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "PortRanges": List[PortRangeTypeDef],
+        "Protocol": ProtocolType,
+        "ClientAffinity": ClientAffinityType,
+    },
+    total=False,
+)
+
 UpdateCustomRoutingListenerRequestRequestTypeDef = TypedDict(
     "UpdateCustomRoutingListenerRequestRequestTypeDef",
     {
         "ListenerArn": str,
         "PortRanges": Sequence[PortRangeTypeDef],
     },
 )
@@ -1242,14 +1101,31 @@
 class CreateEndpointGroupRequestRequestTypeDef(
     _RequiredCreateEndpointGroupRequestRequestTypeDef,
     _OptionalCreateEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
 
+EndpointGroupTypeDef = TypedDict(
+    "EndpointGroupTypeDef",
+    {
+        "EndpointGroupArn": str,
+        "EndpointGroupRegion": str,
+        "EndpointDescriptions": List[EndpointDescriptionTypeDef],
+        "TrafficDialPercentage": float,
+        "HealthCheckPort": int,
+        "HealthCheckProtocol": HealthCheckProtocolType,
+        "HealthCheckPath": str,
+        "HealthCheckIntervalSeconds": int,
+        "ThresholdCount": int,
+        "PortOverrides": List[PortOverrideTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEndpointGroupRequestRequestTypeDef",
     {
         "EndpointGroupArn": str,
     },
 )
 _OptionalUpdateEndpointGroupRequestRequestTypeDef = TypedDict(
@@ -1275,57 +1151,37 @@
     pass
 
 
 DescribeCustomRoutingAcceleratorAttributesResponseTypeDef = TypedDict(
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     {
         "AcceleratorAttributes": CustomRoutingAcceleratorAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCustomRoutingAcceleratorAttributesResponseTypeDef = TypedDict(
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     {
         "AcceleratorAttributes": CustomRoutingAcceleratorAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomRoutingEndpointGroupTypeDef = TypedDict(
     "CustomRoutingEndpointGroupTypeDef",
     {
         "EndpointGroupArn": str,
         "EndpointGroupRegion": str,
         "DestinationDescriptions": List[CustomRoutingDestinationDescriptionTypeDef],
         "EndpointDescriptions": List[CustomRoutingEndpointDescriptionTypeDef],
     },
     total=False,
 )
 
-CustomRoutingListenerTypeDef = TypedDict(
-    "CustomRoutingListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "PortRanges": List[PortRangeOutputTypeDef],
-    },
-    total=False,
-)
-
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "PortRanges": List[PortRangeOutputTypeDef],
-        "Protocol": ProtocolType,
-        "ClientAffinity": ClientAffinityType,
-    },
-    total=False,
-)
-
 DestinationPortMappingTypeDef = TypedDict(
     "DestinationPortMappingTypeDef",
     {
         "AcceleratorArn": str,
         "AcceleratorSocketAddresses": List[SocketAddressTypeDef],
         "EndpointGroupArn": str,
         "EndpointId": str,
@@ -1346,288 +1202,403 @@
         "DestinationSocketAddress": SocketAddressTypeDef,
         "Protocols": List[CustomRoutingProtocolType],
         "DestinationTrafficState": CustomRoutingDestinationTrafficStateType,
     },
     total=False,
 )
 
-EndpointGroupTypeDef = TypedDict(
-    "EndpointGroupTypeDef",
+RemoveEndpointsRequestRequestTypeDef = TypedDict(
+    "RemoveEndpointsRequestRequestTypeDef",
     {
+        "EndpointIdentifiers": Sequence[EndpointIdentifierTypeDef],
         "EndpointGroupArn": str,
-        "EndpointGroupRegion": str,
-        "EndpointDescriptions": List[EndpointDescriptionTypeDef],
-        "TrafficDialPercentage": float,
-        "HealthCheckPort": int,
-        "HealthCheckProtocol": HealthCheckProtocolType,
-        "HealthCheckPath": str,
-        "HealthCheckIntervalSeconds": int,
-        "ThresholdCount": int,
-        "PortOverrides": List[PortOverrideOutputTypeDef],
+    },
+)
+
+ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = TypedDict(
+    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-RemoveEndpointsRequestRequestTypeDef = TypedDict(
-    "RemoveEndpointsRequestRequestTypeDef",
+ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = TypedDict(
+    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
     {
-        "EndpointIdentifiers": Sequence[EndpointIdentifierTypeDef],
-        "EndpointGroupArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = TypedDict(
+    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
+    "_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    {
+        "AcceleratorArn": str,
+    },
+)
+_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
+    "_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef(
+    _RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+    _OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
+    "_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    {
+        "EndpointId": str,
+        "DestinationAddress": str,
+    },
+)
+_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
+    "_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef(
+    _RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+    _OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+        {
+            "AcceleratorArn": str,
+        },
+    )
+)
+_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+        {
+            "EndpointGroupArn": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef(
+    _RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+    _OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef(
+    _RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+    _OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "AcceleratorArn": str,
+    },
+)
+_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_OptionalListListenersRequestListListenersPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListListenersRequestListListenersPaginateTypeDef(
+    _RequiredListListenersRequestListListenersPaginateTypeDef,
+    _OptionalListListenersRequestListListenersPaginateTypeDef,
+):
+    pass
+
+
 CreateAcceleratorResponseTypeDef = TypedDict(
     "CreateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAcceleratorResponseTypeDef = TypedDict(
     "DescribeAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAcceleratorsResponseTypeDef = TypedDict(
     "ListAcceleratorsResponseTypeDef",
     {
         "Accelerators": List[AcceleratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAcceleratorResponseTypeDef = TypedDict(
     "UpdateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomRoutingAcceleratorsResponseTypeDef = TypedDict(
     "ListCustomRoutingAcceleratorsResponseTypeDef",
     {
         "Accelerators": List[CustomRoutingAcceleratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "UpdateCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdvertiseByoipCidrResponseTypeDef = TypedDict(
     "AdvertiseByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeprovisionByoipCidrResponseTypeDef = TypedDict(
     "DeprovisionByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListByoipCidrsResponseTypeDef = TypedDict(
     "ListByoipCidrsResponseTypeDef",
     {
         "ByoipCidrs": List[ByoipCidrTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisionByoipCidrResponseTypeDef = TypedDict(
     "ProvisionByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WithdrawByoipCidrResponseTypeDef = TypedDict(
     "WithdrawByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
-    "CreateCustomRoutingEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
-    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
-    "ListCustomRoutingEndpointGroupsResponseTypeDef",
-    {
-        "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCustomRoutingListenerResponseTypeDef = TypedDict(
     "CreateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomRoutingListenerResponseTypeDef = TypedDict(
     "DescribeCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomRoutingListenersResponseTypeDef = TypedDict(
     "ListCustomRoutingListenersResponseTypeDef",
     {
         "Listeners": List[CustomRoutingListenerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCustomRoutingListenerResponseTypeDef = TypedDict(
     "UpdateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeListenerResponseTypeDef = TypedDict(
     "DescribeListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
-    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
-    {
-        "DestinationPortMappings": List[DestinationPortMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
-    "ListCustomRoutingPortMappingsResponseTypeDef",
-    {
-        "PortMappings": List[PortMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEndpointGroupResponseTypeDef = TypedDict(
     "CreateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointGroupResponseTypeDef = TypedDict(
     "DescribeEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointGroupsResponseTypeDef = TypedDict(
     "ListEndpointGroupsResponseTypeDef",
     {
         "EndpointGroups": List[EndpointGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointGroupResponseTypeDef = TypedDict(
     "UpdateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
+    "CreateCustomRoutingEndpointGroupResponseTypeDef",
+    {
+        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
+    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
+    {
+        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
+    "ListCustomRoutingEndpointGroupsResponseTypeDef",
+    {
+        "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
+    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
+    {
+        "DestinationPortMappings": List[DestinationPortMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
+    "ListCustomRoutingPortMappingsResponseTypeDef",
+    {
+        "PortMappings": List[PortMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator/type_defs.pyi` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -36,27 +36,27 @@
 
 __all__ = (
     "AcceleratorAttributesTypeDef",
     "AcceleratorEventTypeDef",
     "IpSetTypeDef",
     "CustomRoutingEndpointConfigurationTypeDef",
     "CustomRoutingEndpointDescriptionTypeDef",
+    "ResponseMetadataTypeDef",
     "EndpointConfigurationTypeDef",
     "EndpointDescriptionTypeDef",
     "AdvertiseByoipCidrRequestRequestTypeDef",
     "AllowCustomRoutingTrafficRequestRequestTypeDef",
     "ByoipCidrEventTypeDef",
     "CidrAuthorizationContextTypeDef",
     "TagTypeDef",
     "CustomRoutingDestinationConfigurationTypeDef",
     "PortRangeTypeDef",
     "PortOverrideTypeDef",
     "CustomRoutingAcceleratorAttributesTypeDef",
     "CustomRoutingDestinationDescriptionTypeDef",
-    "PortRangeOutputTypeDef",
     "DeleteAcceleratorRequestRequestTypeDef",
     "DeleteCustomRoutingAcceleratorRequestRequestTypeDef",
     "DeleteCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DeleteCustomRoutingListenerRequestRequestTypeDef",
     "DeleteEndpointGroupRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DenyCustomRoutingTrafficRequestRequestTypeDef",
@@ -66,105 +66,102 @@
     "DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorRequestRequestTypeDef",
     "DescribeCustomRoutingEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingListenerRequestRequestTypeDef",
     "DescribeEndpointGroupRequestRequestTypeDef",
     "DescribeListenerRequestRequestTypeDef",
     "SocketAddressTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "PortOverrideOutputTypeDef",
     "EndpointIdentifierTypeDef",
-    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAcceleratorsRequestRequestTypeDef",
-    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
     "ListByoipCidrsRequestRequestTypeDef",
-    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
     "ListCustomRoutingEndpointGroupsRequestRequestTypeDef",
-    "ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
     "ListCustomRoutingListenersRequestRequestTypeDef",
-    "ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
     "ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef",
-    "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
     "ListCustomRoutingPortMappingsRequestRequestTypeDef",
-    "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
     "ListEndpointGroupsRequestRequestTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAcceleratorAttributesRequestRequestTypeDef",
     "UpdateAcceleratorRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef",
     "UpdateCustomRoutingAcceleratorRequestRequestTypeDef",
     "WithdrawByoipCidrRequestRequestTypeDef",
-    "DescribeAcceleratorAttributesResponseTypeDef",
-    "UpdateAcceleratorAttributesResponseTypeDef",
     "AcceleratorTypeDef",
     "CustomRoutingAcceleratorTypeDef",
     "AddCustomRoutingEndpointsRequestRequestTypeDef",
     "AddCustomRoutingEndpointsResponseTypeDef",
+    "DescribeAcceleratorAttributesResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "UpdateAcceleratorAttributesResponseTypeDef",
     "AddEndpointsRequestRequestTypeDef",
     "AddEndpointsResponseTypeDef",
     "ByoipCidrTypeDef",
     "ProvisionByoipCidrRequestRequestTypeDef",
     "CreateAcceleratorRequestRequestTypeDef",
     "CreateCustomRoutingAcceleratorRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateCustomRoutingEndpointGroupRequestRequestTypeDef",
     "CreateCustomRoutingListenerRequestRequestTypeDef",
     "CreateListenerRequestRequestTypeDef",
+    "CustomRoutingListenerTypeDef",
+    "ListenerTypeDef",
     "UpdateCustomRoutingListenerRequestRequestTypeDef",
     "UpdateListenerRequestRequestTypeDef",
     "CreateEndpointGroupRequestRequestTypeDef",
+    "EndpointGroupTypeDef",
     "UpdateEndpointGroupRequestRequestTypeDef",
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     "CustomRoutingEndpointGroupTypeDef",
-    "CustomRoutingListenerTypeDef",
-    "ListenerTypeDef",
     "DestinationPortMappingTypeDef",
     "PortMappingTypeDef",
-    "EndpointGroupTypeDef",
     "RemoveEndpointsRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
+    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
+    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
+    "ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    "ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    "ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+    "ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
     "CreateAcceleratorResponseTypeDef",
     "DescribeAcceleratorResponseTypeDef",
     "ListAcceleratorsResponseTypeDef",
     "UpdateAcceleratorResponseTypeDef",
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     "ListCustomRoutingAcceleratorsResponseTypeDef",
     "UpdateCustomRoutingAcceleratorResponseTypeDef",
     "AdvertiseByoipCidrResponseTypeDef",
     "DeprovisionByoipCidrResponseTypeDef",
     "ListByoipCidrsResponseTypeDef",
     "ProvisionByoipCidrResponseTypeDef",
     "WithdrawByoipCidrResponseTypeDef",
-    "CreateCustomRoutingEndpointGroupResponseTypeDef",
-    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
-    "ListCustomRoutingEndpointGroupsResponseTypeDef",
     "CreateCustomRoutingListenerResponseTypeDef",
     "DescribeCustomRoutingListenerResponseTypeDef",
     "ListCustomRoutingListenersResponseTypeDef",
     "UpdateCustomRoutingListenerResponseTypeDef",
     "CreateListenerResponseTypeDef",
     "DescribeListenerResponseTypeDef",
     "ListListenersResponseTypeDef",
     "UpdateListenerResponseTypeDef",
-    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
-    "ListCustomRoutingPortMappingsResponseTypeDef",
     "CreateEndpointGroupResponseTypeDef",
     "DescribeEndpointGroupResponseTypeDef",
     "ListEndpointGroupsResponseTypeDef",
     "UpdateEndpointGroupResponseTypeDef",
+    "CreateCustomRoutingEndpointGroupResponseTypeDef",
+    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
+    "ListCustomRoutingEndpointGroupsResponseTypeDef",
+    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
+    "ListCustomRoutingPortMappingsResponseTypeDef",
 )
 
 AcceleratorAttributesTypeDef = TypedDict(
     "AcceleratorAttributesTypeDef",
     {
         "FlowLogsEnabled": bool,
         "FlowLogsS3Bucket": str,
@@ -204,14 +201,25 @@
     "CustomRoutingEndpointDescriptionTypeDef",
     {
         "EndpointId": str,
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
 EndpointConfigurationTypeDef = TypedDict(
     "EndpointConfigurationTypeDef",
     {
         "EndpointId": str,
         "Weight": int,
         "ClientIPPreservationEnabled": bool,
     },
@@ -328,23 +336,14 @@
         "FromPort": int,
         "ToPort": int,
         "Protocols": List[ProtocolType],
     },
     total=False,
 )
 
-PortRangeOutputTypeDef = TypedDict(
-    "PortRangeOutputTypeDef",
-    {
-        "FromPort": int,
-        "ToPort": int,
-    },
-    total=False,
-)
-
 DeleteAcceleratorRequestRequestTypeDef = TypedDict(
     "DeleteAcceleratorRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 
@@ -474,30 +473,14 @@
     {
         "IpAddress": str,
         "Port": int,
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
-PortOverrideOutputTypeDef = TypedDict(
-    "PortOverrideOutputTypeDef",
-    {
-        "ListenerPort": int,
-        "EndpointPort": int,
-    },
-    total=False,
-)
-
 _RequiredEndpointIdentifierTypeDef = TypedDict(
     "_RequiredEndpointIdentifierTypeDef",
     {
         "EndpointId": str,
     },
 )
 _OptionalEndpointIdentifierTypeDef = TypedDict(
@@ -509,56 +492,42 @@
 )
 
 class EndpointIdentifierTypeDef(
     _RequiredEndpointIdentifierTypeDef, _OptionalEndpointIdentifierTypeDef
 ):
     pass
 
-ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = TypedDict(
-    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
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
 
 ListAcceleratorsRequestRequestTypeDef = TypedDict(
     "ListAcceleratorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = TypedDict(
-    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListByoipCidrsRequestRequestTypeDef = TypedDict(
     "ListByoipCidrsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = TypedDict(
-    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomRoutingAcceleratorsRequestRequestTypeDef = TypedDict(
     "ListCustomRoutingAcceleratorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -581,34 +550,14 @@
 
 class ListCustomRoutingEndpointGroupsRequestRequestTypeDef(
     _RequiredListCustomRoutingEndpointGroupsRequestRequestTypeDef,
     _OptionalListCustomRoutingEndpointGroupsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
-    "_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    {
-        "AcceleratorArn": str,
-    },
-)
-_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
-    "_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef(
-    _RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-    _OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
-):
-    pass
-
 _RequiredListCustomRoutingListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingListenersRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListCustomRoutingListenersRequestRequestTypeDef = TypedDict(
@@ -622,35 +571,14 @@
 
 class ListCustomRoutingListenersRequestRequestTypeDef(
     _RequiredListCustomRoutingListenersRequestRequestTypeDef,
     _OptionalListCustomRoutingListenersRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
-    "_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    {
-        "EndpointId": str,
-        "DestinationAddress": str,
-    },
-)
-_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
-    "_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef(
-    _RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-    _OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
-):
-    pass
-
 _RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef",
     {
         "EndpointId": str,
         "DestinationAddress": str,
     },
 )
@@ -665,39 +593,14 @@
 
 class ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef(
     _RequiredListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
     _OptionalListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-        {
-            "AcceleratorArn": str,
-        },
-    )
-)
-_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
-        {
-            "EndpointGroupArn": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef(
-    _RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-    _OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
-):
-    pass
-
 _RequiredListCustomRoutingPortMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredListCustomRoutingPortMappingsRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListCustomRoutingPortMappingsRequestRequestTypeDef = TypedDict(
@@ -712,34 +615,14 @@
 
 class ListCustomRoutingPortMappingsRequestRequestTypeDef(
     _RequiredListCustomRoutingPortMappingsRequestRequestTypeDef,
     _OptionalListCustomRoutingPortMappingsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    {
-        "ListenerArn": str,
-    },
-)
-_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef(
-    _RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-    _OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEndpointGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListEndpointGroupsRequestRequestTypeDef",
     {
         "ListenerArn": str,
     },
 )
 _OptionalListEndpointGroupsRequestRequestTypeDef = TypedDict(
@@ -753,34 +636,14 @@
 
 class ListEndpointGroupsRequestRequestTypeDef(
     _RequiredListEndpointGroupsRequestRequestTypeDef,
     _OptionalListEndpointGroupsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "AcceleratorArn": str,
-    },
-)
-_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_OptionalListListenersRequestListListenersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListListenersRequestListListenersPaginateTypeDef(
-    _RequiredListListenersRequestListListenersPaginateTypeDef,
-    _OptionalListListenersRequestListListenersPaginateTypeDef,
-):
-    pass
-
 _RequiredListListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListListenersRequestRequestTypeDef",
     {
         "AcceleratorArn": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -800,51 +663,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
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
 RemoveCustomRoutingEndpointsRequestRequestTypeDef = TypedDict(
     "RemoveCustomRoutingEndpointsRequestRequestTypeDef",
     {
         "EndpointIds": Sequence[str],
         "EndpointGroupArn": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -939,30 +773,14 @@
 WithdrawByoipCidrRequestRequestTypeDef = TypedDict(
     "WithdrawByoipCidrRequestRequestTypeDef",
     {
         "Cidr": str,
     },
 )
 
-DescribeAcceleratorAttributesResponseTypeDef = TypedDict(
-    "DescribeAcceleratorAttributesResponseTypeDef",
-    {
-        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAcceleratorAttributesResponseTypeDef = TypedDict(
-    "UpdateAcceleratorAttributesResponseTypeDef",
-    {
-        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AcceleratorTypeDef = TypedDict(
     "AcceleratorTypeDef",
     {
         "AcceleratorArn": str,
         "Name": str,
         "IpAddressType": IpAddressTypeType,
         "Enabled": bool,
@@ -1002,15 +820,38 @@
 )
 
 AddCustomRoutingEndpointsResponseTypeDef = TypedDict(
     "AddCustomRoutingEndpointsResponseTypeDef",
     {
         "EndpointDescriptions": List[CustomRoutingEndpointDescriptionTypeDef],
         "EndpointGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAcceleratorAttributesResponseTypeDef = TypedDict(
+    "DescribeAcceleratorAttributesResponseTypeDef",
+    {
+        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
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
+UpdateAcceleratorAttributesResponseTypeDef = TypedDict(
+    "UpdateAcceleratorAttributesResponseTypeDef",
+    {
+        "AcceleratorAttributes": AcceleratorAttributesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddEndpointsRequestRequestTypeDef = TypedDict(
     "AddEndpointsRequestRequestTypeDef",
     {
         "EndpointConfigurations": Sequence[EndpointConfigurationTypeDef],
@@ -1019,15 +860,15 @@
 )
 
 AddEndpointsResponseTypeDef = TypedDict(
     "AddEndpointsResponseTypeDef",
     {
         "EndpointDescriptions": List[EndpointDescriptionTypeDef],
         "EndpointGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ByoipCidrTypeDef = TypedDict(
     "ByoipCidrTypeDef",
     {
         "Cidr": str,
@@ -1088,14 +929,22 @@
 
 class CreateCustomRoutingAcceleratorRequestRequestTypeDef(
     _RequiredCreateCustomRoutingAcceleratorRequestRequestTypeDef,
     _OptionalCreateCustomRoutingAcceleratorRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1137,14 +986,34 @@
 )
 
 class CreateListenerRequestRequestTypeDef(
     _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
 ):
     pass
 
+CustomRoutingListenerTypeDef = TypedDict(
+    "CustomRoutingListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "PortRanges": List[PortRangeTypeDef],
+    },
+    total=False,
+)
+
+ListenerTypeDef = TypedDict(
+    "ListenerTypeDef",
+    {
+        "ListenerArn": str,
+        "PortRanges": List[PortRangeTypeDef],
+        "Protocol": ProtocolType,
+        "ClientAffinity": ClientAffinityType,
+    },
+    total=False,
+)
+
 UpdateCustomRoutingListenerRequestRequestTypeDef = TypedDict(
     "UpdateCustomRoutingListenerRequestRequestTypeDef",
     {
         "ListenerArn": str,
         "PortRanges": Sequence[PortRangeTypeDef],
     },
 )
@@ -1195,14 +1064,31 @@
 
 class CreateEndpointGroupRequestRequestTypeDef(
     _RequiredCreateEndpointGroupRequestRequestTypeDef,
     _OptionalCreateEndpointGroupRequestRequestTypeDef,
 ):
     pass
 
+EndpointGroupTypeDef = TypedDict(
+    "EndpointGroupTypeDef",
+    {
+        "EndpointGroupArn": str,
+        "EndpointGroupRegion": str,
+        "EndpointDescriptions": List[EndpointDescriptionTypeDef],
+        "TrafficDialPercentage": float,
+        "HealthCheckPort": int,
+        "HealthCheckProtocol": HealthCheckProtocolType,
+        "HealthCheckPath": str,
+        "HealthCheckIntervalSeconds": int,
+        "ThresholdCount": int,
+        "PortOverrides": List[PortOverrideTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateEndpointGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEndpointGroupRequestRequestTypeDef",
     {
         "EndpointGroupArn": str,
     },
 )
 _OptionalUpdateEndpointGroupRequestRequestTypeDef = TypedDict(
@@ -1226,57 +1112,37 @@
 ):
     pass
 
 DescribeCustomRoutingAcceleratorAttributesResponseTypeDef = TypedDict(
     "DescribeCustomRoutingAcceleratorAttributesResponseTypeDef",
     {
         "AcceleratorAttributes": CustomRoutingAcceleratorAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCustomRoutingAcceleratorAttributesResponseTypeDef = TypedDict(
     "UpdateCustomRoutingAcceleratorAttributesResponseTypeDef",
     {
         "AcceleratorAttributes": CustomRoutingAcceleratorAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomRoutingEndpointGroupTypeDef = TypedDict(
     "CustomRoutingEndpointGroupTypeDef",
     {
         "EndpointGroupArn": str,
         "EndpointGroupRegion": str,
         "DestinationDescriptions": List[CustomRoutingDestinationDescriptionTypeDef],
         "EndpointDescriptions": List[CustomRoutingEndpointDescriptionTypeDef],
     },
     total=False,
 )
 
-CustomRoutingListenerTypeDef = TypedDict(
-    "CustomRoutingListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "PortRanges": List[PortRangeOutputTypeDef],
-    },
-    total=False,
-)
-
-ListenerTypeDef = TypedDict(
-    "ListenerTypeDef",
-    {
-        "ListenerArn": str,
-        "PortRanges": List[PortRangeOutputTypeDef],
-        "Protocol": ProtocolType,
-        "ClientAffinity": ClientAffinityType,
-    },
-    total=False,
-)
-
 DestinationPortMappingTypeDef = TypedDict(
     "DestinationPortMappingTypeDef",
     {
         "AcceleratorArn": str,
         "AcceleratorSocketAddresses": List[SocketAddressTypeDef],
         "EndpointGroupArn": str,
         "EndpointId": str,
@@ -1297,288 +1163,393 @@
         "DestinationSocketAddress": SocketAddressTypeDef,
         "Protocols": List[CustomRoutingProtocolType],
         "DestinationTrafficState": CustomRoutingDestinationTrafficStateType,
     },
     total=False,
 )
 
-EndpointGroupTypeDef = TypedDict(
-    "EndpointGroupTypeDef",
+RemoveEndpointsRequestRequestTypeDef = TypedDict(
+    "RemoveEndpointsRequestRequestTypeDef",
     {
+        "EndpointIdentifiers": Sequence[EndpointIdentifierTypeDef],
         "EndpointGroupArn": str,
-        "EndpointGroupRegion": str,
-        "EndpointDescriptions": List[EndpointDescriptionTypeDef],
-        "TrafficDialPercentage": float,
-        "HealthCheckPort": int,
-        "HealthCheckProtocol": HealthCheckProtocolType,
-        "HealthCheckPath": str,
-        "HealthCheckIntervalSeconds": int,
-        "ThresholdCount": int,
-        "PortOverrides": List[PortOverrideOutputTypeDef],
+    },
+)
+
+ListAcceleratorsRequestListAcceleratorsPaginateTypeDef = TypedDict(
+    "ListAcceleratorsRequestListAcceleratorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-RemoveEndpointsRequestRequestTypeDef = TypedDict(
-    "RemoveEndpointsRequestRequestTypeDef",
+ListByoipCidrsRequestListByoipCidrsPaginateTypeDef = TypedDict(
+    "ListByoipCidrsRequestListByoipCidrsPaginateTypeDef",
     {
-        "EndpointIdentifiers": Sequence[EndpointIdentifierTypeDef],
-        "EndpointGroupArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef = TypedDict(
+    "ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
+    "_RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    {
+        "AcceleratorArn": str,
+    },
+)
+_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef = TypedDict(
+    "_OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef(
+    _RequiredListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+    _OptionalListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+):
+    pass
+
+_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
+    "_RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    {
+        "EndpointId": str,
+        "DestinationAddress": str,
+    },
+)
+_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef = TypedDict(
+    "_OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef(
+    _RequiredListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+    _OptionalListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+):
+    pass
+
+_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+        {
+            "AcceleratorArn": str,
+        },
+    )
+)
+_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef",
+        {
+            "EndpointGroupArn": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef(
+    _RequiredListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+    _OptionalListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+):
+    pass
+
+_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    {
+        "ListenerArn": str,
+    },
+)
+_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef(
+    _RequiredListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+    _OptionalListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
     {
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AcceleratorArn": str,
+    },
+)
+_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_OptionalListListenersRequestListListenersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListListenersRequestListListenersPaginateTypeDef(
+    _RequiredListListenersRequestListListenersPaginateTypeDef,
+    _OptionalListListenersRequestListListenersPaginateTypeDef,
+):
+    pass
+
 CreateAcceleratorResponseTypeDef = TypedDict(
     "CreateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAcceleratorResponseTypeDef = TypedDict(
     "DescribeAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAcceleratorsResponseTypeDef = TypedDict(
     "ListAcceleratorsResponseTypeDef",
     {
         "Accelerators": List[AcceleratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAcceleratorResponseTypeDef = TypedDict(
     "UpdateAcceleratorResponseTypeDef",
     {
         "Accelerator": AcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "CreateCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "DescribeCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomRoutingAcceleratorsResponseTypeDef = TypedDict(
     "ListCustomRoutingAcceleratorsResponseTypeDef",
     {
         "Accelerators": List[CustomRoutingAcceleratorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCustomRoutingAcceleratorResponseTypeDef = TypedDict(
     "UpdateCustomRoutingAcceleratorResponseTypeDef",
     {
         "Accelerator": CustomRoutingAcceleratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdvertiseByoipCidrResponseTypeDef = TypedDict(
     "AdvertiseByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeprovisionByoipCidrResponseTypeDef = TypedDict(
     "DeprovisionByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListByoipCidrsResponseTypeDef = TypedDict(
     "ListByoipCidrsResponseTypeDef",
     {
         "ByoipCidrs": List[ByoipCidrTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ProvisionByoipCidrResponseTypeDef = TypedDict(
     "ProvisionByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WithdrawByoipCidrResponseTypeDef = TypedDict(
     "WithdrawByoipCidrResponseTypeDef",
     {
         "ByoipCidr": ByoipCidrTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
-    "CreateCustomRoutingEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
-    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
-    {
-        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
-    "ListCustomRoutingEndpointGroupsResponseTypeDef",
-    {
-        "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCustomRoutingListenerResponseTypeDef = TypedDict(
     "CreateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomRoutingListenerResponseTypeDef = TypedDict(
     "DescribeCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCustomRoutingListenersResponseTypeDef = TypedDict(
     "ListCustomRoutingListenersResponseTypeDef",
     {
         "Listeners": List[CustomRoutingListenerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCustomRoutingListenerResponseTypeDef = TypedDict(
     "UpdateCustomRoutingListenerResponseTypeDef",
     {
         "Listener": CustomRoutingListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeListenerResponseTypeDef = TypedDict(
     "DescribeListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "Listeners": List[ListenerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "Listener": ListenerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
-    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
-    {
-        "DestinationPortMappings": List[DestinationPortMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
-    "ListCustomRoutingPortMappingsResponseTypeDef",
-    {
-        "PortMappings": List[PortMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEndpointGroupResponseTypeDef = TypedDict(
     "CreateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEndpointGroupResponseTypeDef = TypedDict(
     "DescribeEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEndpointGroupsResponseTypeDef = TypedDict(
     "ListEndpointGroupsResponseTypeDef",
     {
         "EndpointGroups": List[EndpointGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEndpointGroupResponseTypeDef = TypedDict(
     "UpdateEndpointGroupResponseTypeDef",
     {
         "EndpointGroup": EndpointGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
+    "CreateCustomRoutingEndpointGroupResponseTypeDef",
+    {
+        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomRoutingEndpointGroupResponseTypeDef = TypedDict(
+    "DescribeCustomRoutingEndpointGroupResponseTypeDef",
+    {
+        "EndpointGroup": CustomRoutingEndpointGroupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomRoutingEndpointGroupsResponseTypeDef = TypedDict(
+    "ListCustomRoutingEndpointGroupsResponseTypeDef",
+    {
+        "EndpointGroups": List[CustomRoutingEndpointGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomRoutingPortMappingsByDestinationResponseTypeDef = TypedDict(
+    "ListCustomRoutingPortMappingsByDestinationResponseTypeDef",
+    {
+        "DestinationPortMappings": List[DestinationPortMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomRoutingPortMappingsResponseTypeDef = TypedDict(
+    "ListCustomRoutingPortMappingsResponseTypeDef",
+    {
+        "PortMappings": List[PortMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/PKG-INFO` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-globalaccelerator
-Version: 1.28.12
-Summary: Type annotations for boto3.GlobalAccelerator 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GlobalAccelerator 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-globalaccelerator.svg?color=blue)](https://pypi.org/project/mypy-boto3-globalaccelerator)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-globalaccelerator)](https://pepy.tech/project/mypy-boto3-globalaccelerator)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GlobalAccelerator 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
+[boto3.GlobalAccelerator 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/globalaccelerator.html#GlobalAccelerator)
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
 [mypy-boto3-globalaccelerator docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_globalaccelerator/).
 
 See how it helps to find and fix potential bugs:
 
@@ -368,27 +368,27 @@
 ```python
 from mypy_boto3_globalaccelerator.type_defs import (
     AcceleratorAttributesTypeDef,
     AcceleratorEventTypeDef,
     IpSetTypeDef,
     CustomRoutingEndpointConfigurationTypeDef,
     CustomRoutingEndpointDescriptionTypeDef,
+    ResponseMetadataTypeDef,
     EndpointConfigurationTypeDef,
     EndpointDescriptionTypeDef,
     AdvertiseByoipCidrRequestRequestTypeDef,
     AllowCustomRoutingTrafficRequestRequestTypeDef,
     ByoipCidrEventTypeDef,
     CidrAuthorizationContextTypeDef,
     TagTypeDef,
     CustomRoutingDestinationConfigurationTypeDef,
     PortRangeTypeDef,
     PortOverrideTypeDef,
     CustomRoutingAcceleratorAttributesTypeDef,
     CustomRoutingDestinationDescriptionTypeDef,
-    PortRangeOutputTypeDef,
     DeleteAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingAcceleratorRequestRequestTypeDef,
     DeleteCustomRoutingEndpointGroupRequestRequestTypeDef,
     DeleteCustomRoutingListenerRequestRequestTypeDef,
     DeleteEndpointGroupRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DenyCustomRoutingTrafficRequestRequestTypeDef,
@@ -398,105 +398,102 @@
     DescribeCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorRequestRequestTypeDef,
     DescribeCustomRoutingEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingListenerRequestRequestTypeDef,
     DescribeEndpointGroupRequestRequestTypeDef,
     DescribeListenerRequestRequestTypeDef,
     SocketAddressTypeDef,
-    EmptyResponseMetadataTypeDef,
-    PortOverrideOutputTypeDef,
     EndpointIdentifierTypeDef,
-    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAcceleratorsRequestRequestTypeDef,
-    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
     ListByoipCidrsRequestRequestTypeDef,
-    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
     ListCustomRoutingAcceleratorsRequestRequestTypeDef,
     ListCustomRoutingEndpointGroupsRequestRequestTypeDef,
-    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
     ListCustomRoutingListenersRequestRequestTypeDef,
-    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
     ListCustomRoutingPortMappingsByDestinationRequestRequestTypeDef,
-    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
     ListCustomRoutingPortMappingsRequestRequestTypeDef,
-    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
     ListEndpointGroupsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    PaginatorConfigTypeDef,
     RemoveCustomRoutingEndpointsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAcceleratorAttributesRequestRequestTypeDef,
     UpdateAcceleratorRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorAttributesRequestRequestTypeDef,
     UpdateCustomRoutingAcceleratorRequestRequestTypeDef,
     WithdrawByoipCidrRequestRequestTypeDef,
-    DescribeAcceleratorAttributesResponseTypeDef,
-    UpdateAcceleratorAttributesResponseTypeDef,
     AcceleratorTypeDef,
     CustomRoutingAcceleratorTypeDef,
     AddCustomRoutingEndpointsRequestRequestTypeDef,
     AddCustomRoutingEndpointsResponseTypeDef,
+    DescribeAcceleratorAttributesResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    UpdateAcceleratorAttributesResponseTypeDef,
     AddEndpointsRequestRequestTypeDef,
     AddEndpointsResponseTypeDef,
     ByoipCidrTypeDef,
     ProvisionByoipCidrRequestRequestTypeDef,
     CreateAcceleratorRequestRequestTypeDef,
     CreateCustomRoutingAcceleratorRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateCustomRoutingEndpointGroupRequestRequestTypeDef,
     CreateCustomRoutingListenerRequestRequestTypeDef,
     CreateListenerRequestRequestTypeDef,
+    CustomRoutingListenerTypeDef,
+    ListenerTypeDef,
     UpdateCustomRoutingListenerRequestRequestTypeDef,
     UpdateListenerRequestRequestTypeDef,
     CreateEndpointGroupRequestRequestTypeDef,
+    EndpointGroupTypeDef,
     UpdateEndpointGroupRequestRequestTypeDef,
     DescribeCustomRoutingAcceleratorAttributesResponseTypeDef,
     UpdateCustomRoutingAcceleratorAttributesResponseTypeDef,
     CustomRoutingEndpointGroupTypeDef,
-    CustomRoutingListenerTypeDef,
-    ListenerTypeDef,
     DestinationPortMappingTypeDef,
     PortMappingTypeDef,
-    EndpointGroupTypeDef,
     RemoveEndpointsRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    ListAcceleratorsRequestListAcceleratorsPaginateTypeDef,
+    ListByoipCidrsRequestListByoipCidrsPaginateTypeDef,
+    ListCustomRoutingAcceleratorsRequestListCustomRoutingAcceleratorsPaginateTypeDef,
+    ListCustomRoutingListenersRequestListCustomRoutingListenersPaginateTypeDef,
+    ListCustomRoutingPortMappingsByDestinationRequestListCustomRoutingPortMappingsByDestinationPaginateTypeDef,
+    ListCustomRoutingPortMappingsRequestListCustomRoutingPortMappingsPaginateTypeDef,
+    ListEndpointGroupsRequestListEndpointGroupsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
     CreateAcceleratorResponseTypeDef,
     DescribeAcceleratorResponseTypeDef,
     ListAcceleratorsResponseTypeDef,
     UpdateAcceleratorResponseTypeDef,
     CreateCustomRoutingAcceleratorResponseTypeDef,
     DescribeCustomRoutingAcceleratorResponseTypeDef,
     ListCustomRoutingAcceleratorsResponseTypeDef,
     UpdateCustomRoutingAcceleratorResponseTypeDef,
     AdvertiseByoipCidrResponseTypeDef,
     DeprovisionByoipCidrResponseTypeDef,
     ListByoipCidrsResponseTypeDef,
     ProvisionByoipCidrResponseTypeDef,
     WithdrawByoipCidrResponseTypeDef,
-    CreateCustomRoutingEndpointGroupResponseTypeDef,
-    DescribeCustomRoutingEndpointGroupResponseTypeDef,
-    ListCustomRoutingEndpointGroupsResponseTypeDef,
     CreateCustomRoutingListenerResponseTypeDef,
     DescribeCustomRoutingListenerResponseTypeDef,
     ListCustomRoutingListenersResponseTypeDef,
     UpdateCustomRoutingListenerResponseTypeDef,
     CreateListenerResponseTypeDef,
     DescribeListenerResponseTypeDef,
     ListListenersResponseTypeDef,
     UpdateListenerResponseTypeDef,
-    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
-    ListCustomRoutingPortMappingsResponseTypeDef,
     CreateEndpointGroupResponseTypeDef,
     DescribeEndpointGroupResponseTypeDef,
     ListEndpointGroupsResponseTypeDef,
     UpdateEndpointGroupResponseTypeDef,
+    CreateCustomRoutingEndpointGroupResponseTypeDef,
+    DescribeCustomRoutingEndpointGroupResponseTypeDef,
+    ListCustomRoutingEndpointGroupsResponseTypeDef,
+    ListCustomRoutingPortMappingsByDestinationResponseTypeDef,
+    ListCustomRoutingPortMappingsResponseTypeDef,
 )
 
 
 def get_structure() -> AcceleratorAttributesTypeDef:
     return {...}
 ```
```

### Comparing `mypy-boto3-globalaccelerator-1.28.12/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt` & `mypy-boto3-globalaccelerator-1.28.15/mypy_boto3_globalaccelerator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-globalaccelerator-1.28.12/setup.py` & `mypy-boto3-globalaccelerator-1.28.15/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-globalaccelerator",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_globalaccelerator"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GlobalAccelerator 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.GlobalAccelerator 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

