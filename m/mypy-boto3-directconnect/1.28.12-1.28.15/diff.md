# Comparing `tmp/mypy-boto3-directconnect-1.28.12.tar.gz` & `tmp/mypy-boto3-directconnect-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-directconnect-1.28.12.tar", last modified: Thu Jul 27 05:34:34 2023, max compression
+gzip compressed data, was "mypy-boto3-directconnect-1.28.15.tar", last modified: Fri Jul 28 20:42:37 2023, max compression
```

## Comparing `mypy-boto3-directconnect-1.28.12.tar` & `mypy-boto3-directconnect-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.556533 mypy-boto3-directconnect-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20324 2023-07-27 05:34:34.556533 mypy-boto3-directconnect-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.544533 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47262 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55635 2023-07-27 05:20:15.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55586 2023-07-27 05:20:15.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:34.556533 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20324 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-27 05:34:34.000000 mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:34.556533 mypy-boto3-directconnect-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 05:20:14.000000 mypy-boto3-directconnect-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.980960 mypy-boto3-directconnect-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:22:56.000000 mypy-boto3-directconnect-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20226 2023-07-28 20:42:37.980960 mypy-boto3-directconnect-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18715 2023-07-28 20:22:56.000000 mypy-boto3-directconnect-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.972960 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-28 20:22:56.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-28 20:22:56.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-28 20:22:56.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47070 2023-07-28 20:22:57.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46997 2023-07-28 20:22:56.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-07-28 20:22:57.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10896 2023-07-28 20:22:57.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5108 2023-07-28 20:22:57.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-07-28 20:22:57.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:22:56.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54813 2023-07-28 20:22:59.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54766 2023-07-28 20:22:58.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:22:56.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:37.980960 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20226 2023-07-28 20:42:37.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-28 20:42:37.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:37.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:37.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-28 20:42:37.000000 mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:37.980960 mypy-boto3-directconnect-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-28 20:22:55.000000 mypy-boto3-directconnect-1.28.15/setup.py
```

### Comparing `mypy-boto3-directconnect-1.28.12/LICENSE` & `mypy-boto3-directconnect-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.12/PKG-INFO` & `mypy-boto3-directconnect-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-directconnect
-Version: 1.28.12
-Summary: Type annotations for boto3.DirectConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DirectConnect 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-directconnect)](https://pepy.tech/project/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,138 +350,136 @@
 
 `mypy_boto3_directconnect.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
+    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
-    TagOutputTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
-    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
-    RouteFilterPrefixOutputTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
-    LoaResponseMetadataTypeDef,
     LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
+    DeleteInterconnectResponseTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
+    LoaResponseTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
+    InterconnectResponseTypeDef,
+    InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
+    ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
-    DisassociateMacSecKeyResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionTypeDef,
-    InterconnectResponseMetadataTypeDef,
-    InterconnectTypeDef,
-    ResourceTagTypeDef,
+    DisassociateMacSecKeyResponseTypeDef,
+    DirectConnectGatewayAssociationProposalTypeDef,
+    DirectConnectGatewayAssociationTypeDef,
+    VirtualInterfaceResponseTypeDef,
+    VirtualInterfaceTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
-    DirectConnectGatewayAssociationProposalTypeDef,
-    DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
-    VirtualInterfaceTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
+    InterconnectsTypeDef,
     AllocatePrivateVirtualInterfaceRequestRequestTypeDef,
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
+    DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagTypeDef,
-    InterconnectsTypeDef,
-    DescribeTagsResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
```

### Comparing `mypy-boto3-directconnect-1.28.12/README.md` & `mypy-boto3-directconnect-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-directconnect)](https://pepy.tech/project/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -318,138 +318,136 @@
 
 `mypy_boto3_directconnect.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
+    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
-    TagOutputTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
-    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
-    RouteFilterPrefixOutputTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
-    LoaResponseMetadataTypeDef,
     LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
+    DeleteInterconnectResponseTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
+    LoaResponseTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
+    InterconnectResponseTypeDef,
+    InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
+    ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
-    DisassociateMacSecKeyResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionTypeDef,
-    InterconnectResponseMetadataTypeDef,
-    InterconnectTypeDef,
-    ResourceTagTypeDef,
+    DisassociateMacSecKeyResponseTypeDef,
+    DirectConnectGatewayAssociationProposalTypeDef,
+    DirectConnectGatewayAssociationTypeDef,
+    VirtualInterfaceResponseTypeDef,
+    VirtualInterfaceTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
-    DirectConnectGatewayAssociationProposalTypeDef,
-    DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
-    VirtualInterfaceTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
+    InterconnectsTypeDef,
     AllocatePrivateVirtualInterfaceRequestRequestTypeDef,
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
+    DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagTypeDef,
-    InterconnectsTypeDef,
-    DescribeTagsResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
```

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__init__.py` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__init__.pyi` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/__main__.py` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DirectConnect 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.DirectConnect 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect\nOther"
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

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/client.py` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     AllocateTransitVirtualInterfaceResultTypeDef,
     AssociateMacSecKeyResponseTypeDef,
     ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionsTypeDef,
     CreateBGPPeerResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     CreateTransitVirtualInterfaceResultTypeDef,
     DeleteBGPPeerResponseTypeDef,
@@ -51,20 +51,20 @@
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DisassociateMacSecKeyResponseTypeDef,
-    InterconnectResponseMetadataTypeDef,
+    InterconnectResponseTypeDef,
     InterconnectsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagsTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
-    LoaResponseMetadataTypeDef,
+    LoaResponseTypeDef,
     LocationsTypeDef,
     NewBGPPeerTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
@@ -72,15 +72,15 @@
     RouteFilterPrefixTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     TagTypeDef,
     UpdateDirectConnectGatewayAssociationResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     VirtualGatewaysTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceResponseTypeDef,
     VirtualInterfacesTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -142,15 +142,15 @@
         self,
         *,
         bandwidth: str,
         connectionName: str,
         ownerAccount: str,
         interconnectId: str,
         vlan: int
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_connection_on_interconnect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_connection_on_interconnect)
         """
 
@@ -159,45 +159,45 @@
         *,
         connectionId: str,
         ownerAccount: str,
         bandwidth: str,
         connectionName: str,
         vlan: int,
         tags: Sequence[TagTypeDef] = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Creates a hosted connection on the specified interconnect or a link aggregation
         group (LAG) of interconnects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_hosted_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_hosted_connection)
         """
 
     def allocate_private_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a private virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_private_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_private_virtual_interface)
         """
 
     def allocate_public_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a public virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_public_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_public_virtual_interface)
         """
@@ -215,25 +215,25 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_transit_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_transit_virtual_interface)
         """
 
     def associate_connection_with_lag(
         self, *, connectionId: str, lagId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Associates an existing connection with a link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_connection_with_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#associate_connection_with_lag)
         """
 
     def associate_hosted_connection(
         self, *, connectionId: str, parentConnectionId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Associates a hosted connection and its virtual interfaces with a link
         aggregation group (LAG) or interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_hosted_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#associate_hosted_connection)
         """
@@ -247,15 +247,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_mac_sec_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#associate_mac_sec_key)
         """
 
     def associate_virtual_interface(
         self, *, virtualInterfaceId: str, connectionId: str
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Associates a virtual interface with a specified link aggregation group (LAG) or
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#associate_virtual_interface)
         """
@@ -348,15 +348,15 @@
         location: str,
         bandwidth: str,
         connectionName: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
         requestMACSec: bool = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Creates a connection between a customer network and a specific Direct Connect
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_connection)
         """
@@ -410,15 +410,15 @@
         *,
         interconnectName: str,
         bandwidth: str,
         location: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...
-    ) -> InterconnectResponseMetadataTypeDef:
+    ) -> InterconnectResponseTypeDef:
         """
         Creates an interconnect between an Direct Connect Partner's network and a
         specific Direct Connect location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_interconnect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_interconnect)
         """
@@ -431,37 +431,37 @@
         connectionsBandwidth: str,
         lagName: str,
         connectionId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         childConnectionTags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
         requestMACSec: bool = ...
-    ) -> LagResponseMetadataTypeDef:
+    ) -> LagResponseTypeDef:
         """
         Creates a link aggregation group (LAG) with the specified number of bundled
         physical dedicated connections between the customer network and a specific
         Direct Connect location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_lag)
         """
 
     def create_private_virtual_interface(
         self, *, connectionId: str, newPrivateVirtualInterface: NewPrivateVirtualInterfaceTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Creates a private virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_private_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_private_virtual_interface)
         """
 
     def create_public_virtual_interface(
         self, *, connectionId: str, newPublicVirtualInterface: NewPublicVirtualInterfaceTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Creates a public virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_public_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_public_virtual_interface)
         """
 
