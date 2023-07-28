# Comparing `tmp/mypy-boto3-appmesh-1.28.12.tar.gz` & `tmp/mypy-boto3-appmesh-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-appmesh-1.28.12.tar", last modified: Thu Jul 27 05:34:18 2023, max compression
+gzip compressed data, was "mypy-boto3-appmesh-1.28.15.tar", last modified: Fri Jul 28 20:42:16 2023, max compression
```

## Comparing `mypy-boto3-appmesh-1.28.12.tar` & `mypy-boto3-appmesh-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.500577 mypy-boto3-appmesh-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-07-27 05:34:18.500577 mypy-boto3-appmesh-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    25826 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.496577 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30176 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9611 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   122164 2023-07-27 05:17:31.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   121945 2023-07-27 05:17:30.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:18.500577 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27313 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:34:18.000000 mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:18.500577 mypy-boto3-appmesh-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:17:28.000000 mypy-boto3-appmesh-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.272655 mypy-boto3-appmesh-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-07-28 20:42:16.268655 mypy-boto3-appmesh-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22845 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.256654 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30229 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30176 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-07-28 20:19:29.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-28 20:19:29.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   100348 2023-07-28 20:19:32.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100157 2023-07-28 20:19:31.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:16.268655 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24332 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:42:16.000000 mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:16.272655 mypy-boto3-appmesh-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:19:28.000000 mypy-boto3-appmesh-1.28.15/setup.py
```

### Comparing `mypy-boto3-appmesh-1.28.12/LICENSE` & `mypy-boto3-appmesh-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.12/PKG-INFO` & `mypy-boto3-appmesh-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-appmesh
-Version: 1.28.12
-Summary: Type annotations for boto3.AppMesh 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,265 +371,195 @@
 ### Typed dictionaries
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
-    AwsCloudMapInstanceAttributeOutputTypeDef,
     AwsCloudMapInstanceAttributeTypeDef,
-    ListenerTlsFileCertificateOutputTypeDef,
-    ListenerTlsSdsCertificateOutputTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
     DescribeGatewayRouteInputRequestTypeDef,
     DescribeMeshInputRequestTypeDef,
     DescribeRouteInputRequestTypeDef,
     DescribeVirtualGatewayInputRequestTypeDef,
     DescribeVirtualNodeInputRequestTypeDef,
     DescribeVirtualRouterInputRequestTypeDef,
     DescribeVirtualServiceInputRequestTypeDef,
-    DnsServiceDiscoveryOutputTypeDef,
     DnsServiceDiscoveryTypeDef,
-    DurationOutputTypeDef,
     DurationTypeDef,
-    EgressFilterOutputTypeDef,
     EgressFilterTypeDef,
     GatewayRouteStatusTypeDef,
     ResourceMetadataTypeDef,
-    GatewayRouteHostnameMatchOutputTypeDef,
     GatewayRouteHostnameMatchTypeDef,
-    GatewayRouteHostnameRewriteOutputTypeDef,
     GatewayRouteHostnameRewriteTypeDef,
     GatewayRouteRefTypeDef,
-    GatewayRouteVirtualServiceOutputTypeDef,
     GatewayRouteVirtualServiceTypeDef,
-    MatchRangeOutputTypeDef,
     MatchRangeTypeDef,
-    WeightedTargetOutputTypeDef,
     WeightedTargetTypeDef,
-    HealthCheckPolicyOutputTypeDef,
     HealthCheckPolicyTypeDef,
-    HttpPathMatchOutputTypeDef,
     HttpPathMatchTypeDef,
-    HttpGatewayRoutePathRewriteOutputTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
-    HttpGatewayRoutePrefixRewriteOutputTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
-    QueryParameterMatchOutputTypeDef,
     QueryParameterMatchTypeDef,
-    JsonFormatRefOutputTypeDef,
     JsonFormatRefTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagRefOutputTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
-    PortMappingOutputTypeDef,
-    ListenerTlsAcmCertificateOutputTypeDef,
+    PortMappingTypeDef,
     ListenerTlsAcmCertificateTypeDef,
-    TlsValidationContextFileTrustOutputTypeDef,
-    TlsValidationContextSdsTrustOutputTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
-    PortMappingTypeDef,
     MeshStatusTypeDef,
-    MeshServiceDiscoveryOutputTypeDef,
     MeshServiceDiscoveryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
     SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
-    TcpRouteMatchOutputTypeDef,
     TcpRouteMatchTypeDef,
     TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
-    VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
-    VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
-    VirtualGatewayGrpcConnectionPoolOutputTypeDef,
-    VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
-    VirtualGatewayHttpConnectionPoolOutputTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
-    VirtualGatewayHealthCheckPolicyOutputTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
-    VirtualGatewayPortMappingOutputTypeDef,
-    VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
+    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
-    VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
-    VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
-    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
-    VirtualNodeGrpcConnectionPoolOutputTypeDef,
-    VirtualNodeHttp2ConnectionPoolOutputTypeDef,
-    VirtualNodeHttpConnectionPoolOutputTypeDef,
-    VirtualNodeTcpConnectionPoolOutputTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
-    VirtualNodeServiceProviderOutputTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
-    VirtualRouterServiceProviderOutputTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
     AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
-    ClientTlsCertificateOutputTypeDef,
     ClientTlsCertificateTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     GrpcRetryPolicyOutputTypeDef,
-    GrpcTimeoutOutputTypeDef,
-    HttpRetryPolicyOutputTypeDef,
-    HttpTimeoutOutputTypeDef,
-    OutlierDetectionOutputTypeDef,
-    TcpTimeoutOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
+    HttpRetryPolicyOutputTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
-    GrpcGatewayRouteRewriteOutputTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
-    GatewayRouteTargetOutputTypeDef,
     GatewayRouteTargetTypeDef,
-    GrpcMetadataMatchMethodOutputTypeDef,
-    GrpcRouteMetadataMatchMethodOutputTypeDef,
-    HeaderMatchMethodOutputTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
     GrpcRouteActionOutputTypeDef,
-    HttpRouteActionOutputTypeDef,
-    TcpRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
+    HttpRouteActionOutputTypeDef,
     HttpRouteActionTypeDef,
+    TcpRouteActionOutputTypeDef,
     TcpRouteActionTypeDef,
-    HttpGatewayRouteRewriteOutputTypeDef,
     HttpGatewayRouteRewriteTypeDef,
-    HttpQueryParameterOutputTypeDef,
     HttpQueryParameterTypeDef,
     LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
-    VirtualRouterListenerOutputTypeDef,
-    ListenerTlsCertificateOutputTypeDef,
+    VirtualRouterListenerTypeDef,
     ListenerTlsCertificateTypeDef,
-    ListenerTlsValidationContextTrustOutputTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
-    VirtualRouterListenerTypeDef,
-    MeshSpecOutputTypeDef,
     MeshSpecTypeDef,
     SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
     TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
-    VirtualGatewayClientTlsCertificateOutputTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
-    VirtualGatewayConnectionPoolOutputTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
-    VirtualGatewayListenerTlsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
-    VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
-    VirtualNodeConnectionPoolOutputTypeDef,
     VirtualNodeConnectionPoolTypeDef,
-    VirtualServiceProviderOutputTypeDef,
     VirtualServiceProviderTypeDef,
     ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
-    ListenerTimeoutOutputTypeDef,
     ListenerTimeoutTypeDef,
-    GrpcGatewayRouteActionOutputTypeDef,
     GrpcGatewayRouteActionTypeDef,
-    GrpcGatewayRouteMetadataOutputTypeDef,
-    GrpcRouteMetadataOutputTypeDef,
-    HttpGatewayRouteHeaderOutputTypeDef,
-    HttpRouteHeaderOutputTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
     TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
-    HttpGatewayRouteActionOutputTypeDef,
     HttpGatewayRouteActionTypeDef,
     FileAccessLogOutputTypeDef,
     VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
     VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
-    MeshDataTypeDef,
     CreateMeshInputRequestTypeDef,
+    MeshDataTypeDef,
     UpdateMeshInputRequestTypeDef,
     ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
     TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
     VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
     VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
-    VirtualServiceSpecOutputTypeDef,
     VirtualServiceSpecTypeDef,
     GrpcGatewayRouteMatchOutputTypeDef,
-    GrpcRouteMatchOutputTypeDef,
-    HttpGatewayRouteMatchOutputTypeDef,
-    HttpRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
+    GrpcRouteMatchOutputTypeDef,
     GrpcRouteMatchTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
     HttpGatewayRouteMatchTypeDef,
+    HttpRouteMatchOutputTypeDef,
     HttpRouteMatchTypeDef,
     AccessLogOutputTypeDef,
     VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
     VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
@@ -642,24 +572,24 @@
     ListenerTlsTypeDef,
     ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
     VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
     VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
-    VirtualServiceDataTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
+    VirtualServiceDataTypeDef,
     GrpcGatewayRouteOutputTypeDef,
-    GrpcRouteOutputTypeDef,
-    HttpGatewayRouteOutputTypeDef,
-    HttpRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
+    GrpcRouteOutputTypeDef,
     GrpcRouteTypeDef,
+    HttpGatewayRouteOutputTypeDef,
     HttpGatewayRouteTypeDef,
+    HttpRouteOutputTypeDef,
     HttpRouteTypeDef,
     LoggingOutputTypeDef,
     VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
@@ -674,27 +604,27 @@
     VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
     GatewayRouteSpecOutputTypeDef,
-    RouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
+    RouteSpecOutputTypeDef,
     RouteSpecTypeDef,
     BackendDefaultsOutputTypeDef,
     VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
     VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
     GatewayRouteDataTypeDef,
-    RouteDataTypeDef,
     CreateGatewayRouteInputRequestTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
+    RouteDataTypeDef,
     CreateRouteInputRequestTypeDef,
     UpdateRouteInputRequestTypeDef,
     BackendOutputTypeDef,
     BackendTypeDef,
     VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
