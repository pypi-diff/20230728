# Comparing `tmp/mypy-boto3-route53-1.28.12.tar.gz` & `tmp/mypy-boto3-route53-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-route53-1.28.12.tar", last modified: Thu Jul 27 05:44:17 2023, max compression
+gzip compressed data, was "mypy-boto3-route53-1.28.15.tar", last modified: Fri Jul 28 20:43:36 2023, max compression
```

## Comparing `mypy-boto3-route53-1.28.12.tar` & `mypy-boto3-route53-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21404 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/mypy_boto3_route53/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55295 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    55209 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    64627 2023-07-27 05:44:08.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    64556 2023-07-27 05:44:07.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-27 05:44:17.000000 mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:44:17.375381 mypy-boto3-route53-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-27 05:44:06.000000 mypy-boto3-route53-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22649 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21162 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/mypy_boto3_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55295 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55209 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13092 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13090 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63068 2023-07-28 20:37:13.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62997 2023-07-28 20:37:13.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-28 20:37:08.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22649 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-28 20:43:35.000000 mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:36.161760 mypy-boto3-route53-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-07-28 20:37:07.000000 mypy-boto3-route53-1.28.15/setup.py
```

### Comparing `mypy-boto3-route53-1.28.12/LICENSE` & `mypy-boto3-route53-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/PKG-INFO` & `mypy-boto3-route53-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,31 +396,27 @@
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
     ResponseMetadataTypeDef,
-    AlarmIdentifierOutputTypeDef,
     AlarmIdentifierTypeDef,
-    AliasTargetOutputTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
-    CidrRoutingConfigOutputTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
     HostedZoneConfigTypeDef,
     DelegationSetTypeDef,
-    VPCOutputTypeDef,
     CreateKeySigningKeyRequestRequestTypeDef,
     KeySigningKeyTypeDef,
     CreateQueryLoggingConfigRequestRequestTypeDef,
     QueryLoggingConfigTypeDef,
     CreateReusableDelegationSetRequestRequestTypeDef,
     CreateTrafficPolicyInstanceRequestRequestTypeDef,
     TrafficPolicyInstanceTypeDef,
@@ -436,15 +432,14 @@
     DeleteQueryLoggingConfigRequestRequestTypeDef,
     DeleteReusableDelegationSetRequestRequestTypeDef,
     DeleteTrafficPolicyInstanceRequestRequestTypeDef,
     DeleteTrafficPolicyRequestRequestTypeDef,
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
-    GeoLocationOutputTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
@@ -457,15 +452,14 @@
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
-    HostedZoneConfigOutputTypeDef,
     HostedZoneOwnerTypeDef,
     PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
@@ -481,17 +475,15 @@
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    ResourceRecordOutputTypeDef,
     ResourceRecordTypeDef,
-    TagOutputTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
     ChangeCidrCollectionResponseTypeDef,
@@ -510,28 +502,29 @@
     GetTrafficPolicyInstanceCountResponseTypeDef,
     TestDNSAnswerResponseTypeDef,
     HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
+    CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
+    ListVPCAssociationAuthorizationsResponseTypeDef,
     ChangeCidrCollectionRequestRequestTypeDef,
     ChangeTagsForResourceRequestRequestTypeDef,
+    ResourceTagSetTypeDef,
     ListCidrBlocksResponseTypeDef,
     CreateCidrCollectionResponseTypeDef,
     CloudWatchAlarmConfigurationTypeDef,
     ListCidrCollectionsResponseTypeDef,
     CreateHostedZoneRequestRequestTypeDef,
     CreateReusableDelegationSetResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     ListReusableDelegationSetsResponseTypeDef,
-    CreateVPCAssociationAuthorizationResponseTypeDef,
-    ListVPCAssociationAuthorizationsResponseTypeDef,
     CreateKeySigningKeyResponseTypeDef,
     CreateQueryLoggingConfigResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     ListQueryLoggingConfigsResponseTypeDef,
     CreateTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     ListTrafficPolicyInstancesByHostedZoneResponseTypeDef,
@@ -560,29 +553,28 @@
     ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
     ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
-    ResourceTagSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
     ListResourceRecordSetsResponseTypeDef,
     ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-route53-1.28.12/README.md` & `mypy-boto3-route53-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -364,31 +364,27 @@
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
     ResponseMetadataTypeDef,
-    AlarmIdentifierOutputTypeDef,
     AlarmIdentifierTypeDef,
-    AliasTargetOutputTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
-    CidrRoutingConfigOutputTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
     HostedZoneConfigTypeDef,
     DelegationSetTypeDef,
-    VPCOutputTypeDef,
     CreateKeySigningKeyRequestRequestTypeDef,
     KeySigningKeyTypeDef,
     CreateQueryLoggingConfigRequestRequestTypeDef,
     QueryLoggingConfigTypeDef,
     CreateReusableDelegationSetRequestRequestTypeDef,
     CreateTrafficPolicyInstanceRequestRequestTypeDef,
     TrafficPolicyInstanceTypeDef,
@@ -404,15 +400,14 @@
     DeleteQueryLoggingConfigRequestRequestTypeDef,
     DeleteReusableDelegationSetRequestRequestTypeDef,
     DeleteTrafficPolicyInstanceRequestRequestTypeDef,
     DeleteTrafficPolicyRequestRequestTypeDef,
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
-    GeoLocationOutputTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
@@ -425,15 +420,14 @@
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
-    HostedZoneConfigOutputTypeDef,
     HostedZoneOwnerTypeDef,
     PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