@@ -487,15 +487,15 @@
         Deletes the specified BGP peer on the specified virtual interface with the
         specified customer address and ASN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_bgp_peer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#delete_bgp_peer)
         """
 
-    def delete_connection(self, *, connectionId: str) -> ConnectionResponseMetadataTypeDef:
+    def delete_connection(self, *, connectionId: str) -> ConnectionResponseTypeDef:
         """
         Deletes the specified connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#delete_connection)
         """
 
@@ -539,15 +539,15 @@
         """
         Deletes the specified interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_interconnect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#delete_interconnect)
         """
 
-    def delete_lag(self, *, lagId: str) -> LagResponseMetadataTypeDef:
+    def delete_lag(self, *, lagId: str) -> LagResponseTypeDef:
         """
         Deletes the specified link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#delete_lag)
         """
 
@@ -704,15 +704,15 @@
 
     def describe_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
         loaContentType: Literal["application/pdf"] = ...
-    ) -> LoaResponseMetadataTypeDef:
+    ) -> LoaResponseTypeDef:
         """
         Gets the LOA-CFA for a connection, interconnect, or link aggregation group
         (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_loa)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#describe_loa)
         """
@@ -759,15 +759,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_virtual_interfaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#describe_virtual_interfaces)
         """
 
     def disassociate_connection_from_lag(
         self, *, connectionId: str, lagId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Disassociates a connection from a link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.disassociate_connection_from_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#disassociate_connection_from_lag)
         """
 
@@ -853,15 +853,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#untag_resource)
         """
 
     def update_connection(
         self, *, connectionId: str, connectionName: str = ..., encryptionMode: str = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Updates the Direct Connect dedicated connection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#update_connection)
         """
 
@@ -887,30 +887,30 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_direct_connect_gateway_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#update_direct_connect_gateway_association)
         """
 
     def update_lag(
         self, *, lagId: str, lagName: str = ..., minimumLinks: int = ..., encryptionMode: str = ...
-    ) -> LagResponseMetadataTypeDef:
+    ) -> LagResponseTypeDef:
         """
         Updates the attributes of the specified link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#update_lag)
         """
 
     def update_virtual_interface_attributes(
         self,
         *,
         virtualInterfaceId: str,
         mtu: int = ...,
         enableSiteLink: bool = ...,
         virtualInterfaceName: str = ...
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Updates the specified attributes of the specified virtual private interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_virtual_interface_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#update_virtual_interface_attributes)
         """
```

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/client.pyi` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     AllocateTransitVirtualInterfaceResultTypeDef,
     AssociateMacSecKeyResponseTypeDef,
     ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionsTypeDef,
     CreateBGPPeerResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     CreateTransitVirtualInterfaceResultTypeDef,
     DeleteBGPPeerResponseTypeDef,
@@ -51,20 +51,20 @@
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DisassociateMacSecKeyResponseTypeDef,
-    InterconnectResponseMetadataTypeDef,
+    InterconnectResponseTypeDef,
     InterconnectsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagsTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
-    LoaResponseMetadataTypeDef,
+    LoaResponseTypeDef,
     LocationsTypeDef,
     NewBGPPeerTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
@@ -72,15 +72,15 @@
     RouteFilterPrefixTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     TagTypeDef,
     UpdateDirectConnectGatewayAssociationResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     VirtualGatewaysTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceResponseTypeDef,
     VirtualInterfacesTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -136,15 +136,15 @@
         self,
         *,
         bandwidth: str,
         connectionName: str,
         ownerAccount: str,
         interconnectId: str,
         vlan: int
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_connection_on_interconnect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_connection_on_interconnect)
         """
     def allocate_hosted_connection(
@@ -152,43 +152,43 @@
         *,
         connectionId: str,
         ownerAccount: str,
         bandwidth: str,
         connectionName: str,
         vlan: int,
         tags: Sequence[TagTypeDef] = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Creates a hosted connection on the specified interconnect or a link aggregation
         group (LAG) of interconnects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_hosted_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_hosted_connection)
         """
     def allocate_private_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a private virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_private_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_private_virtual_interface)
         """
     def allocate_public_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a public virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_public_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_public_virtual_interface)
         """
@@ -204,24 +204,24 @@
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_transit_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#allocate_transit_virtual_interface)
         """
     def associate_connection_with_lag(
         self, *, connectionId: str, lagId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Associates an existing connection with a link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_connection_with_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#associate_connection_with_lag)
         """
     def associate_hosted_connection(
         self, *, connectionId: str, parentConnectionId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Associates a hosted connection and its virtual interfaces with a link
         aggregation group (LAG) or interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_hosted_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#associate_hosted_connection)
         """
@@ -233,15 +233,15 @@
         Association Key (CAK) pair with an Direct Connect dedicated connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_mac_sec_key)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#associate_mac_sec_key)
         """
     def associate_virtual_interface(
         self, *, virtualInterfaceId: str, connectionId: str
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Associates a virtual interface with a specified link aggregation group (LAG) or
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#associate_virtual_interface)
         """
@@ -325,15 +325,15 @@
         location: str,
         bandwidth: str,
         connectionName: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
         requestMACSec: bool = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Creates a connection between a customer network and a specific Direct Connect
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_connection)
         """
@@ -383,15 +383,15 @@
         *,
         interconnectName: str,
         bandwidth: str,
         location: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...
-    ) -> InterconnectResponseMetadataTypeDef:
+    ) -> InterconnectResponseTypeDef:
         """
         Creates an interconnect between an Direct Connect Partner's network and a
         specific Direct Connect location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_interconnect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_interconnect)
         """
@@ -403,35 +403,35 @@
         connectionsBandwidth: str,
         lagName: str,
         connectionId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         childConnectionTags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
         requestMACSec: bool = ...
-    ) -> LagResponseMetadataTypeDef:
+    ) -> LagResponseTypeDef:
         """
         Creates a link aggregation group (LAG) with the specified number of bundled
         physical dedicated connections between the customer network and a specific
         Direct Connect location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_lag)
         """
     def create_private_virtual_interface(
         self, *, connectionId: str, newPrivateVirtualInterface: NewPrivateVirtualInterfaceTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Creates a private virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_private_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_private_virtual_interface)
         """
     def create_public_virtual_interface(
         self, *, connectionId: str, newPublicVirtualInterface: NewPublicVirtualInterfaceTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Creates a public virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_public_virtual_interface)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#create_public_virtual_interface)
         """
     def create_transit_virtual_interface(
@@ -454,15 +454,15 @@
         """
         Deletes the specified BGP peer on the specified virtual interface with the
         specified customer address and ASN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_bgp_peer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#delete_bgp_peer)
         """
-    def delete_connection(self, *, connectionId: str) -> ConnectionResponseMetadataTypeDef:
+    def delete_connection(self, *, connectionId: str) -> ConnectionResponseTypeDef:
         """
         Deletes the specified connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#delete_connection)
         """
     def delete_direct_connect_gateway(
@@ -501,15 +501,15 @@
     def delete_interconnect(self, *, interconnectId: str) -> DeleteInterconnectResponseTypeDef:
         """
         Deletes the specified interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_interconnect)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#delete_interconnect)
         """
-    def delete_lag(self, *, lagId: str) -> LagResponseMetadataTypeDef:
+    def delete_lag(self, *, lagId: str) -> LagResponseTypeDef:
         """
         Deletes the specified link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#delete_lag)
         """
     def delete_virtual_interface(
@@ -652,15 +652,15 @@
         """
     def describe_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
         loaContentType: Literal["application/pdf"] = ...
-    ) -> LoaResponseMetadataTypeDef:
+    ) -> LoaResponseTypeDef:
         """
         Gets the LOA-CFA for a connection, interconnect, or link aggregation group
         (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_loa)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#describe_loa)
         """