@@ -720,15 +650,15 @@
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeOutputTypeDef:
+def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.12/README.md` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-appmesh
+Version: 1.28.15
+Summary: Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 appmesh type-annotations boto3-stubs mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="mypy-boto3-appmesh"></a>
 
 # mypy-boto3-appmesh
 
 [![PyPI - mypy-boto3-appmesh](https://img.shields.io/pypi/v/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -339,265 +371,195 @@
 ### Typed dictionaries
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
-    AwsCloudMapInstanceAttributeOutputTypeDef,
     AwsCloudMapInstanceAttributeTypeDef,
-    ListenerTlsFileCertificateOutputTypeDef,
-    ListenerTlsSdsCertificateOutputTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
     DescribeGatewayRouteInputRequestTypeDef,
     DescribeMeshInputRequestTypeDef,
     DescribeRouteInputRequestTypeDef,
     DescribeVirtualGatewayInputRequestTypeDef,
     DescribeVirtualNodeInputRequestTypeDef,
     DescribeVirtualRouterInputRequestTypeDef,
     DescribeVirtualServiceInputRequestTypeDef,
-    DnsServiceDiscoveryOutputTypeDef,
     DnsServiceDiscoveryTypeDef,
-    DurationOutputTypeDef,
     DurationTypeDef,
-    EgressFilterOutputTypeDef,
     EgressFilterTypeDef,
     GatewayRouteStatusTypeDef,
     ResourceMetadataTypeDef,
-    GatewayRouteHostnameMatchOutputTypeDef,
     GatewayRouteHostnameMatchTypeDef,
-    GatewayRouteHostnameRewriteOutputTypeDef,
     GatewayRouteHostnameRewriteTypeDef,
     GatewayRouteRefTypeDef,
-    GatewayRouteVirtualServiceOutputTypeDef,
     GatewayRouteVirtualServiceTypeDef,
-    MatchRangeOutputTypeDef,
     MatchRangeTypeDef,
-    WeightedTargetOutputTypeDef,
     WeightedTargetTypeDef,
-    HealthCheckPolicyOutputTypeDef,
     HealthCheckPolicyTypeDef,
-    HttpPathMatchOutputTypeDef,
     HttpPathMatchTypeDef,
-    HttpGatewayRoutePathRewriteOutputTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
-    HttpGatewayRoutePrefixRewriteOutputTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
-    QueryParameterMatchOutputTypeDef,
     QueryParameterMatchTypeDef,
-    JsonFormatRefOutputTypeDef,
     JsonFormatRefTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagRefOutputTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
-    PortMappingOutputTypeDef,
-    ListenerTlsAcmCertificateOutputTypeDef,
+    PortMappingTypeDef,
     ListenerTlsAcmCertificateTypeDef,
-    TlsValidationContextFileTrustOutputTypeDef,
-    TlsValidationContextSdsTrustOutputTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
-    PortMappingTypeDef,
     MeshStatusTypeDef,
-    MeshServiceDiscoveryOutputTypeDef,
     MeshServiceDiscoveryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
     SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
-    TcpRouteMatchOutputTypeDef,
     TcpRouteMatchTypeDef,
     TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
-    VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
-    VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
-    VirtualGatewayGrpcConnectionPoolOutputTypeDef,
-    VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
-    VirtualGatewayHttpConnectionPoolOutputTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
-    VirtualGatewayHealthCheckPolicyOutputTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
-    VirtualGatewayPortMappingOutputTypeDef,
-    VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
+    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
-    VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
-    VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
-    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
-    VirtualNodeGrpcConnectionPoolOutputTypeDef,
-    VirtualNodeHttp2ConnectionPoolOutputTypeDef,
-    VirtualNodeHttpConnectionPoolOutputTypeDef,
-    VirtualNodeTcpConnectionPoolOutputTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
-    VirtualNodeServiceProviderOutputTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
-    VirtualRouterServiceProviderOutputTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
     AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
-    ClientTlsCertificateOutputTypeDef,
     ClientTlsCertificateTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     GrpcRetryPolicyOutputTypeDef,
-    GrpcTimeoutOutputTypeDef,
-    HttpRetryPolicyOutputTypeDef,
-    HttpTimeoutOutputTypeDef,
-    OutlierDetectionOutputTypeDef,
-    TcpTimeoutOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
+    HttpRetryPolicyOutputTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
-    GrpcGatewayRouteRewriteOutputTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
-    GatewayRouteTargetOutputTypeDef,
     GatewayRouteTargetTypeDef,
-    GrpcMetadataMatchMethodOutputTypeDef,
-    GrpcRouteMetadataMatchMethodOutputTypeDef,
-    HeaderMatchMethodOutputTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
     GrpcRouteActionOutputTypeDef,
-    HttpRouteActionOutputTypeDef,
-    TcpRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
+    HttpRouteActionOutputTypeDef,
     HttpRouteActionTypeDef,
+    TcpRouteActionOutputTypeDef,
     TcpRouteActionTypeDef,
-    HttpGatewayRouteRewriteOutputTypeDef,
     HttpGatewayRouteRewriteTypeDef,
-    HttpQueryParameterOutputTypeDef,
     HttpQueryParameterTypeDef,
     LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
-    VirtualRouterListenerOutputTypeDef,
-    ListenerTlsCertificateOutputTypeDef,
+    VirtualRouterListenerTypeDef,
     ListenerTlsCertificateTypeDef,
-    ListenerTlsValidationContextTrustOutputTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
-    VirtualRouterListenerTypeDef,
-    MeshSpecOutputTypeDef,
     MeshSpecTypeDef,
     SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
     TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
-    VirtualGatewayClientTlsCertificateOutputTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
-    VirtualGatewayConnectionPoolOutputTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
-    VirtualGatewayListenerTlsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
-    VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
-    VirtualNodeConnectionPoolOutputTypeDef,
     VirtualNodeConnectionPoolTypeDef,
-    VirtualServiceProviderOutputTypeDef,
     VirtualServiceProviderTypeDef,
     ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
-    ListenerTimeoutOutputTypeDef,
     ListenerTimeoutTypeDef,
-    GrpcGatewayRouteActionOutputTypeDef,
     GrpcGatewayRouteActionTypeDef,
-    GrpcGatewayRouteMetadataOutputTypeDef,
-    GrpcRouteMetadataOutputTypeDef,
-    HttpGatewayRouteHeaderOutputTypeDef,
-    HttpRouteHeaderOutputTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
     TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
-    HttpGatewayRouteActionOutputTypeDef,
     HttpGatewayRouteActionTypeDef,
     FileAccessLogOutputTypeDef,
     VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
     VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
-    MeshDataTypeDef,
     CreateMeshInputRequestTypeDef,
+    MeshDataTypeDef,
     UpdateMeshInputRequestTypeDef,
     ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
     TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
     VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
     VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
-    VirtualServiceSpecOutputTypeDef,
     VirtualServiceSpecTypeDef,
     GrpcGatewayRouteMatchOutputTypeDef,
-    GrpcRouteMatchOutputTypeDef,
-    HttpGatewayRouteMatchOutputTypeDef,
-    HttpRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
+    GrpcRouteMatchOutputTypeDef,
     GrpcRouteMatchTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
     HttpGatewayRouteMatchTypeDef,
+    HttpRouteMatchOutputTypeDef,
     HttpRouteMatchTypeDef,
     AccessLogOutputTypeDef,
     VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
     VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
@@ -610,24 +572,24 @@
     ListenerTlsTypeDef,
     ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
     VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
     VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
-    VirtualServiceDataTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
+    VirtualServiceDataTypeDef,
     GrpcGatewayRouteOutputTypeDef,
-    GrpcRouteOutputTypeDef,
-    HttpGatewayRouteOutputTypeDef,
-    HttpRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
+    GrpcRouteOutputTypeDef,
     GrpcRouteTypeDef,
+    HttpGatewayRouteOutputTypeDef,
     HttpGatewayRouteTypeDef,
+    HttpRouteOutputTypeDef,
     HttpRouteTypeDef,
     LoggingOutputTypeDef,
     VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
@@ -642,27 +604,27 @@
     VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
     GatewayRouteSpecOutputTypeDef,
-    RouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
+    RouteSpecOutputTypeDef,
     RouteSpecTypeDef,
     BackendDefaultsOutputTypeDef,
     VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
     VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
     GatewayRouteDataTypeDef,
-    RouteDataTypeDef,
     CreateGatewayRouteInputRequestTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
+    RouteDataTypeDef,
     CreateRouteInputRequestTypeDef,
     UpdateRouteInputRequestTypeDef,
     BackendOutputTypeDef,
     BackendTypeDef,
     VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
@@ -688,15 +650,15 @@
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeOutputTypeDef:
+def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__init__.py` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__init__.pyi` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/__main__.py` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.AppMesh 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.AppMesh 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/client.py` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/client.pyi` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/literals.py` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/literals.pyi` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/paginator.py` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/paginator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -56,162 +56,136 @@
     "ListTagsForResourcePaginator",
     "ListVirtualGatewaysPaginator",
     "ListVirtualNodesPaginator",
     "ListVirtualRoutersPaginator",
     "ListVirtualServicesPaginator",
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
 class ListGatewayRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listgatewayroutespaginator)
     """
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewayRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listgatewayroutespaginator)
         """
 
-
 class ListMeshesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listmeshespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMeshesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listmeshespaginator)
         """
 
-
 class ListRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listroutespaginator)
     """
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listroutespaginator)
         """
 
-
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listtagsforresourcepaginator)
         """
 
-
 class ListVirtualGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualgatewayspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualgatewayspaginator)
         """
 
-
 class ListVirtualNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualnodespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualNodesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualnodespaginator)
         """
 
-
 class ListVirtualRoutersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualrouterspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualRoutersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualrouterspaginator)
         """
 
-
 class ListVirtualServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualservicespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualservicespaginator)
         """
```

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/paginator.pyi` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,152 +56,146 @@
     "ListTagsForResourcePaginator",
     "ListVirtualGatewaysPaginator",
     "ListVirtualNodesPaginator",
     "ListVirtualRoutersPaginator",
     "ListVirtualServicesPaginator",
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
 class ListGatewayRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listgatewayroutespaginator)
     """
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGatewayRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listgatewayroutespaginator)
         """
 
+
 class ListMeshesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listmeshespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMeshesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listmeshespaginator)
         """
 
+
 class ListRoutesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listroutespaginator)
     """
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listroutespaginator)
         """
 
+
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listtagsforresourcepaginator)
         """
 
+
 class ListVirtualGatewaysPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualgatewayspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualgatewayspaginator)
         """
 
+
 class ListVirtualNodesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualnodespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualNodesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualnodespaginator)
         """
 
+
 class ListVirtualRoutersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualrouterspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualRoutersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualrouterspaginator)
         """
 
+
 class ListVirtualServicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualservicespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListVirtualServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/paginators/#listvirtualservicespaginator)
         """
```

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/type_defs.py` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appmesh service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appmesh.type_defs import AwsCloudMapInstanceAttributeOutputTypeDef
+    from mypy_boto3_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
 
-    data: AwsCloudMapInstanceAttributeOutputTypeDef = {...}
+    data: AwsCloudMapInstanceAttributeTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -44,265 +44,195 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AwsCloudMapInstanceAttributeOutputTypeDef",
     "AwsCloudMapInstanceAttributeTypeDef",
-    "ListenerTlsFileCertificateOutputTypeDef",
-    "ListenerTlsSdsCertificateOutputTypeDef",
     "ListenerTlsFileCertificateTypeDef",
     "ListenerTlsSdsCertificateTypeDef",
     "TagRefTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteGatewayRouteInputRequestTypeDef",
     "DeleteMeshInputRequestTypeDef",
     "DeleteRouteInputRequestTypeDef",
     "DeleteVirtualGatewayInputRequestTypeDef",
     "DeleteVirtualNodeInputRequestTypeDef",
     "DeleteVirtualRouterInputRequestTypeDef",
     "DeleteVirtualServiceInputRequestTypeDef",
     "DescribeGatewayRouteInputRequestTypeDef",
     "DescribeMeshInputRequestTypeDef",
     "DescribeRouteInputRequestTypeDef",
     "DescribeVirtualGatewayInputRequestTypeDef",
     "DescribeVirtualNodeInputRequestTypeDef",
     "DescribeVirtualRouterInputRequestTypeDef",
     "DescribeVirtualServiceInputRequestTypeDef",
-    "DnsServiceDiscoveryOutputTypeDef",
     "DnsServiceDiscoveryTypeDef",
-    "DurationOutputTypeDef",
     "DurationTypeDef",
-    "EgressFilterOutputTypeDef",
     "EgressFilterTypeDef",
     "GatewayRouteStatusTypeDef",
     "ResourceMetadataTypeDef",
-    "GatewayRouteHostnameMatchOutputTypeDef",
     "GatewayRouteHostnameMatchTypeDef",
-    "GatewayRouteHostnameRewriteOutputTypeDef",
     "GatewayRouteHostnameRewriteTypeDef",
     "GatewayRouteRefTypeDef",
-    "GatewayRouteVirtualServiceOutputTypeDef",
     "GatewayRouteVirtualServiceTypeDef",
-    "MatchRangeOutputTypeDef",
     "MatchRangeTypeDef",
-    "WeightedTargetOutputTypeDef",
     "WeightedTargetTypeDef",
-    "HealthCheckPolicyOutputTypeDef",
     "HealthCheckPolicyTypeDef",
-    "HttpPathMatchOutputTypeDef",
     "HttpPathMatchTypeDef",
-    "HttpGatewayRoutePathRewriteOutputTypeDef",
     "HttpGatewayRoutePathRewriteTypeDef",
-    "HttpGatewayRoutePrefixRewriteOutputTypeDef",
     "HttpGatewayRoutePrefixRewriteTypeDef",
-    "QueryParameterMatchOutputTypeDef",
     "QueryParameterMatchTypeDef",
-    "JsonFormatRefOutputTypeDef",
     "JsonFormatRefTypeDef",
-    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListGatewayRoutesInputRequestTypeDef",
-    "ListMeshesInputListMeshesPaginateTypeDef",
     "ListMeshesInputRequestTypeDef",
     "MeshRefTypeDef",
-    "ListRoutesInputListRoutesPaginateTypeDef",
     "ListRoutesInputRequestTypeDef",
     "RouteRefTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagRefOutputTypeDef",
-    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualGatewaysInputRequestTypeDef",
     "VirtualGatewayRefTypeDef",
-    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
-    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
-    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
-    "PortMappingOutputTypeDef",
-    "ListenerTlsAcmCertificateOutputTypeDef",
+    "PortMappingTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
-    "TlsValidationContextFileTrustOutputTypeDef",
-    "TlsValidationContextSdsTrustOutputTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
-    "PortMappingTypeDef",
     "MeshStatusTypeDef",
-    "MeshServiceDiscoveryOutputTypeDef",
     "MeshServiceDiscoveryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RouteStatusTypeDef",
     "SubjectAlternativeNameMatchersOutputTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
-    "TcpRouteMatchOutputTypeDef",
     "TcpRouteMatchTypeDef",
     "TlsValidationContextAcmTrustOutputTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "VirtualGatewayListenerTlsFileCertificateOutputTypeDef",
-    "VirtualGatewayListenerTlsSdsCertificateOutputTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
-    "VirtualGatewayGrpcConnectionPoolOutputTypeDef",
-    "VirtualGatewayHttp2ConnectionPoolOutputTypeDef",
-    "VirtualGatewayHttpConnectionPoolOutputTypeDef",
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     "VirtualGatewayHttp2ConnectionPoolTypeDef",
     "VirtualGatewayHttpConnectionPoolTypeDef",
     "VirtualGatewayStatusTypeDef",
-    "VirtualGatewayHealthCheckPolicyOutputTypeDef",
     "VirtualGatewayHealthCheckPolicyTypeDef",
-    "VirtualGatewayPortMappingOutputTypeDef",
-    "VirtualGatewayListenerTlsAcmCertificateOutputTypeDef",
+    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
-    "VirtualGatewayTlsValidationContextFileTrustOutputTypeDef",
-    "VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
-    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
-    "VirtualNodeGrpcConnectionPoolOutputTypeDef",
-    "VirtualNodeHttp2ConnectionPoolOutputTypeDef",
-    "VirtualNodeHttpConnectionPoolOutputTypeDef",
-    "VirtualNodeTcpConnectionPoolOutputTypeDef",
     "VirtualNodeGrpcConnectionPoolTypeDef",
     "VirtualNodeHttp2ConnectionPoolTypeDef",
     "VirtualNodeHttpConnectionPoolTypeDef",
     "VirtualNodeTcpConnectionPoolTypeDef",
     "VirtualNodeStatusTypeDef",
-    "VirtualNodeServiceProviderOutputTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
-    "VirtualRouterServiceProviderOutputTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
     "AwsCloudMapServiceDiscoveryOutputTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
-    "ClientTlsCertificateOutputTypeDef",
     "ClientTlsCertificateTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "GrpcRetryPolicyOutputTypeDef",
-    "GrpcTimeoutOutputTypeDef",
-    "HttpRetryPolicyOutputTypeDef",
-    "HttpTimeoutOutputTypeDef",
-    "OutlierDetectionOutputTypeDef",
-    "TcpTimeoutOutputTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
+    "HttpRetryPolicyOutputTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
-    "GrpcGatewayRouteRewriteOutputTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
     "ListGatewayRoutesOutputTypeDef",
-    "GatewayRouteTargetOutputTypeDef",
     "GatewayRouteTargetTypeDef",
-    "GrpcMetadataMatchMethodOutputTypeDef",
-    "GrpcRouteMetadataMatchMethodOutputTypeDef",
-    "HeaderMatchMethodOutputTypeDef",
     "GrpcMetadataMatchMethodTypeDef",
     "GrpcRouteMetadataMatchMethodTypeDef",
     "HeaderMatchMethodTypeDef",
     "GrpcRouteActionOutputTypeDef",
-    "HttpRouteActionOutputTypeDef",
-    "TcpRouteActionOutputTypeDef",
     "GrpcRouteActionTypeDef",
+    "HttpRouteActionOutputTypeDef",
     "HttpRouteActionTypeDef",
+    "TcpRouteActionOutputTypeDef",
     "TcpRouteActionTypeDef",
-    "HttpGatewayRouteRewriteOutputTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
-    "HttpQueryParameterOutputTypeDef",
     "HttpQueryParameterTypeDef",
     "LoggingFormatOutputTypeDef",
     "LoggingFormatTypeDef",
+    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    "ListRoutesInputListRoutesPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
-    "VirtualRouterListenerOutputTypeDef",
-    "ListenerTlsCertificateOutputTypeDef",
+    "VirtualRouterListenerTypeDef",
     "ListenerTlsCertificateTypeDef",
-    "ListenerTlsValidationContextTrustOutputTypeDef",
     "ListenerTlsValidationContextTrustTypeDef",
-    "VirtualRouterListenerTypeDef",
-    "MeshSpecOutputTypeDef",
     "MeshSpecTypeDef",
     "SubjectAlternativeNamesOutputTypeDef",
     "SubjectAlternativeNamesTypeDef",
     "TlsValidationContextTrustOutputTypeDef",
     "TlsValidationContextTrustTypeDef",
-    "VirtualGatewayClientTlsCertificateOutputTypeDef",
     "VirtualGatewayClientTlsCertificateTypeDef",
-    "VirtualGatewayConnectionPoolOutputTypeDef",
     "VirtualGatewayConnectionPoolTypeDef",
-    "VirtualGatewayListenerTlsCertificateOutputTypeDef",
     "VirtualGatewayListenerTlsCertificateTypeDef",
-    "VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
     "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextTrustTypeDef",
-    "VirtualNodeConnectionPoolOutputTypeDef",
     "VirtualNodeConnectionPoolTypeDef",
-    "VirtualServiceProviderOutputTypeDef",
     "VirtualServiceProviderTypeDef",
     "ServiceDiscoveryOutputTypeDef",
     "ServiceDiscoveryTypeDef",
-    "ListenerTimeoutOutputTypeDef",
     "ListenerTimeoutTypeDef",
-    "GrpcGatewayRouteActionOutputTypeDef",
     "GrpcGatewayRouteActionTypeDef",
-    "GrpcGatewayRouteMetadataOutputTypeDef",
-    "GrpcRouteMetadataOutputTypeDef",
-    "HttpGatewayRouteHeaderOutputTypeDef",
-    "HttpRouteHeaderOutputTypeDef",
     "GrpcGatewayRouteMetadataTypeDef",
     "GrpcRouteMetadataTypeDef",
     "HttpGatewayRouteHeaderTypeDef",
     "HttpRouteHeaderTypeDef",
     "TcpRouteOutputTypeDef",
     "TcpRouteTypeDef",
-    "HttpGatewayRouteActionOutputTypeDef",
     "HttpGatewayRouteActionTypeDef",
     "FileAccessLogOutputTypeDef",
     "VirtualGatewayFileAccessLogOutputTypeDef",
     "FileAccessLogTypeDef",
     "VirtualGatewayFileAccessLogTypeDef",
     "VirtualRouterSpecOutputTypeDef",
     "VirtualRouterSpecTypeDef",
-    "MeshDataTypeDef",
     "CreateMeshInputRequestTypeDef",
+    "MeshDataTypeDef",
     "UpdateMeshInputRequestTypeDef",
     "ListenerTlsValidationContextOutputTypeDef",
     "ListenerTlsValidationContextTypeDef",
     "TlsValidationContextOutputTypeDef",
     "TlsValidationContextTypeDef",
     "VirtualGatewayListenerTlsValidationContextOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTypeDef",
     "VirtualGatewayTlsValidationContextOutputTypeDef",
     "VirtualGatewayTlsValidationContextTypeDef",
-    "VirtualServiceSpecOutputTypeDef",
     "VirtualServiceSpecTypeDef",
     "GrpcGatewayRouteMatchOutputTypeDef",
-    "GrpcRouteMatchOutputTypeDef",
-    "HttpGatewayRouteMatchOutputTypeDef",
-    "HttpRouteMatchOutputTypeDef",
     "GrpcGatewayRouteMatchTypeDef",
+    "GrpcRouteMatchOutputTypeDef",
     "GrpcRouteMatchTypeDef",
+    "HttpGatewayRouteMatchOutputTypeDef",
     "HttpGatewayRouteMatchTypeDef",
+    "HttpRouteMatchOutputTypeDef",
     "HttpRouteMatchTypeDef",
     "AccessLogOutputTypeDef",
     "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
     "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
@@ -315,24 +245,24 @@
     "ListenerTlsTypeDef",
     "ClientPolicyTlsOutputTypeDef",
     "ClientPolicyTlsTypeDef",
     "VirtualGatewayListenerTlsOutputTypeDef",
     "VirtualGatewayListenerTlsTypeDef",
     "VirtualGatewayClientPolicyTlsOutputTypeDef",
     "VirtualGatewayClientPolicyTlsTypeDef",
-    "VirtualServiceDataTypeDef",
     "CreateVirtualServiceInputRequestTypeDef",
     "UpdateVirtualServiceInputRequestTypeDef",
+    "VirtualServiceDataTypeDef",
     "GrpcGatewayRouteOutputTypeDef",
-    "GrpcRouteOutputTypeDef",
-    "HttpGatewayRouteOutputTypeDef",
-    "HttpRouteOutputTypeDef",
     "GrpcGatewayRouteTypeDef",
+    "GrpcRouteOutputTypeDef",
     "GrpcRouteTypeDef",
+    "HttpGatewayRouteOutputTypeDef",
     "HttpGatewayRouteTypeDef",
+    "HttpRouteOutputTypeDef",
     "HttpRouteTypeDef",
     "LoggingOutputTypeDef",
     "VirtualGatewayLoggingOutputTypeDef",
     "LoggingTypeDef",
     "VirtualGatewayLoggingTypeDef",
     "CreateVirtualRouterOutputTypeDef",
     "DeleteVirtualRouterOutputTypeDef",
@@ -347,27 +277,27 @@
     "VirtualGatewayClientPolicyOutputTypeDef",
     "VirtualGatewayClientPolicyTypeDef",
     "CreateVirtualServiceOutputTypeDef",
     "DeleteVirtualServiceOutputTypeDef",
     "DescribeVirtualServiceOutputTypeDef",
     "UpdateVirtualServiceOutputTypeDef",
     "GatewayRouteSpecOutputTypeDef",
-    "RouteSpecOutputTypeDef",
     "GatewayRouteSpecTypeDef",
+    "RouteSpecOutputTypeDef",
     "RouteSpecTypeDef",
     "BackendDefaultsOutputTypeDef",
     "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
     "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
     "GatewayRouteDataTypeDef",
-    "RouteDataTypeDef",
     "CreateGatewayRouteInputRequestTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
+    "RouteDataTypeDef",
     "CreateRouteInputRequestTypeDef",
     "UpdateRouteInputRequestTypeDef",
     "BackendOutputTypeDef",
     "BackendTypeDef",
     "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
@@ -392,45 +322,22 @@
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
     "UpdateVirtualNodeOutputTypeDef",
 )
 
-AwsCloudMapInstanceAttributeOutputTypeDef = TypedDict(
-    "AwsCloudMapInstanceAttributeOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 AwsCloudMapInstanceAttributeTypeDef = TypedDict(
     "AwsCloudMapInstanceAttributeTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-ListenerTlsFileCertificateOutputTypeDef = TypedDict(
-    "ListenerTlsFileCertificateOutputTypeDef",
-    {
-        "certificateChain": str,
-        "privateKey": str,
-    },
-)
-
-ListenerTlsSdsCertificateOutputTypeDef = TypedDict(
-    "ListenerTlsSdsCertificateOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-
 ListenerTlsFileCertificateTypeDef = TypedDict(
     "ListenerTlsFileCertificateTypeDef",
     {
         "certificateChain": str,
         "privateKey": str,
     },
 )
@@ -446,14 +353,25 @@
     "TagRefTypeDef",
     {
         "key": str,
         "value": str,
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
 _RequiredDeleteGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDeleteGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -748,36 +666,14 @@
 class DescribeVirtualServiceInputRequestTypeDef(
     _RequiredDescribeVirtualServiceInputRequestTypeDef,
     _OptionalDescribeVirtualServiceInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredDnsServiceDiscoveryOutputTypeDef = TypedDict(
-    "_RequiredDnsServiceDiscoveryOutputTypeDef",
-    {
-        "hostname": str,
-    },
-)
-_OptionalDnsServiceDiscoveryOutputTypeDef = TypedDict(
-    "_OptionalDnsServiceDiscoveryOutputTypeDef",
-    {
-        "ipPreference": IpPreferenceType,
-        "responseType": DnsResponseTypeType,
-    },
-    total=False,
-)
-
-
-class DnsServiceDiscoveryOutputTypeDef(
-    _RequiredDnsServiceDiscoveryOutputTypeDef, _OptionalDnsServiceDiscoveryOutputTypeDef
-):
-    pass
-
-
 _RequiredDnsServiceDiscoveryTypeDef = TypedDict(
     "_RequiredDnsServiceDiscoveryTypeDef",
     {
         "hostname": str,
     },
 )
 _OptionalDnsServiceDiscoveryTypeDef = TypedDict(
@@ -792,39 +688,23 @@
 
 class DnsServiceDiscoveryTypeDef(
     _RequiredDnsServiceDiscoveryTypeDef, _OptionalDnsServiceDiscoveryTypeDef
 ):
     pass
 
 
-DurationOutputTypeDef = TypedDict(
-    "DurationOutputTypeDef",
-    {
-        "unit": DurationUnitType,
-        "value": int,
-    },
-    total=False,
-)
-
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "unit": DurationUnitType,
         "value": int,
     },
     total=False,
 )
 
-EgressFilterOutputTypeDef = TypedDict(
-    "EgressFilterOutputTypeDef",
-    {
-        "type": EgressFilterTypeType,
-    },
-)
-
 EgressFilterTypeDef = TypedDict(
     "EgressFilterTypeDef",
     {
         "type": EgressFilterTypeType,
     },
 )
 
@@ -844,40 +724,23 @@
         "meshOwner": str,
         "resourceOwner": str,
         "uid": str,
         "version": int,
     },
 )
 
-GatewayRouteHostnameMatchOutputTypeDef = TypedDict(
-    "GatewayRouteHostnameMatchOutputTypeDef",
-    {
-        "exact": str,
-        "suffix": str,
-    },
-    total=False,
-)
-
 GatewayRouteHostnameMatchTypeDef = TypedDict(
     "GatewayRouteHostnameMatchTypeDef",
     {
         "exact": str,
         "suffix": str,
     },
     total=False,
 )
 
-GatewayRouteHostnameRewriteOutputTypeDef = TypedDict(
-    "GatewayRouteHostnameRewriteOutputTypeDef",
-    {
-        "defaultTargetHostname": DefaultGatewayRouteRewriteType,
-    },
-    total=False,
-)
-
 GatewayRouteHostnameRewriteTypeDef = TypedDict(
     "GatewayRouteHostnameRewriteTypeDef",
     {
         "defaultTargetHostname": DefaultGatewayRouteRewriteType,
     },
     total=False,
 )
@@ -893,66 +756,29 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
-GatewayRouteVirtualServiceOutputTypeDef = TypedDict(
-    "GatewayRouteVirtualServiceOutputTypeDef",
-    {
-        "virtualServiceName": str,
-    },
-)
-
 GatewayRouteVirtualServiceTypeDef = TypedDict(
     "GatewayRouteVirtualServiceTypeDef",
     {
         "virtualServiceName": str,
     },
 )
 
-MatchRangeOutputTypeDef = TypedDict(
-    "MatchRangeOutputTypeDef",
-    {
-        "end": int,
-        "start": int,
-    },
-)
-
 MatchRangeTypeDef = TypedDict(
     "MatchRangeTypeDef",
     {
         "end": int,
         "start": int,
     },
 )
 
-_RequiredWeightedTargetOutputTypeDef = TypedDict(
-    "_RequiredWeightedTargetOutputTypeDef",
-    {
-        "virtualNode": str,
-        "weight": int,
-    },
-)
-_OptionalWeightedTargetOutputTypeDef = TypedDict(
-    "_OptionalWeightedTargetOutputTypeDef",
-    {
-        "port": int,
-    },
-    total=False,
-)
-
-
-class WeightedTargetOutputTypeDef(
-    _RequiredWeightedTargetOutputTypeDef, _OptionalWeightedTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredWeightedTargetTypeDef = TypedDict(
     "_RequiredWeightedTargetTypeDef",
     {
         "virtualNode": str,
         "weight": int,
     },
 )
@@ -965,40 +791,14 @@
 )
 
 
 class WeightedTargetTypeDef(_RequiredWeightedTargetTypeDef, _OptionalWeightedTargetTypeDef):
     pass
 
 
-_RequiredHealthCheckPolicyOutputTypeDef = TypedDict(
-    "_RequiredHealthCheckPolicyOutputTypeDef",
-    {
-        "healthyThreshold": int,
-        "intervalMillis": int,
-        "protocol": PortProtocolType,
-        "timeoutMillis": int,
-        "unhealthyThreshold": int,
-    },
-)
-_OptionalHealthCheckPolicyOutputTypeDef = TypedDict(
-    "_OptionalHealthCheckPolicyOutputTypeDef",
-    {
-        "path": str,
-        "port": int,
-    },
-    total=False,
-)
-
-
-class HealthCheckPolicyOutputTypeDef(
-    _RequiredHealthCheckPolicyOutputTypeDef, _OptionalHealthCheckPolicyOutputTypeDef
-):
-    pass
-
-
 _RequiredHealthCheckPolicyTypeDef = TypedDict(
     "_RequiredHealthCheckPolicyTypeDef",
     {
         "healthyThreshold": int,
         "intervalMillis": int,
         "protocol": PortProtocolType,
         "timeoutMillis": int,
@@ -1017,122 +817,66 @@
 
 class HealthCheckPolicyTypeDef(
     _RequiredHealthCheckPolicyTypeDef, _OptionalHealthCheckPolicyTypeDef
 ):
     pass
 
 
-HttpPathMatchOutputTypeDef = TypedDict(
-    "HttpPathMatchOutputTypeDef",
-    {
-        "exact": str,
-        "regex": str,
-    },
-    total=False,
-)
-
 HttpPathMatchTypeDef = TypedDict(
     "HttpPathMatchTypeDef",
     {
         "exact": str,
         "regex": str,
     },
     total=False,
 )
 
-HttpGatewayRoutePathRewriteOutputTypeDef = TypedDict(
-    "HttpGatewayRoutePathRewriteOutputTypeDef",
-    {
-        "exact": str,
-    },
-    total=False,
-)
-
 HttpGatewayRoutePathRewriteTypeDef = TypedDict(
     "HttpGatewayRoutePathRewriteTypeDef",
     {
         "exact": str,
     },
     total=False,
 )
 
-HttpGatewayRoutePrefixRewriteOutputTypeDef = TypedDict(
-    "HttpGatewayRoutePrefixRewriteOutputTypeDef",
-    {
-        "defaultPrefix": DefaultGatewayRouteRewriteType,
-        "value": str,
-    },
-    total=False,
-)
-
 HttpGatewayRoutePrefixRewriteTypeDef = TypedDict(
     "HttpGatewayRoutePrefixRewriteTypeDef",
     {
         "defaultPrefix": DefaultGatewayRouteRewriteType,
         "value": str,
     },
     total=False,
 )
 
-QueryParameterMatchOutputTypeDef = TypedDict(
-    "QueryParameterMatchOutputTypeDef",
-    {
-        "exact": str,
-    },
-    total=False,
-)
-
 QueryParameterMatchTypeDef = TypedDict(
     "QueryParameterMatchTypeDef",
     {
         "exact": str,
     },
     total=False,
 )
 
-JsonFormatRefOutputTypeDef = TypedDict(
-    "JsonFormatRefOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 JsonFormatRefTypeDef = TypedDict(
     "JsonFormatRefTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualGatewayName": str,
-    },
-)
-_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
-    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGatewayRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListGatewayRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -1149,22 +893,14 @@
 
 class ListGatewayRoutesInputRequestTypeDef(
     _RequiredListGatewayRoutesInputRequestTypeDef, _OptionalListGatewayRoutesInputRequestTypeDef
 ):
     pass
 
 
-ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
-    "ListMeshesInputListMeshesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMeshesInputRequestTypeDef = TypedDict(
     "ListMeshesInputRequestTypeDef",
     {
         "limit": int,
         "nextToken": str,
     },
     total=False,
@@ -1179,38 +915,14 @@
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
     },
 )
 
-_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualRouterName": str,
-    },
-)
-_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRoutesInputListRoutesPaginateTypeDef(
-    _RequiredListRoutesInputListRoutesPaginateTypeDef,
-    _OptionalListRoutesInputListRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -1242,36 +954,14 @@
         "resourceOwner": str,
         "routeName": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1286,45 +976,14 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-TagRefOutputTypeDef = TypedDict(
-    "TagRefOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
-_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
-    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVirtualGatewaysInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualGatewaysInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualGatewaysInputRequestTypeDef = TypedDict(
@@ -1354,37 +1013,14 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
-_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
-    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVirtualNodesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualNodesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualNodesInputRequestTypeDef = TypedDict(
@@ -1414,37 +1050,14 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualNodeName": str,
     },
 )
 
-_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
-    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVirtualRoutersInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualRoutersInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualRoutersInputRequestTypeDef = TypedDict(
@@ -1474,37 +1087,14 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
-_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
-    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVirtualServicesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualServicesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualServicesInputRequestTypeDef = TypedDict(
@@ -1534,117 +1124,59 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualServiceName": str,
     },
 )
 
-PortMappingOutputTypeDef = TypedDict(
-    "PortMappingOutputTypeDef",
+PortMappingTypeDef = TypedDict(
+    "PortMappingTypeDef",
     {
         "port": int,
         "protocol": PortProtocolType,
     },
 )
 
-ListenerTlsAcmCertificateOutputTypeDef = TypedDict(
-    "ListenerTlsAcmCertificateOutputTypeDef",
-    {
-        "certificateArn": str,
-    },
-)
-
 ListenerTlsAcmCertificateTypeDef = TypedDict(
     "ListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
-TlsValidationContextFileTrustOutputTypeDef = TypedDict(
-    "TlsValidationContextFileTrustOutputTypeDef",
-    {
-        "certificateChain": str,
-    },
-)
-
-TlsValidationContextSdsTrustOutputTypeDef = TypedDict(
-    "TlsValidationContextSdsTrustOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-
 TlsValidationContextFileTrustTypeDef = TypedDict(
     "TlsValidationContextFileTrustTypeDef",
     {
         "certificateChain": str,
     },
 )
 
 TlsValidationContextSdsTrustTypeDef = TypedDict(
     "TlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-PortMappingTypeDef = TypedDict(
-    "PortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": PortProtocolType,
-    },
-)
-
 MeshStatusTypeDef = TypedDict(
     "MeshStatusTypeDef",
     {
         "status": MeshStatusCodeType,
     },
     total=False,
 )
 
-MeshServiceDiscoveryOutputTypeDef = TypedDict(
-    "MeshServiceDiscoveryOutputTypeDef",
-    {
-        "ipPreference": IpPreferenceType,
-    },
-    total=False,
-)
-
 MeshServiceDiscoveryTypeDef = TypedDict(
     "MeshServiceDiscoveryTypeDef",
     {
         "ipPreference": IpPreferenceType,
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
 RouteStatusTypeDef = TypedDict(
     "RouteStatusTypeDef",
     {
         "status": RouteStatusCodeType,
     },
 )
 
@@ -1658,22 +1190,14 @@
 SubjectAlternativeNameMatchersTypeDef = TypedDict(
     "SubjectAlternativeNameMatchersTypeDef",
     {
         "exact": Sequence[str],
     },
 )
 
-TcpRouteMatchOutputTypeDef = TypedDict(
-    "TcpRouteMatchOutputTypeDef",
-    {
-        "port": int,
-    },
-    total=False,
-)
-
 TcpRouteMatchTypeDef = TypedDict(
     "TcpRouteMatchTypeDef",
     {
         "port": int,
     },
     total=False,
 )
@@ -1696,29 +1220,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-VirtualGatewayListenerTlsFileCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsFileCertificateOutputTypeDef",
-    {
-        "certificateChain": str,
-        "privateKey": str,
-    },
-)
-
-VirtualGatewayListenerTlsSdsCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsSdsCertificateOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-
 VirtualGatewayListenerTlsFileCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     {
         "certificateChain": str,
         "privateKey": str,
     },
 )
@@ -1726,50 +1235,14 @@
 VirtualGatewayListenerTlsSdsCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
     {
         "secretName": str,
     },
 )
 
-VirtualGatewayGrpcConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualGatewayGrpcConnectionPoolOutputTypeDef",
-    {
-        "maxRequests": int,
-    },
-)
-
-VirtualGatewayHttp2ConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualGatewayHttp2ConnectionPoolOutputTypeDef",
-    {
-        "maxRequests": int,
-    },
-)
-
-_RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef",
-    {
-        "maxConnections": int,
-    },
-)
-_OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef",
-    {
-        "maxPendingRequests": int,
-    },
-    total=False,
-)
-
-
-class VirtualGatewayHttpConnectionPoolOutputTypeDef(
-    _RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef,
-    _OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef,
-):
-    pass
-
-
 VirtualGatewayGrpcConnectionPoolTypeDef = TypedDict(
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     {
         "maxRequests": int,
     },
 )
 
@@ -1805,41 +1278,14 @@
 VirtualGatewayStatusTypeDef = TypedDict(
     "VirtualGatewayStatusTypeDef",
     {
         "status": VirtualGatewayStatusCodeType,
     },
 )
 
-_RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef",
-    {
-        "healthyThreshold": int,
-        "intervalMillis": int,
-        "protocol": VirtualGatewayPortProtocolType,
-        "timeoutMillis": int,
-        "unhealthyThreshold": int,
-    },
-)
-_OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef",
-    {
-        "path": str,
-        "port": int,
-    },
-    total=False,
-)
-
-
-class VirtualGatewayHealthCheckPolicyOutputTypeDef(
-    _RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef,
-    _OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef,
-):
-    pass
-
-
 _RequiredVirtualGatewayHealthCheckPolicyTypeDef = TypedDict(
     "_RequiredVirtualGatewayHealthCheckPolicyTypeDef",
     {
         "healthyThreshold": int,
         "intervalMillis": int,
         "protocol": VirtualGatewayPortProtocolType,
         "timeoutMillis": int,
@@ -1858,129 +1304,57 @@
 
 class VirtualGatewayHealthCheckPolicyTypeDef(
     _RequiredVirtualGatewayHealthCheckPolicyTypeDef, _OptionalVirtualGatewayHealthCheckPolicyTypeDef
 ):
     pass
 
 
-VirtualGatewayPortMappingOutputTypeDef = TypedDict(
-    "VirtualGatewayPortMappingOutputTypeDef",
+VirtualGatewayPortMappingTypeDef = TypedDict(
+    "VirtualGatewayPortMappingTypeDef",
     {
         "port": int,
         "protocol": VirtualGatewayPortProtocolType,
     },
 )
 
-VirtualGatewayListenerTlsAcmCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsAcmCertificateOutputTypeDef",
-    {
-        "certificateArn": str,
-    },
-)
-
 VirtualGatewayListenerTlsAcmCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
-VirtualGatewayTlsValidationContextFileTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayTlsValidationContextFileTrustOutputTypeDef",
-    {
-        "certificateChain": str,
-    },
-)
-
-VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-
 VirtualGatewayTlsValidationContextFileTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     {
         "certificateChain": str,
     },
 )
 
 VirtualGatewayTlsValidationContextSdsTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-VirtualGatewayPortMappingTypeDef = TypedDict(
-    "VirtualGatewayPortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": VirtualGatewayPortProtocolType,
-    },
-)
-
 VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     {
         "certificateAuthorityArns": List[str],
     },
 )
 
 VirtualGatewayTlsValidationContextAcmTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
     },
 )
 
-VirtualNodeGrpcConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualNodeGrpcConnectionPoolOutputTypeDef",
-    {
-        "maxRequests": int,
-    },
-)
-
-VirtualNodeHttp2ConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualNodeHttp2ConnectionPoolOutputTypeDef",
-    {
-        "maxRequests": int,
-    },
-)
-
-_RequiredVirtualNodeHttpConnectionPoolOutputTypeDef = TypedDict(
-    "_RequiredVirtualNodeHttpConnectionPoolOutputTypeDef",
-    {
-        "maxConnections": int,
-    },
-)
-_OptionalVirtualNodeHttpConnectionPoolOutputTypeDef = TypedDict(
-    "_OptionalVirtualNodeHttpConnectionPoolOutputTypeDef",
-    {
-        "maxPendingRequests": int,
-    },
-    total=False,
-)
-
-
-class VirtualNodeHttpConnectionPoolOutputTypeDef(
-    _RequiredVirtualNodeHttpConnectionPoolOutputTypeDef,
-    _OptionalVirtualNodeHttpConnectionPoolOutputTypeDef,
-):
-    pass
-
-
-VirtualNodeTcpConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualNodeTcpConnectionPoolOutputTypeDef",
-    {
-        "maxConnections": int,
-    },
-)
-
 VirtualNodeGrpcConnectionPoolTypeDef = TypedDict(
     "VirtualNodeGrpcConnectionPoolTypeDef",
     {
         "maxRequests": int,
     },
 )
 
@@ -2022,42 +1396,28 @@
 VirtualNodeStatusTypeDef = TypedDict(
     "VirtualNodeStatusTypeDef",
     {
         "status": VirtualNodeStatusCodeType,
     },
 )
 
-VirtualNodeServiceProviderOutputTypeDef = TypedDict(
-    "VirtualNodeServiceProviderOutputTypeDef",
-    {
-        "virtualNodeName": str,
-    },
-)
-
 VirtualNodeServiceProviderTypeDef = TypedDict(
     "VirtualNodeServiceProviderTypeDef",
     {
         "virtualNodeName": str,
     },
 )
 
 VirtualRouterStatusTypeDef = TypedDict(
     "VirtualRouterStatusTypeDef",
     {
         "status": VirtualRouterStatusCodeType,
     },
 )
 
-VirtualRouterServiceProviderOutputTypeDef = TypedDict(
-    "VirtualRouterServiceProviderOutputTypeDef",
-    {
-        "virtualRouterName": str,
-    },
-)
-
 VirtualRouterServiceProviderTypeDef = TypedDict(
     "VirtualRouterServiceProviderTypeDef",
     {
         "virtualRouterName": str,
     },
 )
 
@@ -2074,15 +1434,15 @@
         "namespaceName": str,
         "serviceName": str,
     },
 )
 _OptionalAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
     "_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef",
     {
-        "attributes": List[AwsCloudMapInstanceAttributeOutputTypeDef],
+        "attributes": List[AwsCloudMapInstanceAttributeTypeDef],
         "ipPreference": IpPreferenceType,
     },
     total=False,
 )
 
 
 class AwsCloudMapServiceDiscoveryOutputTypeDef(
@@ -2111,23 +1471,14 @@
 
 class AwsCloudMapServiceDiscoveryTypeDef(
     _RequiredAwsCloudMapServiceDiscoveryTypeDef, _OptionalAwsCloudMapServiceDiscoveryTypeDef
 ):
     pass
 
 
-ClientTlsCertificateOutputTypeDef = TypedDict(
-    "ClientTlsCertificateOutputTypeDef",
-    {
-        "file": ListenerTlsFileCertificateOutputTypeDef,
-        "sds": ListenerTlsSdsCertificateOutputTypeDef,
-    },
-    total=False,
-)
-
 ClientTlsCertificateTypeDef = TypedDict(
     "ClientTlsCertificateTypeDef",
     {
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
@@ -2137,19 +1488,28 @@
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagRefTypeDef],
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagRefTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredGrpcRetryPolicyOutputTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyOutputTypeDef",
     {
         "maxRetries": int,
-        "perRetryTimeout": DurationOutputTypeDef,
+        "perRetryTimeout": DurationTypeDef,
     },
 )
 _OptionalGrpcRetryPolicyOutputTypeDef = TypedDict(
     "_OptionalGrpcRetryPolicyOutputTypeDef",
     {
         "grpcRetryEvents": List[GrpcRetryPolicyEventType],
         "httpRetryEvents": List[str],
@@ -2161,104 +1521,68 @@
 
 class GrpcRetryPolicyOutputTypeDef(
     _RequiredGrpcRetryPolicyOutputTypeDef, _OptionalGrpcRetryPolicyOutputTypeDef
 ):
     pass
 
 
-GrpcTimeoutOutputTypeDef = TypedDict(
-    "GrpcTimeoutOutputTypeDef",
-    {
-        "idle": DurationOutputTypeDef,
-        "perRequest": DurationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
-    "_RequiredHttpRetryPolicyOutputTypeDef",
+_RequiredGrpcRetryPolicyTypeDef = TypedDict(
+    "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
-        "perRetryTimeout": DurationOutputTypeDef,
+        "perRetryTimeout": DurationTypeDef,
     },
 )
-_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
-    "_OptionalHttpRetryPolicyOutputTypeDef",
+_OptionalGrpcRetryPolicyTypeDef = TypedDict(
+    "_OptionalGrpcRetryPolicyTypeDef",
     {
-        "httpRetryEvents": List[str],
-        "tcpRetryEvents": List[Literal["connection-error"]],
+        "grpcRetryEvents": Sequence[GrpcRetryPolicyEventType],
+        "httpRetryEvents": Sequence[str],
+        "tcpRetryEvents": Sequence[Literal["connection-error"]],
     },
     total=False,
 )
 
 
-class HttpRetryPolicyOutputTypeDef(
-    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
-):
+class GrpcRetryPolicyTypeDef(_RequiredGrpcRetryPolicyTypeDef, _OptionalGrpcRetryPolicyTypeDef):
     pass
 
 
-HttpTimeoutOutputTypeDef = TypedDict(
-    "HttpTimeoutOutputTypeDef",
-    {
-        "idle": DurationOutputTypeDef,
-        "perRequest": DurationOutputTypeDef,
-    },
-    total=False,
-)
-
-OutlierDetectionOutputTypeDef = TypedDict(
-    "OutlierDetectionOutputTypeDef",
-    {
-        "baseEjectionDuration": DurationOutputTypeDef,
-        "interval": DurationOutputTypeDef,
-        "maxEjectionPercent": int,
-        "maxServerErrors": int,
-    },
-)
-
-TcpTimeoutOutputTypeDef = TypedDict(
-    "TcpTimeoutOutputTypeDef",
+GrpcTimeoutTypeDef = TypedDict(
+    "GrpcTimeoutTypeDef",
     {
-        "idle": DurationOutputTypeDef,
+        "idle": DurationTypeDef,
+        "perRequest": DurationTypeDef,
     },
     total=False,
 )
 
-_RequiredGrpcRetryPolicyTypeDef = TypedDict(
-    "_RequiredGrpcRetryPolicyTypeDef",
+_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_RequiredHttpRetryPolicyOutputTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
-_OptionalGrpcRetryPolicyTypeDef = TypedDict(
-    "_OptionalGrpcRetryPolicyTypeDef",
+_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_OptionalHttpRetryPolicyOutputTypeDef",
     {
-        "grpcRetryEvents": Sequence[GrpcRetryPolicyEventType],
-        "httpRetryEvents": Sequence[str],
-        "tcpRetryEvents": Sequence[Literal["connection-error"]],
+        "httpRetryEvents": List[str],
+        "tcpRetryEvents": List[Literal["connection-error"]],
     },
     total=False,
 )
 
 
-class GrpcRetryPolicyTypeDef(_RequiredGrpcRetryPolicyTypeDef, _OptionalGrpcRetryPolicyTypeDef):
+class HttpRetryPolicyOutputTypeDef(
+    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
+):
     pass
 
 
-GrpcTimeoutTypeDef = TypedDict(
-    "GrpcTimeoutTypeDef",
-    {
-        "idle": DurationTypeDef,
-        "perRequest": DurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredHttpRetryPolicyTypeDef = TypedDict(
     "_RequiredHttpRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -2299,60 +1623,31 @@
     "TcpTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
     },
     total=False,
 )
 
-GrpcGatewayRouteRewriteOutputTypeDef = TypedDict(
-    "GrpcGatewayRouteRewriteOutputTypeDef",
-    {
-        "hostname": GatewayRouteHostnameRewriteOutputTypeDef,
-    },
-    total=False,
-)
-
 GrpcGatewayRouteRewriteTypeDef = TypedDict(
     "GrpcGatewayRouteRewriteTypeDef",
     {
         "hostname": GatewayRouteHostnameRewriteTypeDef,
     },
     total=False,
 )
 
 ListGatewayRoutesOutputTypeDef = TypedDict(
     "ListGatewayRoutesOutputTypeDef",
     {
         "gatewayRoutes": List[GatewayRouteRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGatewayRouteTargetOutputTypeDef = TypedDict(
-    "_RequiredGatewayRouteTargetOutputTypeDef",
-    {
-        "virtualService": GatewayRouteVirtualServiceOutputTypeDef,
-    },
-)
-_OptionalGatewayRouteTargetOutputTypeDef = TypedDict(
-    "_OptionalGatewayRouteTargetOutputTypeDef",
-    {
-        "port": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class GatewayRouteTargetOutputTypeDef(
-    _RequiredGatewayRouteTargetOutputTypeDef, _OptionalGatewayRouteTargetOutputTypeDef
-):
-    pass
-
-
 _RequiredGatewayRouteTargetTypeDef = TypedDict(
     "_RequiredGatewayRouteTargetTypeDef",
     {
         "virtualService": GatewayRouteVirtualServiceTypeDef,
     },
 )
 _OptionalGatewayRouteTargetTypeDef = TypedDict(
@@ -2366,50 +1661,14 @@
 
 class GatewayRouteTargetTypeDef(
     _RequiredGatewayRouteTargetTypeDef, _OptionalGatewayRouteTargetTypeDef
 ):
     pass
 
 
-GrpcMetadataMatchMethodOutputTypeDef = TypedDict(
-    "GrpcMetadataMatchMethodOutputTypeDef",
-    {
-        "exact": str,
-        "prefix": str,
-        "range": MatchRangeOutputTypeDef,
-        "regex": str,
-        "suffix": str,
-    },
-    total=False,
-)
-
-GrpcRouteMetadataMatchMethodOutputTypeDef = TypedDict(
-    "GrpcRouteMetadataMatchMethodOutputTypeDef",
-    {
-        "exact": str,
-        "prefix": str,
-        "range": MatchRangeOutputTypeDef,
-        "regex": str,
-        "suffix": str,
-    },
-    total=False,
-)
-
-HeaderMatchMethodOutputTypeDef = TypedDict(
-    "HeaderMatchMethodOutputTypeDef",
-    {
-        "exact": str,
-        "prefix": str,
-        "range": MatchRangeOutputTypeDef,
-        "regex": str,
-        "suffix": str,
-    },
-    total=False,
-)
-
 GrpcMetadataMatchMethodTypeDef = TypedDict(
     "GrpcMetadataMatchMethodTypeDef",
     {
         "exact": str,
         "prefix": str,
         "range": MatchRangeTypeDef,
         "regex": str,
@@ -2441,94 +1700,63 @@
     },
     total=False,
 )
 
 GrpcRouteActionOutputTypeDef = TypedDict(
     "GrpcRouteActionOutputTypeDef",
     {
-        "weightedTargets": List[WeightedTargetOutputTypeDef],
+        "weightedTargets": List[WeightedTargetTypeDef],
     },
 )
 
-HttpRouteActionOutputTypeDef = TypedDict(
-    "HttpRouteActionOutputTypeDef",
+GrpcRouteActionTypeDef = TypedDict(
+    "GrpcRouteActionTypeDef",
     {
-        "weightedTargets": List[WeightedTargetOutputTypeDef],
+        "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-TcpRouteActionOutputTypeDef = TypedDict(
-    "TcpRouteActionOutputTypeDef",
+HttpRouteActionOutputTypeDef = TypedDict(
+    "HttpRouteActionOutputTypeDef",
     {
-        "weightedTargets": List[WeightedTargetOutputTypeDef],
+        "weightedTargets": List[WeightedTargetTypeDef],
     },
 )
 
-GrpcRouteActionTypeDef = TypedDict(
-    "GrpcRouteActionTypeDef",
+HttpRouteActionTypeDef = TypedDict(
+    "HttpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-HttpRouteActionTypeDef = TypedDict(
-    "HttpRouteActionTypeDef",
+TcpRouteActionOutputTypeDef = TypedDict(
+    "TcpRouteActionOutputTypeDef",
     {
-        "weightedTargets": Sequence[WeightedTargetTypeDef],
+        "weightedTargets": List[WeightedTargetTypeDef],
     },
 )
 
 TcpRouteActionTypeDef = TypedDict(
     "TcpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-HttpGatewayRouteRewriteOutputTypeDef = TypedDict(
-    "HttpGatewayRouteRewriteOutputTypeDef",
-    {
-        "hostname": GatewayRouteHostnameRewriteOutputTypeDef,
-        "path": HttpGatewayRoutePathRewriteOutputTypeDef,
-        "prefix": HttpGatewayRoutePrefixRewriteOutputTypeDef,
-    },
-    total=False,
-)
-
 HttpGatewayRouteRewriteTypeDef = TypedDict(
     "HttpGatewayRouteRewriteTypeDef",
     {
         "hostname": GatewayRouteHostnameRewriteTypeDef,
         "path": HttpGatewayRoutePathRewriteTypeDef,
         "prefix": HttpGatewayRoutePrefixRewriteTypeDef,
     },
     total=False,
 )
 
-_RequiredHttpQueryParameterOutputTypeDef = TypedDict(
-    "_RequiredHttpQueryParameterOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalHttpQueryParameterOutputTypeDef = TypedDict(
-    "_OptionalHttpQueryParameterOutputTypeDef",
-    {
-        "match": QueryParameterMatchOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class HttpQueryParameterOutputTypeDef(
-    _RequiredHttpQueryParameterOutputTypeDef, _OptionalHttpQueryParameterOutputTypeDef
-):
-    pass
-
-
 _RequiredHttpQueryParameterTypeDef = TypedDict(
     "_RequiredHttpQueryParameterTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpQueryParameterTypeDef = TypedDict(
@@ -2545,153 +1773,279 @@
 ):
     pass
 
 
 LoggingFormatOutputTypeDef = TypedDict(
     "LoggingFormatOutputTypeDef",
     {
-        "json": List[JsonFormatRefOutputTypeDef],
+        "json": List[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
 )
 
 LoggingFormatTypeDef = TypedDict(
     "LoggingFormatTypeDef",
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
 )
 
+_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualGatewayName": str,
+    },
+)
+_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
+    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+):
+    pass
+
+
+ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualRouterName": str,
+    },
+)
+_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRoutesInputListRoutesPaginateTypeDef(
+    _RequiredListRoutesInputListRoutesPaginateTypeDef,
+    _OptionalListRoutesInputListRoutesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
+    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
+    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
+    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
+    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+):
+    pass
+
+
 ListMeshesOutputTypeDef = TypedDict(
     "ListMeshesOutputTypeDef",
     {
         "meshes": List[MeshRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoutesOutputTypeDef = TypedDict(
     "ListRoutesOutputTypeDef",
     {
         "nextToken": str,
         "routes": List[RouteRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "nextToken": str,
-        "tags": List[TagRefOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualGatewaysOutputTypeDef = TypedDict(
     "ListVirtualGatewaysOutputTypeDef",
     {
         "nextToken": str,
         "virtualGateways": List[VirtualGatewayRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualNodesOutputTypeDef = TypedDict(
     "ListVirtualNodesOutputTypeDef",
     {
         "nextToken": str,
         "virtualNodes": List[VirtualNodeRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualRoutersOutputTypeDef = TypedDict(
     "ListVirtualRoutersOutputTypeDef",
     {
         "nextToken": str,
         "virtualRouters": List[VirtualRouterRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualServicesOutputTypeDef = TypedDict(
     "ListVirtualServicesOutputTypeDef",
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VirtualRouterListenerOutputTypeDef = TypedDict(
-    "VirtualRouterListenerOutputTypeDef",
-    {
-        "portMapping": PortMappingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListenerTlsCertificateOutputTypeDef = TypedDict(
-    "ListenerTlsCertificateOutputTypeDef",
+VirtualRouterListenerTypeDef = TypedDict(
+    "VirtualRouterListenerTypeDef",
     {
-        "acm": ListenerTlsAcmCertificateOutputTypeDef,
-        "file": ListenerTlsFileCertificateOutputTypeDef,
-        "sds": ListenerTlsSdsCertificateOutputTypeDef,
+        "portMapping": PortMappingTypeDef,
     },
-    total=False,
 )
 
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-ListenerTlsValidationContextTrustOutputTypeDef = TypedDict(
-    "ListenerTlsValidationContextTrustOutputTypeDef",
-    {
-        "file": TlsValidationContextFileTrustOutputTypeDef,
-        "sds": TlsValidationContextSdsTrustOutputTypeDef,
-    },
-    total=False,
-)
-
 ListenerTlsValidationContextTrustTypeDef = TypedDict(
     "ListenerTlsValidationContextTrustTypeDef",
     {
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualRouterListenerTypeDef = TypedDict(
-    "VirtualRouterListenerTypeDef",
-    {
-        "portMapping": PortMappingTypeDef,
-    },
-)
-
-MeshSpecOutputTypeDef = TypedDict(
-    "MeshSpecOutputTypeDef",
-    {
-        "egressFilter": EgressFilterOutputTypeDef,
-        "serviceDiscovery": MeshServiceDiscoveryOutputTypeDef,
-    },
-    total=False,
-)
-
 MeshSpecTypeDef = TypedDict(
     "MeshSpecTypeDef",
     {
         "egressFilter": EgressFilterTypeDef,
         "serviceDiscovery": MeshServiceDiscoveryTypeDef,
     },
     total=False,
@@ -2711,227 +2065,137 @@
     },
 )
 
 TlsValidationContextTrustOutputTypeDef = TypedDict(
     "TlsValidationContextTrustOutputTypeDef",
     {
         "acm": TlsValidationContextAcmTrustOutputTypeDef,
-        "file": TlsValidationContextFileTrustOutputTypeDef,
-        "sds": TlsValidationContextSdsTrustOutputTypeDef,
+        "file": TlsValidationContextFileTrustTypeDef,
+        "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
 TlsValidationContextTrustTypeDef = TypedDict(
     "TlsValidationContextTrustTypeDef",
     {
         "acm": TlsValidationContextAcmTrustTypeDef,
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayClientTlsCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayClientTlsCertificateOutputTypeDef",
-    {
-        "file": VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
-        "sds": VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayClientTlsCertificateTypeDef = TypedDict(
     "VirtualGatewayClientTlsCertificateTypeDef",
     {
         "file": VirtualGatewayListenerTlsFileCertificateTypeDef,
         "sds": VirtualGatewayListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualGatewayConnectionPoolOutputTypeDef",
-    {
-        "grpc": VirtualGatewayGrpcConnectionPoolOutputTypeDef,
-        "http": VirtualGatewayHttpConnectionPoolOutputTypeDef,
-        "http2": VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayConnectionPoolTypeDef = TypedDict(
     "VirtualGatewayConnectionPoolTypeDef",
     {
         "grpc": VirtualGatewayGrpcConnectionPoolTypeDef,
         "http": VirtualGatewayHttpConnectionPoolTypeDef,
         "http2": VirtualGatewayHttp2ConnectionPoolTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayListenerTlsCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsCertificateOutputTypeDef",
-    {
-        "acm": VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
-        "file": VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
-        "sds": VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayListenerTlsCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsCertificateTypeDef",
     {
         "acm": VirtualGatewayListenerTlsAcmCertificateTypeDef,
         "file": VirtualGatewayListenerTlsFileCertificateTypeDef,
         "sds": VirtualGatewayListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef",
-    {
-        "file": VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
-        "sds": VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayListenerTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
     {
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
 VirtualGatewayTlsValidationContextTrustOutputTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
-        "file": VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
-        "sds": VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
+        "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
+        "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
 VirtualGatewayTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustTypeDef,
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualNodeConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualNodeConnectionPoolOutputTypeDef",
-    {
-        "grpc": VirtualNodeGrpcConnectionPoolOutputTypeDef,
-        "http": VirtualNodeHttpConnectionPoolOutputTypeDef,
-        "http2": VirtualNodeHttp2ConnectionPoolOutputTypeDef,
-        "tcp": VirtualNodeTcpConnectionPoolOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualNodeConnectionPoolTypeDef = TypedDict(
     "VirtualNodeConnectionPoolTypeDef",
     {
         "grpc": VirtualNodeGrpcConnectionPoolTypeDef,
         "http": VirtualNodeHttpConnectionPoolTypeDef,
         "http2": VirtualNodeHttp2ConnectionPoolTypeDef,
         "tcp": VirtualNodeTcpConnectionPoolTypeDef,
     },
     total=False,
 )
 
-VirtualServiceProviderOutputTypeDef = TypedDict(
-    "VirtualServiceProviderOutputTypeDef",
-    {
-        "virtualNode": VirtualNodeServiceProviderOutputTypeDef,
-        "virtualRouter": VirtualRouterServiceProviderOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualServiceProviderTypeDef = TypedDict(
     "VirtualServiceProviderTypeDef",
     {
         "virtualNode": VirtualNodeServiceProviderTypeDef,
         "virtualRouter": VirtualRouterServiceProviderTypeDef,
     },
     total=False,
 )
 
 ServiceDiscoveryOutputTypeDef = TypedDict(
     "ServiceDiscoveryOutputTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryOutputTypeDef,
-        "dns": DnsServiceDiscoveryOutputTypeDef,
+        "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
 ServiceDiscoveryTypeDef = TypedDict(
     "ServiceDiscoveryTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryTypeDef,
         "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
-ListenerTimeoutOutputTypeDef = TypedDict(
-    "ListenerTimeoutOutputTypeDef",
-    {
-        "grpc": GrpcTimeoutOutputTypeDef,
-        "http": HttpTimeoutOutputTypeDef,
-        "http2": HttpTimeoutOutputTypeDef,
-        "tcp": TcpTimeoutOutputTypeDef,
-    },
-    total=False,
-)
-
 ListenerTimeoutTypeDef = TypedDict(
     "ListenerTimeoutTypeDef",
     {
         "grpc": GrpcTimeoutTypeDef,
         "http": HttpTimeoutTypeDef,
         "http2": HttpTimeoutTypeDef,
         "tcp": TcpTimeoutTypeDef,
     },
     total=False,
 )
 
-_RequiredGrpcGatewayRouteActionOutputTypeDef = TypedDict(
-    "_RequiredGrpcGatewayRouteActionOutputTypeDef",
-    {
-        "target": GatewayRouteTargetOutputTypeDef,
-    },
-)
-_OptionalGrpcGatewayRouteActionOutputTypeDef = TypedDict(
-    "_OptionalGrpcGatewayRouteActionOutputTypeDef",
-    {
-        "rewrite": GrpcGatewayRouteRewriteOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class GrpcGatewayRouteActionOutputTypeDef(
-    _RequiredGrpcGatewayRouteActionOutputTypeDef, _OptionalGrpcGatewayRouteActionOutputTypeDef
-):
-    pass
-
-
 _RequiredGrpcGatewayRouteActionTypeDef = TypedDict(
     "_RequiredGrpcGatewayRouteActionTypeDef",
     {
         "target": GatewayRouteTargetTypeDef,
     },
 )
 _OptionalGrpcGatewayRouteActionTypeDef = TypedDict(
@@ -2945,102 +2209,14 @@
 
 class GrpcGatewayRouteActionTypeDef(
     _RequiredGrpcGatewayRouteActionTypeDef, _OptionalGrpcGatewayRouteActionTypeDef
 ):
     pass
 
 
-_RequiredGrpcGatewayRouteMetadataOutputTypeDef = TypedDict(
-    "_RequiredGrpcGatewayRouteMetadataOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGrpcGatewayRouteMetadataOutputTypeDef = TypedDict(
-    "_OptionalGrpcGatewayRouteMetadataOutputTypeDef",
-    {
-        "invert": bool,
-        "match": GrpcMetadataMatchMethodOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class GrpcGatewayRouteMetadataOutputTypeDef(
-    _RequiredGrpcGatewayRouteMetadataOutputTypeDef, _OptionalGrpcGatewayRouteMetadataOutputTypeDef
-):
-    pass
-
-
-_RequiredGrpcRouteMetadataOutputTypeDef = TypedDict(
-    "_RequiredGrpcRouteMetadataOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGrpcRouteMetadataOutputTypeDef = TypedDict(
-    "_OptionalGrpcRouteMetadataOutputTypeDef",
-    {
-        "invert": bool,
-        "match": GrpcRouteMetadataMatchMethodOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class GrpcRouteMetadataOutputTypeDef(
-    _RequiredGrpcRouteMetadataOutputTypeDef, _OptionalGrpcRouteMetadataOutputTypeDef
-):
-    pass
-
-
-_RequiredHttpGatewayRouteHeaderOutputTypeDef = TypedDict(
-    "_RequiredHttpGatewayRouteHeaderOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalHttpGatewayRouteHeaderOutputTypeDef = TypedDict(
-    "_OptionalHttpGatewayRouteHeaderOutputTypeDef",
-    {
-        "invert": bool,
-        "match": HeaderMatchMethodOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class HttpGatewayRouteHeaderOutputTypeDef(
-    _RequiredHttpGatewayRouteHeaderOutputTypeDef, _OptionalHttpGatewayRouteHeaderOutputTypeDef
-):
-    pass
-
-
-_RequiredHttpRouteHeaderOutputTypeDef = TypedDict(
-    "_RequiredHttpRouteHeaderOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalHttpRouteHeaderOutputTypeDef = TypedDict(
-    "_OptionalHttpRouteHeaderOutputTypeDef",
-    {
-        "invert": bool,
-        "match": HeaderMatchMethodOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class HttpRouteHeaderOutputTypeDef(
-    _RequiredHttpRouteHeaderOutputTypeDef, _OptionalHttpRouteHeaderOutputTypeDef
-):
-    pass
-
-
 _RequiredGrpcGatewayRouteMetadataTypeDef = TypedDict(
     "_RequiredGrpcGatewayRouteMetadataTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGrpcGatewayRouteMetadataTypeDef = TypedDict(
@@ -3128,16 +2304,16 @@
     {
         "action": TcpRouteActionOutputTypeDef,
     },
 )
 _OptionalTcpRouteOutputTypeDef = TypedDict(
     "_OptionalTcpRouteOutputTypeDef",
     {
-        "match": TcpRouteMatchOutputTypeDef,
-        "timeout": TcpTimeoutOutputTypeDef,
+        "match": TcpRouteMatchTypeDef,
+        "timeout": TcpTimeoutTypeDef,
     },
     total=False,
 )
 
 
 class TcpRouteOutputTypeDef(_RequiredTcpRouteOutputTypeDef, _OptionalTcpRouteOutputTypeDef):
     pass
@@ -3159,35 +2335,14 @@
 )
 
 
 class TcpRouteTypeDef(_RequiredTcpRouteTypeDef, _OptionalTcpRouteTypeDef):
     pass
 
 
-_RequiredHttpGatewayRouteActionOutputTypeDef = TypedDict(
-    "_RequiredHttpGatewayRouteActionOutputTypeDef",
-    {
-        "target": GatewayRouteTargetOutputTypeDef,
-    },
-)
-_OptionalHttpGatewayRouteActionOutputTypeDef = TypedDict(
-    "_OptionalHttpGatewayRouteActionOutputTypeDef",
-    {
-        "rewrite": HttpGatewayRouteRewriteOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class HttpGatewayRouteActionOutputTypeDef(
-    _RequiredHttpGatewayRouteActionOutputTypeDef, _OptionalHttpGatewayRouteActionOutputTypeDef
-):
-    pass
-
-
 _RequiredHttpGatewayRouteActionTypeDef = TypedDict(
     "_RequiredHttpGatewayRouteActionTypeDef",
     {
         "target": GatewayRouteTargetTypeDef,
     },
 )
 _OptionalHttpGatewayRouteActionTypeDef = TypedDict(
@@ -3287,37 +2442,27 @@
 ):
     pass
 
 
 VirtualRouterSpecOutputTypeDef = TypedDict(
     "VirtualRouterSpecOutputTypeDef",
     {
-        "listeners": List[VirtualRouterListenerOutputTypeDef],
+        "listeners": List[VirtualRouterListenerTypeDef],
     },
     total=False,
 )
 
 VirtualRouterSpecTypeDef = TypedDict(
     "VirtualRouterSpecTypeDef",
     {
         "listeners": Sequence[VirtualRouterListenerTypeDef],
     },
     total=False,
 )
 
-MeshDataTypeDef = TypedDict(
-    "MeshDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": MeshSpecOutputTypeDef,
-        "status": MeshStatusTypeDef,
-    },
-)
-
 _RequiredCreateMeshInputRequestTypeDef = TypedDict(
     "_RequiredCreateMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalCreateMeshInputRequestTypeDef = TypedDict(
@@ -3333,14 +2478,24 @@
 
 class CreateMeshInputRequestTypeDef(
     _RequiredCreateMeshInputRequestTypeDef, _OptionalCreateMeshInputRequestTypeDef
 ):
     pass
 
 
+MeshDataTypeDef = TypedDict(
+    "MeshDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": MeshSpecTypeDef,
+        "status": MeshStatusTypeDef,
+    },
+)
+
 _RequiredUpdateMeshInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalUpdateMeshInputRequestTypeDef = TypedDict(
@@ -3358,15 +2513,15 @@
 ):
     pass
 
 
 _RequiredListenerTlsValidationContextOutputTypeDef = TypedDict(
     "_RequiredListenerTlsValidationContextOutputTypeDef",
     {
-        "trust": ListenerTlsValidationContextTrustOutputTypeDef,
+        "trust": ListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalListenerTlsValidationContextOutputTypeDef = TypedDict(
     "_OptionalListenerTlsValidationContextOutputTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
     },
@@ -3443,15 +2598,15 @@
 ):
     pass
 
 
 _RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef",
     {
-        "trust": VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
+        "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
     "_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
     },
@@ -3528,112 +2683,104 @@
 class VirtualGatewayTlsValidationContextTypeDef(
     _RequiredVirtualGatewayTlsValidationContextTypeDef,
     _OptionalVirtualGatewayTlsValidationContextTypeDef,
 ):
     pass
 
 
-VirtualServiceSpecOutputTypeDef = TypedDict(
-    "VirtualServiceSpecOutputTypeDef",
-    {
-        "provider": VirtualServiceProviderOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualServiceSpecTypeDef = TypedDict(
     "VirtualServiceSpecTypeDef",
     {
         "provider": VirtualServiceProviderTypeDef,
     },
     total=False,
 )
 
 GrpcGatewayRouteMatchOutputTypeDef = TypedDict(
     "GrpcGatewayRouteMatchOutputTypeDef",
     {
-        "hostname": GatewayRouteHostnameMatchOutputTypeDef,
-        "metadata": List[GrpcGatewayRouteMetadataOutputTypeDef],
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "metadata": List[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
-GrpcRouteMatchOutputTypeDef = TypedDict(
-    "GrpcRouteMatchOutputTypeDef",
+GrpcGatewayRouteMatchTypeDef = TypedDict(
+    "GrpcGatewayRouteMatchTypeDef",
     {
-        "metadata": List[GrpcRouteMetadataOutputTypeDef],
-        "methodName": str,
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
-HttpGatewayRouteMatchOutputTypeDef = TypedDict(
-    "HttpGatewayRouteMatchOutputTypeDef",
+GrpcRouteMatchOutputTypeDef = TypedDict(
+    "GrpcRouteMatchOutputTypeDef",
     {
-        "headers": List[HttpGatewayRouteHeaderOutputTypeDef],
-        "hostname": GatewayRouteHostnameMatchOutputTypeDef,
-        "method": HttpMethodType,
-        "path": HttpPathMatchOutputTypeDef,
+        "metadata": List[GrpcRouteMetadataTypeDef],
+        "methodName": str,
         "port": int,
-        "prefix": str,
-        "queryParameters": List[HttpQueryParameterOutputTypeDef],
+        "serviceName": str,
     },
     total=False,
 )
 
-HttpRouteMatchOutputTypeDef = TypedDict(
-    "HttpRouteMatchOutputTypeDef",
+GrpcRouteMatchTypeDef = TypedDict(
+    "GrpcRouteMatchTypeDef",
     {
-        "headers": List[HttpRouteHeaderOutputTypeDef],
-        "method": HttpMethodType,
-        "path": HttpPathMatchOutputTypeDef,
+        "metadata": Sequence[GrpcRouteMetadataTypeDef],
+        "methodName": str,
         "port": int,
-        "prefix": str,
-        "queryParameters": List[HttpQueryParameterOutputTypeDef],
-        "scheme": HttpSchemeType,
+        "serviceName": str,
     },
     total=False,
 )
 
-GrpcGatewayRouteMatchTypeDef = TypedDict(
-    "GrpcGatewayRouteMatchTypeDef",
+HttpGatewayRouteMatchOutputTypeDef = TypedDict(
+    "HttpGatewayRouteMatchOutputTypeDef",
     {
+        "headers": List[HttpGatewayRouteHeaderTypeDef],
         "hostname": GatewayRouteHostnameMatchTypeDef,
-        "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
+        "method": HttpMethodType,
+        "path": HttpPathMatchTypeDef,
         "port": int,
-        "serviceName": str,
+        "prefix": str,
+        "queryParameters": List[HttpQueryParameterTypeDef],
     },
     total=False,
 )
 
-GrpcRouteMatchTypeDef = TypedDict(
-    "GrpcRouteMatchTypeDef",
+HttpGatewayRouteMatchTypeDef = TypedDict(
+    "HttpGatewayRouteMatchTypeDef",
     {
-        "metadata": Sequence[GrpcRouteMetadataTypeDef],
-        "methodName": str,
+        "headers": Sequence[HttpGatewayRouteHeaderTypeDef],
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "method": HttpMethodType,
+        "path": HttpPathMatchTypeDef,
         "port": int,
-        "serviceName": str,
+        "prefix": str,
+        "queryParameters": Sequence[HttpQueryParameterTypeDef],
     },
     total=False,
 )
 
-HttpGatewayRouteMatchTypeDef = TypedDict(
-    "HttpGatewayRouteMatchTypeDef",
+HttpRouteMatchOutputTypeDef = TypedDict(
+    "HttpRouteMatchOutputTypeDef",
     {
-        "headers": Sequence[HttpGatewayRouteHeaderTypeDef],
-        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "headers": List[HttpRouteHeaderTypeDef],
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
-        "queryParameters": Sequence[HttpQueryParameterTypeDef],
+        "queryParameters": List[HttpQueryParameterTypeDef],
+        "scheme": HttpSchemeType,
     },
     total=False,
 )
 
 HttpRouteMatchTypeDef = TypedDict(
     "HttpRouteMatchTypeDef",
     {
@@ -3740,46 +2887,46 @@
     pass
 
 
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMeshOutputTypeDef = TypedDict(
     "DeleteMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMeshOutputTypeDef = TypedDict(
     "DescribeMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMeshOutputTypeDef = TypedDict(
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListenerTlsOutputTypeDef = TypedDict(
     "_RequiredListenerTlsOutputTypeDef",
     {
-        "certificate": ListenerTlsCertificateOutputTypeDef,
+        "certificate": ListenerTlsCertificateTypeDef,
         "mode": ListenerTlsModeType,
     },
 )
 _OptionalListenerTlsOutputTypeDef = TypedDict(
     "_OptionalListenerTlsOutputTypeDef",
     {
         "validation": ListenerTlsValidationContextOutputTypeDef,
@@ -3819,15 +2966,15 @@
     {
         "validation": TlsValidationContextOutputTypeDef,
     },
 )
 _OptionalClientPolicyTlsOutputTypeDef = TypedDict(
     "_OptionalClientPolicyTlsOutputTypeDef",
     {
-        "certificate": ClientTlsCertificateOutputTypeDef,
+        "certificate": ClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": List[int],
     },
     total=False,
 )
 
 
@@ -3857,15 +3004,15 @@
 class ClientPolicyTlsTypeDef(_RequiredClientPolicyTlsTypeDef, _OptionalClientPolicyTlsTypeDef):
     pass
 
 
 _RequiredVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsOutputTypeDef",
     {
-        "certificate": VirtualGatewayListenerTlsCertificateOutputTypeDef,
+        "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
         "mode": VirtualGatewayListenerTlsModeType,
     },
 )
 _OptionalVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
     "_OptionalVirtualGatewayListenerTlsOutputTypeDef",
     {
         "validation": VirtualGatewayListenerTlsValidationContextOutputTypeDef,
@@ -3907,15 +3054,15 @@
     {
         "validation": VirtualGatewayTlsValidationContextOutputTypeDef,
     },
 )
 _OptionalVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
     "_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef",
     {
-        "certificate": VirtualGatewayClientTlsCertificateOutputTypeDef,
+        "certificate": VirtualGatewayClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": List[int],
     },
     total=False,
 )
 
 
@@ -3945,25 +3092,14 @@
 
 class VirtualGatewayClientPolicyTlsTypeDef(
     _RequiredVirtualGatewayClientPolicyTlsTypeDef, _OptionalVirtualGatewayClientPolicyTlsTypeDef
 ):
     pass
 
 
-VirtualServiceDataTypeDef = TypedDict(
-    "VirtualServiceDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualServiceSpecOutputTypeDef,
-        "status": VirtualServiceStatusTypeDef,
-        "virtualServiceName": str,
-    },
-)
-
 _RequiredCreateVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualServiceSpecTypeDef,
         "virtualServiceName": str,
     },
@@ -4007,80 +3143,62 @@
 class UpdateVirtualServiceInputRequestTypeDef(
     _RequiredUpdateVirtualServiceInputRequestTypeDef,
     _OptionalUpdateVirtualServiceInputRequestTypeDef,
 ):
     pass
 
 
+VirtualServiceDataTypeDef = TypedDict(
+    "VirtualServiceDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualServiceSpecTypeDef,
+        "status": VirtualServiceStatusTypeDef,
+        "virtualServiceName": str,
+    },
+)
+
 GrpcGatewayRouteOutputTypeDef = TypedDict(
     "GrpcGatewayRouteOutputTypeDef",
     {
-        "action": GrpcGatewayRouteActionOutputTypeDef,
+        "action": GrpcGatewayRouteActionTypeDef,
         "match": GrpcGatewayRouteMatchOutputTypeDef,
     },
 )
 
+GrpcGatewayRouteTypeDef = TypedDict(
+    "GrpcGatewayRouteTypeDef",
+    {
+        "action": GrpcGatewayRouteActionTypeDef,
+        "match": GrpcGatewayRouteMatchTypeDef,
+    },
+)
+
 _RequiredGrpcRouteOutputTypeDef = TypedDict(
     "_RequiredGrpcRouteOutputTypeDef",
     {
         "action": GrpcRouteActionOutputTypeDef,
         "match": GrpcRouteMatchOutputTypeDef,
     },
 )
 _OptionalGrpcRouteOutputTypeDef = TypedDict(
     "_OptionalGrpcRouteOutputTypeDef",
     {
         "retryPolicy": GrpcRetryPolicyOutputTypeDef,
-        "timeout": GrpcTimeoutOutputTypeDef,
+        "timeout": GrpcTimeoutTypeDef,
     },
     total=False,
 )
 
 
 class GrpcRouteOutputTypeDef(_RequiredGrpcRouteOutputTypeDef, _OptionalGrpcRouteOutputTypeDef):
     pass
 
 
-HttpGatewayRouteOutputTypeDef = TypedDict(
-    "HttpGatewayRouteOutputTypeDef",
-    {
-        "action": HttpGatewayRouteActionOutputTypeDef,
-        "match": HttpGatewayRouteMatchOutputTypeDef,
-    },
-)
-
-_RequiredHttpRouteOutputTypeDef = TypedDict(
-    "_RequiredHttpRouteOutputTypeDef",
-    {
-        "action": HttpRouteActionOutputTypeDef,
-        "match": HttpRouteMatchOutputTypeDef,
-    },
-)
-_OptionalHttpRouteOutputTypeDef = TypedDict(
-    "_OptionalHttpRouteOutputTypeDef",
-    {
-        "retryPolicy": HttpRetryPolicyOutputTypeDef,
-        "timeout": HttpTimeoutOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
-    pass
-
-
-GrpcGatewayRouteTypeDef = TypedDict(
-    "GrpcGatewayRouteTypeDef",
-    {
-        "action": GrpcGatewayRouteActionTypeDef,
-        "match": GrpcGatewayRouteMatchTypeDef,
-    },
-)
-
 _RequiredGrpcRouteTypeDef = TypedDict(
     "_RequiredGrpcRouteTypeDef",
     {
         "action": GrpcRouteActionTypeDef,
         "match": GrpcRouteMatchTypeDef,
     },
 )
@@ -4094,22 +3212,51 @@
 )
 
 
 class GrpcRouteTypeDef(_RequiredGrpcRouteTypeDef, _OptionalGrpcRouteTypeDef):
     pass
 
 
+HttpGatewayRouteOutputTypeDef = TypedDict(
+    "HttpGatewayRouteOutputTypeDef",
+    {
+        "action": HttpGatewayRouteActionTypeDef,
+        "match": HttpGatewayRouteMatchOutputTypeDef,
+    },
+)
+
 HttpGatewayRouteTypeDef = TypedDict(
     "HttpGatewayRouteTypeDef",
     {
         "action": HttpGatewayRouteActionTypeDef,
         "match": HttpGatewayRouteMatchTypeDef,
     },
 )
 
+_RequiredHttpRouteOutputTypeDef = TypedDict(
+    "_RequiredHttpRouteOutputTypeDef",
+    {
+        "action": HttpRouteActionOutputTypeDef,
+        "match": HttpRouteMatchOutputTypeDef,
+    },
+)
+_OptionalHttpRouteOutputTypeDef = TypedDict(
+    "_OptionalHttpRouteOutputTypeDef",
+    {
+        "retryPolicy": HttpRetryPolicyOutputTypeDef,
+        "timeout": HttpTimeoutTypeDef,
+    },
+    total=False,
+)
+
+
+class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
+    pass
+
+
 _RequiredHttpRouteTypeDef = TypedDict(
     "_RequiredHttpRouteTypeDef",
     {
         "action": HttpRouteActionTypeDef,
         "match": HttpRouteMatchTypeDef,
     },
 )
@@ -4159,55 +3306,55 @@
     total=False,
 )
 
 CreateVirtualRouterOutputTypeDef = TypedDict(
     "CreateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualRouterOutputTypeDef = TypedDict(
     "DeleteVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualRouterOutputTypeDef = TypedDict(
     "DescribeVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualRouterOutputTypeDef = TypedDict(
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListenerOutputTypeDef = TypedDict(
     "_RequiredListenerOutputTypeDef",
     {
-        "portMapping": PortMappingOutputTypeDef,
+        "portMapping": PortMappingTypeDef,
     },
 )
 _OptionalListenerOutputTypeDef = TypedDict(
     "_OptionalListenerOutputTypeDef",
     {
-        "connectionPool": VirtualNodeConnectionPoolOutputTypeDef,
-        "healthCheck": HealthCheckPolicyOutputTypeDef,
-        "outlierDetection": OutlierDetectionOutputTypeDef,
-        "timeout": ListenerTimeoutOutputTypeDef,
+        "connectionPool": VirtualNodeConnectionPoolTypeDef,
+        "healthCheck": HealthCheckPolicyTypeDef,
+        "outlierDetection": OutlierDetectionTypeDef,
+        "timeout": ListenerTimeoutTypeDef,
         "tls": ListenerTlsOutputTypeDef,
     },
     total=False,
 )
 
 
 class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
@@ -4252,22 +3399,22 @@
     },
     total=False,
 )
 
 _RequiredVirtualGatewayListenerOutputTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerOutputTypeDef",
     {
-        "portMapping": VirtualGatewayPortMappingOutputTypeDef,
+        "portMapping": VirtualGatewayPortMappingTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerOutputTypeDef = TypedDict(
     "_OptionalVirtualGatewayListenerOutputTypeDef",
     {
-        "connectionPool": VirtualGatewayConnectionPoolOutputTypeDef,
-        "healthCheck": VirtualGatewayHealthCheckPolicyOutputTypeDef,
+        "connectionPool": VirtualGatewayConnectionPoolTypeDef,
+        "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
         "tls": VirtualGatewayListenerTlsOutputTypeDef,
     },
     total=False,
 )
 
 
 class VirtualGatewayListenerOutputTypeDef(
@@ -4315,72 +3462,72 @@
     total=False,
 )
 
 CreateVirtualServiceOutputTypeDef = TypedDict(
     "CreateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualServiceOutputTypeDef = TypedDict(
     "DeleteVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualServiceOutputTypeDef = TypedDict(
     "DescribeVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualServiceOutputTypeDef = TypedDict(
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GatewayRouteSpecOutputTypeDef = TypedDict(
     "GatewayRouteSpecOutputTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteOutputTypeDef,
         "http2Route": HttpGatewayRouteOutputTypeDef,
         "httpRoute": HttpGatewayRouteOutputTypeDef,
         "priority": int,
     },
     total=False,
 )
 
-RouteSpecOutputTypeDef = TypedDict(
-    "RouteSpecOutputTypeDef",
+GatewayRouteSpecTypeDef = TypedDict(
+    "GatewayRouteSpecTypeDef",
     {
-        "grpcRoute": GrpcRouteOutputTypeDef,
-        "http2Route": HttpRouteOutputTypeDef,
-        "httpRoute": HttpRouteOutputTypeDef,
+        "grpcRoute": GrpcGatewayRouteTypeDef,
+        "http2Route": HttpGatewayRouteTypeDef,
+        "httpRoute": HttpGatewayRouteTypeDef,
         "priority": int,
-        "tcpRoute": TcpRouteOutputTypeDef,
     },
     total=False,
 )
 
-GatewayRouteSpecTypeDef = TypedDict(
-    "GatewayRouteSpecTypeDef",
+RouteSpecOutputTypeDef = TypedDict(
+    "RouteSpecOutputTypeDef",
     {
-        "grpcRoute": GrpcGatewayRouteTypeDef,
-        "http2Route": HttpGatewayRouteTypeDef,
-        "httpRoute": HttpGatewayRouteTypeDef,
+        "grpcRoute": GrpcRouteOutputTypeDef,
+        "http2Route": HttpRouteOutputTypeDef,
+        "httpRoute": HttpRouteOutputTypeDef,
         "priority": int,
+        "tcpRoute": TcpRouteOutputTypeDef,
     },
     total=False,
 )
 
 RouteSpecTypeDef = TypedDict(
     "RouteSpecTypeDef",
     {
@@ -4475,26 +3622,14 @@
         "metadata": ResourceMetadataTypeDef,
         "spec": GatewayRouteSpecOutputTypeDef,
         "status": GatewayRouteStatusTypeDef,
         "virtualGatewayName": str,
     },
 )
 
-RouteDataTypeDef = TypedDict(
-    "RouteDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "routeName": str,
-        "spec": RouteSpecOutputTypeDef,
-        "status": RouteStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
 _RequiredCreateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -4538,14 +3673,26 @@
 
 class UpdateGatewayRouteInputRequestTypeDef(
     _RequiredUpdateGatewayRouteInputRequestTypeDef, _OptionalUpdateGatewayRouteInputRequestTypeDef
 ):
     pass
 
 
+RouteDataTypeDef = TypedDict(
+    "RouteDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "routeName": str,
+        "spec": RouteSpecOutputTypeDef,
+        "status": RouteStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredCreateRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -4653,71 +3800,71 @@
     pass
 
 
 CreateGatewayRouteOutputTypeDef = TypedDict(
     "CreateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGatewayRouteOutputTypeDef = TypedDict(
     "DeleteGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGatewayRouteOutputTypeDef = TypedDict(
     "DescribeGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGatewayRouteOutputTypeDef = TypedDict(
     "UpdateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteOutputTypeDef = TypedDict(
     "CreateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRouteOutputTypeDef = TypedDict(
     "DeleteRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRouteOutputTypeDef = TypedDict(
     "DescribeRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteOutputTypeDef = TypedDict(
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualNodeSpecOutputTypeDef = TypedDict(
     "VirtualNodeSpecOutputTypeDef",
     {
         "backendDefaults": BackendDefaultsOutputTypeDef,
@@ -4863,66 +4010,66 @@
     pass
 
 
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualGatewayOutputTypeDef = TypedDict(
     "DeleteVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualGatewayOutputTypeDef = TypedDict(
     "DescribeVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualGatewayOutputTypeDef = TypedDict(
     "UpdateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVirtualNodeOutputTypeDef = TypedDict(
     "CreateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualNodeOutputTypeDef = TypedDict(
     "DeleteVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualNodeOutputTypeDef = TypedDict(
     "DescribeVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualNodeOutputTypeDef = TypedDict(
     "UpdateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh/type_defs.pyi` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for appmesh service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_appmesh.type_defs import AwsCloudMapInstanceAttributeOutputTypeDef