@@ -449,17 +443,15 @@
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    ResourceRecordOutputTypeDef,
     ResourceRecordTypeDef,
-    TagOutputTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
     ChangeCidrCollectionResponseTypeDef,
@@ -478,28 +470,29 @@
     GetTrafficPolicyInstanceCountResponseTypeDef,
     TestDNSAnswerResponseTypeDef,
     HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
+    CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
+    ListVPCAssociationAuthorizationsResponseTypeDef,
     ChangeCidrCollectionRequestRequestTypeDef,
     ChangeTagsForResourceRequestRequestTypeDef,
+    ResourceTagSetTypeDef,
     ListCidrBlocksResponseTypeDef,
     CreateCidrCollectionResponseTypeDef,
     CloudWatchAlarmConfigurationTypeDef,
     ListCidrCollectionsResponseTypeDef,
     CreateHostedZoneRequestRequestTypeDef,
     CreateReusableDelegationSetResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     ListReusableDelegationSetsResponseTypeDef,
-    CreateVPCAssociationAuthorizationResponseTypeDef,
-    ListVPCAssociationAuthorizationsResponseTypeDef,
     CreateKeySigningKeyResponseTypeDef,
     CreateQueryLoggingConfigResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     ListQueryLoggingConfigsResponseTypeDef,
     CreateTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     ListTrafficPolicyInstancesByHostedZoneResponseTypeDef,
@@ -528,29 +521,28 @@
     ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
     ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
-    ResourceTagSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
     ListResourceRecordSetsResponseTypeDef,
     ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/__init__.py` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/__init__.pyi` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/__main__.py` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Route53 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Route53 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53\nOther"
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

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/client.py` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/client.pyi` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/literals.py` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/literals.pyi` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/paginator.py` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/paginator.pyi` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/type_defs.py` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,31 +46,27 @@
 
 
 __all__ = (
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
     "ResponseMetadataTypeDef",
-    "AlarmIdentifierOutputTypeDef",
     "AlarmIdentifierTypeDef",
-    "AliasTargetOutputTypeDef",
     "AliasTargetTypeDef",
     "VPCTypeDef",
     "CidrCollectionChangeTypeDef",
     "TagTypeDef",
     "CidrBlockSummaryTypeDef",
     "CidrCollectionTypeDef",
-    "CidrRoutingConfigOutputTypeDef",
     "CidrRoutingConfigTypeDef",
     "DimensionTypeDef",
     "CollectionSummaryTypeDef",
     "CreateCidrCollectionRequestRequestTypeDef",
     "HostedZoneConfigTypeDef",
     "DelegationSetTypeDef",
-    "VPCOutputTypeDef",
     "CreateKeySigningKeyRequestRequestTypeDef",
     "KeySigningKeyTypeDef",
     "CreateQueryLoggingConfigRequestRequestTypeDef",
     "QueryLoggingConfigTypeDef",
     "CreateReusableDelegationSetRequestRequestTypeDef",
     "CreateTrafficPolicyInstanceRequestRequestTypeDef",
     "TrafficPolicyInstanceTypeDef",
@@ -86,15 +82,14 @@
     "DeleteQueryLoggingConfigRequestRequestTypeDef",
     "DeleteReusableDelegationSetRequestRequestTypeDef",
     "DeleteTrafficPolicyInstanceRequestRequestTypeDef",
     "DeleteTrafficPolicyRequestRequestTypeDef",
     "DisableHostedZoneDNSSECRequestRequestTypeDef",
     "EnableHostedZoneDNSSECRequestRequestTypeDef",
     "GeoLocationDetailsTypeDef",
-    "GeoLocationOutputTypeDef",
     "GeoLocationTypeDef",
     "GetAccountLimitRequestRequestTypeDef",
     "GetChangeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDNSSECRequestRequestTypeDef",
     "GetGeoLocationRequestRequestTypeDef",
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
@@ -107,15 +102,14 @@
     "GetReusableDelegationSetLimitRequestRequestTypeDef",
     "ReusableDelegationSetLimitTypeDef",
     "GetReusableDelegationSetRequestRequestTypeDef",
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     "GetTrafficPolicyRequestRequestTypeDef",
     "StatusReportTypeDef",
     "LinkedServiceTypeDef",
-    "HostedZoneConfigOutputTypeDef",
     "HostedZoneOwnerTypeDef",
     "PaginatorConfigTypeDef",
     "ListCidrBlocksRequestRequestTypeDef",
     "ListCidrCollectionsRequestRequestTypeDef",
     "ListCidrLocationsRequestRequestTypeDef",
     "LocationSummaryTypeDef",
     "ListGeoLocationsRequestRequestTypeDef",
@@ -131,17 +125,15 @@
     "ListTrafficPoliciesRequestRequestTypeDef",
     "TrafficPolicySummaryTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef",
     "ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef",
     "ListTrafficPolicyInstancesRequestRequestTypeDef",
     "ListTrafficPolicyVersionsRequestRequestTypeDef",
     "ListVPCAssociationAuthorizationsRequestRequestTypeDef",
-    "ResourceRecordOutputTypeDef",
     "ResourceRecordTypeDef",
-    "TagOutputTypeDef",
     "TestDNSAnswerRequestRequestTypeDef",
     "UpdateHostedZoneCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyInstanceRequestRequestTypeDef",
     "ActivateKeySigningKeyResponseTypeDef",
     "AssociateVPCWithHostedZoneResponseTypeDef",
     "ChangeCidrCollectionResponseTypeDef",
@@ -160,28 +152,29 @@
     "GetTrafficPolicyInstanceCountResponseTypeDef",
     "TestDNSAnswerResponseTypeDef",
     "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
+    "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
+    "ListVPCAssociationAuthorizationsResponseTypeDef",
     "ChangeCidrCollectionRequestRequestTypeDef",
     "ChangeTagsForResourceRequestRequestTypeDef",
+    "ResourceTagSetTypeDef",
     "ListCidrBlocksResponseTypeDef",
     "CreateCidrCollectionResponseTypeDef",
     "CloudWatchAlarmConfigurationTypeDef",
     "ListCidrCollectionsResponseTypeDef",
     "CreateHostedZoneRequestRequestTypeDef",
     "CreateReusableDelegationSetResponseTypeDef",
     "GetReusableDelegationSetResponseTypeDef",
     "ListReusableDelegationSetsResponseTypeDef",
-    "CreateVPCAssociationAuthorizationResponseTypeDef",
-    "ListVPCAssociationAuthorizationsResponseTypeDef",
     "CreateKeySigningKeyResponseTypeDef",
     "CreateQueryLoggingConfigResponseTypeDef",
     "GetQueryLoggingConfigResponseTypeDef",
     "ListQueryLoggingConfigsResponseTypeDef",
     "CreateTrafficPolicyInstanceResponseTypeDef",
     "GetTrafficPolicyInstanceResponseTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
@@ -210,29 +203,28 @@
     "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
     "ResourceRecordSetOutputTypeDef",
     "ResourceRecordSetTypeDef",
-    "ResourceTagSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     "GetHealthCheckStatusResponseTypeDef",
     "CreateHostedZoneResponseTypeDef",
     "GetHostedZoneResponseTypeDef",
     "ListHostedZonesByNameResponseTypeDef",
     "ListHostedZonesResponseTypeDef",
     "UpdateHostedZoneCommentResponseTypeDef",
     "ListHostedZonesByVPCResponseTypeDef",
     "ListResourceRecordSetsResponseTypeDef",
     "ChangeTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTagsForResourcesResponseTypeDef",
     "CreateHealthCheckResponseTypeDef",
     "GetHealthCheckResponseTypeDef",
     "ListHealthChecksResponseTypeDef",
     "UpdateHealthCheckResponseTypeDef",
     "ChangeBatchTypeDef",
     "ChangeResourceRecordSetsRequestRequestTypeDef",
 )
