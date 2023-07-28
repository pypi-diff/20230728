# Comparing `tmp/mypy-boto3-opensearch-1.28.12.tar.gz` & `tmp/mypy-boto3-opensearch-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-opensearch-1.28.12.tar", last modified: Thu Jul 27 11:49:21 2023, max compression
+gzip compressed data, was "mypy-boto3-opensearch-1.28.15.tar", last modified: Fri Jul 28 20:43:24 2023, max compression
```

## Comparing `mypy-boto3-opensearch-1.28.12.tar` & `mypy-boto3-opensearch-1.28.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.837133 mypy-boto3-opensearch-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-27 11:49:21.837133 mypy-boto3-opensearch-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.829133 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41084 2023-07-27 11:40:56.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41023 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-27 11:40:56.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-27 11:40:56.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    74311 2023-07-27 11:40:58.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    74252 2023-07-27 11:40:57.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:21.837133 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21585 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-27 11:49:21.000000 mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:21.837133 mypy-boto3-opensearch-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 11:40:55.000000 mypy-boto3-opensearch-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19304 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41084 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41023 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15425 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:32:49.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    68707 2023-07-28 20:32:51.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68650 2023-07-28 20:32:50.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20810 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 20:43:23.000000 mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:24.149596 mypy-boto3-opensearch-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:32:48.000000 mypy-boto3-opensearch-1.28.15/setup.py
```

### Comparing `mypy-boto3-opensearch-1.28.12/LICENSE` & `mypy-boto3-opensearch-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.12/PKG-INFO` & `mypy-boto3-opensearch-1.28.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.28.12
-Summary: Type annotations for boto3.OpenSearchService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpenSearchService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,43 +338,37 @@
 ### Typed dictionaries
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
-    AWSDomainInformationOutputTypeDef,
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
-    DurationOutputTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
-    ColdStorageOptionsOutputTypeDef,
-    ZoneAwarenessConfigOutputTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
-    CognitoOptionsOutputTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
-    CrossClusterSearchConnectionPropertiesOutputTypeDef,
     CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
@@ -402,23 +396,16 @@
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
     DescribeReservedInstanceOfferingsRequestRequestTypeDef,
     DescribeReservedInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
-    DomainEndpointOptionsOutputTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
-    EBSOptionsOutputTypeDef,
-    EncryptionAtRestOptionsOutputTypeDef,
-    LogPublishingOptionOutputTypeDef,
-    NodeToNodeEncryptionOptionsOutputTypeDef,
-    SnapshotOptionsOutputTypeDef,
-    SoftwareUpdateOptionsOutputTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
@@ -428,153 +415,145 @@
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVersionsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
-    WindowStartTimeOutputTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
-    SAMLIdpOutputTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
-    DomainInformationContainerOutputTypeDef,
     DomainInformationContainerTypeDef,
     EmptyResponseMetadataTypeDef,
     GetUpgradeStatusResponseTypeDef,
     ListVersionsResponseTypeDef,
     PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
     AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
-    ClusterConfigOutputTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
-    ConnectionPropertiesOutputTypeDef,
     ConnectionPropertiesTypeDef,
+    DomainEndpointOptionsStatusTypeDef,
+    EBSOptionsStatusTypeDef,
+    EncryptionAtRestOptionsStatusTypeDef,
+    LogPublishingOptionsStatusTypeDef,
+    NodeToNodeEncryptionOptionsStatusTypeDef,
+    SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
-    DomainEndpointOptionsStatusTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
-    EBSOptionsStatusTypeDef,
-    EncryptionAtRestOptionsStatusTypeDef,
-    LogPublishingOptionsStatusTypeDef,
-    NodeToNodeEncryptionOptionsStatusTypeDef,
-    SnapshotOptionsStatusTypeDef,
-    SoftwareUpdateOptionsStatusTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
     ListScheduledActionsResponseTypeDef,
     UpdateScheduledActionResponseTypeDef,
-    ListTagsResponseTypeDef,
-    OffPeakWindowOutputTypeDef,
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
-    SAMLOptionsOutputTypeDef,
     SAMLOptionsInputTypeDef,
+    SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
     AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     OutboundConnectionTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
-    OffPeakWindowOptionsOutputTypeDef,
     OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
-    AdvancedSecurityOptionsTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
+    AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
-    AdvancedSecurityOptionsStatusTypeDef,
-    DomainStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
+    AdvancedSecurityOptionsStatusTypeDef,
+    DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationOutputTypeDef:
+def get_structure() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.12/README.md` & `mypy-boto3-opensearch-1.28.15/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,43 +306,37 @@
 ### Typed dictionaries
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
-    AWSDomainInformationOutputTypeDef,
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
-    DurationOutputTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
-    ColdStorageOptionsOutputTypeDef,
-    ZoneAwarenessConfigOutputTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
-    CognitoOptionsOutputTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
-    CrossClusterSearchConnectionPropertiesOutputTypeDef,
     CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
@@ -370,23 +364,16 @@
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
     DescribeReservedInstanceOfferingsRequestRequestTypeDef,
     DescribeReservedInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
-    DomainEndpointOptionsOutputTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
-    EBSOptionsOutputTypeDef,
-    EncryptionAtRestOptionsOutputTypeDef,
-    LogPublishingOptionOutputTypeDef,
-    NodeToNodeEncryptionOptionsOutputTypeDef,
-    SnapshotOptionsOutputTypeDef,
-    SoftwareUpdateOptionsOutputTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
@@ -396,153 +383,145 @@
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVersionsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
-    WindowStartTimeOutputTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
-    SAMLIdpOutputTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
-    DomainInformationContainerOutputTypeDef,
     DomainInformationContainerTypeDef,
     EmptyResponseMetadataTypeDef,
     GetUpgradeStatusResponseTypeDef,
     ListVersionsResponseTypeDef,
     PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
     AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
-    ClusterConfigOutputTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
-    ConnectionPropertiesOutputTypeDef,
     ConnectionPropertiesTypeDef,
+    DomainEndpointOptionsStatusTypeDef,
+    EBSOptionsStatusTypeDef,
+    EncryptionAtRestOptionsStatusTypeDef,
+    LogPublishingOptionsStatusTypeDef,
+    NodeToNodeEncryptionOptionsStatusTypeDef,
+    SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
-    DomainEndpointOptionsStatusTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
-    EBSOptionsStatusTypeDef,
-    EncryptionAtRestOptionsStatusTypeDef,
-    LogPublishingOptionsStatusTypeDef,
-    NodeToNodeEncryptionOptionsStatusTypeDef,
-    SnapshotOptionsStatusTypeDef,
-    SoftwareUpdateOptionsStatusTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
     ListScheduledActionsResponseTypeDef,
     UpdateScheduledActionResponseTypeDef,
-    ListTagsResponseTypeDef,
-    OffPeakWindowOutputTypeDef,
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
-    SAMLOptionsOutputTypeDef,
     SAMLOptionsInputTypeDef,
+    SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
     AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     OutboundConnectionTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
-    OffPeakWindowOptionsOutputTypeDef,
     OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
-    AdvancedSecurityOptionsTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
+    AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
-    AdvancedSecurityOptionsStatusTypeDef,
-    DomainStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
+    AdvancedSecurityOptionsStatusTypeDef,
+    DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationOutputTypeDef:
+def get_structure() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/__main__.py` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.OpenSearchService 1.28.12\nVersion:         1.28.12\nBuilder"
-        " version: 7.15.2\nDocs:           "
+        "Type annotations for boto3.OpenSearchService 1.28.15\nVersion:         1.28.15\nBuilder"
+        " version: 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService\nOther"
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

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/client.py` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/client.pyi` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/literals.py` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/literals.pyi` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/type_defs.py` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for opensearch service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opensearch.type_defs import AWSDomainInformationOutputTypeDef
+    from mypy_boto3_opensearch.type_defs import AWSDomainInformationTypeDef
 
-    data: AWSDomainInformationOutputTypeDef = {...}
+    data: AWSDomainInformationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -64,43 +64,37 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AWSDomainInformationOutputTypeDef",
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
-    "DurationOutputTypeDef",
     "DurationTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
     "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
-    "ColdStorageOptionsOutputTypeDef",
-    "ZoneAwarenessConfigOutputTypeDef",
     "ColdStorageOptionsTypeDef",
     "ZoneAwarenessConfigTypeDef",
-    "CognitoOptionsOutputTypeDef",
     "CognitoOptionsTypeDef",
     "CompatibleVersionsMapTypeDef",
-    "CrossClusterSearchConnectionPropertiesOutputTypeDef",
     "CrossClusterSearchConnectionPropertiesTypeDef",
     "DomainEndpointOptionsTypeDef",
     "EBSOptionsTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "LogPublishingOptionTypeDef",
     "NodeToNodeEncryptionOptionsTypeDef",
     "SnapshotOptionsTypeDef",
@@ -128,23 +122,16 @@
     "DescribeInstanceTypeLimitsRequestRequestTypeDef",
     "DescribePackagesFilterTypeDef",
     "DescribeReservedInstanceOfferingsRequestRequestTypeDef",
     "DescribeReservedInstancesRequestRequestTypeDef",
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
-    "DomainEndpointOptionsOutputTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
-    "EBSOptionsOutputTypeDef",
-    "EncryptionAtRestOptionsOutputTypeDef",
-    "LogPublishingOptionOutputTypeDef",
-    "NodeToNodeEncryptionOptionsOutputTypeDef",
-    "SnapshotOptionsOutputTypeDef",
-    "SoftwareUpdateOptionsOutputTypeDef",
     "VPCDerivedInfoTypeDef",
     "ValidationFailureTypeDef",
     "GetCompatibleVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
@@ -154,173 +141,143 @@
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListVersionsRequestRequestTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
-    "WindowStartTimeOutputTypeDef",
     "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
-    "SAMLIdpOutputTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
-    "DomainInformationContainerOutputTypeDef",
     "DomainInformationContainerTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetUpgradeStatusResponseTypeDef",
     "ListVersionsResponseTypeDef",
     "PurchaseReservedInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
     "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
-    "ClusterConfigOutputTypeDef",
     "ClusterConfigTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleVersionsResponseTypeDef",
-    "ConnectionPropertiesOutputTypeDef",
     "ConnectionPropertiesTypeDef",