+    from mypy_boto3_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
 
-    data: AwsCloudMapInstanceAttributeOutputTypeDef = {...}
+    data: AwsCloudMapInstanceAttributeTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -43,265 +43,195 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AwsCloudMapInstanceAttributeOutputTypeDef",
     "AwsCloudMapInstanceAttributeTypeDef",
-    "ListenerTlsFileCertificateOutputTypeDef",
-    "ListenerTlsSdsCertificateOutputTypeDef",
     "ListenerTlsFileCertificateTypeDef",
     "ListenerTlsSdsCertificateTypeDef",
     "TagRefTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteGatewayRouteInputRequestTypeDef",
     "DeleteMeshInputRequestTypeDef",
     "DeleteRouteInputRequestTypeDef",
     "DeleteVirtualGatewayInputRequestTypeDef",
     "DeleteVirtualNodeInputRequestTypeDef",
     "DeleteVirtualRouterInputRequestTypeDef",
     "DeleteVirtualServiceInputRequestTypeDef",
     "DescribeGatewayRouteInputRequestTypeDef",
     "DescribeMeshInputRequestTypeDef",
     "DescribeRouteInputRequestTypeDef",
     "DescribeVirtualGatewayInputRequestTypeDef",
     "DescribeVirtualNodeInputRequestTypeDef",
     "DescribeVirtualRouterInputRequestTypeDef",
     "DescribeVirtualServiceInputRequestTypeDef",