@@ -281,39 +273,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-AlarmIdentifierOutputTypeDef = TypedDict(
-    "AlarmIdentifierOutputTypeDef",
-    {
-        "Region": CloudWatchRegionType,
-        "Name": str,
-    },
-)
-
 AlarmIdentifierTypeDef = TypedDict(
     "AlarmIdentifierTypeDef",
     {
         "Region": CloudWatchRegionType,
         "Name": str,
     },
 )
 
-AliasTargetOutputTypeDef = TypedDict(
-    "AliasTargetOutputTypeDef",
-    {
-        "HostedZoneId": str,
-        "DNSName": str,
-        "EvaluateTargetHealth": bool,
-    },
-)
-
 AliasTargetTypeDef = TypedDict(
     "AliasTargetTypeDef",
     {
         "HostedZoneId": str,
         "DNSName": str,
         "EvaluateTargetHealth": bool,
     },
@@ -362,22 +337,14 @@
         "Id": str,
         "Name": str,
         "Version": int,
     },
     total=False,
 )
 
-CidrRoutingConfigOutputTypeDef = TypedDict(
-    "CidrRoutingConfigOutputTypeDef",
-    {
-        "CollectionId": str,
-        "LocationName": str,
-    },
-)
-
 CidrRoutingConfigTypeDef = TypedDict(
     "CidrRoutingConfigTypeDef",
     {
         "CollectionId": str,
         "LocationName": str,
     },
 )
@@ -434,23 +401,14 @@
 )
 
 
 class DelegationSetTypeDef(_RequiredDelegationSetTypeDef, _OptionalDelegationSetTypeDef):
     pass
 
 
-VPCOutputTypeDef = TypedDict(
-    "VPCOutputTypeDef",
-    {
-        "VPCRegion": VPCRegionType,
-        "VPCId": str,
-    },
-    total=False,
-)
-
 CreateKeySigningKeyRequestRequestTypeDef = TypedDict(
     "CreateKeySigningKeyRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HostedZoneId": str,
         "KeyManagementServiceArn": str,
         "Name": str,
@@ -713,24 +671,14 @@
         "CountryName": str,
         "SubdivisionCode": str,
         "SubdivisionName": str,
     },
     total=False,
 )
 