+    "DomainEndpointOptionsStatusTypeDef",
+    "EBSOptionsStatusTypeDef",
+    "EncryptionAtRestOptionsStatusTypeDef",
+    "LogPublishingOptionsStatusTypeDef",
+    "NodeToNodeEncryptionOptionsStatusTypeDef",
+    "SnapshotOptionsStatusTypeDef",
+    "SoftwareUpdateOptionsStatusTypeDef",
     "CreateVpcEndpointRequestRequestTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
     "DescribeDomainNodesResponseTypeDef",
     "DescribeInboundConnectionsRequestRequestTypeDef",
     "DescribeOutboundConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
-    "DomainEndpointOptionsStatusTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
-    "EBSOptionsStatusTypeDef",
-    "EncryptionAtRestOptionsStatusTypeDef",
-    "LogPublishingOptionsStatusTypeDef",
-    "NodeToNodeEncryptionOptionsStatusTypeDef",
-    "SnapshotOptionsStatusTypeDef",
-    "SoftwareUpdateOptionsStatusTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "DryRunProgressStatusTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
     "InstanceLimitsTypeDef",
     "ListInstanceTypeDetailsResponseTypeDef",
     "ListScheduledActionsResponseTypeDef",
     "UpdateScheduledActionResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "OffPeakWindowOutputTypeDef",
     "OffPeakWindowTypeDef",
     "ReservedInstanceOfferingTypeDef",
     "ReservedInstanceTypeDef",
-    "SAMLOptionsOutputTypeDef",
     "SAMLOptionsInputTypeDef",
+    "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
     "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
+    "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
     "OutboundConnectionTypeDef",
-    "CreateOutboundConnectionRequestRequestTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
     "ListDomainsForPackageResponseTypeDef",
     "ListPackagesForDomainResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DeletePackageResponseTypeDef",
     "DescribePackagesResponseTypeDef",
     "UpdatePackageResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DescribeVpcEndpointsResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
-    "OffPeakWindowOptionsOutputTypeDef",
     "OffPeakWindowOptionsTypeDef",
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     "DescribeReservedInstancesResponseTypeDef",
-    "AdvancedSecurityOptionsTypeDef",
     "AdvancedSecurityOptionsInputTypeDef",
+    "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
-    "AdvancedSecurityOptionsStatusTypeDef",
-    "DomainStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
+    "AdvancedSecurityOptionsStatusTypeDef",
+    "DomainStatusTypeDef",
     "DescribeInstanceTypeLimitsResponseTypeDef",
     "DomainConfigTypeDef",
     "CreateDomainResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "DescribeDomainsResponseTypeDef",
     "DescribeDryRunProgressResponseTypeDef",
     "DescribeDomainConfigResponseTypeDef",
     "UpdateDomainConfigResponseTypeDef",
 )
 
-_RequiredAWSDomainInformationOutputTypeDef = TypedDict(
-    "_RequiredAWSDomainInformationOutputTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalAWSDomainInformationOutputTypeDef = TypedDict(
-    "_OptionalAWSDomainInformationOutputTypeDef",
-    {
-        "OwnerId": str,
-        "Region": str,
-    },
-    total=False,
-)
-
-
-class AWSDomainInformationOutputTypeDef(
-    _RequiredAWSDomainInformationOutputTypeDef, _OptionalAWSDomainInformationOutputTypeDef
-):
-    pass
-
-
 _RequiredAWSDomainInformationTypeDef = TypedDict(
     "_RequiredAWSDomainInformationTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalAWSDomainInformationTypeDef = TypedDict(
@@ -438,23 +395,14 @@
         "ActionType": ScheduledAutoTuneActionTypeType,
         "Action": str,
         "Severity": ScheduledAutoTuneSeverityTypeType,
     },
     total=False,
 )
 
-DurationOutputTypeDef = TypedDict(
-    "DurationOutputTypeDef",
-    {
-        "Value": int,
-        "Unit": Literal["HOURS"],
-    },
-    total=False,
-)
-
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "Value": int,
         "Unit": Literal["HOURS"],
     },
     total=False,
@@ -544,29 +492,14 @@
         "Status": str,
         "Description": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
-ColdStorageOptionsOutputTypeDef = TypedDict(
-    "ColdStorageOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-
-ZoneAwarenessConfigOutputTypeDef = TypedDict(
-    "ZoneAwarenessConfigOutputTypeDef",
-    {
-        "AvailabilityZoneCount": int,
-    },
-    total=False,
-)
-
 ColdStorageOptionsTypeDef = TypedDict(
     "ColdStorageOptionsTypeDef",
     {
         "Enabled": bool,
     },
 )
 
@@ -574,25 +507,14 @@
     "ZoneAwarenessConfigTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
     total=False,
 )
 