-    "DnsServiceDiscoveryOutputTypeDef",
     "DnsServiceDiscoveryTypeDef",
-    "DurationOutputTypeDef",
     "DurationTypeDef",
-    "EgressFilterOutputTypeDef",
     "EgressFilterTypeDef",
     "GatewayRouteStatusTypeDef",
     "ResourceMetadataTypeDef",
-    "GatewayRouteHostnameMatchOutputTypeDef",
     "GatewayRouteHostnameMatchTypeDef",
-    "GatewayRouteHostnameRewriteOutputTypeDef",
     "GatewayRouteHostnameRewriteTypeDef",
     "GatewayRouteRefTypeDef",
-    "GatewayRouteVirtualServiceOutputTypeDef",
     "GatewayRouteVirtualServiceTypeDef",
-    "MatchRangeOutputTypeDef",
     "MatchRangeTypeDef",
-    "WeightedTargetOutputTypeDef",
     "WeightedTargetTypeDef",
-    "HealthCheckPolicyOutputTypeDef",
     "HealthCheckPolicyTypeDef",
-    "HttpPathMatchOutputTypeDef",
     "HttpPathMatchTypeDef",
-    "HttpGatewayRoutePathRewriteOutputTypeDef",
     "HttpGatewayRoutePathRewriteTypeDef",