@@ -701,15 +701,15 @@
         Displays all virtual interfaces for an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_virtual_interfaces)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#describe_virtual_interfaces)
         """
     def disassociate_connection_from_lag(
         self, *, connectionId: str, lagId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Disassociates a connection from a link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.disassociate_connection_from_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#disassociate_connection_from_lag)
         """
     def disassociate_mac_sec_key(
@@ -787,15 +787,15 @@
         Removes one or more tags from the specified Direct Connect resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.untag_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#untag_resource)
         """
     def update_connection(
         self, *, connectionId: str, connectionName: str = ..., encryptionMode: str = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Updates the Direct Connect dedicated connection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_connection)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#update_connection)
         """
     def update_direct_connect_gateway(
@@ -818,29 +818,29 @@
         Updates the specified attributes of the Direct Connect gateway association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_direct_connect_gateway_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#update_direct_connect_gateway_association)
         """
     def update_lag(
         self, *, lagId: str, lagName: str = ..., minimumLinks: int = ..., encryptionMode: str = ...
-    ) -> LagResponseMetadataTypeDef:
+    ) -> LagResponseTypeDef:
         """
         Updates the attributes of the specified link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_lag)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#update_lag)
         """
     def update_virtual_interface_attributes(
         self,
         *,
         virtualInterfaceId: str,
         mtu: int = ...,
         enableSiteLink: bool = ...,
         virtualInterfaceName: str = ...
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Updates the specified attributes of the specified virtual private interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_virtual_interface_attributes)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/client/#update_virtual_interface_attributes)
         """
     @overload
```

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/literals.py` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/literals.pyi` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/paginator.py` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,71 +36,66 @@
 
 __all__ = (
     "DescribeDirectConnectGatewayAssociationsPaginator",
     "DescribeDirectConnectGatewayAttachmentsPaginator",
     "DescribeDirectConnectGatewaysPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class DescribeDirectConnectGatewayAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectConnectGatewayAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
         """
 
-
 class DescribeDirectConnectGatewayAttachmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
     """
 
     def paginate(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectConnectGatewayAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
         """
 
-
 class DescribeDirectConnectGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayspaginator)
     """
 
     def paginate(
-        self, *, directConnectGatewayId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, directConnectGatewayId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectConnectGatewaysResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayspaginator)
         """
```

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/paginator.pyi` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,66 +36,71 @@
 
 __all__ = (
     "DescribeDirectConnectGatewayAssociationsPaginator",
     "DescribeDirectConnectGatewayAttachmentsPaginator",
     "DescribeDirectConnectGatewaysPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class DescribeDirectConnectGatewayAssociationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
     """
 
     def paginate(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectConnectGatewayAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
         """
 
+
 class DescribeDirectConnectGatewayAttachmentsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
     """
 
     def paginate(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectConnectGatewayAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
         """
 
+
 class DescribeDirectConnectGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayspaginator)
     """
 
     def paginate(
-        self, *, directConnectGatewayId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, directConnectGatewayId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeDirectConnectGatewaysResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/paginators/#describedirectconnectgatewayspaginator)
         """
```

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/type_defs.py` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,138 +41,136 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "RouteFilterPrefixTypeDef",
+    "ResponseMetadataTypeDef",
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     "TagTypeDef",
     "AssociateConnectionWithLagRequestRequestTypeDef",
     "AssociateHostedConnectionRequestRequestTypeDef",
     "AssociateMacSecKeyRequestRequestTypeDef",
     "MacSecKeyTypeDef",
     "AssociateVirtualInterfaceRequestRequestTypeDef",
     "AssociatedGatewayTypeDef",
     "BGPPeerTypeDef",
     "ConfirmConnectionRequestRequestTypeDef",
-    "ConfirmConnectionResponseTypeDef",
     "ConfirmCustomerAgreementRequestRequestTypeDef",
-    "ConfirmCustomerAgreementResponseTypeDef",
     "ConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    "TagOutputTypeDef",
     "NewBGPPeerTypeDef",
     "CreateDirectConnectGatewayRequestRequestTypeDef",
     "DirectConnectGatewayTypeDef",
     "CustomerAgreementTypeDef",
     "DeleteBGPPeerRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationRequestRequestTypeDef",
     "DeleteDirectConnectGatewayRequestRequestTypeDef",
     "DeleteInterconnectRequestRequestTypeDef",
-    "DeleteInterconnectResponseTypeDef",
     "DeleteLagRequestRequestTypeDef",
     "DeleteVirtualInterfaceRequestRequestTypeDef",
-    "DeleteVirtualInterfaceResponseTypeDef",
     "DescribeConnectionLoaRequestRequestTypeDef",
     "LoaTypeDef",
     "DescribeConnectionsOnInterconnectRequestRequestTypeDef",
     "DescribeConnectionsRequestRequestTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef",
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     "DirectConnectGatewayAttachmentTypeDef",
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     "DescribeHostedConnectionsRequestRequestTypeDef",
     "DescribeInterconnectLoaRequestRequestTypeDef",
     "DescribeInterconnectsRequestRequestTypeDef",
     "DescribeLagsRequestRequestTypeDef",
     "DescribeLoaRequestRequestTypeDef",
     "DescribeRouterConfigurationRequestRequestTypeDef",
     "RouterTypeTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DescribeVirtualInterfacesRequestRequestTypeDef",
-    "RouteFilterPrefixOutputTypeDef",
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     "DisassociateMacSecKeyRequestRequestTypeDef",
     "ListVirtualInterfaceTestHistoryRequestRequestTypeDef",
     "VirtualInterfaceTestHistoryTypeDef",
-    "LoaResponseMetadataTypeDef",
     "LocationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartBgpFailoverTestRequestRequestTypeDef",
     "StopBgpFailoverTestRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "UpdateDirectConnectGatewayRequestRequestTypeDef",
     "UpdateLagRequestRequestTypeDef",
     "UpdateVirtualInterfaceAttributesRequestRequestTypeDef",
     "VirtualGatewayTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
+    "ConfirmConnectionResponseTypeDef",
+    "ConfirmCustomerAgreementResponseTypeDef",
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    "DeleteInterconnectResponseTypeDef",
+    "DeleteVirtualInterfaceResponseTypeDef",
+    "LoaResponseTypeDef",
     "AllocateHostedConnectionRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateInterconnectRequestRequestTypeDef",
     "CreateLagRequestRequestTypeDef",
+    "InterconnectResponseTypeDef",
+    "InterconnectTypeDef",
     "NewPrivateVirtualInterfaceAllocationTypeDef",
     "NewPrivateVirtualInterfaceTypeDef",
     "NewPublicVirtualInterfaceAllocationTypeDef",
     "NewPublicVirtualInterfaceTypeDef",
     "NewTransitVirtualInterfaceAllocationTypeDef",
     "NewTransitVirtualInterfaceTypeDef",
+    "ResourceTagTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateMacSecKeyResponseTypeDef",
-    "DisassociateMacSecKeyResponseTypeDef",
-    "ConnectionResponseMetadataTypeDef",
+    "ConnectionResponseTypeDef",
     "ConnectionTypeDef",
-    "InterconnectResponseMetadataTypeDef",
-    "InterconnectTypeDef",
-    "ResourceTagTypeDef",
+    "DisassociateMacSecKeyResponseTypeDef",
+    "DirectConnectGatewayAssociationProposalTypeDef",
+    "DirectConnectGatewayAssociationTypeDef",
+    "VirtualInterfaceResponseTypeDef",
+    "VirtualInterfaceTypeDef",
     "CreateBGPPeerRequestRequestTypeDef",
     "CreateDirectConnectGatewayResultTypeDef",
     "DeleteDirectConnectGatewayResultTypeDef",
     "DescribeDirectConnectGatewaysResultTypeDef",
     "UpdateDirectConnectGatewayResponseTypeDef",
     "DescribeCustomerMetadataResponseTypeDef",
     "DescribeConnectionLoaResponseTypeDef",
     "DescribeInterconnectLoaResponseTypeDef",
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     "DescribeRouterConfigurationResponseTypeDef",
-    "DirectConnectGatewayAssociationProposalTypeDef",
-    "DirectConnectGatewayAssociationTypeDef",
-    "VirtualInterfaceResponseMetadataTypeDef",
-    "VirtualInterfaceTypeDef",
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     "StartBgpFailoverTestResponseTypeDef",
     "StopBgpFailoverTestResponseTypeDef",
     "LocationsTypeDef",
     "VirtualGatewaysTypeDef",
+    "InterconnectsTypeDef",
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     "CreatePrivateVirtualInterfaceRequestRequestTypeDef",
     "AllocatePublicVirtualInterfaceRequestRequestTypeDef",
     "CreatePublicVirtualInterfaceRequestRequestTypeDef",
     "AllocateTransitVirtualInterfaceRequestRequestTypeDef",
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
+    "DescribeTagsResponseTypeDef",
     "ConnectionsTypeDef",
-    "LagResponseMetadataTypeDef",
+    "LagResponseTypeDef",
     "LagTypeDef",
-    "InterconnectsTypeDef",
-    "DescribeTagsResponseTypeDef",
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
@@ -189,14 +187,25 @@
     "RouteFilterPrefixTypeDef",
     {
         "cidr": str,
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
 AllocateConnectionOnInterconnectRequestRequestTypeDef = TypedDict(
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     {
         "bandwidth": str,
         "connectionName": str,
         "ownerAccount": str,
         "interconnectId": str,
@@ -313,38 +322,22 @@
 ConfirmConnectionRequestRequestTypeDef = TypedDict(
     "ConfirmConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 
-ConfirmConnectionResponseTypeDef = TypedDict(
-    "ConfirmConnectionResponseTypeDef",
-    {
-        "connectionState": ConnectionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmCustomerAgreementRequestRequestTypeDef = TypedDict(
     "ConfirmCustomerAgreementRequestRequestTypeDef",
     {
         "agreementName": str,
     },
     total=False,
 )
 
-ConfirmCustomerAgreementResponseTypeDef = TypedDict(
-    "ConfirmCustomerAgreementResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
@@ -360,72 +353,29 @@
 class ConfirmPrivateVirtualInterfaceRequestRequestTypeDef(
     _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
 ):
     pass
 
 
-ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmPublicVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
-ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmTransitVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
         "directConnectGatewayId": str,
     },
 )
 
-ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
 NewBGPPeerTypeDef = TypedDict(
     "NewBGPPeerTypeDef",
     {
         "asn": int,
         "authKey": str,
         "addressFamily": AddressFamilyType,
         "amazonAddress": str,
@@ -523,44 +473,28 @@
 DeleteInterconnectRequestRequestTypeDef = TypedDict(
     "DeleteInterconnectRequestRequestTypeDef",
     {
         "interconnectId": str,
     },
 )
 
-DeleteInterconnectResponseTypeDef = TypedDict(
-    "DeleteInterconnectResponseTypeDef",
-    {
-        "interconnectState": InterconnectStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLagRequestRequestTypeDef = TypedDict(
     "DeleteLagRequestRequestTypeDef",
     {
         "lagId": str,
     },
 )
 
 DeleteVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
-DeleteVirtualInterfaceResponseTypeDef = TypedDict(
-    "DeleteVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectionLoaRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 _OptionalDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
@@ -612,22 +546,20 @@
         "associatedGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "associationId": str,
-        "associatedGatewayId": str,
-        "directConnectGatewayId": str,
-        "virtualGatewayId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
     {
@@ -637,24 +569,14 @@
         "maxResults": int,
         "nextToken": str,
         "virtualGatewayId": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "virtualInterfaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "virtualInterfaceId": str,
         "maxResults": int,
         "nextToken": str,
@@ -672,23 +594,14 @@
         "attachmentState": DirectConnectGatewayAttachmentStateType,
         "attachmentType": DirectConnectGatewayAttachmentTypeType,
         "stateChangeError": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectConnectGatewaysRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -810,22 +723,14 @@
     {
         "connectionId": str,
         "virtualInterfaceId": str,
     },
     total=False,
 )
 
-RouteFilterPrefixOutputTypeDef = TypedDict(
-    "RouteFilterPrefixOutputTypeDef",
-    {
-        "cidr": str,
-    },
-    total=False,
-)
-
 DisassociateConnectionFromLagRequestRequestTypeDef = TypedDict(
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     {
         "connectionId": str,
         "lagId": str,
     },
 )
@@ -862,57 +767,27 @@
         "testDurationInMinutes": int,
         "startTime": datetime,
         "endTime": datetime,
     },
     total=False,
 )
 
-LoaResponseMetadataTypeDef = TypedDict(
-    "LoaResponseMetadataTypeDef",
-    {
-        "loaContent": bytes,
-        "loaContentType": Literal["application/pdf"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "locationCode": str,
         "locationName": str,
         "region": str,
         "availablePortSpeeds": List[str],
         "availableProviders": List[str],
         "availableMacSecPortSpeeds": List[str],
     },
     total=False,
 )
 
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
 _RequiredStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartBgpFailoverTestRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
@@ -1112,14 +987,79 @@
         "associationId": str,
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "removeAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
+ConfirmConnectionResponseTypeDef = TypedDict(
+    "ConfirmConnectionResponseTypeDef",
+    {
+        "connectionState": ConnectionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmCustomerAgreementResponseTypeDef = TypedDict(
+    "ConfirmCustomerAgreementResponseTypeDef",
+    {
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInterconnectResponseTypeDef = TypedDict(
+    "DeleteInterconnectResponseTypeDef",
+    {
+        "interconnectState": InterconnectStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVirtualInterfaceResponseTypeDef = TypedDict(
+    "DeleteVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoaResponseTypeDef = TypedDict(
+    "LoaResponseTypeDef",
+    {
+        "loaContent": bytes,
+        "loaContentType": Literal["application/pdf"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAllocateHostedConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAllocateHostedConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
         "ownerAccount": str,
         "bandwidth": str,
         "connectionName": str,
@@ -1218,14 +1158,58 @@
 
 class CreateLagRequestRequestTypeDef(
     _RequiredCreateLagRequestRequestTypeDef, _OptionalCreateLagRequestRequestTypeDef
 ):
     pass
 
 
+InterconnectResponseTypeDef = TypedDict(
+    "InterconnectResponseTypeDef",
+    {
+        "interconnectId": str,
+        "interconnectName": str,
+        "interconnectState": InterconnectStateType,
+        "region": str,
+        "location": str,
+        "bandwidth": str,
+        "loaIssueTime": datetime,
+        "lagId": str,
+        "awsDevice": str,
+        "jumboFrameCapable": bool,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "hasLogicalRedundancy": HasLogicalRedundancyType,
+        "tags": List[TagTypeDef],
+        "providerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InterconnectTypeDef = TypedDict(
+    "InterconnectTypeDef",
+    {
+        "interconnectId": str,
+        "interconnectName": str,
+        "interconnectState": InterconnectStateType,
+        "region": str,
+        "location": str,
+        "bandwidth": str,
+        "loaIssueTime": datetime,
+        "lagId": str,
+        "awsDevice": str,
+        "jumboFrameCapable": bool,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "hasLogicalRedundancy": HasLogicalRedundancyType,
+        "tags": List[TagTypeDef],
+        "providerName": str,
+    },
+    total=False,
+)
+
 _RequiredNewPrivateVirtualInterfaceAllocationTypeDef = TypedDict(
     "_RequiredNewPrivateVirtualInterfaceAllocationTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1369,42 +1353,42 @@
         "directConnectGatewayId": str,
         "tags": Sequence[TagTypeDef],
         "enableSiteLink": bool,
     },
     total=False,
 )
 
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "resourceArn": str,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
 AssociateMacSecKeyResponseTypeDef = TypedDict(
     "AssociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociateMacSecKeyResponseTypeDef = TypedDict(
-    "DisassociateMacSecKeyResponseTypeDef",
-    {
-        "connectionId": str,
-        "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ConnectionResponseMetadataTypeDef = TypedDict(
-    "ConnectionResponseMetadataTypeDef",
+ConnectionResponseTypeDef = TypedDict(
+    "ConnectionResponseTypeDef",
     {
         "ownerAccount": str,
         "connectionId": str,
         "connectionName": str,
         "connectionState": ConnectionStateType,
         "region": str,
         "location": str,
@@ -1414,21 +1398,21 @@
         "loaIssueTime": datetime,
         "lagId": str,
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ownerAccount": str,
@@ -1443,73 +1427,126 @@
         "loaIssueTime": datetime,
         "lagId": str,
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
     },
     total=False,
 )
 
-InterconnectResponseMetadataTypeDef = TypedDict(
-    "InterconnectResponseMetadataTypeDef",
+DisassociateMacSecKeyResponseTypeDef = TypedDict(
+    "DisassociateMacSecKeyResponseTypeDef",
     {
-        "interconnectId": str,
-        "interconnectName": str,
-        "interconnectState": InterconnectStateType,
-        "region": str,
-        "location": str,
-        "bandwidth": str,
-        "loaIssueTime": datetime,
-        "lagId": str,
-        "awsDevice": str,
-        "jumboFrameCapable": bool,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
-        "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "connectionId": str,
+        "macSecKeys": List[MacSecKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InterconnectTypeDef = TypedDict(
-    "InterconnectTypeDef",
+DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
+    "DirectConnectGatewayAssociationProposalTypeDef",
     {
-        "interconnectId": str,
-        "interconnectName": str,
-        "interconnectState": InterconnectStateType,
-        "region": str,
+        "proposalId": str,
+        "directConnectGatewayId": str,
+        "directConnectGatewayOwnerAccount": str,
+        "proposalState": DirectConnectGatewayAssociationProposalStateType,
+        "associatedGateway": AssociatedGatewayTypeDef,
+        "existingAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
+        "requestedAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
+    },
+    total=False,
+)
+
+DirectConnectGatewayAssociationTypeDef = TypedDict(
+    "DirectConnectGatewayAssociationTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "directConnectGatewayOwnerAccount": str,
+        "associationState": DirectConnectGatewayAssociationStateType,
+        "stateChangeError": str,
+        "associatedGateway": AssociatedGatewayTypeDef,
+        "associationId": str,
+        "allowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
+        "virtualGatewayId": str,
+        "virtualGatewayRegion": str,
+        "virtualGatewayOwnerAccount": str,
+    },
+    total=False,
+)
+
+VirtualInterfaceResponseTypeDef = TypedDict(
+    "VirtualInterfaceResponseTypeDef",
+    {
+        "ownerAccount": str,
+        "virtualInterfaceId": str,
         "location": str,
-        "bandwidth": str,
-        "loaIssueTime": datetime,
-        "lagId": str,
-        "awsDevice": str,
+        "connectionId": str,
+        "virtualInterfaceType": str,
+        "virtualInterfaceName": str,
+        "vlan": int,
+        "asn": int,
+        "amazonSideAsn": int,
+        "authKey": str,
+        "amazonAddress": str,
+        "customerAddress": str,
+        "addressFamily": AddressFamilyType,
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "customerRouterConfig": str,
+        "mtu": int,
         "jumboFrameCapable": bool,
+        "virtualGatewayId": str,
+        "directConnectGatewayId": str,
+        "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
+        "bgpPeers": List[BGPPeerTypeDef],
+        "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
-        "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
-        "providerName": str,
+        "tags": List[TagTypeDef],
+        "siteLinkEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResourceTagTypeDef = TypedDict(
-    "ResourceTagTypeDef",
+VirtualInterfaceTypeDef = TypedDict(
+    "VirtualInterfaceTypeDef",
     {
-        "resourceArn": str,
-        "tags": List[TagOutputTypeDef],
+        "ownerAccount": str,
+        "virtualInterfaceId": str,
+        "location": str,
+        "connectionId": str,
+        "virtualInterfaceType": str,
+        "virtualInterfaceName": str,
+        "vlan": int,
+        "asn": int,
+        "amazonSideAsn": int,
+        "authKey": str,
+        "amazonAddress": str,
+        "customerAddress": str,
+        "addressFamily": AddressFamilyType,
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "customerRouterConfig": str,
+        "mtu": int,
+        "jumboFrameCapable": bool,
+        "virtualGatewayId": str,
+        "directConnectGatewayId": str,
+        "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
+        "bgpPeers": List[BGPPeerTypeDef],
+        "region": str,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "tags": List[TagTypeDef],
+        "siteLinkEnabled": bool,
     },
     total=False,
 )
 
 CreateBGPPeerRequestRequestTypeDef = TypedDict(
     "CreateBGPPeerRequestRequestTypeDef",
     {
@@ -1519,223 +1556,165 @@
     total=False,
 )
 
 CreateDirectConnectGatewayResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewaysResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysResultTypeDef",
     {
         "directConnectGateways": List[DirectConnectGatewayTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectConnectGatewayResponseTypeDef = TypedDict(
     "UpdateDirectConnectGatewayResponseTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomerMetadataResponseTypeDef = TypedDict(
     "DescribeCustomerMetadataResponseTypeDef",
     {
         "agreements": List[CustomerAgreementTypeDef],
         "nniPartnerType": NniPartnerTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectionLoaResponseTypeDef = TypedDict(
     "DescribeConnectionLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInterconnectLoaResponseTypeDef = TypedDict(
     "DescribeInterconnectLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeDirectConnectGatewayAttachmentsResultTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
-    {
-        "directConnectGatewayAttachments": List[DirectConnectGatewayAttachmentTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeRouterConfigurationResponseTypeDef = TypedDict(
-    "DescribeRouterConfigurationResponseTypeDef",
+DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
     {
-        "customerRouterConfig": str,
-        "router": RouterTypeTypeDef,
-        "virtualInterfaceId": str,
-        "virtualInterfaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "associationId": str,
+        "associatedGatewayId": str,
+        "directConnectGatewayId": str,
+        "virtualGatewayId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
-    "DirectConnectGatewayAssociationProposalTypeDef",
+DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
     {
-        "proposalId": str,
         "directConnectGatewayId": str,
-        "directConnectGatewayOwnerAccount": str,
-        "proposalState": DirectConnectGatewayAssociationProposalStateType,
-        "associatedGateway": AssociatedGatewayTypeDef,
-        "existingAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
-        "requestedAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
+        "virtualInterfaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DirectConnectGatewayAssociationTypeDef = TypedDict(
-    "DirectConnectGatewayAssociationTypeDef",
+DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     {
         "directConnectGatewayId": str,
-        "directConnectGatewayOwnerAccount": str,
-        "associationState": DirectConnectGatewayAssociationStateType,
-        "stateChangeError": str,
-        "associatedGateway": AssociatedGatewayTypeDef,
-        "associationId": str,
-        "allowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
-        "virtualGatewayId": str,
-        "virtualGatewayRegion": str,
-        "virtualGatewayOwnerAccount": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-VirtualInterfaceResponseMetadataTypeDef = TypedDict(
-    "VirtualInterfaceResponseMetadataTypeDef",
+DescribeDirectConnectGatewayAttachmentsResultTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     {
-        "ownerAccount": str,
-        "virtualInterfaceId": str,
-        "location": str,
-        "connectionId": str,
-        "virtualInterfaceType": str,
-        "virtualInterfaceName": str,
-        "vlan": int,
-        "asn": int,
-        "amazonSideAsn": int,
-        "authKey": str,
-        "amazonAddress": str,
-        "customerAddress": str,
-        "addressFamily": AddressFamilyType,
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "customerRouterConfig": str,
-        "mtu": int,
-        "jumboFrameCapable": bool,
-        "virtualGatewayId": str,
-        "directConnectGatewayId": str,
-        "routeFilterPrefixes": List[RouteFilterPrefixOutputTypeDef],
-        "bgpPeers": List[BGPPeerTypeDef],
-        "region": str,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "tags": List[TagOutputTypeDef],
-        "siteLinkEnabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "directConnectGatewayAttachments": List[DirectConnectGatewayAttachmentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VirtualInterfaceTypeDef = TypedDict(
-    "VirtualInterfaceTypeDef",
+DescribeRouterConfigurationResponseTypeDef = TypedDict(
+    "DescribeRouterConfigurationResponseTypeDef",
     {
-        "ownerAccount": str,
+        "customerRouterConfig": str,
+        "router": RouterTypeTypeDef,
         "virtualInterfaceId": str,
-        "location": str,
-        "connectionId": str,
-        "virtualInterfaceType": str,
         "virtualInterfaceName": str,
-        "vlan": int,
-        "asn": int,
-        "amazonSideAsn": int,
-        "authKey": str,
-        "amazonAddress": str,
-        "customerAddress": str,
-        "addressFamily": AddressFamilyType,
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "customerRouterConfig": str,
-        "mtu": int,
-        "jumboFrameCapable": bool,
-        "virtualGatewayId": str,
-        "directConnectGatewayId": str,
-        "routeFilterPrefixes": List[RouteFilterPrefixOutputTypeDef],
-        "bgpPeers": List[BGPPeerTypeDef],
-        "region": str,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "tags": List[TagOutputTypeDef],
-        "siteLinkEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListVirtualInterfaceTestHistoryResponseTypeDef = TypedDict(
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     {
         "virtualInterfaceTestHistory": List[VirtualInterfaceTestHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBgpFailoverTestResponseTypeDef = TypedDict(
     "StartBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBgpFailoverTestResponseTypeDef = TypedDict(
     "StopBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LocationsTypeDef = TypedDict(
     "LocationsTypeDef",
     {
         "locations": List[LocationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualGatewaysTypeDef = TypedDict(
     "VirtualGatewaysTypeDef",
     {
         "virtualGateways": List[VirtualGatewayTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InterconnectsTypeDef = TypedDict(
+    "InterconnectsTypeDef",
+    {
+        "interconnects": List[InterconnectTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocatePrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
@@ -1782,24 +1761,32 @@
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
         "newTransitVirtualInterface": NewTransitVirtualInterfaceTypeDef,
     },
 )
 
+DescribeTagsResponseTypeDef = TypedDict(
+    "DescribeTagsResponseTypeDef",
+    {
+        "resourceTags": List[ResourceTagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConnectionsTypeDef = TypedDict(
     "ConnectionsTypeDef",
     {
         "connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LagResponseMetadataTypeDef = TypedDict(
-    "LagResponseMetadataTypeDef",
+LagResponseTypeDef = TypedDict(
+    "LagResponseTypeDef",
     {
         "connectionsBandwidth": str,
         "numberOfConnections": int,
         "lagId": str,
         "ownerAccount": str,
         "lagName": str,
         "lagState": LagStateType,
@@ -1809,20 +1796,20 @@
         "awsDevice": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "connections": List[ConnectionTypeDef],
         "allowsHostedConnections": bool,
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LagTypeDef = TypedDict(
     "LagTypeDef",
     {
         "connectionsBandwidth": str,
@@ -1837,147 +1824,131 @@
         "awsDevice": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "connections": List[ConnectionTypeDef],
         "allowsHostedConnections": bool,
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
     },
     total=False,
 )
 
-InterconnectsTypeDef = TypedDict(
-    "InterconnectsTypeDef",
-    {
-        "interconnects": List[InterconnectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeTagsResponseTypeDef = TypedDict(
-    "DescribeTagsResponseTypeDef",
-    {
-        "resourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewayAssociationProposalsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     {
         "directConnectGatewayAssociationProposals": List[
             DirectConnectGatewayAssociationProposalTypeDef
         ],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewayAssociationsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
     {
         "directConnectGatewayAssociations": List[DirectConnectGatewayAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "UpdateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "AllocateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBGPPeerResponseTypeDef = TypedDict(
     "CreateBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "CreateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBGPPeerResponseTypeDef = TypedDict(
     "DeleteBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualInterfacesTypeDef = TypedDict(
     "VirtualInterfacesTypeDef",
     {
         "virtualInterfaces": List[VirtualInterfaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LagsTypeDef = TypedDict(
     "LagsTypeDef",
     {
         "lags": List[LagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect/type_defs.pyi` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -40,138 +40,136 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "RouteFilterPrefixTypeDef",
+    "ResponseMetadataTypeDef",
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     "TagTypeDef",
     "AssociateConnectionWithLagRequestRequestTypeDef",
     "AssociateHostedConnectionRequestRequestTypeDef",
     "AssociateMacSecKeyRequestRequestTypeDef",
     "MacSecKeyTypeDef",
     "AssociateVirtualInterfaceRequestRequestTypeDef",
     "AssociatedGatewayTypeDef",
     "BGPPeerTypeDef",
     "ConfirmConnectionRequestRequestTypeDef",
-    "ConfirmConnectionResponseTypeDef",
     "ConfirmCustomerAgreementRequestRequestTypeDef",
-    "ConfirmCustomerAgreementResponseTypeDef",
     "ConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    "TagOutputTypeDef",
     "NewBGPPeerTypeDef",
     "CreateDirectConnectGatewayRequestRequestTypeDef",
     "DirectConnectGatewayTypeDef",
     "CustomerAgreementTypeDef",
     "DeleteBGPPeerRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationRequestRequestTypeDef",
     "DeleteDirectConnectGatewayRequestRequestTypeDef",
     "DeleteInterconnectRequestRequestTypeDef",
-    "DeleteInterconnectResponseTypeDef",
     "DeleteLagRequestRequestTypeDef",
     "DeleteVirtualInterfaceRequestRequestTypeDef",
-    "DeleteVirtualInterfaceResponseTypeDef",
     "DescribeConnectionLoaRequestRequestTypeDef",
     "LoaTypeDef",
     "DescribeConnectionsOnInterconnectRequestRequestTypeDef",
     "DescribeConnectionsRequestRequestTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef",
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     "DirectConnectGatewayAttachmentTypeDef",
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     "DescribeHostedConnectionsRequestRequestTypeDef",
     "DescribeInterconnectLoaRequestRequestTypeDef",
     "DescribeInterconnectsRequestRequestTypeDef",
     "DescribeLagsRequestRequestTypeDef",
     "DescribeLoaRequestRequestTypeDef",
     "DescribeRouterConfigurationRequestRequestTypeDef",
     "RouterTypeTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DescribeVirtualInterfacesRequestRequestTypeDef",
-    "RouteFilterPrefixOutputTypeDef",
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     "DisassociateMacSecKeyRequestRequestTypeDef",
     "ListVirtualInterfaceTestHistoryRequestRequestTypeDef",
     "VirtualInterfaceTestHistoryTypeDef",
-    "LoaResponseMetadataTypeDef",
     "LocationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartBgpFailoverTestRequestRequestTypeDef",
     "StopBgpFailoverTestRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "UpdateDirectConnectGatewayRequestRequestTypeDef",
     "UpdateLagRequestRequestTypeDef",
     "UpdateVirtualInterfaceAttributesRequestRequestTypeDef",
     "VirtualGatewayTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
+    "ConfirmConnectionResponseTypeDef",
+    "ConfirmCustomerAgreementResponseTypeDef",
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    "DeleteInterconnectResponseTypeDef",
+    "DeleteVirtualInterfaceResponseTypeDef",
+    "LoaResponseTypeDef",
     "AllocateHostedConnectionRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateInterconnectRequestRequestTypeDef",
     "CreateLagRequestRequestTypeDef",
+    "InterconnectResponseTypeDef",
+    "InterconnectTypeDef",
     "NewPrivateVirtualInterfaceAllocationTypeDef",
     "NewPrivateVirtualInterfaceTypeDef",
     "NewPublicVirtualInterfaceAllocationTypeDef",
     "NewPublicVirtualInterfaceTypeDef",
     "NewTransitVirtualInterfaceAllocationTypeDef",
     "NewTransitVirtualInterfaceTypeDef",
+    "ResourceTagTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateMacSecKeyResponseTypeDef",
-    "DisassociateMacSecKeyResponseTypeDef",
-    "ConnectionResponseMetadataTypeDef",
+    "ConnectionResponseTypeDef",
     "ConnectionTypeDef",
-    "InterconnectResponseMetadataTypeDef",
-    "InterconnectTypeDef",
-    "ResourceTagTypeDef",
+    "DisassociateMacSecKeyResponseTypeDef",
+    "DirectConnectGatewayAssociationProposalTypeDef",
+    "DirectConnectGatewayAssociationTypeDef",
+    "VirtualInterfaceResponseTypeDef",
+    "VirtualInterfaceTypeDef",
     "CreateBGPPeerRequestRequestTypeDef",
     "CreateDirectConnectGatewayResultTypeDef",
     "DeleteDirectConnectGatewayResultTypeDef",
     "DescribeDirectConnectGatewaysResultTypeDef",
     "UpdateDirectConnectGatewayResponseTypeDef",
     "DescribeCustomerMetadataResponseTypeDef",
     "DescribeConnectionLoaResponseTypeDef",
     "DescribeInterconnectLoaResponseTypeDef",
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     "DescribeRouterConfigurationResponseTypeDef",
-    "DirectConnectGatewayAssociationProposalTypeDef",
-    "DirectConnectGatewayAssociationTypeDef",
-    "VirtualInterfaceResponseMetadataTypeDef",
-    "VirtualInterfaceTypeDef",
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     "StartBgpFailoverTestResponseTypeDef",
     "StopBgpFailoverTestResponseTypeDef",
     "LocationsTypeDef",
     "VirtualGatewaysTypeDef",
+    "InterconnectsTypeDef",
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     "CreatePrivateVirtualInterfaceRequestRequestTypeDef",
     "AllocatePublicVirtualInterfaceRequestRequestTypeDef",
     "CreatePublicVirtualInterfaceRequestRequestTypeDef",
     "AllocateTransitVirtualInterfaceRequestRequestTypeDef",
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
+    "DescribeTagsResponseTypeDef",
     "ConnectionsTypeDef",
-    "LagResponseMetadataTypeDef",
+    "LagResponseTypeDef",
     "LagTypeDef",
-    "InterconnectsTypeDef",
-    "DescribeTagsResponseTypeDef",
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
@@ -188,14 +186,25 @@
     "RouteFilterPrefixTypeDef",
     {
         "cidr": str,
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
 AllocateConnectionOnInterconnectRequestRequestTypeDef = TypedDict(
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     {
         "bandwidth": str,
         "connectionName": str,
         "ownerAccount": str,
         "interconnectId": str,
@@ -308,38 +317,22 @@
 ConfirmConnectionRequestRequestTypeDef = TypedDict(
     "ConfirmConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 
-ConfirmConnectionResponseTypeDef = TypedDict(
-    "ConfirmConnectionResponseTypeDef",
-    {
-        "connectionState": ConnectionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmCustomerAgreementRequestRequestTypeDef = TypedDict(
     "ConfirmCustomerAgreementRequestRequestTypeDef",
     {
         "agreementName": str,
     },
     total=False,
 )
 
-ConfirmCustomerAgreementResponseTypeDef = TypedDict(
-    "ConfirmCustomerAgreementResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
@@ -353,70 +346,29 @@
 
 class ConfirmPrivateVirtualInterfaceRequestRequestTypeDef(
     _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
 ):
     pass
 
-ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmPublicVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
-ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmTransitVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
         "directConnectGatewayId": str,
     },
 )
 
-ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "value": str,
-    },
-    total=False,
-)
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
 NewBGPPeerTypeDef = TypedDict(
     "NewBGPPeerTypeDef",
     {
         "asn": int,
         "authKey": str,
         "addressFamily": AddressFamilyType,
         "amazonAddress": str,
@@ -512,44 +464,28 @@
 DeleteInterconnectRequestRequestTypeDef = TypedDict(
     "DeleteInterconnectRequestRequestTypeDef",
     {
         "interconnectId": str,
     },
 )
 
-DeleteInterconnectResponseTypeDef = TypedDict(
-    "DeleteInterconnectResponseTypeDef",
-    {
-        "interconnectState": InterconnectStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLagRequestRequestTypeDef = TypedDict(
     "DeleteLagRequestRequestTypeDef",
     {
         "lagId": str,
     },
 )
 
 DeleteVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
-DeleteVirtualInterfaceResponseTypeDef = TypedDict(
-    "DeleteVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectionLoaRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 _OptionalDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
@@ -599,22 +535,20 @@
         "associatedGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "associationId": str,
-        "associatedGatewayId": str,
-        "directConnectGatewayId": str,
-        "virtualGatewayId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
     {
@@ -624,24 +558,14 @@
         "maxResults": int,
         "nextToken": str,
         "virtualGatewayId": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "virtualInterfaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "virtualInterfaceId": str,
         "maxResults": int,
         "nextToken": str,
@@ -659,23 +583,14 @@
         "attachmentState": DirectConnectGatewayAttachmentStateType,
         "attachmentType": DirectConnectGatewayAttachmentTypeType,
         "stateChangeError": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectConnectGatewaysRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -791,22 +706,14 @@
     {
         "connectionId": str,
         "virtualInterfaceId": str,
     },
     total=False,
 )
 
-RouteFilterPrefixOutputTypeDef = TypedDict(
-    "RouteFilterPrefixOutputTypeDef",
-    {
-        "cidr": str,
-    },
-    total=False,
-)
-
 DisassociateConnectionFromLagRequestRequestTypeDef = TypedDict(
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     {
         "connectionId": str,
         "lagId": str,
     },
 )
@@ -843,57 +750,27 @@
         "testDurationInMinutes": int,
         "startTime": datetime,
         "endTime": datetime,
     },
     total=False,
 )
 
-LoaResponseMetadataTypeDef = TypedDict(
-    "LoaResponseMetadataTypeDef",
-    {
-        "loaContent": bytes,
-        "loaContentType": Literal["application/pdf"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "locationCode": str,
         "locationName": str,
         "region": str,
         "availablePortSpeeds": List[str],
         "availableProviders": List[str],
         "availableMacSecPortSpeeds": List[str],
     },
     total=False,
 )
 
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
 _RequiredStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartBgpFailoverTestRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
@@ -1079,14 +956,79 @@
         "associationId": str,
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "removeAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
+ConfirmConnectionResponseTypeDef = TypedDict(
+    "ConfirmConnectionResponseTypeDef",
+    {
+        "connectionState": ConnectionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmCustomerAgreementResponseTypeDef = TypedDict(
+    "ConfirmCustomerAgreementResponseTypeDef",
+    {
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInterconnectResponseTypeDef = TypedDict(
+    "DeleteInterconnectResponseTypeDef",
+    {
+        "interconnectState": InterconnectStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVirtualInterfaceResponseTypeDef = TypedDict(
+    "DeleteVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoaResponseTypeDef = TypedDict(
+    "LoaResponseTypeDef",
+    {
+        "loaContent": bytes,
+        "loaContentType": Literal["application/pdf"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAllocateHostedConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAllocateHostedConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
         "ownerAccount": str,
         "bandwidth": str,
         "connectionName": str,
@@ -1177,14 +1119,58 @@
 )
 
 class CreateLagRequestRequestTypeDef(
     _RequiredCreateLagRequestRequestTypeDef, _OptionalCreateLagRequestRequestTypeDef
 ):
     pass
 
+InterconnectResponseTypeDef = TypedDict(
+    "InterconnectResponseTypeDef",
+    {
+        "interconnectId": str,
+        "interconnectName": str,
+        "interconnectState": InterconnectStateType,
+        "region": str,
+        "location": str,
+        "bandwidth": str,
+        "loaIssueTime": datetime,
+        "lagId": str,
+        "awsDevice": str,
+        "jumboFrameCapable": bool,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "hasLogicalRedundancy": HasLogicalRedundancyType,
+        "tags": List[TagTypeDef],
+        "providerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InterconnectTypeDef = TypedDict(
+    "InterconnectTypeDef",
+    {
+        "interconnectId": str,
+        "interconnectName": str,
+        "interconnectState": InterconnectStateType,
+        "region": str,
+        "location": str,
+        "bandwidth": str,
+        "loaIssueTime": datetime,
+        "lagId": str,
+        "awsDevice": str,
+        "jumboFrameCapable": bool,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "hasLogicalRedundancy": HasLogicalRedundancyType,
+        "tags": List[TagTypeDef],
+        "providerName": str,
+    },
+    total=False,
+)
+
 _RequiredNewPrivateVirtualInterfaceAllocationTypeDef = TypedDict(
     "_RequiredNewPrivateVirtualInterfaceAllocationTypeDef",
     {
         "virtualInterfaceName": str,
         "vlan": int,
         "asn": int,
     },
@@ -1320,42 +1306,42 @@
         "directConnectGatewayId": str,
         "tags": Sequence[TagTypeDef],
         "enableSiteLink": bool,
     },
     total=False,
 )
 
+ResourceTagTypeDef = TypedDict(
+    "ResourceTagTypeDef",
+    {
+        "resourceArn": str,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
 
 AssociateMacSecKeyResponseTypeDef = TypedDict(
     "AssociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DisassociateMacSecKeyResponseTypeDef = TypedDict(
-    "DisassociateMacSecKeyResponseTypeDef",
-    {
-        "connectionId": str,
-        "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ConnectionResponseMetadataTypeDef = TypedDict(
-    "ConnectionResponseMetadataTypeDef",
+ConnectionResponseTypeDef = TypedDict(
+    "ConnectionResponseTypeDef",
     {
         "ownerAccount": str,
         "connectionId": str,
         "connectionName": str,
         "connectionState": ConnectionStateType,
         "region": str,
         "location": str,
@@ -1365,21 +1351,21 @@
         "loaIssueTime": datetime,
         "lagId": str,
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ownerAccount": str,
@@ -1394,73 +1380,126 @@
         "loaIssueTime": datetime,
         "lagId": str,
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
     },
     total=False,
 )
 
-InterconnectResponseMetadataTypeDef = TypedDict(
-    "InterconnectResponseMetadataTypeDef",
+DisassociateMacSecKeyResponseTypeDef = TypedDict(
+    "DisassociateMacSecKeyResponseTypeDef",
     {
-        "interconnectId": str,
-        "interconnectName": str,
-        "interconnectState": InterconnectStateType,
-        "region": str,
-        "location": str,
-        "bandwidth": str,
-        "loaIssueTime": datetime,
-        "lagId": str,
-        "awsDevice": str,
-        "jumboFrameCapable": bool,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
-        "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "connectionId": str,
+        "macSecKeys": List[MacSecKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InterconnectTypeDef = TypedDict(
-    "InterconnectTypeDef",
+DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
+    "DirectConnectGatewayAssociationProposalTypeDef",
     {
-        "interconnectId": str,
-        "interconnectName": str,
-        "interconnectState": InterconnectStateType,
-        "region": str,
+        "proposalId": str,
+        "directConnectGatewayId": str,
+        "directConnectGatewayOwnerAccount": str,
+        "proposalState": DirectConnectGatewayAssociationProposalStateType,
+        "associatedGateway": AssociatedGatewayTypeDef,
+        "existingAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
+        "requestedAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
+    },
+    total=False,
+)
+
+DirectConnectGatewayAssociationTypeDef = TypedDict(
+    "DirectConnectGatewayAssociationTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "directConnectGatewayOwnerAccount": str,
+        "associationState": DirectConnectGatewayAssociationStateType,
+        "stateChangeError": str,
+        "associatedGateway": AssociatedGatewayTypeDef,
+        "associationId": str,
+        "allowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixTypeDef],
+        "virtualGatewayId": str,
+        "virtualGatewayRegion": str,
+        "virtualGatewayOwnerAccount": str,
+    },
+    total=False,
+)
+
+VirtualInterfaceResponseTypeDef = TypedDict(
+    "VirtualInterfaceResponseTypeDef",
+    {
+        "ownerAccount": str,
+        "virtualInterfaceId": str,
         "location": str,
-        "bandwidth": str,
-        "loaIssueTime": datetime,
-        "lagId": str,
-        "awsDevice": str,
+        "connectionId": str,
+        "virtualInterfaceType": str,
+        "virtualInterfaceName": str,
+        "vlan": int,
+        "asn": int,
+        "amazonSideAsn": int,
+        "authKey": str,
+        "amazonAddress": str,
+        "customerAddress": str,
+        "addressFamily": AddressFamilyType,
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "customerRouterConfig": str,
+        "mtu": int,
         "jumboFrameCapable": bool,
+        "virtualGatewayId": str,
+        "directConnectGatewayId": str,
+        "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
+        "bgpPeers": List[BGPPeerTypeDef],
+        "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
-        "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
-        "providerName": str,
+        "tags": List[TagTypeDef],
+        "siteLinkEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResourceTagTypeDef = TypedDict(
-    "ResourceTagTypeDef",
+VirtualInterfaceTypeDef = TypedDict(
+    "VirtualInterfaceTypeDef",
     {
-        "resourceArn": str,
-        "tags": List[TagOutputTypeDef],
+        "ownerAccount": str,
+        "virtualInterfaceId": str,
+        "location": str,
+        "connectionId": str,
+        "virtualInterfaceType": str,
+        "virtualInterfaceName": str,
+        "vlan": int,
+        "asn": int,
+        "amazonSideAsn": int,
+        "authKey": str,
+        "amazonAddress": str,
+        "customerAddress": str,
+        "addressFamily": AddressFamilyType,
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "customerRouterConfig": str,
+        "mtu": int,
+        "jumboFrameCapable": bool,
+        "virtualGatewayId": str,
+        "directConnectGatewayId": str,
+        "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
+        "bgpPeers": List[BGPPeerTypeDef],
+        "region": str,
+        "awsDeviceV2": str,
+        "awsLogicalDeviceId": str,
+        "tags": List[TagTypeDef],
+        "siteLinkEnabled": bool,
     },
     total=False,
 )
 
 CreateBGPPeerRequestRequestTypeDef = TypedDict(
     "CreateBGPPeerRequestRequestTypeDef",
     {
@@ -1470,223 +1509,165 @@
     total=False,
 )
 
 CreateDirectConnectGatewayResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewaysResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysResultTypeDef",
     {
         "directConnectGateways": List[DirectConnectGatewayTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectConnectGatewayResponseTypeDef = TypedDict(
     "UpdateDirectConnectGatewayResponseTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomerMetadataResponseTypeDef = TypedDict(
     "DescribeCustomerMetadataResponseTypeDef",
     {
         "agreements": List[CustomerAgreementTypeDef],
         "nniPartnerType": NniPartnerTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectionLoaResponseTypeDef = TypedDict(
     "DescribeConnectionLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInterconnectLoaResponseTypeDef = TypedDict(
     "DescribeInterconnectLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeDirectConnectGatewayAttachmentsResultTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
-    {
-        "directConnectGatewayAttachments": List[DirectConnectGatewayAttachmentTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeRouterConfigurationResponseTypeDef = TypedDict(
-    "DescribeRouterConfigurationResponseTypeDef",
+DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
     {
-        "customerRouterConfig": str,
-        "router": RouterTypeTypeDef,
-        "virtualInterfaceId": str,
-        "virtualInterfaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "associationId": str,
+        "associatedGatewayId": str,
+        "directConnectGatewayId": str,
+        "virtualGatewayId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
-    "DirectConnectGatewayAssociationProposalTypeDef",
+DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
     {
-        "proposalId": str,
         "directConnectGatewayId": str,
-        "directConnectGatewayOwnerAccount": str,
-        "proposalState": DirectConnectGatewayAssociationProposalStateType,
-        "associatedGateway": AssociatedGatewayTypeDef,
-        "existingAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
-        "requestedAllowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
+        "virtualInterfaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DirectConnectGatewayAssociationTypeDef = TypedDict(
-    "DirectConnectGatewayAssociationTypeDef",
+DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     {
         "directConnectGatewayId": str,
-        "directConnectGatewayOwnerAccount": str,
-        "associationState": DirectConnectGatewayAssociationStateType,
-        "stateChangeError": str,
-        "associatedGateway": AssociatedGatewayTypeDef,
-        "associationId": str,
-        "allowedPrefixesToDirectConnectGateway": List[RouteFilterPrefixOutputTypeDef],
-        "virtualGatewayId": str,
-        "virtualGatewayRegion": str,
-        "virtualGatewayOwnerAccount": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-VirtualInterfaceResponseMetadataTypeDef = TypedDict(
-    "VirtualInterfaceResponseMetadataTypeDef",
+DescribeDirectConnectGatewayAttachmentsResultTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     {
-        "ownerAccount": str,
-        "virtualInterfaceId": str,
-        "location": str,
-        "connectionId": str,
-        "virtualInterfaceType": str,
-        "virtualInterfaceName": str,
-        "vlan": int,
-        "asn": int,
-        "amazonSideAsn": int,
-        "authKey": str,
-        "amazonAddress": str,
-        "customerAddress": str,
-        "addressFamily": AddressFamilyType,
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "customerRouterConfig": str,
-        "mtu": int,
-        "jumboFrameCapable": bool,
-        "virtualGatewayId": str,
-        "directConnectGatewayId": str,
-        "routeFilterPrefixes": List[RouteFilterPrefixOutputTypeDef],
-        "bgpPeers": List[BGPPeerTypeDef],
-        "region": str,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "tags": List[TagOutputTypeDef],
-        "siteLinkEnabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "directConnectGatewayAttachments": List[DirectConnectGatewayAttachmentTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VirtualInterfaceTypeDef = TypedDict(
-    "VirtualInterfaceTypeDef",
+DescribeRouterConfigurationResponseTypeDef = TypedDict(
+    "DescribeRouterConfigurationResponseTypeDef",
     {
-        "ownerAccount": str,
+        "customerRouterConfig": str,
+        "router": RouterTypeTypeDef,
         "virtualInterfaceId": str,
-        "location": str,
-        "connectionId": str,
-        "virtualInterfaceType": str,
         "virtualInterfaceName": str,
-        "vlan": int,
-        "asn": int,
-        "amazonSideAsn": int,
-        "authKey": str,
-        "amazonAddress": str,
-        "customerAddress": str,
-        "addressFamily": AddressFamilyType,
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "customerRouterConfig": str,
-        "mtu": int,
-        "jumboFrameCapable": bool,
-        "virtualGatewayId": str,
-        "directConnectGatewayId": str,
-        "routeFilterPrefixes": List[RouteFilterPrefixOutputTypeDef],
-        "bgpPeers": List[BGPPeerTypeDef],
-        "region": str,
-        "awsDeviceV2": str,
-        "awsLogicalDeviceId": str,
-        "tags": List[TagOutputTypeDef],
-        "siteLinkEnabled": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ListVirtualInterfaceTestHistoryResponseTypeDef = TypedDict(
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     {
         "virtualInterfaceTestHistory": List[VirtualInterfaceTestHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBgpFailoverTestResponseTypeDef = TypedDict(
     "StartBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBgpFailoverTestResponseTypeDef = TypedDict(
     "StopBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LocationsTypeDef = TypedDict(
     "LocationsTypeDef",
     {
         "locations": List[LocationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualGatewaysTypeDef = TypedDict(
     "VirtualGatewaysTypeDef",
     {
         "virtualGateways": List[VirtualGatewayTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InterconnectsTypeDef = TypedDict(
+    "InterconnectsTypeDef",
+    {
+        "interconnects": List[InterconnectTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocatePrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
@@ -1733,24 +1714,32 @@
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
         "newTransitVirtualInterface": NewTransitVirtualInterfaceTypeDef,
     },
 )
 
+DescribeTagsResponseTypeDef = TypedDict(
+    "DescribeTagsResponseTypeDef",
+    {
+        "resourceTags": List[ResourceTagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ConnectionsTypeDef = TypedDict(
     "ConnectionsTypeDef",
     {
         "connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LagResponseMetadataTypeDef = TypedDict(
-    "LagResponseMetadataTypeDef",
+LagResponseTypeDef = TypedDict(
+    "LagResponseTypeDef",
     {
         "connectionsBandwidth": str,
         "numberOfConnections": int,
         "lagId": str,
         "ownerAccount": str,
         "lagName": str,
         "lagState": LagStateType,
@@ -1760,20 +1749,20 @@
         "awsDevice": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "connections": List[ConnectionTypeDef],
         "allowsHostedConnections": bool,
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LagTypeDef = TypedDict(
     "LagTypeDef",
     {
         "connectionsBandwidth": str,
@@ -1788,147 +1777,131 @@
         "awsDevice": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "connections": List[ConnectionTypeDef],
         "allowsHostedConnections": bool,
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
     },
     total=False,
 )
 
-InterconnectsTypeDef = TypedDict(
-    "InterconnectsTypeDef",
-    {
-        "interconnects": List[InterconnectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeTagsResponseTypeDef = TypedDict(
-    "DescribeTagsResponseTypeDef",
-    {
-        "resourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewayAssociationProposalsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     {
         "directConnectGatewayAssociationProposals": List[
             DirectConnectGatewayAssociationProposalTypeDef
         ],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewayAssociationsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
     {
         "directConnectGatewayAssociations": List[DirectConnectGatewayAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "UpdateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "AllocateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBGPPeerResponseTypeDef = TypedDict(
     "CreateBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "CreateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBGPPeerResponseTypeDef = TypedDict(
     "DeleteBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualInterfacesTypeDef = TypedDict(
     "VirtualInterfacesTypeDef",
     {
         "virtualInterfaces": List[VirtualInterfaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LagsTypeDef = TypedDict(
     "LagsTypeDef",
     {
         "lags": List[LagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/PKG-INFO` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-directconnect
-Version: 1.28.12
-Summary: Type annotations for boto3.DirectConnect 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.DirectConnect 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-directconnect.svg?color=blue)](https://pypi.org/project/mypy-boto3-directconnect)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-directconnect)](https://pepy.tech/project/mypy-boto3-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DirectConnect 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
+[boto3.DirectConnect 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [mypy-boto3-directconnect docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_directconnect/).
 
 See how it helps to find and fix potential bugs:
 
@@ -350,138 +350,136 @@
 
 `mypy_boto3_directconnect.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
+    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
-    TagOutputTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
-    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
-    RouteFilterPrefixOutputTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
-    LoaResponseMetadataTypeDef,
     LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
+    DeleteInterconnectResponseTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
+    LoaResponseTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
+    InterconnectResponseTypeDef,
+    InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
+    ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
-    DisassociateMacSecKeyResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionTypeDef,
-    InterconnectResponseMetadataTypeDef,
-    InterconnectTypeDef,
-    ResourceTagTypeDef,
+    DisassociateMacSecKeyResponseTypeDef,
+    DirectConnectGatewayAssociationProposalTypeDef,
+    DirectConnectGatewayAssociationTypeDef,
+    VirtualInterfaceResponseTypeDef,
+    VirtualInterfaceTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
-    DirectConnectGatewayAssociationProposalTypeDef,
-    DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
-    VirtualInterfaceTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
+    InterconnectsTypeDef,
     AllocatePrivateVirtualInterfaceRequestRequestTypeDef,
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
+    DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagTypeDef,
-    InterconnectsTypeDef,
-    DescribeTagsResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
```

### Comparing `mypy-boto3-directconnect-1.28.12/mypy_boto3_directconnect.egg-info/SOURCES.txt` & `mypy-boto3-directconnect-1.28.15/mypy_boto3_directconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-directconnect-1.28.12/setup.py` & `mypy-boto3-directconnect-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-directconnect",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_directconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.DirectConnect 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.DirectConnect 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