-CognitoOptionsOutputTypeDef = TypedDict(
-    "CognitoOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "UserPoolId": str,
-        "IdentityPoolId": str,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
 CognitoOptionsTypeDef = TypedDict(
     "CognitoOptionsTypeDef",
     {
         "Enabled": bool,
         "UserPoolId": str,
         "IdentityPoolId": str,
         "RoleArn": str,
@@ -605,22 +527,14 @@
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
 )
 
-CrossClusterSearchConnectionPropertiesOutputTypeDef = TypedDict(
-    "CrossClusterSearchConnectionPropertiesOutputTypeDef",
-    {
-        "SkipUnavailable": SkipUnavailableStatusType,
-    },
-    total=False,
-)
-
 CrossClusterSearchConnectionPropertiesTypeDef = TypedDict(
     "CrossClusterSearchConnectionPropertiesTypeDef",
     {
         "SkipUnavailable": SkipUnavailableStatusType,
     },
     total=False,
 )
@@ -973,26 +887,14 @@
     "DissociatePackageRequestRequestTypeDef",
     {
         "PackageID": str,
         "DomainName": str,
     },
 )
 
-DomainEndpointOptionsOutputTypeDef = TypedDict(
-    "DomainEndpointOptionsOutputTypeDef",
-    {
-        "EnforceHTTPS": bool,
-        "TLSSecurityPolicy": TLSSecurityPolicyType,
-        "CustomEndpointEnabled": bool,
-        "CustomEndpoint": str,
-        "CustomEndpointCertificateArn": str,
-    },
-    total=False,
-)
-
 DomainInfoTypeDef = TypedDict(
     "DomainInfoTypeDef",
     {
         "DomainName": str,
         "EngineType": EngineTypeType,
     },
     total=False,
@@ -1003,68 +905,14 @@
     {
         "ErrorType": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-EBSOptionsOutputTypeDef = TypedDict(
-    "EBSOptionsOutputTypeDef",
-    {
-        "EBSEnabled": bool,
-        "VolumeType": VolumeTypeType,
-        "VolumeSize": int,
-        "Iops": int,
-        "Throughput": int,
-    },
-    total=False,
-)
-
-EncryptionAtRestOptionsOutputTypeDef = TypedDict(
-    "EncryptionAtRestOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-LogPublishingOptionOutputTypeDef = TypedDict(
-    "LogPublishingOptionOutputTypeDef",
-    {
-        "CloudWatchLogsLogGroupArn": str,
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-NodeToNodeEncryptionOptionsOutputTypeDef = TypedDict(
-    "NodeToNodeEncryptionOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-SnapshotOptionsOutputTypeDef = TypedDict(
-    "SnapshotOptionsOutputTypeDef",
-    {
-        "AutomatedSnapshotStartHour": int,
-    },
-    total=False,
-)
-
-SoftwareUpdateOptionsOutputTypeDef = TypedDict(
-    "SoftwareUpdateOptionsOutputTypeDef",
-    {
-        "AutoSoftwareUpdateEnabled": bool,
-    },
-    total=False,
-)
-
 VPCDerivedInfoTypeDef = TypedDict(
     "VPCDerivedInfoTypeDef",
     {
         "VPCId": str,
         "SubnetIds": List[str],
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
@@ -1316,22 +1164,14 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ARN": str,
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
 ListVersionsRequestRequestTypeDef = TypedDict(
     "ListVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1385,22 +1225,14 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-WindowStartTimeOutputTypeDef = TypedDict(
-    "WindowStartTimeOutputTypeDef",
-    {
-        "Hours": int,
-        "Minutes": int,
-    },
-)
-
 WindowStartTimeTypeDef = TypedDict(
     "WindowStartTimeTypeDef",
     {
         "Hours": int,
         "Minutes": int,
     },
 )
@@ -1456,22 +1288,14 @@
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
 
-SAMLIdpOutputTypeDef = TypedDict(
-    "SAMLIdpOutputTypeDef",
-    {
-        "MetadataContent": str,
-        "EntityId": str,
-    },
-)
-
 SAMLIdpTypeDef = TypedDict(
     "SAMLIdpTypeDef",
     {
         "MetadataContent": str,
         "EntityId": str,
     },
 )
@@ -1563,22 +1387,14 @@
         "UpgradeStepStatus": UpgradeStatusType,
         "Issues": List[str],
         "ProgressPercent": float,
     },
     total=False,
 )
 
-DomainInformationContainerOutputTypeDef = TypedDict(
-    "DomainInformationContainerOutputTypeDef",
-    {
-        "AWSDomainInformation": AWSDomainInformationOutputTypeDef,
-    },
-    total=False,
-)
-
 DomainInformationContainerTypeDef = TypedDict(
     "DomainInformationContainerTypeDef",
     {
         "AWSDomainInformation": AWSDomainInformationTypeDef,
     },
     total=False,
 )
@@ -1646,14 +1462,22 @@
     "AddTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1675,15 +1499,15 @@
     total=False,
 )
 
 AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleOutputTypeDef",
     {
         "StartAt": datetime,
-        "Duration": DurationOutputTypeDef,
+        "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
     total=False,
 )
 
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
@@ -1742,33 +1566,14 @@
         "CompletedProperties": List[str],
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
     },
     total=False,
 )
 
-ClusterConfigOutputTypeDef = TypedDict(
-    "ClusterConfigOutputTypeDef",
-    {
-        "InstanceType": OpenSearchPartitionInstanceTypeType,
-        "InstanceCount": int,
-        "DedicatedMasterEnabled": bool,
-        "ZoneAwarenessEnabled": bool,
-        "ZoneAwarenessConfig": ZoneAwarenessConfigOutputTypeDef,
-        "DedicatedMasterType": OpenSearchPartitionInstanceTypeType,
-        "DedicatedMasterCount": int,
-        "WarmEnabled": bool,
-        "WarmType": OpenSearchWarmPartitionInstanceTypeType,
-        "WarmCount": int,
-        "ColdStorageOptions": ColdStorageOptionsOutputTypeDef,
-        "MultiAZWithStandbyEnabled": bool,
-    },
-    total=False,
-)
-
 ClusterConfigTypeDef = TypedDict(
     "ClusterConfigTypeDef",
     {
         "InstanceType": OpenSearchPartitionInstanceTypeType,
         "InstanceCount": int,
         "DedicatedMasterEnabled": bool,
         "ZoneAwarenessEnabled": bool,
@@ -1783,41 +1588,90 @@
     },
     total=False,
 )
 
 CognitoOptionsStatusTypeDef = TypedDict(
     "CognitoOptionsStatusTypeDef",
     {
-        "Options": CognitoOptionsOutputTypeDef,
+        "Options": CognitoOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 GetCompatibleVersionsResponseTypeDef = TypedDict(
     "GetCompatibleVersionsResponseTypeDef",
     {
         "CompatibleVersions": List[CompatibleVersionsMapTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConnectionPropertiesOutputTypeDef = TypedDict(
-    "ConnectionPropertiesOutputTypeDef",
+ConnectionPropertiesTypeDef = TypedDict(
+    "ConnectionPropertiesTypeDef",
     {
         "Endpoint": str,
-        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesOutputTypeDef,
+        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
     },
     total=False,
 )
 
-ConnectionPropertiesTypeDef = TypedDict(
-    "ConnectionPropertiesTypeDef",
+DomainEndpointOptionsStatusTypeDef = TypedDict(
+    "DomainEndpointOptionsStatusTypeDef",
     {
-        "Endpoint": str,
-        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
+        "Options": DomainEndpointOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+EBSOptionsStatusTypeDef = TypedDict(
+    "EBSOptionsStatusTypeDef",
+    {
+        "Options": EBSOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+EncryptionAtRestOptionsStatusTypeDef = TypedDict(
+    "EncryptionAtRestOptionsStatusTypeDef",
+    {
+        "Options": EncryptionAtRestOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+LogPublishingOptionsStatusTypeDef = TypedDict(
+    "LogPublishingOptionsStatusTypeDef",
+    {
+        "Options": Dict[LogTypeType, LogPublishingOptionTypeDef],
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
+NodeToNodeEncryptionOptionsStatusTypeDef = TypedDict(
+    "NodeToNodeEncryptionOptionsStatusTypeDef",
+    {
+        "Options": NodeToNodeEncryptionOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+SnapshotOptionsStatusTypeDef = TypedDict(
+    "SnapshotOptionsStatusTypeDef",
+    {
+        "Options": SnapshotOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+SoftwareUpdateOptionsStatusTypeDef = TypedDict(
+    "SoftwareUpdateOptionsStatusTypeDef",
+    {
+        "Options": SoftwareUpdateOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcEndpointRequestRequestTypeDef",
     {
@@ -1954,22 +1808,14 @@
         "Filters": Sequence[DescribePackagesFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DomainEndpointOptionsStatusTypeDef = TypedDict(
-    "DomainEndpointOptionsStatusTypeDef",
-    {
-        "Options": DomainEndpointOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2002,64 +1848,14 @@
         "LastUpdatedAt": datetime,
         "AvailablePackageVersion": str,
         "ErrorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-EBSOptionsStatusTypeDef = TypedDict(
-    "EBSOptionsStatusTypeDef",
-    {
-        "Options": EBSOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-EncryptionAtRestOptionsStatusTypeDef = TypedDict(
-    "EncryptionAtRestOptionsStatusTypeDef",
-    {
-        "Options": EncryptionAtRestOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-LogPublishingOptionsStatusTypeDef = TypedDict(
-    "LogPublishingOptionsStatusTypeDef",
-    {
-        "Options": Dict[LogTypeType, LogPublishingOptionOutputTypeDef],
-        "Status": OptionStatusTypeDef,
-    },
-    total=False,
-)
-
-NodeToNodeEncryptionOptionsStatusTypeDef = TypedDict(
-    "NodeToNodeEncryptionOptionsStatusTypeDef",
-    {
-        "Options": NodeToNodeEncryptionOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-SnapshotOptionsStatusTypeDef = TypedDict(
-    "SnapshotOptionsStatusTypeDef",
-    {
-        "Options": SnapshotOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-SoftwareUpdateOptionsStatusTypeDef = TypedDict(
-    "SoftwareUpdateOptionsStatusTypeDef",
-    {
-        "Options": SoftwareUpdateOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-    total=False,
-)
-
 VPCDerivedInfoStatusTypeDef = TypedDict(
     "VPCDerivedInfoStatusTypeDef",
     {
         "Options": VPCDerivedInfoTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -2141,30 +1937,14 @@
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-OffPeakWindowOutputTypeDef = TypedDict(
-    "OffPeakWindowOutputTypeDef",
-    {
-        "WindowStartTime": WindowStartTimeOutputTypeDef,
-    },
-    total=False,
-)
-
 OffPeakWindowTypeDef = TypedDict(
     "OffPeakWindowTypeDef",
     {
         "WindowStartTime": WindowStartTimeTypeDef,
     },
     total=False,
 )
@@ -2201,33 +1981,33 @@
         "State": str,
         "PaymentOption": ReservedInstancePaymentOptionType,
         "RecurringCharges": List[RecurringChargeTypeDef],
     },
     total=False,
 )
 
-SAMLOptionsOutputTypeDef = TypedDict(
-    "SAMLOptionsOutputTypeDef",
+SAMLOptionsInputTypeDef = TypedDict(
+    "SAMLOptionsInputTypeDef",
     {
         "Enabled": bool,
-        "Idp": SAMLIdpOutputTypeDef,
+        "Idp": SAMLIdpTypeDef,
+        "MasterUserName": str,
+        "MasterBackendRole": str,
         "SubjectKey": str,
         "RolesKey": str,
         "SessionTimeoutMinutes": int,
     },
     total=False,
 )
 
-SAMLOptionsInputTypeDef = TypedDict(
-    "SAMLOptionsInputTypeDef",
+SAMLOptionsOutputTypeDef = TypedDict(
+    "SAMLOptionsOutputTypeDef",
     {
         "Enabled": bool,
         "Idp": SAMLIdpTypeDef,
-        "MasterUserName": str,
-        "MasterBackendRole": str,
         "SubjectKey": str,
         "RolesKey": str,
         "SessionTimeoutMinutes": int,
     },
     total=False,
 )
 
@@ -2251,16 +2031,16 @@
     },
     total=False,
 )
 
 InboundConnectionTypeDef = TypedDict(
     "InboundConnectionTypeDef",
     {
-        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionId": str,
         "ConnectionStatus": InboundConnectionStatusTypeDef,
         "ConnectionMode": ConnectionModeType,
     },
     total=False,
 )
 
@@ -2332,47 +2112,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterConfigStatusTypeDef = TypedDict(
     "ClusterConfigStatusTypeDef",
     {
-        "Options": ClusterConfigOutputTypeDef,
+        "Options": ClusterConfigTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
-CreateOutboundConnectionResponseTypeDef = TypedDict(
-    "CreateOutboundConnectionResponseTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionId": str,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-OutboundConnectionTypeDef = TypedDict(
-    "OutboundConnectionTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
-        "ConnectionId": str,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
     {
         "LocalDomainInfo": DomainInformationContainerTypeDef,
         "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionAlias": str,
     },
@@ -2390,14 +2142,42 @@
 class CreateOutboundConnectionRequestRequestTypeDef(
     _RequiredCreateOutboundConnectionRequestRequestTypeDef,
     _OptionalCreateOutboundConnectionRequestRequestTypeDef,
 ):
     pass
 
 
+CreateOutboundConnectionResponseTypeDef = TypedDict(
+    "CreateOutboundConnectionResponseTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionId": str,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OutboundConnectionTypeDef = TypedDict(
+    "OutboundConnectionTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionId": str,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+    },
+    total=False,
+)
+
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2482,23 +2262,14 @@
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OffPeakWindowOptionsOutputTypeDef = TypedDict(
-    "OffPeakWindowOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "OffPeakWindow": OffPeakWindowOutputTypeDef,
-    },
-    total=False,
-)
-
 OffPeakWindowOptionsTypeDef = TypedDict(
     "OffPeakWindowOptionsTypeDef",
     {
         "Enabled": bool,
         "OffPeakWindow": OffPeakWindowTypeDef,
     },
     total=False,
@@ -2518,33 +2289,33 @@
     {
         "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdvancedSecurityOptionsTypeDef = TypedDict(
-    "AdvancedSecurityOptionsTypeDef",
+AdvancedSecurityOptionsInputTypeDef = TypedDict(
+    "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
-        "SAMLOptions": SAMLOptionsOutputTypeDef,
-        "AnonymousAuthDisableDate": datetime,
+        "MasterUserOptions": MasterUserOptionsTypeDef,
+        "SAMLOptions": SAMLOptionsInputTypeDef,
         "AnonymousAuthEnabled": bool,
     },
     total=False,
 )
 
-AdvancedSecurityOptionsInputTypeDef = TypedDict(
-    "AdvancedSecurityOptionsInputTypeDef",
+AdvancedSecurityOptionsTypeDef = TypedDict(
+    "AdvancedSecurityOptionsTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
-        "MasterUserOptions": MasterUserOptionsTypeDef,
-        "SAMLOptions": SAMLOptionsInputTypeDef,
+        "SAMLOptions": SAMLOptionsOutputTypeDef,
+        "AnonymousAuthDisableDate": datetime,
         "AnonymousAuthEnabled": bool,
     },
     total=False,
 )
 
 LimitsTypeDef = TypedDict(
     "LimitsTypeDef",
@@ -2632,72 +2403,20 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OffPeakWindowOptionsStatusTypeDef = TypedDict(
     "OffPeakWindowOptionsStatusTypeDef",
     {
-        "Options": OffPeakWindowOptionsOutputTypeDef,
+        "Options": OffPeakWindowOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
     total=False,
 )
 
-AdvancedSecurityOptionsStatusTypeDef = TypedDict(
-    "AdvancedSecurityOptionsStatusTypeDef",
-    {
-        "Options": AdvancedSecurityOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-_RequiredDomainStatusTypeDef = TypedDict(
-    "_RequiredDomainStatusTypeDef",
-    {
-        "DomainId": str,
-        "DomainName": str,
-        "ARN": str,
-        "ClusterConfig": ClusterConfigOutputTypeDef,
-    },
-)
-_OptionalDomainStatusTypeDef = TypedDict(
-    "_OptionalDomainStatusTypeDef",
-    {
-        "Created": bool,
-        "Deleted": bool,
-        "Endpoint": str,
-        "Endpoints": Dict[str, str],
-        "Processing": bool,
-        "UpgradeProcessing": bool,
-        "EngineVersion": str,
-        "EBSOptions": EBSOptionsOutputTypeDef,
-        "AccessPolicies": str,
-        "SnapshotOptions": SnapshotOptionsOutputTypeDef,
-        "VPCOptions": VPCDerivedInfoTypeDef,
-        "CognitoOptions": CognitoOptionsOutputTypeDef,
-        "EncryptionAtRestOptions": EncryptionAtRestOptionsOutputTypeDef,
-        "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsOutputTypeDef,
-        "AdvancedOptions": Dict[str, str],
-        "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionOutputTypeDef],
-        "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "DomainEndpointOptions": DomainEndpointOptionsOutputTypeDef,
-        "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
-        "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
-        "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "OffPeakWindowOptions": OffPeakWindowOptionsOutputTypeDef,
-        "SoftwareUpdateOptions": SoftwareUpdateOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
-    pass
-
-
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
@@ -2765,14 +2484,66 @@
 class UpdateDomainConfigRequestRequestTypeDef(
     _RequiredUpdateDomainConfigRequestRequestTypeDef,
     _OptionalUpdateDomainConfigRequestRequestTypeDef,
 ):
     pass
 
 
+AdvancedSecurityOptionsStatusTypeDef = TypedDict(
+    "AdvancedSecurityOptionsStatusTypeDef",
+    {
+        "Options": AdvancedSecurityOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+_RequiredDomainStatusTypeDef = TypedDict(
+    "_RequiredDomainStatusTypeDef",
+    {
+        "DomainId": str,
+        "DomainName": str,
+        "ARN": str,
+        "ClusterConfig": ClusterConfigTypeDef,
+    },
+)
+_OptionalDomainStatusTypeDef = TypedDict(
+    "_OptionalDomainStatusTypeDef",
+    {
+        "Created": bool,
+        "Deleted": bool,
+        "Endpoint": str,
+        "Endpoints": Dict[str, str],
+        "Processing": bool,
+        "UpgradeProcessing": bool,
+        "EngineVersion": str,
+        "EBSOptions": EBSOptionsTypeDef,
+        "AccessPolicies": str,
+        "SnapshotOptions": SnapshotOptionsTypeDef,
+        "VPCOptions": VPCDerivedInfoTypeDef,
+        "CognitoOptions": CognitoOptionsTypeDef,
+        "EncryptionAtRestOptions": EncryptionAtRestOptionsTypeDef,
+        "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsTypeDef,
+        "AdvancedOptions": Dict[str, str],
+        "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionTypeDef],
+        "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
+        "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
+        "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
+        "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
+        "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
+    pass
+
+
 DescribeInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch/type_defs.pyi` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for opensearch service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_opensearch.type_defs import AWSDomainInformationOutputTypeDef
+    from mypy_boto3_opensearch.type_defs import AWSDomainInformationTypeDef
 
-    data: AWSDomainInformationOutputTypeDef = {...}
+    data: AWSDomainInformationTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -63,43 +63,37 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AWSDomainInformationOutputTypeDef",
     "AWSDomainInformationTypeDef",
     "AcceptInboundConnectionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "OptionStatusTypeDef",
     "TagTypeDef",
     "AdditionalLimitTypeDef",
     "MasterUserOptionsTypeDef",
     "AssociatePackageRequestRequestTypeDef",
     "AuthorizeVpcEndpointAccessRequestRequestTypeDef",
     "AuthorizedPrincipalTypeDef",
     "ScheduledAutoTuneDetailsTypeDef",
-    "DurationOutputTypeDef",
     "DurationTypeDef",
     "AutoTuneOptionsOutputTypeDef",
     "AutoTuneStatusTypeDef",
     "AvailabilityZoneInfoTypeDef",
     "CancelServiceSoftwareUpdateRequestRequestTypeDef",
     "ServiceSoftwareOptionsTypeDef",
     "ChangeProgressDetailsTypeDef",
     "ChangeProgressStageTypeDef",
-    "ColdStorageOptionsOutputTypeDef",
-    "ZoneAwarenessConfigOutputTypeDef",
     "ColdStorageOptionsTypeDef",
     "ZoneAwarenessConfigTypeDef",
-    "CognitoOptionsOutputTypeDef",
     "CognitoOptionsTypeDef",
     "CompatibleVersionsMapTypeDef",
-    "CrossClusterSearchConnectionPropertiesOutputTypeDef",
     "CrossClusterSearchConnectionPropertiesTypeDef",
     "DomainEndpointOptionsTypeDef",
     "EBSOptionsTypeDef",
     "EncryptionAtRestOptionsTypeDef",
     "LogPublishingOptionTypeDef",
     "NodeToNodeEncryptionOptionsTypeDef",
     "SnapshotOptionsTypeDef",
@@ -127,23 +121,16 @@
     "DescribeInstanceTypeLimitsRequestRequestTypeDef",
     "DescribePackagesFilterTypeDef",
     "DescribeReservedInstanceOfferingsRequestRequestTypeDef",
     "DescribeReservedInstancesRequestRequestTypeDef",
     "DescribeVpcEndpointsRequestRequestTypeDef",
     "VpcEndpointErrorTypeDef",
     "DissociatePackageRequestRequestTypeDef",
-    "DomainEndpointOptionsOutputTypeDef",
     "DomainInfoTypeDef",
     "ErrorDetailsTypeDef",
-    "EBSOptionsOutputTypeDef",
-    "EncryptionAtRestOptionsOutputTypeDef",
-    "LogPublishingOptionOutputTypeDef",
-    "NodeToNodeEncryptionOptionsOutputTypeDef",
-    "SnapshotOptionsOutputTypeDef",
-    "SoftwareUpdateOptionsOutputTypeDef",
     "VPCDerivedInfoTypeDef",
     "ValidationFailureTypeDef",
     "GetCompatibleVersionsRequestRequestTypeDef",
     "GetPackageVersionHistoryRequestRequestTypeDef",
     "PackageVersionHistoryTypeDef",
     "GetUpgradeHistoryRequestRequestTypeDef",
     "GetUpgradeStatusRequestRequestTypeDef",
@@ -153,171 +140,143 @@
     "ListDomainNamesRequestRequestTypeDef",
     "ListDomainsForPackageRequestRequestTypeDef",
     "ListInstanceTypeDetailsRequestRequestTypeDef",
     "ListPackagesForDomainRequestRequestTypeDef",
     "ListScheduledActionsRequestRequestTypeDef",
     "ScheduledActionTypeDef",
     "ListTagsRequestRequestTypeDef",
-    "TagOutputTypeDef",
     "ListVersionsRequestRequestTypeDef",
     "ListVpcEndpointAccessRequestRequestTypeDef",
     "ListVpcEndpointsForDomainRequestRequestTypeDef",
     "ListVpcEndpointsRequestRequestTypeDef",
-    "WindowStartTimeOutputTypeDef",
     "WindowStartTimeTypeDef",
     "PurchaseReservedInstanceOfferingRequestRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectInboundConnectionRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
-    "SAMLIdpOutputTypeDef",
     "SAMLIdpTypeDef",
     "StartServiceSoftwareUpdateRequestRequestTypeDef",
     "StorageTypeLimitTypeDef",
     "UpdateScheduledActionRequestRequestTypeDef",
     "UpgradeDomainRequestRequestTypeDef",
     "UpgradeStepItemTypeDef",
-    "DomainInformationContainerOutputTypeDef",
     "DomainInformationContainerTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetUpgradeStatusResponseTypeDef",
     "ListVersionsResponseTypeDef",
     "PurchaseReservedInstanceOfferingResponseTypeDef",
     "AccessPoliciesStatusTypeDef",
     "AdvancedOptionsStatusTypeDef",
     "VersionStatusTypeDef",
     "AddTagsRequestRequestTypeDef",
+    "ListTagsResponseTypeDef",
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     "ListVpcEndpointAccessResponseTypeDef",
     "AutoTuneDetailsTypeDef",
     "AutoTuneMaintenanceScheduleOutputTypeDef",
     "AutoTuneMaintenanceScheduleTypeDef",
     "EnvironmentInfoTypeDef",
     "CancelServiceSoftwareUpdateResponseTypeDef",
     "StartServiceSoftwareUpdateResponseTypeDef",
     "UpgradeDomainResponseTypeDef",
     "ChangeProgressStatusDetailsTypeDef",
-    "ClusterConfigOutputTypeDef",
     "ClusterConfigTypeDef",
     "CognitoOptionsStatusTypeDef",
     "GetCompatibleVersionsResponseTypeDef",
-    "ConnectionPropertiesOutputTypeDef",
     "ConnectionPropertiesTypeDef",
+    "DomainEndpointOptionsStatusTypeDef",
+    "EBSOptionsStatusTypeDef",
+    "EncryptionAtRestOptionsStatusTypeDef",
+    "LogPublishingOptionsStatusTypeDef",
+    "NodeToNodeEncryptionOptionsStatusTypeDef",
+    "SnapshotOptionsStatusTypeDef",
+    "SoftwareUpdateOptionsStatusTypeDef",
     "CreateVpcEndpointRequestRequestTypeDef",
     "UpdateVpcEndpointRequestRequestTypeDef",
     "CreatePackageRequestRequestTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "DeleteVpcEndpointResponseTypeDef",
     "ListVpcEndpointsForDomainResponseTypeDef",
     "ListVpcEndpointsResponseTypeDef",
     "DescribeDomainNodesResponseTypeDef",
     "DescribeInboundConnectionsRequestRequestTypeDef",
     "DescribeOutboundConnectionsRequestRequestTypeDef",
     "DescribePackagesRequestRequestTypeDef",
-    "DomainEndpointOptionsStatusTypeDef",
     "ListDomainNamesResponseTypeDef",
     "DomainPackageDetailsTypeDef",
     "PackageDetailsTypeDef",
-    "EBSOptionsStatusTypeDef",
-    "EncryptionAtRestOptionsStatusTypeDef",
-    "LogPublishingOptionsStatusTypeDef",
-    "NodeToNodeEncryptionOptionsStatusTypeDef",
-    "SnapshotOptionsStatusTypeDef",
-    "SoftwareUpdateOptionsStatusTypeDef",
     "VPCDerivedInfoStatusTypeDef",
     "VpcEndpointTypeDef",
     "DryRunProgressStatusTypeDef",
     "GetPackageVersionHistoryResponseTypeDef",
     "InstanceLimitsTypeDef",
     "ListInstanceTypeDetailsResponseTypeDef",
     "ListScheduledActionsResponseTypeDef",
     "UpdateScheduledActionResponseTypeDef",
-    "ListTagsResponseTypeDef",
-    "OffPeakWindowOutputTypeDef",
     "OffPeakWindowTypeDef",
     "ReservedInstanceOfferingTypeDef",
     "ReservedInstanceTypeDef",
-    "SAMLOptionsOutputTypeDef",
     "SAMLOptionsInputTypeDef",
+    "SAMLOptionsOutputTypeDef",
     "StorageTypeTypeDef",
     "UpgradeHistoryTypeDef",
     "InboundConnectionTypeDef",
     "AutoTuneTypeDef",
     "AutoTuneOptionsExtraOutputTypeDef",
     "AutoTuneOptionsInputTypeDef",
     "AutoTuneOptionsTypeDef",
     "DescribeDomainHealthResponseTypeDef",
     "DescribeDomainChangeProgressResponseTypeDef",
     "ClusterConfigStatusTypeDef",
+    "CreateOutboundConnectionRequestRequestTypeDef",
     "CreateOutboundConnectionResponseTypeDef",
     "OutboundConnectionTypeDef",
-    "CreateOutboundConnectionRequestRequestTypeDef",
     "AssociatePackageResponseTypeDef",
     "DissociatePackageResponseTypeDef",
     "ListDomainsForPackageResponseTypeDef",
     "ListPackagesForDomainResponseTypeDef",
     "CreatePackageResponseTypeDef",
     "DeletePackageResponseTypeDef",
     "DescribePackagesResponseTypeDef",
     "UpdatePackageResponseTypeDef",
     "CreateVpcEndpointResponseTypeDef",
     "DescribeVpcEndpointsResponseTypeDef",
     "UpdateVpcEndpointResponseTypeDef",
-    "OffPeakWindowOptionsOutputTypeDef",
     "OffPeakWindowOptionsTypeDef",
     "DescribeReservedInstanceOfferingsResponseTypeDef",
     "DescribeReservedInstancesResponseTypeDef",
-    "AdvancedSecurityOptionsTypeDef",
     "AdvancedSecurityOptionsInputTypeDef",
+    "AdvancedSecurityOptionsTypeDef",
     "LimitsTypeDef",
     "GetUpgradeHistoryResponseTypeDef",
     "AcceptInboundConnectionResponseTypeDef",
     "DeleteInboundConnectionResponseTypeDef",
     "DescribeInboundConnectionsResponseTypeDef",
     "RejectInboundConnectionResponseTypeDef",
     "DescribeDomainAutoTunesResponseTypeDef",
     "AutoTuneOptionsStatusTypeDef",
     "DeleteOutboundConnectionResponseTypeDef",
     "DescribeOutboundConnectionsResponseTypeDef",
     "OffPeakWindowOptionsStatusTypeDef",
-    "AdvancedSecurityOptionsStatusTypeDef",
-    "DomainStatusTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateDomainConfigRequestRequestTypeDef",
+    "AdvancedSecurityOptionsStatusTypeDef",
+    "DomainStatusTypeDef",
     "DescribeInstanceTypeLimitsResponseTypeDef",
     "DomainConfigTypeDef",
     "CreateDomainResponseTypeDef",
     "DeleteDomainResponseTypeDef",
     "DescribeDomainResponseTypeDef",
     "DescribeDomainsResponseTypeDef",
     "DescribeDryRunProgressResponseTypeDef",
     "DescribeDomainConfigResponseTypeDef",
     "UpdateDomainConfigResponseTypeDef",
 )
 
-_RequiredAWSDomainInformationOutputTypeDef = TypedDict(
-    "_RequiredAWSDomainInformationOutputTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalAWSDomainInformationOutputTypeDef = TypedDict(
-    "_OptionalAWSDomainInformationOutputTypeDef",
-    {
-        "OwnerId": str,
-        "Region": str,
-    },
-    total=False,
-)
-
-class AWSDomainInformationOutputTypeDef(
-    _RequiredAWSDomainInformationOutputTypeDef, _OptionalAWSDomainInformationOutputTypeDef
-):
-    pass
-
 _RequiredAWSDomainInformationTypeDef = TypedDict(
     "_RequiredAWSDomainInformationTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalAWSDomainInformationTypeDef = TypedDict(
@@ -431,23 +390,14 @@
         "ActionType": ScheduledAutoTuneActionTypeType,
         "Action": str,
         "Severity": ScheduledAutoTuneSeverityTypeType,
     },
     total=False,
 )
 
-DurationOutputTypeDef = TypedDict(
-    "DurationOutputTypeDef",
-    {
-        "Value": int,
-        "Unit": Literal["HOURS"],
-    },
-    total=False,
-)
-
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "Value": int,
         "Unit": Literal["HOURS"],
     },
     total=False,
@@ -535,29 +485,14 @@
         "Status": str,
         "Description": str,
         "LastUpdated": datetime,
     },
     total=False,
 )
 
-ColdStorageOptionsOutputTypeDef = TypedDict(
-    "ColdStorageOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-)
-
-ZoneAwarenessConfigOutputTypeDef = TypedDict(
-    "ZoneAwarenessConfigOutputTypeDef",
-    {
-        "AvailabilityZoneCount": int,
-    },
-    total=False,
-)
-
 ColdStorageOptionsTypeDef = TypedDict(
     "ColdStorageOptionsTypeDef",
     {
         "Enabled": bool,
     },
 )
 
@@ -565,25 +500,14 @@
     "ZoneAwarenessConfigTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
     total=False,
 )
 
-CognitoOptionsOutputTypeDef = TypedDict(
-    "CognitoOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "UserPoolId": str,
-        "IdentityPoolId": str,
-        "RoleArn": str,
-    },
-    total=False,
-)
-
 CognitoOptionsTypeDef = TypedDict(
     "CognitoOptionsTypeDef",
     {
         "Enabled": bool,
         "UserPoolId": str,
         "IdentityPoolId": str,
         "RoleArn": str,
@@ -596,22 +520,14 @@
     {
         "SourceVersion": str,
         "TargetVersions": List[str],
     },
     total=False,
 )
 
-CrossClusterSearchConnectionPropertiesOutputTypeDef = TypedDict(
-    "CrossClusterSearchConnectionPropertiesOutputTypeDef",
-    {
-        "SkipUnavailable": SkipUnavailableStatusType,
-    },
-    total=False,
-)
-
 CrossClusterSearchConnectionPropertiesTypeDef = TypedDict(
     "CrossClusterSearchConnectionPropertiesTypeDef",
     {
         "SkipUnavailable": SkipUnavailableStatusType,
     },
     total=False,
 )
@@ -956,26 +872,14 @@
     "DissociatePackageRequestRequestTypeDef",
     {
         "PackageID": str,
         "DomainName": str,
     },
 )
 
-DomainEndpointOptionsOutputTypeDef = TypedDict(
-    "DomainEndpointOptionsOutputTypeDef",
-    {
-        "EnforceHTTPS": bool,
-        "TLSSecurityPolicy": TLSSecurityPolicyType,
-        "CustomEndpointEnabled": bool,
-        "CustomEndpoint": str,
-        "CustomEndpointCertificateArn": str,
-    },
-    total=False,
-)
-
 DomainInfoTypeDef = TypedDict(
     "DomainInfoTypeDef",
     {
         "DomainName": str,
         "EngineType": EngineTypeType,
     },
     total=False,
@@ -986,68 +890,14 @@
     {
         "ErrorType": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-EBSOptionsOutputTypeDef = TypedDict(
-    "EBSOptionsOutputTypeDef",
-    {
-        "EBSEnabled": bool,
-        "VolumeType": VolumeTypeType,
-        "VolumeSize": int,
-        "Iops": int,
-        "Throughput": int,
-    },
-    total=False,
-)
-
-EncryptionAtRestOptionsOutputTypeDef = TypedDict(
-    "EncryptionAtRestOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-LogPublishingOptionOutputTypeDef = TypedDict(
-    "LogPublishingOptionOutputTypeDef",
-    {
-        "CloudWatchLogsLogGroupArn": str,
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-NodeToNodeEncryptionOptionsOutputTypeDef = TypedDict(
-    "NodeToNodeEncryptionOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-SnapshotOptionsOutputTypeDef = TypedDict(
-    "SnapshotOptionsOutputTypeDef",
-    {
-        "AutomatedSnapshotStartHour": int,
-    },
-    total=False,
-)
-
-SoftwareUpdateOptionsOutputTypeDef = TypedDict(
-    "SoftwareUpdateOptionsOutputTypeDef",
-    {
-        "AutoSoftwareUpdateEnabled": bool,
-    },
-    total=False,
-)
-
 VPCDerivedInfoTypeDef = TypedDict(
     "VPCDerivedInfoTypeDef",
     {
         "VPCId": str,
         "SubnetIds": List[str],
         "AvailabilityZones": List[str],
         "SecurityGroupIds": List[str],
@@ -1285,22 +1135,14 @@
 ListTagsRequestRequestTypeDef = TypedDict(
     "ListTagsRequestRequestTypeDef",
     {
         "ARN": str,
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
 ListVersionsRequestRequestTypeDef = TypedDict(
     "ListVersionsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1350,22 +1192,14 @@
     "ListVpcEndpointsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-WindowStartTimeOutputTypeDef = TypedDict(
-    "WindowStartTimeOutputTypeDef",
-    {
-        "Hours": int,
-        "Minutes": int,
-    },
-)
-
 WindowStartTimeTypeDef = TypedDict(
     "WindowStartTimeTypeDef",
     {
         "Hours": int,
         "Minutes": int,
     },
 )
@@ -1419,22 +1253,14 @@
     "RevokeVpcEndpointAccessRequestRequestTypeDef",
     {
         "DomainName": str,
         "Account": str,
     },
 )
 
-SAMLIdpOutputTypeDef = TypedDict(
-    "SAMLIdpOutputTypeDef",
-    {
-        "MetadataContent": str,
-        "EntityId": str,
-    },
-)
-
 SAMLIdpTypeDef = TypedDict(
     "SAMLIdpTypeDef",
     {
         "MetadataContent": str,
         "EntityId": str,
     },
 )
@@ -1520,22 +1346,14 @@
         "UpgradeStepStatus": UpgradeStatusType,
         "Issues": List[str],
         "ProgressPercent": float,
     },
     total=False,
 )
 
-DomainInformationContainerOutputTypeDef = TypedDict(
-    "DomainInformationContainerOutputTypeDef",
-    {
-        "AWSDomainInformation": AWSDomainInformationOutputTypeDef,
-    },
-    total=False,
-)
-
 DomainInformationContainerTypeDef = TypedDict(
     "DomainInformationContainerTypeDef",
     {
         "AWSDomainInformation": AWSDomainInformationTypeDef,
     },
     total=False,
 )
@@ -1603,14 +1421,22 @@
     "AddTagsRequestRequestTypeDef",
     {
         "ARN": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AuthorizeVpcEndpointAccessResponseTypeDef = TypedDict(
     "AuthorizeVpcEndpointAccessResponseTypeDef",
     {
         "AuthorizedPrincipal": AuthorizedPrincipalTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1632,15 +1458,15 @@
     total=False,
 )
 
 AutoTuneMaintenanceScheduleOutputTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleOutputTypeDef",
     {
         "StartAt": datetime,
-        "Duration": DurationOutputTypeDef,
+        "Duration": DurationTypeDef,
         "CronExpressionForRecurrence": str,
     },
     total=False,
 )
 
 AutoTuneMaintenanceScheduleTypeDef = TypedDict(
     "AutoTuneMaintenanceScheduleTypeDef",
@@ -1699,33 +1525,14 @@
         "CompletedProperties": List[str],
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
     },
     total=False,
 )
 
-ClusterConfigOutputTypeDef = TypedDict(
-    "ClusterConfigOutputTypeDef",
-    {
-        "InstanceType": OpenSearchPartitionInstanceTypeType,
-        "InstanceCount": int,
-        "DedicatedMasterEnabled": bool,
-        "ZoneAwarenessEnabled": bool,
-        "ZoneAwarenessConfig": ZoneAwarenessConfigOutputTypeDef,
-        "DedicatedMasterType": OpenSearchPartitionInstanceTypeType,
-        "DedicatedMasterCount": int,
-        "WarmEnabled": bool,
-        "WarmType": OpenSearchWarmPartitionInstanceTypeType,
-        "WarmCount": int,
-        "ColdStorageOptions": ColdStorageOptionsOutputTypeDef,
-        "MultiAZWithStandbyEnabled": bool,
-    },
-    total=False,
-)
-
 ClusterConfigTypeDef = TypedDict(
     "ClusterConfigTypeDef",
     {
         "InstanceType": OpenSearchPartitionInstanceTypeType,
         "InstanceCount": int,
         "DedicatedMasterEnabled": bool,
         "ZoneAwarenessEnabled": bool,
@@ -1740,41 +1547,90 @@
     },
     total=False,
 )
 
 CognitoOptionsStatusTypeDef = TypedDict(
     "CognitoOptionsStatusTypeDef",
     {
-        "Options": CognitoOptionsOutputTypeDef,
+        "Options": CognitoOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
 GetCompatibleVersionsResponseTypeDef = TypedDict(
     "GetCompatibleVersionsResponseTypeDef",
     {
         "CompatibleVersions": List[CompatibleVersionsMapTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConnectionPropertiesOutputTypeDef = TypedDict(
-    "ConnectionPropertiesOutputTypeDef",
+ConnectionPropertiesTypeDef = TypedDict(
+    "ConnectionPropertiesTypeDef",
     {
         "Endpoint": str,
-        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesOutputTypeDef,
+        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
     },
     total=False,
 )
 
-ConnectionPropertiesTypeDef = TypedDict(
-    "ConnectionPropertiesTypeDef",
+DomainEndpointOptionsStatusTypeDef = TypedDict(
+    "DomainEndpointOptionsStatusTypeDef",
     {
-        "Endpoint": str,
-        "CrossClusterSearch": CrossClusterSearchConnectionPropertiesTypeDef,
+        "Options": DomainEndpointOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+EBSOptionsStatusTypeDef = TypedDict(
+    "EBSOptionsStatusTypeDef",
+    {
+        "Options": EBSOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+EncryptionAtRestOptionsStatusTypeDef = TypedDict(
+    "EncryptionAtRestOptionsStatusTypeDef",
+    {
+        "Options": EncryptionAtRestOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+LogPublishingOptionsStatusTypeDef = TypedDict(
+    "LogPublishingOptionsStatusTypeDef",
+    {
+        "Options": Dict[LogTypeType, LogPublishingOptionTypeDef],
+        "Status": OptionStatusTypeDef,
+    },
+    total=False,
+)
+
+NodeToNodeEncryptionOptionsStatusTypeDef = TypedDict(
+    "NodeToNodeEncryptionOptionsStatusTypeDef",
+    {
+        "Options": NodeToNodeEncryptionOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+SnapshotOptionsStatusTypeDef = TypedDict(
+    "SnapshotOptionsStatusTypeDef",
+    {
+        "Options": SnapshotOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+SoftwareUpdateOptionsStatusTypeDef = TypedDict(
+    "SoftwareUpdateOptionsStatusTypeDef",
+    {
+        "Options": SoftwareUpdateOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcEndpointRequestRequestTypeDef",
     {
@@ -1905,22 +1761,14 @@
         "Filters": Sequence[DescribePackagesFilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DomainEndpointOptionsStatusTypeDef = TypedDict(
-    "DomainEndpointOptionsStatusTypeDef",
-    {
-        "Options": DomainEndpointOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "DomainNames": List[DomainInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1953,64 +1801,14 @@
         "LastUpdatedAt": datetime,
         "AvailablePackageVersion": str,
         "ErrorDetails": ErrorDetailsTypeDef,
     },
     total=False,
 )
 
-EBSOptionsStatusTypeDef = TypedDict(
-    "EBSOptionsStatusTypeDef",
-    {
-        "Options": EBSOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-EncryptionAtRestOptionsStatusTypeDef = TypedDict(
-    "EncryptionAtRestOptionsStatusTypeDef",
-    {
-        "Options": EncryptionAtRestOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-LogPublishingOptionsStatusTypeDef = TypedDict(
-    "LogPublishingOptionsStatusTypeDef",
-    {
-        "Options": Dict[LogTypeType, LogPublishingOptionOutputTypeDef],
-        "Status": OptionStatusTypeDef,
-    },
-    total=False,
-)
-
-NodeToNodeEncryptionOptionsStatusTypeDef = TypedDict(
-    "NodeToNodeEncryptionOptionsStatusTypeDef",
-    {
-        "Options": NodeToNodeEncryptionOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-SnapshotOptionsStatusTypeDef = TypedDict(
-    "SnapshotOptionsStatusTypeDef",
-    {
-        "Options": SnapshotOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-SoftwareUpdateOptionsStatusTypeDef = TypedDict(
-    "SoftwareUpdateOptionsStatusTypeDef",
-    {
-        "Options": SoftwareUpdateOptionsOutputTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-    total=False,
-)
-
 VPCDerivedInfoStatusTypeDef = TypedDict(
     "VPCDerivedInfoStatusTypeDef",
     {
         "Options": VPCDerivedInfoTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
@@ -2090,30 +1888,14 @@
     "UpdateScheduledActionResponseTypeDef",
     {
         "ScheduledAction": ScheduledActionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-OffPeakWindowOutputTypeDef = TypedDict(
-    "OffPeakWindowOutputTypeDef",
-    {
-        "WindowStartTime": WindowStartTimeOutputTypeDef,
-    },
-    total=False,
-)
-
 OffPeakWindowTypeDef = TypedDict(
     "OffPeakWindowTypeDef",
     {
         "WindowStartTime": WindowStartTimeTypeDef,
     },
     total=False,
 )
@@ -2150,33 +1932,33 @@
         "State": str,
         "PaymentOption": ReservedInstancePaymentOptionType,
         "RecurringCharges": List[RecurringChargeTypeDef],
     },
     total=False,
 )
 
-SAMLOptionsOutputTypeDef = TypedDict(
-    "SAMLOptionsOutputTypeDef",
+SAMLOptionsInputTypeDef = TypedDict(
+    "SAMLOptionsInputTypeDef",
     {
         "Enabled": bool,
-        "Idp": SAMLIdpOutputTypeDef,
+        "Idp": SAMLIdpTypeDef,
+        "MasterUserName": str,
+        "MasterBackendRole": str,
         "SubjectKey": str,
         "RolesKey": str,
         "SessionTimeoutMinutes": int,
     },
     total=False,
 )
 
-SAMLOptionsInputTypeDef = TypedDict(
-    "SAMLOptionsInputTypeDef",
+SAMLOptionsOutputTypeDef = TypedDict(
+    "SAMLOptionsOutputTypeDef",
     {
         "Enabled": bool,
         "Idp": SAMLIdpTypeDef,
-        "MasterUserName": str,
-        "MasterBackendRole": str,
         "SubjectKey": str,
         "RolesKey": str,
         "SessionTimeoutMinutes": int,
     },
     total=False,
 )
 
@@ -2200,16 +1982,16 @@
     },
     total=False,
 )
 
 InboundConnectionTypeDef = TypedDict(
     "InboundConnectionTypeDef",
     {
-        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionId": str,
         "ConnectionStatus": InboundConnectionStatusTypeDef,
         "ConnectionMode": ConnectionModeType,
     },
     total=False,
 )
 
@@ -2281,47 +2063,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClusterConfigStatusTypeDef = TypedDict(
     "ClusterConfigStatusTypeDef",
     {
-        "Options": ClusterConfigOutputTypeDef,
+        "Options": ClusterConfigTypeDef,
         "Status": OptionStatusTypeDef,
     },
 )
 
-CreateOutboundConnectionResponseTypeDef = TypedDict(
-    "CreateOutboundConnectionResponseTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionId": str,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-OutboundConnectionTypeDef = TypedDict(
-    "OutboundConnectionTypeDef",
-    {
-        "LocalDomainInfo": DomainInformationContainerOutputTypeDef,
-        "RemoteDomainInfo": DomainInformationContainerOutputTypeDef,
-        "ConnectionId": str,
-        "ConnectionAlias": str,
-        "ConnectionStatus": OutboundConnectionStatusTypeDef,
-        "ConnectionMode": ConnectionModeType,
-        "ConnectionProperties": ConnectionPropertiesOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateOutboundConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOutboundConnectionRequestRequestTypeDef",
     {
         "LocalDomainInfo": DomainInformationContainerTypeDef,
         "RemoteDomainInfo": DomainInformationContainerTypeDef,
         "ConnectionAlias": str,
     },
@@ -2337,14 +2091,42 @@
 
 class CreateOutboundConnectionRequestRequestTypeDef(
     _RequiredCreateOutboundConnectionRequestRequestTypeDef,
     _OptionalCreateOutboundConnectionRequestRequestTypeDef,
 ):
     pass
 
+CreateOutboundConnectionResponseTypeDef = TypedDict(
+    "CreateOutboundConnectionResponseTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionId": str,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OutboundConnectionTypeDef = TypedDict(
+    "OutboundConnectionTypeDef",
+    {
+        "LocalDomainInfo": DomainInformationContainerTypeDef,
+        "RemoteDomainInfo": DomainInformationContainerTypeDef,
+        "ConnectionId": str,
+        "ConnectionAlias": str,
+        "ConnectionStatus": OutboundConnectionStatusTypeDef,
+        "ConnectionMode": ConnectionModeType,
+        "ConnectionProperties": ConnectionPropertiesTypeDef,
+    },
+    total=False,
+)
+
 AssociatePackageResponseTypeDef = TypedDict(
     "AssociatePackageResponseTypeDef",
     {
         "DomainPackageDetails": DomainPackageDetailsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2429,23 +2211,14 @@
     "UpdateVpcEndpointResponseTypeDef",
     {
         "VpcEndpoint": VpcEndpointTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-OffPeakWindowOptionsOutputTypeDef = TypedDict(
-    "OffPeakWindowOptionsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "OffPeakWindow": OffPeakWindowOutputTypeDef,
-    },
-    total=False,
-)
-
 OffPeakWindowOptionsTypeDef = TypedDict(
     "OffPeakWindowOptionsTypeDef",
     {
         "Enabled": bool,
         "OffPeakWindow": OffPeakWindowTypeDef,
     },
     total=False,
@@ -2465,33 +2238,33 @@
     {
         "NextToken": str,
         "ReservedInstances": List[ReservedInstanceTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdvancedSecurityOptionsTypeDef = TypedDict(
-    "AdvancedSecurityOptionsTypeDef",
+AdvancedSecurityOptionsInputTypeDef = TypedDict(
+    "AdvancedSecurityOptionsInputTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
-        "SAMLOptions": SAMLOptionsOutputTypeDef,
-        "AnonymousAuthDisableDate": datetime,
+        "MasterUserOptions": MasterUserOptionsTypeDef,
+        "SAMLOptions": SAMLOptionsInputTypeDef,
         "AnonymousAuthEnabled": bool,
     },
     total=False,
 )
 
-AdvancedSecurityOptionsInputTypeDef = TypedDict(
-    "AdvancedSecurityOptionsInputTypeDef",
+AdvancedSecurityOptionsTypeDef = TypedDict(
+    "AdvancedSecurityOptionsTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
-        "MasterUserOptions": MasterUserOptionsTypeDef,
-        "SAMLOptions": SAMLOptionsInputTypeDef,
+        "SAMLOptions": SAMLOptionsOutputTypeDef,
+        "AnonymousAuthDisableDate": datetime,
         "AnonymousAuthEnabled": bool,
     },
     total=False,
 )
 
 LimitsTypeDef = TypedDict(
     "LimitsTypeDef",
@@ -2579,70 +2352,20 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OffPeakWindowOptionsStatusTypeDef = TypedDict(
     "OffPeakWindowOptionsStatusTypeDef",
     {
-        "Options": OffPeakWindowOptionsOutputTypeDef,
+        "Options": OffPeakWindowOptionsTypeDef,
         "Status": OptionStatusTypeDef,
     },
     total=False,
 )
 
-AdvancedSecurityOptionsStatusTypeDef = TypedDict(
-    "AdvancedSecurityOptionsStatusTypeDef",
-    {
-        "Options": AdvancedSecurityOptionsTypeDef,
-        "Status": OptionStatusTypeDef,
-    },
-)
-
-_RequiredDomainStatusTypeDef = TypedDict(
-    "_RequiredDomainStatusTypeDef",
-    {
-        "DomainId": str,
-        "DomainName": str,
-        "ARN": str,
-        "ClusterConfig": ClusterConfigOutputTypeDef,
-    },
-)
-_OptionalDomainStatusTypeDef = TypedDict(
-    "_OptionalDomainStatusTypeDef",
-    {
-        "Created": bool,
-        "Deleted": bool,
-        "Endpoint": str,
-        "Endpoints": Dict[str, str],
-        "Processing": bool,
-        "UpgradeProcessing": bool,
-        "EngineVersion": str,
-        "EBSOptions": EBSOptionsOutputTypeDef,
-        "AccessPolicies": str,
-        "SnapshotOptions": SnapshotOptionsOutputTypeDef,
-        "VPCOptions": VPCDerivedInfoTypeDef,
-        "CognitoOptions": CognitoOptionsOutputTypeDef,
-        "EncryptionAtRestOptions": EncryptionAtRestOptionsOutputTypeDef,
-        "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsOutputTypeDef,
-        "AdvancedOptions": Dict[str, str],
-        "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionOutputTypeDef],
-        "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
-        "DomainEndpointOptions": DomainEndpointOptionsOutputTypeDef,
-        "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
-        "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
-        "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
-        "OffPeakWindowOptions": OffPeakWindowOptionsOutputTypeDef,
-        "SoftwareUpdateOptions": SoftwareUpdateOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
-    pass
-
 _RequiredCreateDomainRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDomainRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalCreateDomainRequestRequestTypeDef = TypedDict(
@@ -2706,14 +2429,64 @@
 
 class UpdateDomainConfigRequestRequestTypeDef(
     _RequiredUpdateDomainConfigRequestRequestTypeDef,
     _OptionalUpdateDomainConfigRequestRequestTypeDef,
 ):
     pass
 
+AdvancedSecurityOptionsStatusTypeDef = TypedDict(
+    "AdvancedSecurityOptionsStatusTypeDef",
+    {
+        "Options": AdvancedSecurityOptionsTypeDef,
+        "Status": OptionStatusTypeDef,
+    },
+)
+
+_RequiredDomainStatusTypeDef = TypedDict(
+    "_RequiredDomainStatusTypeDef",
+    {
+        "DomainId": str,
+        "DomainName": str,
+        "ARN": str,
+        "ClusterConfig": ClusterConfigTypeDef,
+    },
+)
+_OptionalDomainStatusTypeDef = TypedDict(
+    "_OptionalDomainStatusTypeDef",
+    {
+        "Created": bool,
+        "Deleted": bool,
+        "Endpoint": str,
+        "Endpoints": Dict[str, str],
+        "Processing": bool,
+        "UpgradeProcessing": bool,
+        "EngineVersion": str,
+        "EBSOptions": EBSOptionsTypeDef,
+        "AccessPolicies": str,
+        "SnapshotOptions": SnapshotOptionsTypeDef,
+        "VPCOptions": VPCDerivedInfoTypeDef,
+        "CognitoOptions": CognitoOptionsTypeDef,
+        "EncryptionAtRestOptions": EncryptionAtRestOptionsTypeDef,
+        "NodeToNodeEncryptionOptions": NodeToNodeEncryptionOptionsTypeDef,
+        "AdvancedOptions": Dict[str, str],
+        "LogPublishingOptions": Dict[LogTypeType, LogPublishingOptionTypeDef],
+        "ServiceSoftwareOptions": ServiceSoftwareOptionsTypeDef,
+        "DomainEndpointOptions": DomainEndpointOptionsTypeDef,
+        "AdvancedSecurityOptions": AdvancedSecurityOptionsTypeDef,
+        "AutoTuneOptions": AutoTuneOptionsOutputTypeDef,
+        "ChangeProgressDetails": ChangeProgressDetailsTypeDef,
+        "OffPeakWindowOptions": OffPeakWindowOptionsTypeDef,
+        "SoftwareUpdateOptions": SoftwareUpdateOptionsTypeDef,
+    },
+    total=False,
+)
+
+class DomainStatusTypeDef(_RequiredDomainStatusTypeDef, _OptionalDomainStatusTypeDef):
+    pass
+
 DescribeInstanceTypeLimitsResponseTypeDef = TypedDict(
     "DescribeInstanceTypeLimitsResponseTypeDef",
     {
         "LimitsByRole": Dict[str, LimitsTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/PKG-INFO` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-opensearch
-Version: 1.28.12
-Summary: Type annotations for boto3.OpenSearchService 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.OpenSearchService 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-opensearch.svg?color=blue)](https://pypi.org/project/mypy-boto3-opensearch)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-opensearch)](https://pepy.tech/project/mypy-boto3-opensearch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.OpenSearchService 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
+[boto3.OpenSearchService 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opensearch.html#OpenSearchService)
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
 [mypy-boto3-opensearch docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_opensearch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -338,43 +338,37 @@
 ### Typed dictionaries
 
 `mypy_boto3_opensearch.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_opensearch.type_defs import (
-    AWSDomainInformationOutputTypeDef,
     AWSDomainInformationTypeDef,
     AcceptInboundConnectionRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     OptionStatusTypeDef,
     TagTypeDef,
     AdditionalLimitTypeDef,
     MasterUserOptionsTypeDef,
     AssociatePackageRequestRequestTypeDef,
     AuthorizeVpcEndpointAccessRequestRequestTypeDef,
     AuthorizedPrincipalTypeDef,
     ScheduledAutoTuneDetailsTypeDef,
-    DurationOutputTypeDef,
     DurationTypeDef,
     AutoTuneOptionsOutputTypeDef,
     AutoTuneStatusTypeDef,
     AvailabilityZoneInfoTypeDef,
     CancelServiceSoftwareUpdateRequestRequestTypeDef,
     ServiceSoftwareOptionsTypeDef,
     ChangeProgressDetailsTypeDef,
     ChangeProgressStageTypeDef,
-    ColdStorageOptionsOutputTypeDef,
-    ZoneAwarenessConfigOutputTypeDef,
     ColdStorageOptionsTypeDef,
     ZoneAwarenessConfigTypeDef,
-    CognitoOptionsOutputTypeDef,
     CognitoOptionsTypeDef,
     CompatibleVersionsMapTypeDef,
-    CrossClusterSearchConnectionPropertiesOutputTypeDef,
     CrossClusterSearchConnectionPropertiesTypeDef,
     DomainEndpointOptionsTypeDef,
     EBSOptionsTypeDef,
     EncryptionAtRestOptionsTypeDef,
     LogPublishingOptionTypeDef,
     NodeToNodeEncryptionOptionsTypeDef,
     SnapshotOptionsTypeDef,
@@ -402,23 +396,16 @@
     DescribeInstanceTypeLimitsRequestRequestTypeDef,
     DescribePackagesFilterTypeDef,
     DescribeReservedInstanceOfferingsRequestRequestTypeDef,
     DescribeReservedInstancesRequestRequestTypeDef,
     DescribeVpcEndpointsRequestRequestTypeDef,
     VpcEndpointErrorTypeDef,
     DissociatePackageRequestRequestTypeDef,
-    DomainEndpointOptionsOutputTypeDef,
     DomainInfoTypeDef,
     ErrorDetailsTypeDef,
-    EBSOptionsOutputTypeDef,
-    EncryptionAtRestOptionsOutputTypeDef,
-    LogPublishingOptionOutputTypeDef,
-    NodeToNodeEncryptionOptionsOutputTypeDef,
-    SnapshotOptionsOutputTypeDef,
-    SoftwareUpdateOptionsOutputTypeDef,
     VPCDerivedInfoTypeDef,
     ValidationFailureTypeDef,
     GetCompatibleVersionsRequestRequestTypeDef,
     GetPackageVersionHistoryRequestRequestTypeDef,
     PackageVersionHistoryTypeDef,
     GetUpgradeHistoryRequestRequestTypeDef,
     GetUpgradeStatusRequestRequestTypeDef,
@@ -428,153 +415,145 @@
     ListDomainNamesRequestRequestTypeDef,
     ListDomainsForPackageRequestRequestTypeDef,
     ListInstanceTypeDetailsRequestRequestTypeDef,
     ListPackagesForDomainRequestRequestTypeDef,
     ListScheduledActionsRequestRequestTypeDef,
     ScheduledActionTypeDef,
     ListTagsRequestRequestTypeDef,
-    TagOutputTypeDef,
     ListVersionsRequestRequestTypeDef,
     ListVpcEndpointAccessRequestRequestTypeDef,
     ListVpcEndpointsForDomainRequestRequestTypeDef,
     ListVpcEndpointsRequestRequestTypeDef,
-    WindowStartTimeOutputTypeDef,
     WindowStartTimeTypeDef,
     PurchaseReservedInstanceOfferingRequestRequestTypeDef,
     RecurringChargeTypeDef,
     RejectInboundConnectionRequestRequestTypeDef,
     RemoveTagsRequestRequestTypeDef,
     RevokeVpcEndpointAccessRequestRequestTypeDef,
-    SAMLIdpOutputTypeDef,
     SAMLIdpTypeDef,
     StartServiceSoftwareUpdateRequestRequestTypeDef,
     StorageTypeLimitTypeDef,
     UpdateScheduledActionRequestRequestTypeDef,
     UpgradeDomainRequestRequestTypeDef,
     UpgradeStepItemTypeDef,
-    DomainInformationContainerOutputTypeDef,
     DomainInformationContainerTypeDef,
     EmptyResponseMetadataTypeDef,
     GetUpgradeStatusResponseTypeDef,
     ListVersionsResponseTypeDef,
     PurchaseReservedInstanceOfferingResponseTypeDef,
     AccessPoliciesStatusTypeDef,
     AdvancedOptionsStatusTypeDef,
     VersionStatusTypeDef,
     AddTagsRequestRequestTypeDef,
+    ListTagsResponseTypeDef,
     AuthorizeVpcEndpointAccessResponseTypeDef,
     ListVpcEndpointAccessResponseTypeDef,
     AutoTuneDetailsTypeDef,
     AutoTuneMaintenanceScheduleOutputTypeDef,
     AutoTuneMaintenanceScheduleTypeDef,
     EnvironmentInfoTypeDef,
     CancelServiceSoftwareUpdateResponseTypeDef,
     StartServiceSoftwareUpdateResponseTypeDef,
     UpgradeDomainResponseTypeDef,
     ChangeProgressStatusDetailsTypeDef,
-    ClusterConfigOutputTypeDef,
     ClusterConfigTypeDef,
     CognitoOptionsStatusTypeDef,
     GetCompatibleVersionsResponseTypeDef,
-    ConnectionPropertiesOutputTypeDef,
     ConnectionPropertiesTypeDef,
+    DomainEndpointOptionsStatusTypeDef,
+    EBSOptionsStatusTypeDef,
+    EncryptionAtRestOptionsStatusTypeDef,
+    LogPublishingOptionsStatusTypeDef,
+    NodeToNodeEncryptionOptionsStatusTypeDef,
+    SnapshotOptionsStatusTypeDef,
+    SoftwareUpdateOptionsStatusTypeDef,
     CreateVpcEndpointRequestRequestTypeDef,
     UpdateVpcEndpointRequestRequestTypeDef,
     CreatePackageRequestRequestTypeDef,
     UpdatePackageRequestRequestTypeDef,
     DeleteVpcEndpointResponseTypeDef,
     ListVpcEndpointsForDomainResponseTypeDef,
     ListVpcEndpointsResponseTypeDef,
     DescribeDomainNodesResponseTypeDef,
     DescribeInboundConnectionsRequestRequestTypeDef,
     DescribeOutboundConnectionsRequestRequestTypeDef,
     DescribePackagesRequestRequestTypeDef,
-    DomainEndpointOptionsStatusTypeDef,
     ListDomainNamesResponseTypeDef,
     DomainPackageDetailsTypeDef,
     PackageDetailsTypeDef,
-    EBSOptionsStatusTypeDef,
-    EncryptionAtRestOptionsStatusTypeDef,
-    LogPublishingOptionsStatusTypeDef,
-    NodeToNodeEncryptionOptionsStatusTypeDef,
-    SnapshotOptionsStatusTypeDef,
-    SoftwareUpdateOptionsStatusTypeDef,
     VPCDerivedInfoStatusTypeDef,
     VpcEndpointTypeDef,
     DryRunProgressStatusTypeDef,
     GetPackageVersionHistoryResponseTypeDef,
     InstanceLimitsTypeDef,
     ListInstanceTypeDetailsResponseTypeDef,
     ListScheduledActionsResponseTypeDef,
     UpdateScheduledActionResponseTypeDef,
-    ListTagsResponseTypeDef,
-    OffPeakWindowOutputTypeDef,
     OffPeakWindowTypeDef,
     ReservedInstanceOfferingTypeDef,
     ReservedInstanceTypeDef,
-    SAMLOptionsOutputTypeDef,
     SAMLOptionsInputTypeDef,
+    SAMLOptionsOutputTypeDef,
     StorageTypeTypeDef,
     UpgradeHistoryTypeDef,
     InboundConnectionTypeDef,
     AutoTuneTypeDef,
     AutoTuneOptionsExtraOutputTypeDef,
     AutoTuneOptionsInputTypeDef,
     AutoTuneOptionsTypeDef,
     DescribeDomainHealthResponseTypeDef,
     DescribeDomainChangeProgressResponseTypeDef,
     ClusterConfigStatusTypeDef,
+    CreateOutboundConnectionRequestRequestTypeDef,
     CreateOutboundConnectionResponseTypeDef,
     OutboundConnectionTypeDef,
-    CreateOutboundConnectionRequestRequestTypeDef,
     AssociatePackageResponseTypeDef,
     DissociatePackageResponseTypeDef,
     ListDomainsForPackageResponseTypeDef,
     ListPackagesForDomainResponseTypeDef,
     CreatePackageResponseTypeDef,
     DeletePackageResponseTypeDef,
     DescribePackagesResponseTypeDef,
     UpdatePackageResponseTypeDef,
     CreateVpcEndpointResponseTypeDef,
     DescribeVpcEndpointsResponseTypeDef,
     UpdateVpcEndpointResponseTypeDef,
-    OffPeakWindowOptionsOutputTypeDef,
     OffPeakWindowOptionsTypeDef,
     DescribeReservedInstanceOfferingsResponseTypeDef,
     DescribeReservedInstancesResponseTypeDef,
-    AdvancedSecurityOptionsTypeDef,
     AdvancedSecurityOptionsInputTypeDef,
+    AdvancedSecurityOptionsTypeDef,
     LimitsTypeDef,
     GetUpgradeHistoryResponseTypeDef,
     AcceptInboundConnectionResponseTypeDef,
     DeleteInboundConnectionResponseTypeDef,
     DescribeInboundConnectionsResponseTypeDef,
     RejectInboundConnectionResponseTypeDef,
     DescribeDomainAutoTunesResponseTypeDef,
     AutoTuneOptionsStatusTypeDef,
     DeleteOutboundConnectionResponseTypeDef,
     DescribeOutboundConnectionsResponseTypeDef,
     OffPeakWindowOptionsStatusTypeDef,
-    AdvancedSecurityOptionsStatusTypeDef,
-    DomainStatusTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateDomainConfigRequestRequestTypeDef,
+    AdvancedSecurityOptionsStatusTypeDef,
+    DomainStatusTypeDef,
     DescribeInstanceTypeLimitsResponseTypeDef,
     DomainConfigTypeDef,
     CreateDomainResponseTypeDef,
     DeleteDomainResponseTypeDef,
     DescribeDomainResponseTypeDef,
     DescribeDomainsResponseTypeDef,
     DescribeDryRunProgressResponseTypeDef,
     DescribeDomainConfigResponseTypeDef,
     UpdateDomainConfigResponseTypeDef,
 )
 
 
-def get_structure() -> AWSDomainInformationOutputTypeDef:
+def get_structure() -> AWSDomainInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-opensearch-1.28.12/mypy_boto3_opensearch.egg-info/SOURCES.txt` & `mypy-boto3-opensearch-1.28.15/mypy_boto3_opensearch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-opensearch-1.28.12/setup.py` & `mypy-boto3-opensearch-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-opensearch",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_opensearch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.OpenSearchService 1.28.12 service generated with"
-        " mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.OpenSearchService 1.28.15 service generated with"
+        " mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