-    "HttpGatewayRoutePrefixRewriteOutputTypeDef",
     "HttpGatewayRoutePrefixRewriteTypeDef",
-    "QueryParameterMatchOutputTypeDef",
     "QueryParameterMatchTypeDef",
-    "JsonFormatRefOutputTypeDef",
     "JsonFormatRefTypeDef",
-    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListGatewayRoutesInputRequestTypeDef",
-    "ListMeshesInputListMeshesPaginateTypeDef",
     "ListMeshesInputRequestTypeDef",
     "MeshRefTypeDef",
-    "ListRoutesInputListRoutesPaginateTypeDef",
     "ListRoutesInputRequestTypeDef",
     "RouteRefTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "TagRefOutputTypeDef",
-    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualGatewaysInputRequestTypeDef",
     "VirtualGatewayRefTypeDef",
-    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
-    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
-    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
-    "PortMappingOutputTypeDef",
-    "ListenerTlsAcmCertificateOutputTypeDef",
+    "PortMappingTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
-    "TlsValidationContextFileTrustOutputTypeDef",
-    "TlsValidationContextSdsTrustOutputTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
-    "PortMappingTypeDef",
     "MeshStatusTypeDef",
-    "MeshServiceDiscoveryOutputTypeDef",
     "MeshServiceDiscoveryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RouteStatusTypeDef",
     "SubjectAlternativeNameMatchersOutputTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
-    "TcpRouteMatchOutputTypeDef",
     "TcpRouteMatchTypeDef",
     "TlsValidationContextAcmTrustOutputTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "VirtualGatewayListenerTlsFileCertificateOutputTypeDef",
-    "VirtualGatewayListenerTlsSdsCertificateOutputTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
-    "VirtualGatewayGrpcConnectionPoolOutputTypeDef",
-    "VirtualGatewayHttp2ConnectionPoolOutputTypeDef",
-    "VirtualGatewayHttpConnectionPoolOutputTypeDef",
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     "VirtualGatewayHttp2ConnectionPoolTypeDef",
     "VirtualGatewayHttpConnectionPoolTypeDef",
     "VirtualGatewayStatusTypeDef",
-    "VirtualGatewayHealthCheckPolicyOutputTypeDef",
     "VirtualGatewayHealthCheckPolicyTypeDef",
-    "VirtualGatewayPortMappingOutputTypeDef",
-    "VirtualGatewayListenerTlsAcmCertificateOutputTypeDef",
+    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
-    "VirtualGatewayTlsValidationContextFileTrustOutputTypeDef",
-    "VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
-    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
-    "VirtualNodeGrpcConnectionPoolOutputTypeDef",
-    "VirtualNodeHttp2ConnectionPoolOutputTypeDef",
-    "VirtualNodeHttpConnectionPoolOutputTypeDef",
-    "VirtualNodeTcpConnectionPoolOutputTypeDef",
     "VirtualNodeGrpcConnectionPoolTypeDef",
     "VirtualNodeHttp2ConnectionPoolTypeDef",
     "VirtualNodeHttpConnectionPoolTypeDef",
     "VirtualNodeTcpConnectionPoolTypeDef",
     "VirtualNodeStatusTypeDef",
-    "VirtualNodeServiceProviderOutputTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
-    "VirtualRouterServiceProviderOutputTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
     "AwsCloudMapServiceDiscoveryOutputTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
-    "ClientTlsCertificateOutputTypeDef",
     "ClientTlsCertificateTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
     "GrpcRetryPolicyOutputTypeDef",
-    "GrpcTimeoutOutputTypeDef",
-    "HttpRetryPolicyOutputTypeDef",
-    "HttpTimeoutOutputTypeDef",
-    "OutlierDetectionOutputTypeDef",
-    "TcpTimeoutOutputTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
+    "HttpRetryPolicyOutputTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
-    "GrpcGatewayRouteRewriteOutputTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
     "ListGatewayRoutesOutputTypeDef",
-    "GatewayRouteTargetOutputTypeDef",
     "GatewayRouteTargetTypeDef",
-    "GrpcMetadataMatchMethodOutputTypeDef",
-    "GrpcRouteMetadataMatchMethodOutputTypeDef",
-    "HeaderMatchMethodOutputTypeDef",
     "GrpcMetadataMatchMethodTypeDef",
     "GrpcRouteMetadataMatchMethodTypeDef",
     "HeaderMatchMethodTypeDef",
     "GrpcRouteActionOutputTypeDef",
-    "HttpRouteActionOutputTypeDef",
-    "TcpRouteActionOutputTypeDef",
     "GrpcRouteActionTypeDef",
+    "HttpRouteActionOutputTypeDef",
     "HttpRouteActionTypeDef",
+    "TcpRouteActionOutputTypeDef",
     "TcpRouteActionTypeDef",
-    "HttpGatewayRouteRewriteOutputTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
-    "HttpQueryParameterOutputTypeDef",
     "HttpQueryParameterTypeDef",
     "LoggingFormatOutputTypeDef",
     "LoggingFormatTypeDef",
+    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    "ListRoutesInputListRoutesPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
-    "VirtualRouterListenerOutputTypeDef",
-    "ListenerTlsCertificateOutputTypeDef",
+    "VirtualRouterListenerTypeDef",
     "ListenerTlsCertificateTypeDef",
-    "ListenerTlsValidationContextTrustOutputTypeDef",
     "ListenerTlsValidationContextTrustTypeDef",
-    "VirtualRouterListenerTypeDef",
-    "MeshSpecOutputTypeDef",
     "MeshSpecTypeDef",
     "SubjectAlternativeNamesOutputTypeDef",
     "SubjectAlternativeNamesTypeDef",
     "TlsValidationContextTrustOutputTypeDef",
     "TlsValidationContextTrustTypeDef",
-    "VirtualGatewayClientTlsCertificateOutputTypeDef",
     "VirtualGatewayClientTlsCertificateTypeDef",
-    "VirtualGatewayConnectionPoolOutputTypeDef",
     "VirtualGatewayConnectionPoolTypeDef",
-    "VirtualGatewayListenerTlsCertificateOutputTypeDef",
     "VirtualGatewayListenerTlsCertificateTypeDef",
-    "VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
     "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextTrustTypeDef",
-    "VirtualNodeConnectionPoolOutputTypeDef",
     "VirtualNodeConnectionPoolTypeDef",
-    "VirtualServiceProviderOutputTypeDef",
     "VirtualServiceProviderTypeDef",
     "ServiceDiscoveryOutputTypeDef",
     "ServiceDiscoveryTypeDef",
-    "ListenerTimeoutOutputTypeDef",
     "ListenerTimeoutTypeDef",
-    "GrpcGatewayRouteActionOutputTypeDef",
     "GrpcGatewayRouteActionTypeDef",
-    "GrpcGatewayRouteMetadataOutputTypeDef",
-    "GrpcRouteMetadataOutputTypeDef",
-    "HttpGatewayRouteHeaderOutputTypeDef",
-    "HttpRouteHeaderOutputTypeDef",
     "GrpcGatewayRouteMetadataTypeDef",
     "GrpcRouteMetadataTypeDef",
     "HttpGatewayRouteHeaderTypeDef",
     "HttpRouteHeaderTypeDef",
     "TcpRouteOutputTypeDef",
     "TcpRouteTypeDef",
-    "HttpGatewayRouteActionOutputTypeDef",
     "HttpGatewayRouteActionTypeDef",
     "FileAccessLogOutputTypeDef",
     "VirtualGatewayFileAccessLogOutputTypeDef",
     "FileAccessLogTypeDef",
     "VirtualGatewayFileAccessLogTypeDef",
     "VirtualRouterSpecOutputTypeDef",
     "VirtualRouterSpecTypeDef",
-    "MeshDataTypeDef",
     "CreateMeshInputRequestTypeDef",
+    "MeshDataTypeDef",
     "UpdateMeshInputRequestTypeDef",
     "ListenerTlsValidationContextOutputTypeDef",
     "ListenerTlsValidationContextTypeDef",
     "TlsValidationContextOutputTypeDef",
     "TlsValidationContextTypeDef",
     "VirtualGatewayListenerTlsValidationContextOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTypeDef",
     "VirtualGatewayTlsValidationContextOutputTypeDef",
     "VirtualGatewayTlsValidationContextTypeDef",
-    "VirtualServiceSpecOutputTypeDef",
     "VirtualServiceSpecTypeDef",
     "GrpcGatewayRouteMatchOutputTypeDef",
-    "GrpcRouteMatchOutputTypeDef",
-    "HttpGatewayRouteMatchOutputTypeDef",
-    "HttpRouteMatchOutputTypeDef",
     "GrpcGatewayRouteMatchTypeDef",
+    "GrpcRouteMatchOutputTypeDef",
     "GrpcRouteMatchTypeDef",
+    "HttpGatewayRouteMatchOutputTypeDef",
     "HttpGatewayRouteMatchTypeDef",
+    "HttpRouteMatchOutputTypeDef",
     "HttpRouteMatchTypeDef",
     "AccessLogOutputTypeDef",
     "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
     "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
@@ -314,24 +244,24 @@
     "ListenerTlsTypeDef",
     "ClientPolicyTlsOutputTypeDef",
     "ClientPolicyTlsTypeDef",
     "VirtualGatewayListenerTlsOutputTypeDef",
     "VirtualGatewayListenerTlsTypeDef",
     "VirtualGatewayClientPolicyTlsOutputTypeDef",
     "VirtualGatewayClientPolicyTlsTypeDef",
-    "VirtualServiceDataTypeDef",
     "CreateVirtualServiceInputRequestTypeDef",
     "UpdateVirtualServiceInputRequestTypeDef",
+    "VirtualServiceDataTypeDef",
     "GrpcGatewayRouteOutputTypeDef",
-    "GrpcRouteOutputTypeDef",
-    "HttpGatewayRouteOutputTypeDef",
-    "HttpRouteOutputTypeDef",
     "GrpcGatewayRouteTypeDef",
+    "GrpcRouteOutputTypeDef",
     "GrpcRouteTypeDef",
+    "HttpGatewayRouteOutputTypeDef",
     "HttpGatewayRouteTypeDef",
+    "HttpRouteOutputTypeDef",
     "HttpRouteTypeDef",
     "LoggingOutputTypeDef",
     "VirtualGatewayLoggingOutputTypeDef",
     "LoggingTypeDef",
     "VirtualGatewayLoggingTypeDef",
     "CreateVirtualRouterOutputTypeDef",
     "DeleteVirtualRouterOutputTypeDef",
@@ -346,27 +276,27 @@
     "VirtualGatewayClientPolicyOutputTypeDef",
     "VirtualGatewayClientPolicyTypeDef",
     "CreateVirtualServiceOutputTypeDef",
     "DeleteVirtualServiceOutputTypeDef",
     "DescribeVirtualServiceOutputTypeDef",
     "UpdateVirtualServiceOutputTypeDef",
     "GatewayRouteSpecOutputTypeDef",
-    "RouteSpecOutputTypeDef",
     "GatewayRouteSpecTypeDef",
+    "RouteSpecOutputTypeDef",
     "RouteSpecTypeDef",
     "BackendDefaultsOutputTypeDef",
     "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
     "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
     "GatewayRouteDataTypeDef",
-    "RouteDataTypeDef",
     "CreateGatewayRouteInputRequestTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
+    "RouteDataTypeDef",
     "CreateRouteInputRequestTypeDef",
     "UpdateRouteInputRequestTypeDef",
     "BackendOutputTypeDef",
     "BackendTypeDef",
     "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
@@ -391,45 +321,22 @@
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
     "UpdateVirtualNodeOutputTypeDef",
 )
 
-AwsCloudMapInstanceAttributeOutputTypeDef = TypedDict(
-    "AwsCloudMapInstanceAttributeOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 AwsCloudMapInstanceAttributeTypeDef = TypedDict(
     "AwsCloudMapInstanceAttributeTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-ListenerTlsFileCertificateOutputTypeDef = TypedDict(
-    "ListenerTlsFileCertificateOutputTypeDef",
-    {
-        "certificateChain": str,
-        "privateKey": str,
-    },
-)
-
-ListenerTlsSdsCertificateOutputTypeDef = TypedDict(
-    "ListenerTlsSdsCertificateOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-
 ListenerTlsFileCertificateTypeDef = TypedDict(
     "ListenerTlsFileCertificateTypeDef",
     {
         "certificateChain": str,
         "privateKey": str,
     },
 )
@@ -445,14 +352,25 @@
     "TagRefTypeDef",
     {
         "key": str,
         "value": str,
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
 _RequiredDeleteGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDeleteGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -721,34 +639,14 @@
 
 class DescribeVirtualServiceInputRequestTypeDef(
     _RequiredDescribeVirtualServiceInputRequestTypeDef,
     _OptionalDescribeVirtualServiceInputRequestTypeDef,
 ):
     pass
 
-_RequiredDnsServiceDiscoveryOutputTypeDef = TypedDict(
-    "_RequiredDnsServiceDiscoveryOutputTypeDef",
-    {
-        "hostname": str,
-    },
-)
-_OptionalDnsServiceDiscoveryOutputTypeDef = TypedDict(
-    "_OptionalDnsServiceDiscoveryOutputTypeDef",
-    {
-        "ipPreference": IpPreferenceType,
-        "responseType": DnsResponseTypeType,
-    },
-    total=False,
-)
-
-class DnsServiceDiscoveryOutputTypeDef(
-    _RequiredDnsServiceDiscoveryOutputTypeDef, _OptionalDnsServiceDiscoveryOutputTypeDef
-):
-    pass
-
 _RequiredDnsServiceDiscoveryTypeDef = TypedDict(
     "_RequiredDnsServiceDiscoveryTypeDef",
     {
         "hostname": str,
     },
 )
 _OptionalDnsServiceDiscoveryTypeDef = TypedDict(
@@ -761,39 +659,23 @@
 )
 
 class DnsServiceDiscoveryTypeDef(
     _RequiredDnsServiceDiscoveryTypeDef, _OptionalDnsServiceDiscoveryTypeDef
 ):
     pass
 
-DurationOutputTypeDef = TypedDict(
-    "DurationOutputTypeDef",
-    {
-        "unit": DurationUnitType,
-        "value": int,
-    },
-    total=False,
-)
-
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "unit": DurationUnitType,
         "value": int,
     },
     total=False,
 )
 
-EgressFilterOutputTypeDef = TypedDict(
-    "EgressFilterOutputTypeDef",
-    {
-        "type": EgressFilterTypeType,
-    },
-)
-
 EgressFilterTypeDef = TypedDict(
     "EgressFilterTypeDef",
     {
         "type": EgressFilterTypeType,
     },
 )
 
@@ -813,40 +695,23 @@
         "meshOwner": str,
         "resourceOwner": str,
         "uid": str,
         "version": int,
     },
 )
 
-GatewayRouteHostnameMatchOutputTypeDef = TypedDict(
-    "GatewayRouteHostnameMatchOutputTypeDef",
-    {
-        "exact": str,
-        "suffix": str,
-    },
-    total=False,
-)
-
 GatewayRouteHostnameMatchTypeDef = TypedDict(
     "GatewayRouteHostnameMatchTypeDef",
     {
         "exact": str,
         "suffix": str,
     },
     total=False,
 )
 
-GatewayRouteHostnameRewriteOutputTypeDef = TypedDict(
-    "GatewayRouteHostnameRewriteOutputTypeDef",
-    {
-        "defaultTargetHostname": DefaultGatewayRouteRewriteType,
-    },
-    total=False,
-)
-
 GatewayRouteHostnameRewriteTypeDef = TypedDict(
     "GatewayRouteHostnameRewriteTypeDef",
     {
         "defaultTargetHostname": DefaultGatewayRouteRewriteType,
     },
     total=False,
 )
@@ -862,64 +727,29 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
-GatewayRouteVirtualServiceOutputTypeDef = TypedDict(
-    "GatewayRouteVirtualServiceOutputTypeDef",
-    {
-        "virtualServiceName": str,
-    },
-)
-
 GatewayRouteVirtualServiceTypeDef = TypedDict(
     "GatewayRouteVirtualServiceTypeDef",
     {
         "virtualServiceName": str,
     },
 )
 
-MatchRangeOutputTypeDef = TypedDict(
-    "MatchRangeOutputTypeDef",
-    {
-        "end": int,
-        "start": int,
-    },
-)
-
 MatchRangeTypeDef = TypedDict(
     "MatchRangeTypeDef",
     {
         "end": int,
         "start": int,
     },
 )
 