-GeoLocationOutputTypeDef = TypedDict(
-    "GeoLocationOutputTypeDef",
-    {
-        "ContinentCode": str,
-        "CountryCode": str,
-        "SubdivisionCode": str,
-    },
-    total=False,
-)
-
 GeoLocationTypeDef = TypedDict(
     "GeoLocationTypeDef",
     {
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
@@ -880,23 +828,14 @@
     {
         "ServicePrincipal": str,
         "Description": str,
     },
     total=False,
 )
 
-HostedZoneConfigOutputTypeDef = TypedDict(
-    "HostedZoneConfigOutputTypeDef",
-    {
-        "Comment": str,
-        "PrivateZone": bool,
-    },
-    total=False,
-)
-
 HostedZoneOwnerTypeDef = TypedDict(
     "HostedZoneOwnerTypeDef",
     {
         "OwningAccount": str,
         "OwningService": str,
     },
     total=False,
@@ -1221,37 +1160,21 @@
 class ListVPCAssociationAuthorizationsRequestRequestTypeDef(
     _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef,
     _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef,
 ):
     pass
 
 
-ResourceRecordOutputTypeDef = TypedDict(
-    "ResourceRecordOutputTypeDef",
-    {
-        "Value": str,
-    },
-)
-
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "Value": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 _RequiredTestDNSAnswerRequestRequestTypeDef = TypedDict(
     "_RequiredTestDNSAnswerRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "RecordName": str,
         "RecordType": RRTypeType,
     },
@@ -1475,15 +1398,15 @@
         "MeasureLatency": bool,
         "Inverted": bool,
         "Disabled": bool,
         "HealthThreshold": int,
         "ChildHealthChecks": List[str],
         "EnableSNI": bool,
         "Regions": List[HealthCheckRegionType],
-        "AlarmIdentifier": AlarmIdentifierOutputTypeDef,
+        "AlarmIdentifier": AlarmIdentifierTypeDef,
         "InsufficientDataHealthStatus": InsufficientDataHealthStatusType,
         "RoutingControlArn": str,
     },
     total=False,
 )
 
 
@@ -1593,14 +1516,23 @@
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
     },
 )
 
+CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
+    "CreateVPCAssociationAuthorizationResponseTypeDef",
+    {
+        "HostedZoneId": str,
+        "VPC": VPCTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteVPCAssociationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
     },
 )
@@ -1624,14 +1556,24 @@
 class DisassociateVPCFromHostedZoneRequestRequestTypeDef(
     _RequiredDisassociateVPCFromHostedZoneRequestRequestTypeDef,
     _OptionalDisassociateVPCFromHostedZoneRequestRequestTypeDef,
 ):
     pass
 
 
+ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
+    "ListVPCAssociationAuthorizationsResponseTypeDef",
+    {
+        "HostedZoneId": str,
+        "NextToken": str,
+        "VPCs": List[VPCTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredChangeCidrCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredChangeCidrCollectionRequestRequestTypeDef",
     {
         "Id": str,
         "Changes": Sequence[CidrCollectionChangeTypeDef],
     },
 )
@@ -1671,14 +1613,24 @@
 class ChangeTagsForResourceRequestRequestTypeDef(
     _RequiredChangeTagsForResourceRequestRequestTypeDef,
     _OptionalChangeTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
+ResourceTagSetTypeDef = TypedDict(
+    "ResourceTagSetTypeDef",
+    {
+        "ResourceType": TagResourceTypeType,
+        "ResourceId": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 ListCidrBlocksResponseTypeDef = TypedDict(
     "ListCidrBlocksResponseTypeDef",
     {
         "NextToken": str,
         "CidrBlocks": List[CidrBlockSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1778,33 +1730,14 @@
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
-    "CreateVPCAssociationAuthorizationResponseTypeDef",
-    {
-        "HostedZoneId": str,
-        "VPC": VPCOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
-    "ListVPCAssociationAuthorizationsResponseTypeDef",
-    {
-        "HostedZoneId": str,
-        "NextToken": str,
-        "VPCs": List[VPCOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateKeySigningKeyResponseTypeDef = TypedDict(
     "CreateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
         "KeySigningKey": KeySigningKeyTypeDef,
         "Location": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -2032,15 +1965,15 @@
         "Name": str,
         "CallerReference": str,
     },
 )
 _OptionalHostedZoneTypeDef = TypedDict(
     "_OptionalHostedZoneTypeDef",
     {
-        "Config": HostedZoneConfigOutputTypeDef,
+        "Config": HostedZoneConfigTypeDef,
         "ResourceRecordSetCount": int,
         "LinkedService": LinkedServiceTypeDef,
     },
     total=False,
 )
 
 
@@ -2210,23 +2143,23 @@
 )
 _OptionalResourceRecordSetOutputTypeDef = TypedDict(
     "_OptionalResourceRecordSetOutputTypeDef",
     {
         "SetIdentifier": str,
         "Weight": int,
         "Region": ResourceRecordSetRegionType,
-        "GeoLocation": GeoLocationOutputTypeDef,
+        "GeoLocation": GeoLocationTypeDef,
         "Failover": ResourceRecordSetFailoverType,
         "MultiValueAnswer": bool,
         "TTL": int,
-        "ResourceRecords": List[ResourceRecordOutputTypeDef],
-        "AliasTarget": AliasTargetOutputTypeDef,
+        "ResourceRecords": List[ResourceRecordTypeDef],
+        "AliasTarget": AliasTargetTypeDef,
         "HealthCheckId": str,
         "TrafficPolicyInstanceId": str,
-        "CidrRoutingConfig": CidrRoutingConfigOutputTypeDef,
+        "CidrRoutingConfig": CidrRoutingConfigTypeDef,
     },
     total=False,
 )
 
 
 class ResourceRecordSetOutputTypeDef(
     _RequiredResourceRecordSetOutputTypeDef, _OptionalResourceRecordSetOutputTypeDef
@@ -2263,32 +2196,38 @@
 
 class ResourceRecordSetTypeDef(
     _RequiredResourceRecordSetTypeDef, _OptionalResourceRecordSetTypeDef
 ):
     pass
 
 
-ResourceTagSetTypeDef = TypedDict(
-    "ResourceTagSetTypeDef",
-    {
-        "ResourceType": TagResourceTypeType,
-        "ResourceId": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 CreateHealthCheckRequestRequestTypeDef = TypedDict(
     "CreateHealthCheckRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceTagSet": ResourceTagSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourcesResponseTypeDef = TypedDict(
+    "ListTagsForResourcesResponseTypeDef",
+    {
+        "ResourceTagSets": List[ResourceTagSetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
         "CallerReference": str,
         "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
         "HealthCheckVersion": int,
@@ -2326,26 +2265,26 @@
 
 CreateHostedZoneResponseTypeDef = TypedDict(
     "CreateHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "ChangeInfo": ChangeInfoTypeDef,
         "DelegationSet": DelegationSetTypeDef,
-        "VPC": VPCOutputTypeDef,
+        "VPC": VPCTypeDef,
         "Location": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHostedZoneResponseTypeDef = TypedDict(
     "GetHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "DelegationSet": DelegationSetTypeDef,
-        "VPCs": List[VPCOutputTypeDef],
+        "VPCs": List[VPCTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByNameResponseTypeDef = TypedDict(
     "ListHostedZonesByNameResponseTypeDef",
     {
@@ -2407,30 +2346,14 @@
     "ChangeTypeDef",
     {
         "Action": ChangeActionType,
         "ResourceRecordSet": ResourceRecordSetTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceTagSet": ResourceTagSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourcesResponseTypeDef = TypedDict(
-    "ListTagsForResourcesResponseTypeDef",
-    {
-        "ResourceTagSets": List[ResourceTagSetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/type_defs.pyi` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -45,31 +45,27 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
     "ResponseMetadataTypeDef",
-    "AlarmIdentifierOutputTypeDef",
     "AlarmIdentifierTypeDef",
-    "AliasTargetOutputTypeDef",
     "AliasTargetTypeDef",
     "VPCTypeDef",
     "CidrCollectionChangeTypeDef",
     "TagTypeDef",
     "CidrBlockSummaryTypeDef",
     "CidrCollectionTypeDef",
-    "CidrRoutingConfigOutputTypeDef",
     "CidrRoutingConfigTypeDef",
     "DimensionTypeDef",
     "CollectionSummaryTypeDef",
     "CreateCidrCollectionRequestRequestTypeDef",
     "HostedZoneConfigTypeDef",
     "DelegationSetTypeDef",
-    "VPCOutputTypeDef",
     "CreateKeySigningKeyRequestRequestTypeDef",
     "KeySigningKeyTypeDef",
     "CreateQueryLoggingConfigRequestRequestTypeDef",
     "QueryLoggingConfigTypeDef",
     "CreateReusableDelegationSetRequestRequestTypeDef",
     "CreateTrafficPolicyInstanceRequestRequestTypeDef",
     "TrafficPolicyInstanceTypeDef",
@@ -85,15 +81,14 @@
     "DeleteQueryLoggingConfigRequestRequestTypeDef",
     "DeleteReusableDelegationSetRequestRequestTypeDef",
     "DeleteTrafficPolicyInstanceRequestRequestTypeDef",
     "DeleteTrafficPolicyRequestRequestTypeDef",
     "DisableHostedZoneDNSSECRequestRequestTypeDef",
     "EnableHostedZoneDNSSECRequestRequestTypeDef",
     "GeoLocationDetailsTypeDef",
-    "GeoLocationOutputTypeDef",
     "GeoLocationTypeDef",
     "GetAccountLimitRequestRequestTypeDef",
     "GetChangeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "GetDNSSECRequestRequestTypeDef",
     "GetGeoLocationRequestRequestTypeDef",
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
@@ -106,15 +101,14 @@
     "GetReusableDelegationSetLimitRequestRequestTypeDef",
     "ReusableDelegationSetLimitTypeDef",
     "GetReusableDelegationSetRequestRequestTypeDef",
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     "GetTrafficPolicyRequestRequestTypeDef",
     "StatusReportTypeDef",
     "LinkedServiceTypeDef",
-    "HostedZoneConfigOutputTypeDef",
     "HostedZoneOwnerTypeDef",
     "PaginatorConfigTypeDef",
     "ListCidrBlocksRequestRequestTypeDef",
     "ListCidrCollectionsRequestRequestTypeDef",
     "ListCidrLocationsRequestRequestTypeDef",
     "LocationSummaryTypeDef",
     "ListGeoLocationsRequestRequestTypeDef",
@@ -130,17 +124,15 @@
     "ListTrafficPoliciesRequestRequestTypeDef",
     "TrafficPolicySummaryTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef",
     "ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef",
     "ListTrafficPolicyInstancesRequestRequestTypeDef",
     "ListTrafficPolicyVersionsRequestRequestTypeDef",
     "ListVPCAssociationAuthorizationsRequestRequestTypeDef",
-    "ResourceRecordOutputTypeDef",
     "ResourceRecordTypeDef",
-    "TagOutputTypeDef",
     "TestDNSAnswerRequestRequestTypeDef",
     "UpdateHostedZoneCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyInstanceRequestRequestTypeDef",
     "ActivateKeySigningKeyResponseTypeDef",
     "AssociateVPCWithHostedZoneResponseTypeDef",
     "ChangeCidrCollectionResponseTypeDef",
@@ -159,28 +151,29 @@
     "GetTrafficPolicyInstanceCountResponseTypeDef",
     "TestDNSAnswerResponseTypeDef",
     "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
+    "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
+    "ListVPCAssociationAuthorizationsResponseTypeDef",
     "ChangeCidrCollectionRequestRequestTypeDef",
     "ChangeTagsForResourceRequestRequestTypeDef",
+    "ResourceTagSetTypeDef",
     "ListCidrBlocksResponseTypeDef",
     "CreateCidrCollectionResponseTypeDef",
     "CloudWatchAlarmConfigurationTypeDef",
     "ListCidrCollectionsResponseTypeDef",
     "CreateHostedZoneRequestRequestTypeDef",
     "CreateReusableDelegationSetResponseTypeDef",
     "GetReusableDelegationSetResponseTypeDef",
     "ListReusableDelegationSetsResponseTypeDef",
-    "CreateVPCAssociationAuthorizationResponseTypeDef",
-    "ListVPCAssociationAuthorizationsResponseTypeDef",
     "CreateKeySigningKeyResponseTypeDef",
     "CreateQueryLoggingConfigResponseTypeDef",
     "GetQueryLoggingConfigResponseTypeDef",
     "ListQueryLoggingConfigsResponseTypeDef",
     "CreateTrafficPolicyInstanceResponseTypeDef",
     "GetTrafficPolicyInstanceResponseTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
@@ -209,29 +202,28 @@
     "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
     "ResourceRecordSetOutputTypeDef",
     "ResourceRecordSetTypeDef",
-    "ResourceTagSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     "GetHealthCheckStatusResponseTypeDef",
     "CreateHostedZoneResponseTypeDef",
     "GetHostedZoneResponseTypeDef",
     "ListHostedZonesByNameResponseTypeDef",
     "ListHostedZonesResponseTypeDef",
     "UpdateHostedZoneCommentResponseTypeDef",
     "ListHostedZonesByVPCResponseTypeDef",
     "ListResourceRecordSetsResponseTypeDef",
     "ChangeTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTagsForResourcesResponseTypeDef",
     "CreateHealthCheckResponseTypeDef",
     "GetHealthCheckResponseTypeDef",
     "ListHealthChecksResponseTypeDef",
     "UpdateHealthCheckResponseTypeDef",
     "ChangeBatchTypeDef",
     "ChangeResourceRecordSetsRequestRequestTypeDef",
 )
@@ -278,39 +270,22 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-AlarmIdentifierOutputTypeDef = TypedDict(
-    "AlarmIdentifierOutputTypeDef",
-    {
-        "Region": CloudWatchRegionType,
-        "Name": str,
-    },
-)
-
 AlarmIdentifierTypeDef = TypedDict(
     "AlarmIdentifierTypeDef",
     {
         "Region": CloudWatchRegionType,
         "Name": str,
     },
 )
 
-AliasTargetOutputTypeDef = TypedDict(
-    "AliasTargetOutputTypeDef",
-    {
-        "HostedZoneId": str,
-        "DNSName": str,
-        "EvaluateTargetHealth": bool,
-    },
-)
-
 AliasTargetTypeDef = TypedDict(
     "AliasTargetTypeDef",
     {
         "HostedZoneId": str,
         "DNSName": str,
         "EvaluateTargetHealth": bool,
     },
@@ -359,22 +334,14 @@
         "Id": str,
         "Name": str,
         "Version": int,
     },
     total=False,
 )
 
-CidrRoutingConfigOutputTypeDef = TypedDict(
-    "CidrRoutingConfigOutputTypeDef",
-    {
-        "CollectionId": str,
-        "LocationName": str,
-    },
-)
-
 CidrRoutingConfigTypeDef = TypedDict(
     "CidrRoutingConfigTypeDef",
     {
         "CollectionId": str,
         "LocationName": str,
     },
 )
@@ -429,23 +396,14 @@
     },
     total=False,
 )
 
 class DelegationSetTypeDef(_RequiredDelegationSetTypeDef, _OptionalDelegationSetTypeDef):
     pass
 
-VPCOutputTypeDef = TypedDict(
-    "VPCOutputTypeDef",
-    {
-        "VPCRegion": VPCRegionType,
-        "VPCId": str,
-    },
-    total=False,
-)
-
 CreateKeySigningKeyRequestRequestTypeDef = TypedDict(
     "CreateKeySigningKeyRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HostedZoneId": str,
         "KeyManagementServiceArn": str,
         "Name": str,
@@ -700,24 +658,14 @@
         "CountryName": str,
         "SubdivisionCode": str,
         "SubdivisionName": str,
     },
     total=False,
 )
 
-GeoLocationOutputTypeDef = TypedDict(
-    "GeoLocationOutputTypeDef",
-    {
-        "ContinentCode": str,
-        "CountryCode": str,
-        "SubdivisionCode": str,
-    },
-    total=False,
-)
-
 GeoLocationTypeDef = TypedDict(
     "GeoLocationTypeDef",
     {
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
@@ -867,23 +815,14 @@
     {
         "ServicePrincipal": str,
         "Description": str,
     },
     total=False,
 )
 
-HostedZoneConfigOutputTypeDef = TypedDict(
-    "HostedZoneConfigOutputTypeDef",
-    {
-        "Comment": str,
-        "PrivateZone": bool,
-    },
-    total=False,
-)
-
 HostedZoneOwnerTypeDef = TypedDict(
     "HostedZoneOwnerTypeDef",
     {
         "OwningAccount": str,
         "OwningService": str,
     },
     total=False,
@@ -1192,37 +1131,21 @@
 
 class ListVPCAssociationAuthorizationsRequestRequestTypeDef(
     _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef,
     _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef,
 ):
     pass
 
-ResourceRecordOutputTypeDef = TypedDict(
-    "ResourceRecordOutputTypeDef",
-    {
-        "Value": str,
-    },
-)
-
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "Value": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 _RequiredTestDNSAnswerRequestRequestTypeDef = TypedDict(
     "_RequiredTestDNSAnswerRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "RecordName": str,
         "RecordType": RRTypeType,
     },
@@ -1442,15 +1365,15 @@
         "MeasureLatency": bool,
         "Inverted": bool,
         "Disabled": bool,
         "HealthThreshold": int,
         "ChildHealthChecks": List[str],
         "EnableSNI": bool,
         "Regions": List[HealthCheckRegionType],
-        "AlarmIdentifier": AlarmIdentifierOutputTypeDef,
+        "AlarmIdentifier": AlarmIdentifierTypeDef,
         "InsufficientDataHealthStatus": InsufficientDataHealthStatusType,
         "RoutingControlArn": str,
     },
     total=False,
 )
 
 class HealthCheckConfigOutputTypeDef(
@@ -1552,14 +1475,23 @@
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
     },
 )
 
+CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
+    "CreateVPCAssociationAuthorizationResponseTypeDef",
+    {
+        "HostedZoneId": str,
+        "VPC": VPCTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeleteVPCAssociationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
     },
 )
@@ -1581,14 +1513,24 @@
 
 class DisassociateVPCFromHostedZoneRequestRequestTypeDef(
     _RequiredDisassociateVPCFromHostedZoneRequestRequestTypeDef,
     _OptionalDisassociateVPCFromHostedZoneRequestRequestTypeDef,
 ):
     pass
 
+ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
+    "ListVPCAssociationAuthorizationsResponseTypeDef",
+    {
+        "HostedZoneId": str,
+        "NextToken": str,
+        "VPCs": List[VPCTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredChangeCidrCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredChangeCidrCollectionRequestRequestTypeDef",
     {
         "Id": str,
         "Changes": Sequence[CidrCollectionChangeTypeDef],
     },
 )
@@ -1624,14 +1566,24 @@
 
 class ChangeTagsForResourceRequestRequestTypeDef(
     _RequiredChangeTagsForResourceRequestRequestTypeDef,
     _OptionalChangeTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+ResourceTagSetTypeDef = TypedDict(
+    "ResourceTagSetTypeDef",
+    {
+        "ResourceType": TagResourceTypeType,
+        "ResourceId": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 ListCidrBlocksResponseTypeDef = TypedDict(
     "ListCidrBlocksResponseTypeDef",
     {
         "NextToken": str,
         "CidrBlocks": List[CidrBlockSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1727,33 +1679,14 @@
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
-    "CreateVPCAssociationAuthorizationResponseTypeDef",
-    {
-        "HostedZoneId": str,
-        "VPC": VPCOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
-    "ListVPCAssociationAuthorizationsResponseTypeDef",
-    {
-        "HostedZoneId": str,
-        "NextToken": str,
-        "VPCs": List[VPCOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateKeySigningKeyResponseTypeDef = TypedDict(
     "CreateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
         "KeySigningKey": KeySigningKeyTypeDef,
         "Location": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1979,15 +1912,15 @@
         "Name": str,
         "CallerReference": str,
     },
 )
 _OptionalHostedZoneTypeDef = TypedDict(
     "_OptionalHostedZoneTypeDef",
     {
-        "Config": HostedZoneConfigOutputTypeDef,
+        "Config": HostedZoneConfigTypeDef,
         "ResourceRecordSetCount": int,
         "LinkedService": LinkedServiceTypeDef,
     },
     total=False,
 )
 
 class HostedZoneTypeDef(_RequiredHostedZoneTypeDef, _OptionalHostedZoneTypeDef):
@@ -2147,23 +2080,23 @@
 )
 _OptionalResourceRecordSetOutputTypeDef = TypedDict(
     "_OptionalResourceRecordSetOutputTypeDef",
     {
         "SetIdentifier": str,
         "Weight": int,
         "Region": ResourceRecordSetRegionType,
-        "GeoLocation": GeoLocationOutputTypeDef,
+        "GeoLocation": GeoLocationTypeDef,
         "Failover": ResourceRecordSetFailoverType,
         "MultiValueAnswer": bool,
         "TTL": int,
-        "ResourceRecords": List[ResourceRecordOutputTypeDef],
-        "AliasTarget": AliasTargetOutputTypeDef,
+        "ResourceRecords": List[ResourceRecordTypeDef],
+        "AliasTarget": AliasTargetTypeDef,
         "HealthCheckId": str,
         "TrafficPolicyInstanceId": str,
-        "CidrRoutingConfig": CidrRoutingConfigOutputTypeDef,
+        "CidrRoutingConfig": CidrRoutingConfigTypeDef,
     },
     total=False,
 )
 
 class ResourceRecordSetOutputTypeDef(
     _RequiredResourceRecordSetOutputTypeDef, _OptionalResourceRecordSetOutputTypeDef
 ):
@@ -2196,32 +2129,38 @@
 )
 
 class ResourceRecordSetTypeDef(
     _RequiredResourceRecordSetTypeDef, _OptionalResourceRecordSetTypeDef
 ):
     pass
 
-ResourceTagSetTypeDef = TypedDict(
-    "ResourceTagSetTypeDef",
-    {
-        "ResourceType": TagResourceTypeType,
-        "ResourceId": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 CreateHealthCheckRequestRequestTypeDef = TypedDict(
     "CreateHealthCheckRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
 )
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "ResourceTagSet": ResourceTagSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourcesResponseTypeDef = TypedDict(
+    "ListTagsForResourcesResponseTypeDef",
+    {
+        "ResourceTagSets": List[ResourceTagSetTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
         "CallerReference": str,
         "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
         "HealthCheckVersion": int,
@@ -2257,26 +2196,26 @@
 
 CreateHostedZoneResponseTypeDef = TypedDict(
     "CreateHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "ChangeInfo": ChangeInfoTypeDef,
         "DelegationSet": DelegationSetTypeDef,
-        "VPC": VPCOutputTypeDef,
+        "VPC": VPCTypeDef,
         "Location": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHostedZoneResponseTypeDef = TypedDict(
     "GetHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "DelegationSet": DelegationSetTypeDef,
-        "VPCs": List[VPCOutputTypeDef],
+        "VPCs": List[VPCTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByNameResponseTypeDef = TypedDict(
     "ListHostedZonesByNameResponseTypeDef",
     {
@@ -2338,30 +2277,14 @@
     "ChangeTypeDef",
     {
         "Action": ChangeActionType,
         "ResourceRecordSet": ResourceRecordSetTypeDef,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "ResourceTagSet": ResourceTagSetTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ListTagsForResourcesResponseTypeDef = TypedDict(
-    "ListTagsForResourcesResponseTypeDef",
-    {
-        "ResourceTagSets": List[ResourceTagSetTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/waiter.py` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53/waiter.pyi` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/PKG-INFO` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-route53
-Version: 1.28.12
-Summary: Type annotations for boto3.Route53 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-route53.svg?color=blue)](https://pypi.org/project/mypy-boto3-route53)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-route53)](https://pepy.tech/project/mypy-boto3-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Route53 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
+[boto3.Route53 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [mypy-boto3-route53 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -396,31 +396,27 @@
 
 ```python
 from mypy_boto3_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
     ResponseMetadataTypeDef,
-    AlarmIdentifierOutputTypeDef,
     AlarmIdentifierTypeDef,
-    AliasTargetOutputTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
-    CidrRoutingConfigOutputTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
     HostedZoneConfigTypeDef,
     DelegationSetTypeDef,
-    VPCOutputTypeDef,
     CreateKeySigningKeyRequestRequestTypeDef,
     KeySigningKeyTypeDef,
     CreateQueryLoggingConfigRequestRequestTypeDef,
     QueryLoggingConfigTypeDef,
     CreateReusableDelegationSetRequestRequestTypeDef,
     CreateTrafficPolicyInstanceRequestRequestTypeDef,
     TrafficPolicyInstanceTypeDef,
@@ -436,15 +432,14 @@
     DeleteQueryLoggingConfigRequestRequestTypeDef,
     DeleteReusableDelegationSetRequestRequestTypeDef,
     DeleteTrafficPolicyInstanceRequestRequestTypeDef,
     DeleteTrafficPolicyRequestRequestTypeDef,
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
-    GeoLocationOutputTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
@@ -457,15 +452,14 @@
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
-    HostedZoneConfigOutputTypeDef,
     HostedZoneOwnerTypeDef,
     PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
@@ -481,17 +475,15 @@
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    ResourceRecordOutputTypeDef,
     ResourceRecordTypeDef,
-    TagOutputTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
     ChangeCidrCollectionResponseTypeDef,
@@ -510,28 +502,29 @@
     GetTrafficPolicyInstanceCountResponseTypeDef,
     TestDNSAnswerResponseTypeDef,
     HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
+    CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
+    ListVPCAssociationAuthorizationsResponseTypeDef,
     ChangeCidrCollectionRequestRequestTypeDef,
     ChangeTagsForResourceRequestRequestTypeDef,
+    ResourceTagSetTypeDef,
     ListCidrBlocksResponseTypeDef,
     CreateCidrCollectionResponseTypeDef,
     CloudWatchAlarmConfigurationTypeDef,
     ListCidrCollectionsResponseTypeDef,
     CreateHostedZoneRequestRequestTypeDef,
     CreateReusableDelegationSetResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     ListReusableDelegationSetsResponseTypeDef,
-    CreateVPCAssociationAuthorizationResponseTypeDef,
-    ListVPCAssociationAuthorizationsResponseTypeDef,
     CreateKeySigningKeyResponseTypeDef,
     CreateQueryLoggingConfigResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     ListQueryLoggingConfigsResponseTypeDef,
     CreateTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     ListTrafficPolicyInstancesByHostedZoneResponseTypeDef,
@@ -560,29 +553,28 @@
     ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
     ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
-    ResourceTagSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
     ListResourceRecordSetsResponseTypeDef,
     ChangeTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTagsForResourcesResponseTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
```

### Comparing `mypy-boto3-route53-1.28.12/mypy_boto3_route53.egg-info/SOURCES.txt` & `mypy-boto3-route53-1.28.15/mypy_boto3_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-route53-1.28.12/setup.py` & `mypy-boto3-route53-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-route53",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_route53"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Route53 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Route53 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