-_RequiredWeightedTargetOutputTypeDef = TypedDict(
-    "_RequiredWeightedTargetOutputTypeDef",
-    {
-        "virtualNode": str,
-        "weight": int,
-    },
-)
-_OptionalWeightedTargetOutputTypeDef = TypedDict(
-    "_OptionalWeightedTargetOutputTypeDef",
-    {
-        "port": int,
-    },
-    total=False,
-)
-
-class WeightedTargetOutputTypeDef(
-    _RequiredWeightedTargetOutputTypeDef, _OptionalWeightedTargetOutputTypeDef
-):
-    pass
-
 _RequiredWeightedTargetTypeDef = TypedDict(
     "_RequiredWeightedTargetTypeDef",
     {
         "virtualNode": str,
         "weight": int,
     },
 )
@@ -930,38 +760,14 @@
     },
     total=False,
 )
 
 class WeightedTargetTypeDef(_RequiredWeightedTargetTypeDef, _OptionalWeightedTargetTypeDef):
     pass
 
-_RequiredHealthCheckPolicyOutputTypeDef = TypedDict(
-    "_RequiredHealthCheckPolicyOutputTypeDef",
-    {
-        "healthyThreshold": int,
-        "intervalMillis": int,
-        "protocol": PortProtocolType,
-        "timeoutMillis": int,
-        "unhealthyThreshold": int,
-    },
-)
-_OptionalHealthCheckPolicyOutputTypeDef = TypedDict(
-    "_OptionalHealthCheckPolicyOutputTypeDef",
-    {
-        "path": str,
-        "port": int,
-    },
-    total=False,
-)
-
-class HealthCheckPolicyOutputTypeDef(
-    _RequiredHealthCheckPolicyOutputTypeDef, _OptionalHealthCheckPolicyOutputTypeDef
-):
-    pass
-
 _RequiredHealthCheckPolicyTypeDef = TypedDict(
     "_RequiredHealthCheckPolicyTypeDef",
     {
         "healthyThreshold": int,
         "intervalMillis": int,
         "protocol": PortProtocolType,
         "timeoutMillis": int,
@@ -978,120 +784,66 @@
 )
 
 class HealthCheckPolicyTypeDef(
     _RequiredHealthCheckPolicyTypeDef, _OptionalHealthCheckPolicyTypeDef
 ):
     pass
 
-HttpPathMatchOutputTypeDef = TypedDict(
-    "HttpPathMatchOutputTypeDef",
-    {
-        "exact": str,
-        "regex": str,
-    },
-    total=False,
-)
-
 HttpPathMatchTypeDef = TypedDict(
     "HttpPathMatchTypeDef",
     {
         "exact": str,
         "regex": str,
     },
     total=False,
 )
 
-HttpGatewayRoutePathRewriteOutputTypeDef = TypedDict(
-    "HttpGatewayRoutePathRewriteOutputTypeDef",
-    {
-        "exact": str,
-    },
-    total=False,
-)
-
 HttpGatewayRoutePathRewriteTypeDef = TypedDict(
     "HttpGatewayRoutePathRewriteTypeDef",
     {
         "exact": str,
     },
     total=False,
 )
 
-HttpGatewayRoutePrefixRewriteOutputTypeDef = TypedDict(
-    "HttpGatewayRoutePrefixRewriteOutputTypeDef",
-    {
-        "defaultPrefix": DefaultGatewayRouteRewriteType,
-        "value": str,
-    },
-    total=False,
-)
-
 HttpGatewayRoutePrefixRewriteTypeDef = TypedDict(
     "HttpGatewayRoutePrefixRewriteTypeDef",
     {
         "defaultPrefix": DefaultGatewayRouteRewriteType,
         "value": str,
     },
     total=False,
 )
 
-QueryParameterMatchOutputTypeDef = TypedDict(
-    "QueryParameterMatchOutputTypeDef",
-    {
-        "exact": str,
-    },
-    total=False,
-)
-
 QueryParameterMatchTypeDef = TypedDict(
     "QueryParameterMatchTypeDef",
     {
         "exact": str,
     },
     total=False,
 )
 
-JsonFormatRefOutputTypeDef = TypedDict(
-    "JsonFormatRefOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 JsonFormatRefTypeDef = TypedDict(
     "JsonFormatRefTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualGatewayName": str,
-    },
-)
-_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
-    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-):
-    pass
-
 _RequiredListGatewayRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListGatewayRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -1106,22 +858,14 @@
 )
 
 class ListGatewayRoutesInputRequestTypeDef(
     _RequiredListGatewayRoutesInputRequestTypeDef, _OptionalListGatewayRoutesInputRequestTypeDef
 ):
     pass
 
-ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
-    "ListMeshesInputListMeshesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMeshesInputRequestTypeDef = TypedDict(
     "ListMeshesInputRequestTypeDef",
     {
         "limit": int,
         "nextToken": str,
     },
     total=False,
@@ -1136,36 +880,14 @@
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
     },
 )
 
-_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualRouterName": str,
-    },
-)
-_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRoutesInputListRoutesPaginateTypeDef(
-    _RequiredListRoutesInputListRoutesPaginateTypeDef,
-    _OptionalListRoutesInputListRoutesPaginateTypeDef,
-):
-    pass
-
 _RequiredListRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -1195,34 +917,14 @@
         "resourceOwner": str,
         "routeName": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1235,43 +937,14 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-TagRefOutputTypeDef = TypedDict(
-    "TagRefOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
-_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
-    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-):
-    pass
-
 _RequiredListVirtualGatewaysInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualGatewaysInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualGatewaysInputRequestTypeDef = TypedDict(
@@ -1299,35 +972,14 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
-_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
-    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-):
-    pass
-
 _RequiredListVirtualNodesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualNodesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualNodesInputRequestTypeDef = TypedDict(
@@ -1355,35 +1007,14 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualNodeName": str,
     },
 )
 
-_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
-    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-):
-    pass
-
 _RequiredListVirtualRoutersInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualRoutersInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualRoutersInputRequestTypeDef = TypedDict(
@@ -1411,35 +1042,14 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
-_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
-    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-):
-    pass
-
 _RequiredListVirtualServicesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualServicesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualServicesInputRequestTypeDef = TypedDict(
@@ -1467,117 +1077,59 @@
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualServiceName": str,
     },
 )
 
-PortMappingOutputTypeDef = TypedDict(
-    "PortMappingOutputTypeDef",
+PortMappingTypeDef = TypedDict(
+    "PortMappingTypeDef",
     {
         "port": int,
         "protocol": PortProtocolType,
     },
 )
 
-ListenerTlsAcmCertificateOutputTypeDef = TypedDict(
-    "ListenerTlsAcmCertificateOutputTypeDef",
-    {
-        "certificateArn": str,
-    },
-)
-
 ListenerTlsAcmCertificateTypeDef = TypedDict(
     "ListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
-TlsValidationContextFileTrustOutputTypeDef = TypedDict(
-    "TlsValidationContextFileTrustOutputTypeDef",
-    {
-        "certificateChain": str,
-    },
-)
-
-TlsValidationContextSdsTrustOutputTypeDef = TypedDict(
-    "TlsValidationContextSdsTrustOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-
 TlsValidationContextFileTrustTypeDef = TypedDict(
     "TlsValidationContextFileTrustTypeDef",
     {
         "certificateChain": str,
     },
 )
 
 TlsValidationContextSdsTrustTypeDef = TypedDict(
     "TlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-PortMappingTypeDef = TypedDict(
-    "PortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": PortProtocolType,
-    },
-)
-
 MeshStatusTypeDef = TypedDict(
     "MeshStatusTypeDef",
     {
         "status": MeshStatusCodeType,
     },
     total=False,
 )
 
-MeshServiceDiscoveryOutputTypeDef = TypedDict(
-    "MeshServiceDiscoveryOutputTypeDef",
-    {
-        "ipPreference": IpPreferenceType,
-    },
-    total=False,
-)
-
 MeshServiceDiscoveryTypeDef = TypedDict(
     "MeshServiceDiscoveryTypeDef",
     {
         "ipPreference": IpPreferenceType,
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
 RouteStatusTypeDef = TypedDict(
     "RouteStatusTypeDef",
     {
         "status": RouteStatusCodeType,
     },
 )
 
@@ -1591,22 +1143,14 @@
 SubjectAlternativeNameMatchersTypeDef = TypedDict(
     "SubjectAlternativeNameMatchersTypeDef",
     {
         "exact": Sequence[str],
     },
 )
 
-TcpRouteMatchOutputTypeDef = TypedDict(
-    "TcpRouteMatchOutputTypeDef",
-    {
-        "port": int,
-    },
-    total=False,
-)
-
 TcpRouteMatchTypeDef = TypedDict(
     "TcpRouteMatchTypeDef",
     {
         "port": int,
     },
     total=False,
 )
@@ -1629,29 +1173,14 @@
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-VirtualGatewayListenerTlsFileCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsFileCertificateOutputTypeDef",
-    {
-        "certificateChain": str,
-        "privateKey": str,
-    },
-)
-
-VirtualGatewayListenerTlsSdsCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsSdsCertificateOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-
 VirtualGatewayListenerTlsFileCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     {
         "certificateChain": str,
         "privateKey": str,
     },
 )
@@ -1659,48 +1188,14 @@
 VirtualGatewayListenerTlsSdsCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
     {
         "secretName": str,
     },
 )
 
-VirtualGatewayGrpcConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualGatewayGrpcConnectionPoolOutputTypeDef",
-    {
-        "maxRequests": int,
-    },
-)
-
-VirtualGatewayHttp2ConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualGatewayHttp2ConnectionPoolOutputTypeDef",
-    {
-        "maxRequests": int,
-    },
-)
-
-_RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef",
-    {
-        "maxConnections": int,
-    },
-)
-_OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef",
-    {
-        "maxPendingRequests": int,
-    },
-    total=False,
-)
-
-class VirtualGatewayHttpConnectionPoolOutputTypeDef(
-    _RequiredVirtualGatewayHttpConnectionPoolOutputTypeDef,
-    _OptionalVirtualGatewayHttpConnectionPoolOutputTypeDef,
-):
-    pass
-
 VirtualGatewayGrpcConnectionPoolTypeDef = TypedDict(
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     {
         "maxRequests": int,
     },
 )
 
@@ -1734,39 +1229,14 @@
 VirtualGatewayStatusTypeDef = TypedDict(
     "VirtualGatewayStatusTypeDef",
     {
         "status": VirtualGatewayStatusCodeType,
     },
 )
 
-_RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef = TypedDict(
-    "_RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef",
-    {
-        "healthyThreshold": int,
-        "intervalMillis": int,
-        "protocol": VirtualGatewayPortProtocolType,
-        "timeoutMillis": int,
-        "unhealthyThreshold": int,
-    },
-)
-_OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef = TypedDict(
-    "_OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef",
-    {
-        "path": str,
-        "port": int,
-    },
-    total=False,
-)
-
-class VirtualGatewayHealthCheckPolicyOutputTypeDef(
-    _RequiredVirtualGatewayHealthCheckPolicyOutputTypeDef,
-    _OptionalVirtualGatewayHealthCheckPolicyOutputTypeDef,
-):
-    pass
-
 _RequiredVirtualGatewayHealthCheckPolicyTypeDef = TypedDict(
     "_RequiredVirtualGatewayHealthCheckPolicyTypeDef",
     {
         "healthyThreshold": int,
         "intervalMillis": int,
         "protocol": VirtualGatewayPortProtocolType,
         "timeoutMillis": int,
@@ -1783,127 +1253,57 @@
 )
 
 class VirtualGatewayHealthCheckPolicyTypeDef(
     _RequiredVirtualGatewayHealthCheckPolicyTypeDef, _OptionalVirtualGatewayHealthCheckPolicyTypeDef
 ):
     pass
 
-VirtualGatewayPortMappingOutputTypeDef = TypedDict(
-    "VirtualGatewayPortMappingOutputTypeDef",
+VirtualGatewayPortMappingTypeDef = TypedDict(
+    "VirtualGatewayPortMappingTypeDef",
     {
         "port": int,
         "protocol": VirtualGatewayPortProtocolType,
     },
 )
 
-VirtualGatewayListenerTlsAcmCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsAcmCertificateOutputTypeDef",
-    {
-        "certificateArn": str,
-    },
-)
-
 VirtualGatewayListenerTlsAcmCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
-VirtualGatewayTlsValidationContextFileTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayTlsValidationContextFileTrustOutputTypeDef",
-    {
-        "certificateChain": str,
-    },
-)
-
-VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef",
-    {
-        "secretName": str,
-    },
-)
-
 VirtualGatewayTlsValidationContextFileTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     {
         "certificateChain": str,
     },
 )
 
 VirtualGatewayTlsValidationContextSdsTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-VirtualGatewayPortMappingTypeDef = TypedDict(
-    "VirtualGatewayPortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": VirtualGatewayPortProtocolType,
-    },
-)
-
 VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     {
         "certificateAuthorityArns": List[str],
     },
 )
 
 VirtualGatewayTlsValidationContextAcmTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
     },
 )
 
-VirtualNodeGrpcConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualNodeGrpcConnectionPoolOutputTypeDef",
-    {
-        "maxRequests": int,
-    },
-)
-
-VirtualNodeHttp2ConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualNodeHttp2ConnectionPoolOutputTypeDef",
-    {
-        "maxRequests": int,
-    },
-)
-
-_RequiredVirtualNodeHttpConnectionPoolOutputTypeDef = TypedDict(
-    "_RequiredVirtualNodeHttpConnectionPoolOutputTypeDef",
-    {
-        "maxConnections": int,
-    },
-)
-_OptionalVirtualNodeHttpConnectionPoolOutputTypeDef = TypedDict(
-    "_OptionalVirtualNodeHttpConnectionPoolOutputTypeDef",
-    {
-        "maxPendingRequests": int,
-    },
-    total=False,
-)
-
-class VirtualNodeHttpConnectionPoolOutputTypeDef(
-    _RequiredVirtualNodeHttpConnectionPoolOutputTypeDef,
-    _OptionalVirtualNodeHttpConnectionPoolOutputTypeDef,
-):
-    pass
-
-VirtualNodeTcpConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualNodeTcpConnectionPoolOutputTypeDef",
-    {
-        "maxConnections": int,
-    },
-)
-
 VirtualNodeGrpcConnectionPoolTypeDef = TypedDict(
     "VirtualNodeGrpcConnectionPoolTypeDef",
     {
         "maxRequests": int,
     },
 )
 
@@ -1943,42 +1343,28 @@
 VirtualNodeStatusTypeDef = TypedDict(
     "VirtualNodeStatusTypeDef",
     {
         "status": VirtualNodeStatusCodeType,
     },
 )
 
-VirtualNodeServiceProviderOutputTypeDef = TypedDict(
-    "VirtualNodeServiceProviderOutputTypeDef",
-    {
-        "virtualNodeName": str,
-    },
-)
-
 VirtualNodeServiceProviderTypeDef = TypedDict(
     "VirtualNodeServiceProviderTypeDef",
     {
         "virtualNodeName": str,
     },
 )
 
 VirtualRouterStatusTypeDef = TypedDict(
     "VirtualRouterStatusTypeDef",
     {
         "status": VirtualRouterStatusCodeType,
     },
 )
 
-VirtualRouterServiceProviderOutputTypeDef = TypedDict(
-    "VirtualRouterServiceProviderOutputTypeDef",
-    {
-        "virtualRouterName": str,
-    },
-)
-
 VirtualRouterServiceProviderTypeDef = TypedDict(
     "VirtualRouterServiceProviderTypeDef",
     {
         "virtualRouterName": str,
     },
 )
 
@@ -1995,15 +1381,15 @@
         "namespaceName": str,
         "serviceName": str,
     },
 )
 _OptionalAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
     "_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef",
     {
-        "attributes": List[AwsCloudMapInstanceAttributeOutputTypeDef],
+        "attributes": List[AwsCloudMapInstanceAttributeTypeDef],
         "ipPreference": IpPreferenceType,
     },
     total=False,
 )
 
 class AwsCloudMapServiceDiscoveryOutputTypeDef(
     _RequiredAwsCloudMapServiceDiscoveryOutputTypeDef,
@@ -2028,23 +1414,14 @@
 )
 
 class AwsCloudMapServiceDiscoveryTypeDef(
     _RequiredAwsCloudMapServiceDiscoveryTypeDef, _OptionalAwsCloudMapServiceDiscoveryTypeDef
 ):
     pass
 
-ClientTlsCertificateOutputTypeDef = TypedDict(
-    "ClientTlsCertificateOutputTypeDef",
-    {
-        "file": ListenerTlsFileCertificateOutputTypeDef,
-        "sds": ListenerTlsSdsCertificateOutputTypeDef,
-    },
-    total=False,
-)
-
 ClientTlsCertificateTypeDef = TypedDict(
     "ClientTlsCertificateTypeDef",
     {
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
@@ -2054,19 +1431,28 @@
     "TagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagRefTypeDef],
     },
 )
 
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "nextToken": str,
+        "tags": List[TagRefTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredGrpcRetryPolicyOutputTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyOutputTypeDef",
     {
         "maxRetries": int,
-        "perRetryTimeout": DurationOutputTypeDef,
+        "perRetryTimeout": DurationTypeDef,
     },
 )
 _OptionalGrpcRetryPolicyOutputTypeDef = TypedDict(
     "_OptionalGrpcRetryPolicyOutputTypeDef",
     {
         "grpcRetryEvents": List[GrpcRetryPolicyEventType],
         "httpRetryEvents": List[str],
@@ -2076,71 +1462,14 @@
 )
 
 class GrpcRetryPolicyOutputTypeDef(
     _RequiredGrpcRetryPolicyOutputTypeDef, _OptionalGrpcRetryPolicyOutputTypeDef
 ):
     pass
 
-GrpcTimeoutOutputTypeDef = TypedDict(
-    "GrpcTimeoutOutputTypeDef",
-    {
-        "idle": DurationOutputTypeDef,
-        "perRequest": DurationOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
-    "_RequiredHttpRetryPolicyOutputTypeDef",
-    {
-        "maxRetries": int,
-        "perRetryTimeout": DurationOutputTypeDef,
-    },
-)
-_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
-    "_OptionalHttpRetryPolicyOutputTypeDef",
-    {
-        "httpRetryEvents": List[str],
-        "tcpRetryEvents": List[Literal["connection-error"]],
-    },
-    total=False,
-)
-
-class HttpRetryPolicyOutputTypeDef(
-    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
-):
-    pass
-
-HttpTimeoutOutputTypeDef = TypedDict(
-    "HttpTimeoutOutputTypeDef",
-    {
-        "idle": DurationOutputTypeDef,
-        "perRequest": DurationOutputTypeDef,
-    },
-    total=False,
-)
-
-OutlierDetectionOutputTypeDef = TypedDict(
-    "OutlierDetectionOutputTypeDef",
-    {
-        "baseEjectionDuration": DurationOutputTypeDef,
-        "interval": DurationOutputTypeDef,
-        "maxEjectionPercent": int,
-        "maxServerErrors": int,
-    },
-)
-
-TcpTimeoutOutputTypeDef = TypedDict(
-    "TcpTimeoutOutputTypeDef",
-    {
-        "idle": DurationOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredGrpcRetryPolicyTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -2162,14 +1491,35 @@
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
 )
 
+_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_RequiredHttpRetryPolicyOutputTypeDef",
+    {
+        "maxRetries": int,
+        "perRetryTimeout": DurationTypeDef,
+    },
+)
+_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_OptionalHttpRetryPolicyOutputTypeDef",
+    {
+        "httpRetryEvents": List[str],
+        "tcpRetryEvents": List[Literal["connection-error"]],
+    },
+    total=False,
+)
+
+class HttpRetryPolicyOutputTypeDef(
+    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
+):
+    pass
+
 _RequiredHttpRetryPolicyTypeDef = TypedDict(
     "_RequiredHttpRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -2208,57 +1558,30 @@
     "TcpTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
     },
     total=False,
 )
 
-GrpcGatewayRouteRewriteOutputTypeDef = TypedDict(
-    "GrpcGatewayRouteRewriteOutputTypeDef",
-    {
-        "hostname": GatewayRouteHostnameRewriteOutputTypeDef,
-    },
-    total=False,
-)
-
 GrpcGatewayRouteRewriteTypeDef = TypedDict(
     "GrpcGatewayRouteRewriteTypeDef",
     {
         "hostname": GatewayRouteHostnameRewriteTypeDef,
     },
     total=False,
 )
 
 ListGatewayRoutesOutputTypeDef = TypedDict(
     "ListGatewayRoutesOutputTypeDef",
     {
         "gatewayRoutes": List[GatewayRouteRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGatewayRouteTargetOutputTypeDef = TypedDict(
-    "_RequiredGatewayRouteTargetOutputTypeDef",
-    {
-        "virtualService": GatewayRouteVirtualServiceOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalGatewayRouteTargetOutputTypeDef = TypedDict(
-    "_OptionalGatewayRouteTargetOutputTypeDef",
-    {
-        "port": int,
-    },
-    total=False,
-)
-
-class GatewayRouteTargetOutputTypeDef(
-    _RequiredGatewayRouteTargetOutputTypeDef, _OptionalGatewayRouteTargetOutputTypeDef
-):
-    pass
 
 _RequiredGatewayRouteTargetTypeDef = TypedDict(
     "_RequiredGatewayRouteTargetTypeDef",
     {
         "virtualService": GatewayRouteVirtualServiceTypeDef,
     },
 )
@@ -2271,50 +1594,14 @@
 )
 
 class GatewayRouteTargetTypeDef(
     _RequiredGatewayRouteTargetTypeDef, _OptionalGatewayRouteTargetTypeDef
 ):
     pass
 
-GrpcMetadataMatchMethodOutputTypeDef = TypedDict(
-    "GrpcMetadataMatchMethodOutputTypeDef",
-    {
-        "exact": str,
-        "prefix": str,
-        "range": MatchRangeOutputTypeDef,
-        "regex": str,
-        "suffix": str,
-    },
-    total=False,
-)
-
-GrpcRouteMetadataMatchMethodOutputTypeDef = TypedDict(
-    "GrpcRouteMetadataMatchMethodOutputTypeDef",
-    {
-        "exact": str,
-        "prefix": str,
-        "range": MatchRangeOutputTypeDef,
-        "regex": str,
-        "suffix": str,
-    },
-    total=False,
-)
-
-HeaderMatchMethodOutputTypeDef = TypedDict(
-    "HeaderMatchMethodOutputTypeDef",
-    {
-        "exact": str,
-        "prefix": str,
-        "range": MatchRangeOutputTypeDef,
-        "regex": str,
-        "suffix": str,
-    },
-    total=False,
-)
-
 GrpcMetadataMatchMethodTypeDef = TypedDict(
     "GrpcMetadataMatchMethodTypeDef",
     {
         "exact": str,
         "prefix": str,
         "range": MatchRangeTypeDef,
         "regex": str,
@@ -2346,92 +1633,63 @@
     },
     total=False,
 )
 
 GrpcRouteActionOutputTypeDef = TypedDict(
     "GrpcRouteActionOutputTypeDef",
     {
-        "weightedTargets": List[WeightedTargetOutputTypeDef],
+        "weightedTargets": List[WeightedTargetTypeDef],
     },
 )
 
-HttpRouteActionOutputTypeDef = TypedDict(
-    "HttpRouteActionOutputTypeDef",
+GrpcRouteActionTypeDef = TypedDict(
+    "GrpcRouteActionTypeDef",
     {
-        "weightedTargets": List[WeightedTargetOutputTypeDef],
+        "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-TcpRouteActionOutputTypeDef = TypedDict(
-    "TcpRouteActionOutputTypeDef",
+HttpRouteActionOutputTypeDef = TypedDict(
+    "HttpRouteActionOutputTypeDef",
     {
-        "weightedTargets": List[WeightedTargetOutputTypeDef],
+        "weightedTargets": List[WeightedTargetTypeDef],
     },
 )
 
-GrpcRouteActionTypeDef = TypedDict(
-    "GrpcRouteActionTypeDef",
+HttpRouteActionTypeDef = TypedDict(
+    "HttpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-HttpRouteActionTypeDef = TypedDict(
-    "HttpRouteActionTypeDef",
+TcpRouteActionOutputTypeDef = TypedDict(
+    "TcpRouteActionOutputTypeDef",
     {
-        "weightedTargets": Sequence[WeightedTargetTypeDef],
+        "weightedTargets": List[WeightedTargetTypeDef],
     },
 )
 
 TcpRouteActionTypeDef = TypedDict(
     "TcpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
-HttpGatewayRouteRewriteOutputTypeDef = TypedDict(
-    "HttpGatewayRouteRewriteOutputTypeDef",
-    {
-        "hostname": GatewayRouteHostnameRewriteOutputTypeDef,
-        "path": HttpGatewayRoutePathRewriteOutputTypeDef,
-        "prefix": HttpGatewayRoutePrefixRewriteOutputTypeDef,
-    },
-    total=False,
-)
-
 HttpGatewayRouteRewriteTypeDef = TypedDict(
     "HttpGatewayRouteRewriteTypeDef",
     {
         "hostname": GatewayRouteHostnameRewriteTypeDef,
         "path": HttpGatewayRoutePathRewriteTypeDef,
         "prefix": HttpGatewayRoutePrefixRewriteTypeDef,
     },
     total=False,
 )
 
-_RequiredHttpQueryParameterOutputTypeDef = TypedDict(
-    "_RequiredHttpQueryParameterOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalHttpQueryParameterOutputTypeDef = TypedDict(
-    "_OptionalHttpQueryParameterOutputTypeDef",
-    {
-        "match": QueryParameterMatchOutputTypeDef,
-    },
-    total=False,
-)
-
-class HttpQueryParameterOutputTypeDef(
-    _RequiredHttpQueryParameterOutputTypeDef, _OptionalHttpQueryParameterOutputTypeDef
-):
-    pass
-
 _RequiredHttpQueryParameterTypeDef = TypedDict(
     "_RequiredHttpQueryParameterTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpQueryParameterTypeDef = TypedDict(
@@ -2446,153 +1704,265 @@
     _RequiredHttpQueryParameterTypeDef, _OptionalHttpQueryParameterTypeDef
 ):
     pass
 
 LoggingFormatOutputTypeDef = TypedDict(
     "LoggingFormatOutputTypeDef",
     {
-        "json": List[JsonFormatRefOutputTypeDef],
+        "json": List[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
 )
 
 LoggingFormatTypeDef = TypedDict(
     "LoggingFormatTypeDef",
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
 )
 
+_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualGatewayName": str,
+    },
+)
+_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
+    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+):
+    pass
+
+ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualRouterName": str,
+    },
+)
+_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRoutesInputListRoutesPaginateTypeDef(
+    _RequiredListRoutesInputListRoutesPaginateTypeDef,
+    _OptionalListRoutesInputListRoutesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
+    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+):
+    pass
+
+_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
+    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+):
+    pass
+
+_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
+    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+):
+    pass
+
+_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
+    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+):
+    pass
+
 ListMeshesOutputTypeDef = TypedDict(
     "ListMeshesOutputTypeDef",
     {
         "meshes": List[MeshRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoutesOutputTypeDef = TypedDict(
     "ListRoutesOutputTypeDef",
     {
         "nextToken": str,
         "routes": List[RouteRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "nextToken": str,
-        "tags": List[TagRefOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualGatewaysOutputTypeDef = TypedDict(
     "ListVirtualGatewaysOutputTypeDef",
     {
         "nextToken": str,
         "virtualGateways": List[VirtualGatewayRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualNodesOutputTypeDef = TypedDict(
     "ListVirtualNodesOutputTypeDef",
     {
         "nextToken": str,
         "virtualNodes": List[VirtualNodeRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualRoutersOutputTypeDef = TypedDict(
     "ListVirtualRoutersOutputTypeDef",
     {
         "nextToken": str,
         "virtualRouters": List[VirtualRouterRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualServicesOutputTypeDef = TypedDict(
     "ListVirtualServicesOutputTypeDef",
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VirtualRouterListenerOutputTypeDef = TypedDict(
-    "VirtualRouterListenerOutputTypeDef",
-    {
-        "portMapping": PortMappingOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListenerTlsCertificateOutputTypeDef = TypedDict(
-    "ListenerTlsCertificateOutputTypeDef",
+VirtualRouterListenerTypeDef = TypedDict(
+    "VirtualRouterListenerTypeDef",
     {
-        "acm": ListenerTlsAcmCertificateOutputTypeDef,
-        "file": ListenerTlsFileCertificateOutputTypeDef,
-        "sds": ListenerTlsSdsCertificateOutputTypeDef,
+        "portMapping": PortMappingTypeDef,
     },
-    total=False,
 )
 
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-ListenerTlsValidationContextTrustOutputTypeDef = TypedDict(
-    "ListenerTlsValidationContextTrustOutputTypeDef",
-    {
-        "file": TlsValidationContextFileTrustOutputTypeDef,
-        "sds": TlsValidationContextSdsTrustOutputTypeDef,
-    },
-    total=False,
-)
-
 ListenerTlsValidationContextTrustTypeDef = TypedDict(
     "ListenerTlsValidationContextTrustTypeDef",
     {
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualRouterListenerTypeDef = TypedDict(
-    "VirtualRouterListenerTypeDef",
-    {
-        "portMapping": PortMappingTypeDef,
-    },
-)
-
-MeshSpecOutputTypeDef = TypedDict(
-    "MeshSpecOutputTypeDef",
-    {
-        "egressFilter": EgressFilterOutputTypeDef,
-        "serviceDiscovery": MeshServiceDiscoveryOutputTypeDef,
-    },
-    total=False,
-)
-
 MeshSpecTypeDef = TypedDict(
     "MeshSpecTypeDef",
     {
         "egressFilter": EgressFilterTypeDef,
         "serviceDiscovery": MeshServiceDiscoveryTypeDef,
     },
     total=False,
@@ -2612,225 +1982,137 @@
     },
 )
 
 TlsValidationContextTrustOutputTypeDef = TypedDict(
     "TlsValidationContextTrustOutputTypeDef",
     {
         "acm": TlsValidationContextAcmTrustOutputTypeDef,
-        "file": TlsValidationContextFileTrustOutputTypeDef,
-        "sds": TlsValidationContextSdsTrustOutputTypeDef,
+        "file": TlsValidationContextFileTrustTypeDef,
+        "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
 TlsValidationContextTrustTypeDef = TypedDict(
     "TlsValidationContextTrustTypeDef",
     {
         "acm": TlsValidationContextAcmTrustTypeDef,
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayClientTlsCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayClientTlsCertificateOutputTypeDef",
-    {
-        "file": VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
-        "sds": VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayClientTlsCertificateTypeDef = TypedDict(
     "VirtualGatewayClientTlsCertificateTypeDef",
     {
         "file": VirtualGatewayListenerTlsFileCertificateTypeDef,
         "sds": VirtualGatewayListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualGatewayConnectionPoolOutputTypeDef",
-    {
-        "grpc": VirtualGatewayGrpcConnectionPoolOutputTypeDef,
-        "http": VirtualGatewayHttpConnectionPoolOutputTypeDef,
-        "http2": VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayConnectionPoolTypeDef = TypedDict(
     "VirtualGatewayConnectionPoolTypeDef",
     {
         "grpc": VirtualGatewayGrpcConnectionPoolTypeDef,
         "http": VirtualGatewayHttpConnectionPoolTypeDef,
         "http2": VirtualGatewayHttp2ConnectionPoolTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayListenerTlsCertificateOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsCertificateOutputTypeDef",
-    {
-        "acm": VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
-        "file": VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
-        "sds": VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayListenerTlsCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsCertificateTypeDef",
     {
         "acm": VirtualGatewayListenerTlsAcmCertificateTypeDef,
         "file": VirtualGatewayListenerTlsFileCertificateTypeDef,
         "sds": VirtualGatewayListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
-VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef = TypedDict(
-    "VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef",
-    {
-        "file": VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
-        "sds": VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualGatewayListenerTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
     {
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
 VirtualGatewayTlsValidationContextTrustOutputTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
-        "file": VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
-        "sds": VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
+        "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
+        "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
 VirtualGatewayTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustTypeDef,
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualNodeConnectionPoolOutputTypeDef = TypedDict(
-    "VirtualNodeConnectionPoolOutputTypeDef",
-    {
-        "grpc": VirtualNodeGrpcConnectionPoolOutputTypeDef,
-        "http": VirtualNodeHttpConnectionPoolOutputTypeDef,
-        "http2": VirtualNodeHttp2ConnectionPoolOutputTypeDef,
-        "tcp": VirtualNodeTcpConnectionPoolOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualNodeConnectionPoolTypeDef = TypedDict(
     "VirtualNodeConnectionPoolTypeDef",
     {
         "grpc": VirtualNodeGrpcConnectionPoolTypeDef,
         "http": VirtualNodeHttpConnectionPoolTypeDef,
         "http2": VirtualNodeHttp2ConnectionPoolTypeDef,
         "tcp": VirtualNodeTcpConnectionPoolTypeDef,
     },
     total=False,
 )
 
-VirtualServiceProviderOutputTypeDef = TypedDict(
-    "VirtualServiceProviderOutputTypeDef",
-    {
-        "virtualNode": VirtualNodeServiceProviderOutputTypeDef,
-        "virtualRouter": VirtualRouterServiceProviderOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualServiceProviderTypeDef = TypedDict(
     "VirtualServiceProviderTypeDef",
     {
         "virtualNode": VirtualNodeServiceProviderTypeDef,
         "virtualRouter": VirtualRouterServiceProviderTypeDef,
     },
     total=False,
 )
 
 ServiceDiscoveryOutputTypeDef = TypedDict(
     "ServiceDiscoveryOutputTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryOutputTypeDef,
-        "dns": DnsServiceDiscoveryOutputTypeDef,
+        "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
 ServiceDiscoveryTypeDef = TypedDict(
     "ServiceDiscoveryTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryTypeDef,
         "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
-ListenerTimeoutOutputTypeDef = TypedDict(
-    "ListenerTimeoutOutputTypeDef",
-    {
-        "grpc": GrpcTimeoutOutputTypeDef,
-        "http": HttpTimeoutOutputTypeDef,
-        "http2": HttpTimeoutOutputTypeDef,
-        "tcp": TcpTimeoutOutputTypeDef,
-    },
-    total=False,
-)
-
 ListenerTimeoutTypeDef = TypedDict(
     "ListenerTimeoutTypeDef",
     {
         "grpc": GrpcTimeoutTypeDef,
         "http": HttpTimeoutTypeDef,
         "http2": HttpTimeoutTypeDef,
         "tcp": TcpTimeoutTypeDef,
     },
     total=False,
 )
 
-_RequiredGrpcGatewayRouteActionOutputTypeDef = TypedDict(
-    "_RequiredGrpcGatewayRouteActionOutputTypeDef",
-    {
-        "target": GatewayRouteTargetOutputTypeDef,
-    },
-)
-_OptionalGrpcGatewayRouteActionOutputTypeDef = TypedDict(
-    "_OptionalGrpcGatewayRouteActionOutputTypeDef",
-    {
-        "rewrite": GrpcGatewayRouteRewriteOutputTypeDef,
-    },
-    total=False,
-)
-
-class GrpcGatewayRouteActionOutputTypeDef(
-    _RequiredGrpcGatewayRouteActionOutputTypeDef, _OptionalGrpcGatewayRouteActionOutputTypeDef
-):
-    pass
-
 _RequiredGrpcGatewayRouteActionTypeDef = TypedDict(
     "_RequiredGrpcGatewayRouteActionTypeDef",
     {
         "target": GatewayRouteTargetTypeDef,
     },
 )
 _OptionalGrpcGatewayRouteActionTypeDef = TypedDict(
@@ -2842,94 +2124,14 @@
 )
 
 class GrpcGatewayRouteActionTypeDef(
     _RequiredGrpcGatewayRouteActionTypeDef, _OptionalGrpcGatewayRouteActionTypeDef
 ):
     pass
 
-_RequiredGrpcGatewayRouteMetadataOutputTypeDef = TypedDict(
-    "_RequiredGrpcGatewayRouteMetadataOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGrpcGatewayRouteMetadataOutputTypeDef = TypedDict(
-    "_OptionalGrpcGatewayRouteMetadataOutputTypeDef",
-    {
-        "invert": bool,
-        "match": GrpcMetadataMatchMethodOutputTypeDef,
-    },
-    total=False,
-)
-
-class GrpcGatewayRouteMetadataOutputTypeDef(
-    _RequiredGrpcGatewayRouteMetadataOutputTypeDef, _OptionalGrpcGatewayRouteMetadataOutputTypeDef
-):
-    pass
-
-_RequiredGrpcRouteMetadataOutputTypeDef = TypedDict(
-    "_RequiredGrpcRouteMetadataOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalGrpcRouteMetadataOutputTypeDef = TypedDict(
-    "_OptionalGrpcRouteMetadataOutputTypeDef",
-    {
-        "invert": bool,
-        "match": GrpcRouteMetadataMatchMethodOutputTypeDef,
-    },
-    total=False,
-)
-
-class GrpcRouteMetadataOutputTypeDef(
-    _RequiredGrpcRouteMetadataOutputTypeDef, _OptionalGrpcRouteMetadataOutputTypeDef
-):
-    pass
-
-_RequiredHttpGatewayRouteHeaderOutputTypeDef = TypedDict(
-    "_RequiredHttpGatewayRouteHeaderOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalHttpGatewayRouteHeaderOutputTypeDef = TypedDict(
-    "_OptionalHttpGatewayRouteHeaderOutputTypeDef",
-    {
-        "invert": bool,
-        "match": HeaderMatchMethodOutputTypeDef,
-    },
-    total=False,
-)
-
-class HttpGatewayRouteHeaderOutputTypeDef(
-    _RequiredHttpGatewayRouteHeaderOutputTypeDef, _OptionalHttpGatewayRouteHeaderOutputTypeDef
-):
-    pass
-
-_RequiredHttpRouteHeaderOutputTypeDef = TypedDict(
-    "_RequiredHttpRouteHeaderOutputTypeDef",
-    {
-        "name": str,
-    },
-)
-_OptionalHttpRouteHeaderOutputTypeDef = TypedDict(
-    "_OptionalHttpRouteHeaderOutputTypeDef",
-    {
-        "invert": bool,
-        "match": HeaderMatchMethodOutputTypeDef,
-    },
-    total=False,
-)
-
-class HttpRouteHeaderOutputTypeDef(
-    _RequiredHttpRouteHeaderOutputTypeDef, _OptionalHttpRouteHeaderOutputTypeDef
-):
-    pass
-
 _RequiredGrpcGatewayRouteMetadataTypeDef = TypedDict(
     "_RequiredGrpcGatewayRouteMetadataTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGrpcGatewayRouteMetadataTypeDef = TypedDict(
@@ -3009,16 +2211,16 @@
     {
         "action": TcpRouteActionOutputTypeDef,
     },
 )
 _OptionalTcpRouteOutputTypeDef = TypedDict(
     "_OptionalTcpRouteOutputTypeDef",
     {
-        "match": TcpRouteMatchOutputTypeDef,
-        "timeout": TcpTimeoutOutputTypeDef,
+        "match": TcpRouteMatchTypeDef,
+        "timeout": TcpTimeoutTypeDef,
     },
     total=False,
 )
 
 class TcpRouteOutputTypeDef(_RequiredTcpRouteOutputTypeDef, _OptionalTcpRouteOutputTypeDef):
     pass
 
@@ -3036,33 +2238,14 @@
     },
     total=False,
 )
 
 class TcpRouteTypeDef(_RequiredTcpRouteTypeDef, _OptionalTcpRouteTypeDef):
     pass
 
-_RequiredHttpGatewayRouteActionOutputTypeDef = TypedDict(
-    "_RequiredHttpGatewayRouteActionOutputTypeDef",
-    {
-        "target": GatewayRouteTargetOutputTypeDef,
-    },
-)
-_OptionalHttpGatewayRouteActionOutputTypeDef = TypedDict(
-    "_OptionalHttpGatewayRouteActionOutputTypeDef",
-    {
-        "rewrite": HttpGatewayRouteRewriteOutputTypeDef,
-    },
-    total=False,
-)
-
-class HttpGatewayRouteActionOutputTypeDef(
-    _RequiredHttpGatewayRouteActionOutputTypeDef, _OptionalHttpGatewayRouteActionOutputTypeDef
-):
-    pass
-
 _RequiredHttpGatewayRouteActionTypeDef = TypedDict(
     "_RequiredHttpGatewayRouteActionTypeDef",
     {
         "target": GatewayRouteTargetTypeDef,
     },
 )
 _OptionalHttpGatewayRouteActionTypeDef = TypedDict(
@@ -3152,37 +2335,27 @@
     _RequiredVirtualGatewayFileAccessLogTypeDef, _OptionalVirtualGatewayFileAccessLogTypeDef
 ):
     pass
 
 VirtualRouterSpecOutputTypeDef = TypedDict(
     "VirtualRouterSpecOutputTypeDef",
     {
-        "listeners": List[VirtualRouterListenerOutputTypeDef],
+        "listeners": List[VirtualRouterListenerTypeDef],
     },
     total=False,
 )
 
 VirtualRouterSpecTypeDef = TypedDict(
     "VirtualRouterSpecTypeDef",
     {
         "listeners": Sequence[VirtualRouterListenerTypeDef],
     },
     total=False,
 )
 
-MeshDataTypeDef = TypedDict(
-    "MeshDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": MeshSpecOutputTypeDef,
-        "status": MeshStatusTypeDef,
-    },
-)
-
 _RequiredCreateMeshInputRequestTypeDef = TypedDict(
     "_RequiredCreateMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalCreateMeshInputRequestTypeDef = TypedDict(
@@ -3196,14 +2369,24 @@
 )
 
 class CreateMeshInputRequestTypeDef(
     _RequiredCreateMeshInputRequestTypeDef, _OptionalCreateMeshInputRequestTypeDef
 ):
     pass
 
+MeshDataTypeDef = TypedDict(
+    "MeshDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": MeshSpecTypeDef,
+        "status": MeshStatusTypeDef,
+    },
+)
+
 _RequiredUpdateMeshInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalUpdateMeshInputRequestTypeDef = TypedDict(
@@ -3219,15 +2402,15 @@
     _RequiredUpdateMeshInputRequestTypeDef, _OptionalUpdateMeshInputRequestTypeDef
 ):
     pass
 
 _RequiredListenerTlsValidationContextOutputTypeDef = TypedDict(
     "_RequiredListenerTlsValidationContextOutputTypeDef",
     {
-        "trust": ListenerTlsValidationContextTrustOutputTypeDef,
+        "trust": ListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalListenerTlsValidationContextOutputTypeDef = TypedDict(
     "_OptionalListenerTlsValidationContextOutputTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
     },
@@ -3296,15 +2479,15 @@
     _RequiredTlsValidationContextTypeDef, _OptionalTlsValidationContextTypeDef
 ):
     pass
 
 _RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef",
     {
-        "trust": VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
+        "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
     "_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
     },
@@ -3373,112 +2556,104 @@
 
 class VirtualGatewayTlsValidationContextTypeDef(
     _RequiredVirtualGatewayTlsValidationContextTypeDef,
     _OptionalVirtualGatewayTlsValidationContextTypeDef,
 ):
     pass
 
-VirtualServiceSpecOutputTypeDef = TypedDict(
-    "VirtualServiceSpecOutputTypeDef",
-    {
-        "provider": VirtualServiceProviderOutputTypeDef,
-    },
-    total=False,
-)
-
 VirtualServiceSpecTypeDef = TypedDict(
     "VirtualServiceSpecTypeDef",
     {
         "provider": VirtualServiceProviderTypeDef,
     },
     total=False,
 )
 
 GrpcGatewayRouteMatchOutputTypeDef = TypedDict(
     "GrpcGatewayRouteMatchOutputTypeDef",
     {
-        "hostname": GatewayRouteHostnameMatchOutputTypeDef,
-        "metadata": List[GrpcGatewayRouteMetadataOutputTypeDef],
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "metadata": List[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
-GrpcRouteMatchOutputTypeDef = TypedDict(
-    "GrpcRouteMatchOutputTypeDef",
+GrpcGatewayRouteMatchTypeDef = TypedDict(
+    "GrpcGatewayRouteMatchTypeDef",
     {
-        "metadata": List[GrpcRouteMetadataOutputTypeDef],
-        "methodName": str,
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
-HttpGatewayRouteMatchOutputTypeDef = TypedDict(
-    "HttpGatewayRouteMatchOutputTypeDef",
+GrpcRouteMatchOutputTypeDef = TypedDict(
+    "GrpcRouteMatchOutputTypeDef",
     {
-        "headers": List[HttpGatewayRouteHeaderOutputTypeDef],
-        "hostname": GatewayRouteHostnameMatchOutputTypeDef,
-        "method": HttpMethodType,
-        "path": HttpPathMatchOutputTypeDef,
+        "metadata": List[GrpcRouteMetadataTypeDef],
+        "methodName": str,
         "port": int,
-        "prefix": str,
-        "queryParameters": List[HttpQueryParameterOutputTypeDef],
+        "serviceName": str,
     },
     total=False,
 )
 
-HttpRouteMatchOutputTypeDef = TypedDict(
-    "HttpRouteMatchOutputTypeDef",
+GrpcRouteMatchTypeDef = TypedDict(
+    "GrpcRouteMatchTypeDef",
     {
-        "headers": List[HttpRouteHeaderOutputTypeDef],
-        "method": HttpMethodType,
-        "path": HttpPathMatchOutputTypeDef,
+        "metadata": Sequence[GrpcRouteMetadataTypeDef],
+        "methodName": str,
         "port": int,
-        "prefix": str,
-        "queryParameters": List[HttpQueryParameterOutputTypeDef],
-        "scheme": HttpSchemeType,
+        "serviceName": str,
     },
     total=False,
 )
 
-GrpcGatewayRouteMatchTypeDef = TypedDict(
-    "GrpcGatewayRouteMatchTypeDef",
+HttpGatewayRouteMatchOutputTypeDef = TypedDict(
+    "HttpGatewayRouteMatchOutputTypeDef",
     {
+        "headers": List[HttpGatewayRouteHeaderTypeDef],
         "hostname": GatewayRouteHostnameMatchTypeDef,
-        "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
+        "method": HttpMethodType,
+        "path": HttpPathMatchTypeDef,
         "port": int,
-        "serviceName": str,
+        "prefix": str,
+        "queryParameters": List[HttpQueryParameterTypeDef],
     },
     total=False,
 )
 
-GrpcRouteMatchTypeDef = TypedDict(
-    "GrpcRouteMatchTypeDef",
+HttpGatewayRouteMatchTypeDef = TypedDict(
+    "HttpGatewayRouteMatchTypeDef",
     {
-        "metadata": Sequence[GrpcRouteMetadataTypeDef],
-        "methodName": str,
+        "headers": Sequence[HttpGatewayRouteHeaderTypeDef],
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "method": HttpMethodType,
+        "path": HttpPathMatchTypeDef,
         "port": int,
-        "serviceName": str,
+        "prefix": str,
+        "queryParameters": Sequence[HttpQueryParameterTypeDef],
     },
     total=False,
 )
 
-HttpGatewayRouteMatchTypeDef = TypedDict(
-    "HttpGatewayRouteMatchTypeDef",
+HttpRouteMatchOutputTypeDef = TypedDict(
+    "HttpRouteMatchOutputTypeDef",
     {
-        "headers": Sequence[HttpGatewayRouteHeaderTypeDef],
-        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "headers": List[HttpRouteHeaderTypeDef],
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
-        "queryParameters": Sequence[HttpQueryParameterTypeDef],
+        "queryParameters": List[HttpQueryParameterTypeDef],
+        "scheme": HttpSchemeType,
     },
     total=False,
 )
 
 HttpRouteMatchTypeDef = TypedDict(
     "HttpRouteMatchTypeDef",
     {
@@ -3581,46 +2756,46 @@
 ):
     pass
 
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMeshOutputTypeDef = TypedDict(
     "DeleteMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMeshOutputTypeDef = TypedDict(
     "DescribeMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMeshOutputTypeDef = TypedDict(
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListenerTlsOutputTypeDef = TypedDict(
     "_RequiredListenerTlsOutputTypeDef",
     {
-        "certificate": ListenerTlsCertificateOutputTypeDef,
+        "certificate": ListenerTlsCertificateTypeDef,
         "mode": ListenerTlsModeType,
     },
 )
 _OptionalListenerTlsOutputTypeDef = TypedDict(
     "_OptionalListenerTlsOutputTypeDef",
     {
         "validation": ListenerTlsValidationContextOutputTypeDef,
@@ -3656,15 +2831,15 @@
     {
         "validation": TlsValidationContextOutputTypeDef,
     },
 )
 _OptionalClientPolicyTlsOutputTypeDef = TypedDict(
     "_OptionalClientPolicyTlsOutputTypeDef",
     {
-        "certificate": ClientTlsCertificateOutputTypeDef,
+        "certificate": ClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": List[int],
     },
     total=False,
 )
 
 class ClientPolicyTlsOutputTypeDef(
@@ -3690,15 +2865,15 @@
 
 class ClientPolicyTlsTypeDef(_RequiredClientPolicyTlsTypeDef, _OptionalClientPolicyTlsTypeDef):
     pass
 
 _RequiredVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsOutputTypeDef",
     {
-        "certificate": VirtualGatewayListenerTlsCertificateOutputTypeDef,
+        "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
         "mode": VirtualGatewayListenerTlsModeType,
     },
 )
 _OptionalVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
     "_OptionalVirtualGatewayListenerTlsOutputTypeDef",
     {
         "validation": VirtualGatewayListenerTlsValidationContextOutputTypeDef,
@@ -3736,15 +2911,15 @@
     {
         "validation": VirtualGatewayTlsValidationContextOutputTypeDef,
     },
 )
 _OptionalVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
     "_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef",
     {
-        "certificate": VirtualGatewayClientTlsCertificateOutputTypeDef,
+        "certificate": VirtualGatewayClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": List[int],
     },
     total=False,
 )
 
 class VirtualGatewayClientPolicyTlsOutputTypeDef(
@@ -3770,25 +2945,14 @@
 )
 
 class VirtualGatewayClientPolicyTlsTypeDef(
     _RequiredVirtualGatewayClientPolicyTlsTypeDef, _OptionalVirtualGatewayClientPolicyTlsTypeDef
 ):
     pass
 
-VirtualServiceDataTypeDef = TypedDict(
-    "VirtualServiceDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualServiceSpecOutputTypeDef,
-        "status": VirtualServiceStatusTypeDef,
-        "virtualServiceName": str,
-    },
-)
-
 _RequiredCreateVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualServiceSpecTypeDef,
         "virtualServiceName": str,
     },
@@ -3828,76 +2992,60 @@
 
 class UpdateVirtualServiceInputRequestTypeDef(
     _RequiredUpdateVirtualServiceInputRequestTypeDef,
     _OptionalUpdateVirtualServiceInputRequestTypeDef,
 ):
     pass
 
+VirtualServiceDataTypeDef = TypedDict(
+    "VirtualServiceDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualServiceSpecTypeDef,
+        "status": VirtualServiceStatusTypeDef,
+        "virtualServiceName": str,
+    },
+)
+
 GrpcGatewayRouteOutputTypeDef = TypedDict(
     "GrpcGatewayRouteOutputTypeDef",
     {
-        "action": GrpcGatewayRouteActionOutputTypeDef,
+        "action": GrpcGatewayRouteActionTypeDef,
         "match": GrpcGatewayRouteMatchOutputTypeDef,
     },
 )
 
+GrpcGatewayRouteTypeDef = TypedDict(
+    "GrpcGatewayRouteTypeDef",
+    {
+        "action": GrpcGatewayRouteActionTypeDef,
+        "match": GrpcGatewayRouteMatchTypeDef,
+    },
+)
+
 _RequiredGrpcRouteOutputTypeDef = TypedDict(
     "_RequiredGrpcRouteOutputTypeDef",
     {
         "action": GrpcRouteActionOutputTypeDef,
         "match": GrpcRouteMatchOutputTypeDef,
     },
 )
 _OptionalGrpcRouteOutputTypeDef = TypedDict(
     "_OptionalGrpcRouteOutputTypeDef",
     {
         "retryPolicy": GrpcRetryPolicyOutputTypeDef,
-        "timeout": GrpcTimeoutOutputTypeDef,
+        "timeout": GrpcTimeoutTypeDef,
     },
     total=False,
 )
 
 class GrpcRouteOutputTypeDef(_RequiredGrpcRouteOutputTypeDef, _OptionalGrpcRouteOutputTypeDef):
     pass
 
-HttpGatewayRouteOutputTypeDef = TypedDict(
-    "HttpGatewayRouteOutputTypeDef",
-    {
-        "action": HttpGatewayRouteActionOutputTypeDef,
-        "match": HttpGatewayRouteMatchOutputTypeDef,
-    },
-)
-
-_RequiredHttpRouteOutputTypeDef = TypedDict(
-    "_RequiredHttpRouteOutputTypeDef",
-    {
-        "action": HttpRouteActionOutputTypeDef,
-        "match": HttpRouteMatchOutputTypeDef,
-    },
-)
-_OptionalHttpRouteOutputTypeDef = TypedDict(
-    "_OptionalHttpRouteOutputTypeDef",
-    {
-        "retryPolicy": HttpRetryPolicyOutputTypeDef,
-        "timeout": HttpTimeoutOutputTypeDef,
-    },
-    total=False,
-)
-
-class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
-    pass
-
-GrpcGatewayRouteTypeDef = TypedDict(
-    "GrpcGatewayRouteTypeDef",
-    {
-        "action": GrpcGatewayRouteActionTypeDef,
-        "match": GrpcGatewayRouteMatchTypeDef,
-    },
-)
-
 _RequiredGrpcRouteTypeDef = TypedDict(
     "_RequiredGrpcRouteTypeDef",
     {
         "action": GrpcRouteActionTypeDef,
         "match": GrpcRouteMatchTypeDef,
     },
 )
@@ -3909,22 +3057,49 @@
     },
     total=False,
 )
 
 class GrpcRouteTypeDef(_RequiredGrpcRouteTypeDef, _OptionalGrpcRouteTypeDef):
     pass
 
+HttpGatewayRouteOutputTypeDef = TypedDict(
+    "HttpGatewayRouteOutputTypeDef",
+    {
+        "action": HttpGatewayRouteActionTypeDef,
+        "match": HttpGatewayRouteMatchOutputTypeDef,
+    },
+)
+
 HttpGatewayRouteTypeDef = TypedDict(
     "HttpGatewayRouteTypeDef",
     {
         "action": HttpGatewayRouteActionTypeDef,
         "match": HttpGatewayRouteMatchTypeDef,
     },
 )
 
+_RequiredHttpRouteOutputTypeDef = TypedDict(
+    "_RequiredHttpRouteOutputTypeDef",
+    {
+        "action": HttpRouteActionOutputTypeDef,
+        "match": HttpRouteMatchOutputTypeDef,
+    },
+)
+_OptionalHttpRouteOutputTypeDef = TypedDict(
+    "_OptionalHttpRouteOutputTypeDef",
+    {
+        "retryPolicy": HttpRetryPolicyOutputTypeDef,
+        "timeout": HttpTimeoutTypeDef,
+    },
+    total=False,
+)
+
+class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
+    pass
+
 _RequiredHttpRouteTypeDef = TypedDict(
     "_RequiredHttpRouteTypeDef",
     {
         "action": HttpRouteActionTypeDef,
         "match": HttpRouteMatchTypeDef,
     },
 )
@@ -3972,55 +3147,55 @@
     total=False,
 )
 
 CreateVirtualRouterOutputTypeDef = TypedDict(
     "CreateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualRouterOutputTypeDef = TypedDict(
     "DeleteVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualRouterOutputTypeDef = TypedDict(
     "DescribeVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualRouterOutputTypeDef = TypedDict(
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListenerOutputTypeDef = TypedDict(
     "_RequiredListenerOutputTypeDef",
     {
-        "portMapping": PortMappingOutputTypeDef,
+        "portMapping": PortMappingTypeDef,
     },
 )
 _OptionalListenerOutputTypeDef = TypedDict(
     "_OptionalListenerOutputTypeDef",
     {
-        "connectionPool": VirtualNodeConnectionPoolOutputTypeDef,
-        "healthCheck": HealthCheckPolicyOutputTypeDef,
-        "outlierDetection": OutlierDetectionOutputTypeDef,
-        "timeout": ListenerTimeoutOutputTypeDef,
+        "connectionPool": VirtualNodeConnectionPoolTypeDef,
+        "healthCheck": HealthCheckPolicyTypeDef,
+        "outlierDetection": OutlierDetectionTypeDef,
+        "timeout": ListenerTimeoutTypeDef,
         "tls": ListenerTlsOutputTypeDef,
     },
     total=False,
 )
 
 class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
     pass
@@ -4061,22 +3236,22 @@
     },
     total=False,
 )
 
 _RequiredVirtualGatewayListenerOutputTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerOutputTypeDef",
     {
-        "portMapping": VirtualGatewayPortMappingOutputTypeDef,
+        "portMapping": VirtualGatewayPortMappingTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerOutputTypeDef = TypedDict(
     "_OptionalVirtualGatewayListenerOutputTypeDef",
     {
-        "connectionPool": VirtualGatewayConnectionPoolOutputTypeDef,
-        "healthCheck": VirtualGatewayHealthCheckPolicyOutputTypeDef,
+        "connectionPool": VirtualGatewayConnectionPoolTypeDef,
+        "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
         "tls": VirtualGatewayListenerTlsOutputTypeDef,
     },
     total=False,
 )
 
 class VirtualGatewayListenerOutputTypeDef(
     _RequiredVirtualGatewayListenerOutputTypeDef, _OptionalVirtualGatewayListenerOutputTypeDef
@@ -4120,72 +3295,72 @@
     total=False,
 )
 
 CreateVirtualServiceOutputTypeDef = TypedDict(
     "CreateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualServiceOutputTypeDef = TypedDict(
     "DeleteVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualServiceOutputTypeDef = TypedDict(
     "DescribeVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualServiceOutputTypeDef = TypedDict(
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GatewayRouteSpecOutputTypeDef = TypedDict(
     "GatewayRouteSpecOutputTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteOutputTypeDef,
         "http2Route": HttpGatewayRouteOutputTypeDef,
         "httpRoute": HttpGatewayRouteOutputTypeDef,
         "priority": int,
     },
     total=False,
 )
 
-RouteSpecOutputTypeDef = TypedDict(
-    "RouteSpecOutputTypeDef",
+GatewayRouteSpecTypeDef = TypedDict(
+    "GatewayRouteSpecTypeDef",
     {
-        "grpcRoute": GrpcRouteOutputTypeDef,
-        "http2Route": HttpRouteOutputTypeDef,
-        "httpRoute": HttpRouteOutputTypeDef,
+        "grpcRoute": GrpcGatewayRouteTypeDef,
+        "http2Route": HttpGatewayRouteTypeDef,
+        "httpRoute": HttpGatewayRouteTypeDef,
         "priority": int,
-        "tcpRoute": TcpRouteOutputTypeDef,
     },
     total=False,
 )
 
-GatewayRouteSpecTypeDef = TypedDict(
-    "GatewayRouteSpecTypeDef",
+RouteSpecOutputTypeDef = TypedDict(
+    "RouteSpecOutputTypeDef",
     {
-        "grpcRoute": GrpcGatewayRouteTypeDef,
-        "http2Route": HttpGatewayRouteTypeDef,
-        "httpRoute": HttpGatewayRouteTypeDef,
+        "grpcRoute": GrpcRouteOutputTypeDef,
+        "http2Route": HttpRouteOutputTypeDef,
+        "httpRoute": HttpRouteOutputTypeDef,
         "priority": int,
+        "tcpRoute": TcpRouteOutputTypeDef,
     },
     total=False,
 )
 
 RouteSpecTypeDef = TypedDict(
     "RouteSpecTypeDef",
     {
@@ -4276,26 +3451,14 @@
         "metadata": ResourceMetadataTypeDef,
         "spec": GatewayRouteSpecOutputTypeDef,
         "status": GatewayRouteStatusTypeDef,
         "virtualGatewayName": str,
     },
 )
 
-RouteDataTypeDef = TypedDict(
-    "RouteDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "routeName": str,
-        "spec": RouteSpecOutputTypeDef,
-        "status": RouteStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
 _RequiredCreateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -4335,14 +3498,26 @@
 )
 
 class UpdateGatewayRouteInputRequestTypeDef(
     _RequiredUpdateGatewayRouteInputRequestTypeDef, _OptionalUpdateGatewayRouteInputRequestTypeDef
 ):
     pass
 
+RouteDataTypeDef = TypedDict(
+    "RouteDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "routeName": str,
+        "spec": RouteSpecOutputTypeDef,
+        "status": RouteStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredCreateRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -4442,71 +3617,71 @@
 ):
     pass
 
 CreateGatewayRouteOutputTypeDef = TypedDict(
     "CreateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGatewayRouteOutputTypeDef = TypedDict(
     "DeleteGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGatewayRouteOutputTypeDef = TypedDict(
     "DescribeGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGatewayRouteOutputTypeDef = TypedDict(
     "UpdateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteOutputTypeDef = TypedDict(
     "CreateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRouteOutputTypeDef = TypedDict(
     "DeleteRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRouteOutputTypeDef = TypedDict(
     "DescribeRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteOutputTypeDef = TypedDict(
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualNodeSpecOutputTypeDef = TypedDict(
     "VirtualNodeSpecOutputTypeDef",
     {
         "backendDefaults": BackendDefaultsOutputTypeDef,
@@ -4644,66 +3819,66 @@
 ):
     pass
 
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualGatewayOutputTypeDef = TypedDict(
     "DeleteVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualGatewayOutputTypeDef = TypedDict(
     "DescribeVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualGatewayOutputTypeDef = TypedDict(
     "UpdateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVirtualNodeOutputTypeDef = TypedDict(
     "CreateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualNodeOutputTypeDef = TypedDict(
     "DeleteVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualNodeOutputTypeDef = TypedDict(
     "DescribeVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualNodeOutputTypeDef = TypedDict(
     "UpdateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/PKG-INFO` & `mypy-boto3-appmesh-1.28.15/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-appmesh
-Version: 1.28.12
-Summary: Type annotations for boto3.AppMesh 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 appmesh type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="mypy-boto3-appmesh"></a>
 
 # mypy-boto3-appmesh
 
 [![PyPI - mypy-boto3-appmesh](https://img.shields.io/pypi/v/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-appmesh.svg?color=blue)](https://pypi.org/project/mypy-boto3-appmesh)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-appmesh)](https://pepy.tech/project/mypy-boto3-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.AppMesh 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
+[boto3.AppMesh 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [mypy-boto3-appmesh docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_appmesh/).
 
 See how it helps to find and fix potential bugs:
 
@@ -371,265 +339,195 @@
 ### Typed dictionaries
 
 `mypy_boto3_appmesh.type_defs` module contains structures and shapes assembled
 to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_appmesh.type_defs import (
-    AwsCloudMapInstanceAttributeOutputTypeDef,
     AwsCloudMapInstanceAttributeTypeDef,
-    ListenerTlsFileCertificateOutputTypeDef,
-    ListenerTlsSdsCertificateOutputTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
     DescribeGatewayRouteInputRequestTypeDef,
     DescribeMeshInputRequestTypeDef,
     DescribeRouteInputRequestTypeDef,
     DescribeVirtualGatewayInputRequestTypeDef,
     DescribeVirtualNodeInputRequestTypeDef,
     DescribeVirtualRouterInputRequestTypeDef,
     DescribeVirtualServiceInputRequestTypeDef,
-    DnsServiceDiscoveryOutputTypeDef,
     DnsServiceDiscoveryTypeDef,
-    DurationOutputTypeDef,
     DurationTypeDef,
-    EgressFilterOutputTypeDef,
     EgressFilterTypeDef,
     GatewayRouteStatusTypeDef,
     ResourceMetadataTypeDef,
-    GatewayRouteHostnameMatchOutputTypeDef,
     GatewayRouteHostnameMatchTypeDef,
-    GatewayRouteHostnameRewriteOutputTypeDef,
     GatewayRouteHostnameRewriteTypeDef,
     GatewayRouteRefTypeDef,
-    GatewayRouteVirtualServiceOutputTypeDef,
     GatewayRouteVirtualServiceTypeDef,
-    MatchRangeOutputTypeDef,
     MatchRangeTypeDef,
-    WeightedTargetOutputTypeDef,
     WeightedTargetTypeDef,
-    HealthCheckPolicyOutputTypeDef,
     HealthCheckPolicyTypeDef,
-    HttpPathMatchOutputTypeDef,
     HttpPathMatchTypeDef,
-    HttpGatewayRoutePathRewriteOutputTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
-    HttpGatewayRoutePrefixRewriteOutputTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
-    QueryParameterMatchOutputTypeDef,
     QueryParameterMatchTypeDef,
-    JsonFormatRefOutputTypeDef,
     JsonFormatRefTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    TagRefOutputTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
-    PortMappingOutputTypeDef,
-    ListenerTlsAcmCertificateOutputTypeDef,
+    PortMappingTypeDef,
     ListenerTlsAcmCertificateTypeDef,
-    TlsValidationContextFileTrustOutputTypeDef,
-    TlsValidationContextSdsTrustOutputTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
-    PortMappingTypeDef,
     MeshStatusTypeDef,
-    MeshServiceDiscoveryOutputTypeDef,
     MeshServiceDiscoveryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
     SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
-    TcpRouteMatchOutputTypeDef,
     TcpRouteMatchTypeDef,
     TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
-    VirtualGatewayListenerTlsFileCertificateOutputTypeDef,
-    VirtualGatewayListenerTlsSdsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
-    VirtualGatewayGrpcConnectionPoolOutputTypeDef,
-    VirtualGatewayHttp2ConnectionPoolOutputTypeDef,
-    VirtualGatewayHttpConnectionPoolOutputTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
-    VirtualGatewayHealthCheckPolicyOutputTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
-    VirtualGatewayPortMappingOutputTypeDef,
-    VirtualGatewayListenerTlsAcmCertificateOutputTypeDef,
+    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
-    VirtualGatewayTlsValidationContextFileTrustOutputTypeDef,
-    VirtualGatewayTlsValidationContextSdsTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
-    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
-    VirtualNodeGrpcConnectionPoolOutputTypeDef,
-    VirtualNodeHttp2ConnectionPoolOutputTypeDef,
-    VirtualNodeHttpConnectionPoolOutputTypeDef,
-    VirtualNodeTcpConnectionPoolOutputTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
-    VirtualNodeServiceProviderOutputTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
-    VirtualRouterServiceProviderOutputTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
     AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
-    ClientTlsCertificateOutputTypeDef,
     ClientTlsCertificateTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
     GrpcRetryPolicyOutputTypeDef,
-    GrpcTimeoutOutputTypeDef,
-    HttpRetryPolicyOutputTypeDef,
-    HttpTimeoutOutputTypeDef,
-    OutlierDetectionOutputTypeDef,
-    TcpTimeoutOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
+    HttpRetryPolicyOutputTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
-    GrpcGatewayRouteRewriteOutputTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
-    GatewayRouteTargetOutputTypeDef,
     GatewayRouteTargetTypeDef,
-    GrpcMetadataMatchMethodOutputTypeDef,
-    GrpcRouteMetadataMatchMethodOutputTypeDef,
-    HeaderMatchMethodOutputTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
     GrpcRouteActionOutputTypeDef,
-    HttpRouteActionOutputTypeDef,
-    TcpRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
+    HttpRouteActionOutputTypeDef,
     HttpRouteActionTypeDef,
+    TcpRouteActionOutputTypeDef,
     TcpRouteActionTypeDef,
-    HttpGatewayRouteRewriteOutputTypeDef,
     HttpGatewayRouteRewriteTypeDef,
-    HttpQueryParameterOutputTypeDef,
     HttpQueryParameterTypeDef,
     LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
-    VirtualRouterListenerOutputTypeDef,
-    ListenerTlsCertificateOutputTypeDef,
+    VirtualRouterListenerTypeDef,
     ListenerTlsCertificateTypeDef,
-    ListenerTlsValidationContextTrustOutputTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
-    VirtualRouterListenerTypeDef,
-    MeshSpecOutputTypeDef,
     MeshSpecTypeDef,
     SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
     TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
-    VirtualGatewayClientTlsCertificateOutputTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
-    VirtualGatewayConnectionPoolOutputTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
-    VirtualGatewayListenerTlsCertificateOutputTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
-    VirtualGatewayListenerTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
-    VirtualNodeConnectionPoolOutputTypeDef,
     VirtualNodeConnectionPoolTypeDef,
-    VirtualServiceProviderOutputTypeDef,
     VirtualServiceProviderTypeDef,
     ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
-    ListenerTimeoutOutputTypeDef,
     ListenerTimeoutTypeDef,
-    GrpcGatewayRouteActionOutputTypeDef,
     GrpcGatewayRouteActionTypeDef,
-    GrpcGatewayRouteMetadataOutputTypeDef,
-    GrpcRouteMetadataOutputTypeDef,
-    HttpGatewayRouteHeaderOutputTypeDef,
-    HttpRouteHeaderOutputTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
     TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
-    HttpGatewayRouteActionOutputTypeDef,
     HttpGatewayRouteActionTypeDef,
     FileAccessLogOutputTypeDef,
     VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
     VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
-    MeshDataTypeDef,
     CreateMeshInputRequestTypeDef,
+    MeshDataTypeDef,
     UpdateMeshInputRequestTypeDef,
     ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
     TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
     VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
     VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
-    VirtualServiceSpecOutputTypeDef,
     VirtualServiceSpecTypeDef,
     GrpcGatewayRouteMatchOutputTypeDef,
-    GrpcRouteMatchOutputTypeDef,
-    HttpGatewayRouteMatchOutputTypeDef,
-    HttpRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
+    GrpcRouteMatchOutputTypeDef,
     GrpcRouteMatchTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
     HttpGatewayRouteMatchTypeDef,
+    HttpRouteMatchOutputTypeDef,
     HttpRouteMatchTypeDef,
     AccessLogOutputTypeDef,
     VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
     VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
@@ -642,24 +540,24 @@
     ListenerTlsTypeDef,
     ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
     VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
     VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
-    VirtualServiceDataTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
+    VirtualServiceDataTypeDef,
     GrpcGatewayRouteOutputTypeDef,
-    GrpcRouteOutputTypeDef,
-    HttpGatewayRouteOutputTypeDef,
-    HttpRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
+    GrpcRouteOutputTypeDef,
     GrpcRouteTypeDef,
+    HttpGatewayRouteOutputTypeDef,
     HttpGatewayRouteTypeDef,
+    HttpRouteOutputTypeDef,
     HttpRouteTypeDef,
     LoggingOutputTypeDef,
     VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
@@ -674,27 +572,27 @@
     VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
     GatewayRouteSpecOutputTypeDef,
-    RouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
+    RouteSpecOutputTypeDef,
     RouteSpecTypeDef,
     BackendDefaultsOutputTypeDef,
     VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
     VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
     GatewayRouteDataTypeDef,
-    RouteDataTypeDef,
     CreateGatewayRouteInputRequestTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
+    RouteDataTypeDef,
     CreateRouteInputRequestTypeDef,
     UpdateRouteInputRequestTypeDef,
     BackendOutputTypeDef,
     BackendTypeDef,
     VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
@@ -720,15 +618,15 @@
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeOutputTypeDef:
+def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-appmesh-1.28.12/mypy_boto3_appmesh.egg-info/SOURCES.txt` & `mypy-boto3-appmesh-1.28.15/mypy_boto3_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-appmesh-1.28.12/setup.py` & `mypy-boto3-appmesh-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-appmesh",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.AppMesh 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.AppMesh 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

