# Comparing `tmp/mypy-boto3-lightsail-1.28.12.tar.gz` & `tmp/mypy-boto3-lightsail-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-lightsail-1.28.12.tar", last modified: Thu Jul 27 05:34:57 2023, max compression
+gzip compressed data, was "mypy-boto3-lightsail-1.28.15.tar", last modified: Fri Jul 28 20:43:10 2023, max compression
```

## Comparing `mypy-boto3-lightsail-1.28.12.tar` & `mypy-boto3-lightsail-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.292455 mypy-boto3-lightsail-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36949 2023-07-27 05:34:57.284455 mypy-boto3-lightsail-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35454 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.284455 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   113940 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   113754 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-07-27 05:25:26.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23001 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22978 2023-07-27 05:25:25.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   150553 2023-07-27 05:25:28.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   150452 2023-07-27 05:25:27.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:57.284455 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36949 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:57.000000 mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:57.292455 mypy-boto3-lightsail-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:25:24.000000 mypy-boto3-lightsail-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:10.509409 mypy-boto3-lightsail-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-07-28 20:43:10.505408 mypy-boto3-lightsail-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35193 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:10.505408 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113940 2023-07-28 20:30:17.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113754 2023-07-28 20:30:16.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25315 2023-07-28 20:30:18.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25313 2023-07-28 20:30:17.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-07-28 20:30:17.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22938 2023-07-28 20:30:17.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   147985 2023-07-28 20:30:22.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   147886 2023-07-28 20:30:20.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:10.505408 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:43:10.000000 mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:10.509409 mypy-boto3-lightsail-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:30:14.000000 mypy-boto3-lightsail-1.28.15/setup.py
```

### Comparing `mypy-boto3-lightsail-1.28.12/LICENSE` & `mypy-boto3-lightsail-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.12/PKG-INFO` & `mypy-boto3-lightsail-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.28.12
-Summary: Type annotations for boto3.Lightsail 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -474,40 +474,37 @@
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
-    AccessRulesOutputTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
     BlueprintTypeDef,
-    BucketAccessLogConfigOutputTypeDef,
     BucketAccessLogConfigTypeDef,
     BucketBundleTypeDef,
     BucketStateTypeDef,
     ResourceReceivingAccessTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     BundleTypeDef,
-    CacheBehaviorOutputTypeDef,
-    CacheBehaviorPerPathOutputTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
     CookieObjectOutputTypeDef,
     HeaderObjectOutputTypeDef,
     QueryStringObjectOutputTypeDef,
     CookieObjectTypeDef,
     HeaderObjectTypeDef,
@@ -516,23 +513,21 @@
     CloudFormationStackRecordSourceInfoTypeDef,
     DestinationInfoTypeDef,
     ContainerImageTypeDef,
     ContainerOutputTypeDef,
     ContainerTypeDef,
     ContainerServiceECRImagePullerRoleRequestTypeDef,
     ContainerServiceECRImagePullerRoleTypeDef,
-    ContainerServiceHealthCheckConfigOutputTypeDef,
     ContainerServiceHealthCheckConfigTypeDef,
     ContainerServiceLogEventTypeDef,
     ContainerServicePowerTypeDef,
     ContainerServiceRegistryLoginTypeDef,
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
-    TagTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
@@ -563,139 +558,110 @@
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     DomainEntryOutputTypeDef,
     ResourceRecordTypeDef,
-    DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
-    GetActiveNamesResultTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
-    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
     GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
-    GetBundlesRequestGetBundlesPaginateTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
-    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
-    GetContainerAPIMetadataResultTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
     GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
-    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
-    GetDisksRequestGetDisksPaginateTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
-    GetDistributionLatestCacheResetResultTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainsRequestGetDomainsPaginateTypeDef,
     GetDomainsRequestRequestTypeDef,
-    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
     GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
-    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
-    GetInstancesRequestGetInstancesPaginateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
-    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
     GetKeyPairsRequestRequestTypeDef,
     GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
-    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
-    GetOperationsRequestGetOperationsPaginateTypeDef,
     GetOperationsRequestRequestTypeDef,
     GetRegionsRequestRequestTypeDef,
-    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
-    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
-    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
     GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
-    GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
-    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
-    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
-    RelationalDatabaseParameterOutputTypeDef,
+    RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
-    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
-    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
-    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetStaticIpsRequestRequestTypeDef,
     HostKeyAttributesTypeDef,
     ImportKeyPairRequestRequestTypeDef,
     PasswordDataTypeDef,
     InstanceHealthSummaryTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstancePortInfoTypeDef,
     MonthlyTransferTypeDef,
-    IsVpcPeeredResultTypeDef,
     OriginTypeDef,
     LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef,
     LoadBalancerTlsCertificateDomainValidationOptionTypeDef,
     LoadBalancerTlsCertificateSummaryTypeDef,
     NameServersUpdateStateTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PendingModifiedRelationalDatabaseValuesTypeDef,
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
-    RelationalDatabaseParameterTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
     StopGUISessionRequestRequestTypeDef,
@@ -710,24 +676,43 @@
     UpdateRelationalDatabaseRequestRequestTypeDef,
     AccessKeyTypeDef,
     AddOnRequestTypeDef,
     AlarmTypeDef,
     ContactMethodTypeDef,
     OperationTypeDef,
     StaticIpTypeDef,
+    DownloadDefaultKeyPairResultTypeDef,
+    GetActiveNamesResultTypeDef,
+    GetContainerAPIMetadataResultTypeDef,
+    GetDistributionLatestCacheResetResultTypeDef,
+    GetRelationalDatabaseLogStreamsResultTypeDef,
+    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
+    IsVpcPeeredResultTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
+    CreateBucketRequestRequestTypeDef,
+    CreateCertificateRequestRequestTypeDef,
+    CreateDiskSnapshotRequestRequestTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    CreateInstanceSnapshotRequestRequestTypeDef,
+    CreateKeyPairRequestRequestTypeDef,
+    CreateLoadBalancerRequestRequestTypeDef,
+    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    CreateRelationalDatabaseRequestRequestTypeDef,
+    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetBundlesResultTypeDef,
     CacheSettingsOutputTypeDef,
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
@@ -736,57 +721,65 @@
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
-    CreateBucketRequestRequestTypeDef,
-    CreateCertificateRequestRequestTypeDef,
-    CreateDiskSnapshotRequestRequestTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    CreateInstanceSnapshotRequestRequestTypeDef,
-    CreateKeyPairRequestRequestTypeDef,
-    CreateLoadBalancerRequestRequestTypeDef,
-    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    CreateRelationalDatabaseRequestRequestTypeDef,
-    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
+    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
+    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
+    GetBundlesRequestGetBundlesPaginateTypeDef,
+    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
+    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
+    GetDisksRequestGetDisksPaginateTypeDef,
+    GetDomainsRequestGetDomainsPaginateTypeDef,
+    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
+    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
+    GetInstancesRequestGetInstancesPaginateTypeDef,
+    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
+    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
+    GetOperationsRequestGetOperationsPaginateTypeDef,
+    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
+    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
+    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
+    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
+    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetBucketMetricDataResultTypeDef,
     GetContainerServiceMetricDataResultTypeDef,
     GetDistributionMetricDataResultTypeDef,
     GetInstanceMetricDataResultTypeDef,
     GetLoadBalancerMetricDataResultTypeDef,
     GetRelationalDatabaseMetricDataResultTypeDef,
     GetInstancePortStatesResultTypeDef,
     GetInstanceStateResultTypeDef,
     GetLoadBalancerTlsPoliciesResultTypeDef,
     GetRelationalDatabaseBlueprintsResultTypeDef,
     GetRelationalDatabaseBundlesResultTypeDef,
     GetRelationalDatabaseEventsResultTypeDef,
     GetRelationalDatabaseLogEventsResultTypeDef,
     GetRelationalDatabaseParametersResultTypeDef,
+    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     InstanceAccessDetailsTypeDef,
     InstanceNetworkingTypeDef,
     LoadBalancerTlsCertificateDomainValidationRecordTypeDef,
     LoadBalancerTlsCertificateRenewalSummaryTypeDef,
     LoadBalancerTypeDef,
     RegisteredDomainDelegationInfoTypeDef,
     RelationalDatabaseTypeDef,
-    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     GetBucketAccessKeysResultTypeDef,
     CreateDiskFromSnapshotRequestRequestTypeDef,
     CreateDiskRequestRequestTypeDef,
     CreateInstancesFromSnapshotRequestRequestTypeDef,
     CreateInstancesRequestRequestTypeDef,
     EnableAddOnRequestRequestTypeDef,
     GetAlarmsResultTypeDef,
```

### Comparing `mypy-boto3-lightsail-1.28.12/README.md` & `mypy-boto3-lightsail-1.28.15/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -442,40 +442,37 @@
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
-    AccessRulesOutputTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
     BlueprintTypeDef,
-    BucketAccessLogConfigOutputTypeDef,
     BucketAccessLogConfigTypeDef,
     BucketBundleTypeDef,
     BucketStateTypeDef,
     ResourceReceivingAccessTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     BundleTypeDef,
-    CacheBehaviorOutputTypeDef,
-    CacheBehaviorPerPathOutputTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
     CookieObjectOutputTypeDef,
     HeaderObjectOutputTypeDef,
     QueryStringObjectOutputTypeDef,
     CookieObjectTypeDef,
     HeaderObjectTypeDef,
@@ -484,23 +481,21 @@
     CloudFormationStackRecordSourceInfoTypeDef,
     DestinationInfoTypeDef,
     ContainerImageTypeDef,
     ContainerOutputTypeDef,
     ContainerTypeDef,
     ContainerServiceECRImagePullerRoleRequestTypeDef,
     ContainerServiceECRImagePullerRoleTypeDef,
-    ContainerServiceHealthCheckConfigOutputTypeDef,
     ContainerServiceHealthCheckConfigTypeDef,
     ContainerServiceLogEventTypeDef,
     ContainerServicePowerTypeDef,
     ContainerServiceRegistryLoginTypeDef,
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
-    TagTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
@@ -531,139 +526,110 @@
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     DomainEntryOutputTypeDef,
     ResourceRecordTypeDef,
-    DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
-    GetActiveNamesResultTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
-    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
     GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
-    GetBundlesRequestGetBundlesPaginateTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
-    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
-    GetContainerAPIMetadataResultTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
     GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
-    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
-    GetDisksRequestGetDisksPaginateTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
-    GetDistributionLatestCacheResetResultTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainsRequestGetDomainsPaginateTypeDef,
     GetDomainsRequestRequestTypeDef,
-    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
     GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
-    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
-    GetInstancesRequestGetInstancesPaginateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
-    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
     GetKeyPairsRequestRequestTypeDef,
     GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
-    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
-    GetOperationsRequestGetOperationsPaginateTypeDef,
     GetOperationsRequestRequestTypeDef,
     GetRegionsRequestRequestTypeDef,
-    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
-    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
-    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
     GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
-    GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
-    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
-    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
-    RelationalDatabaseParameterOutputTypeDef,
+    RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
-    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
-    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
-    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetStaticIpsRequestRequestTypeDef,
     HostKeyAttributesTypeDef,
     ImportKeyPairRequestRequestTypeDef,
     PasswordDataTypeDef,
     InstanceHealthSummaryTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstancePortInfoTypeDef,
     MonthlyTransferTypeDef,
-    IsVpcPeeredResultTypeDef,
     OriginTypeDef,
     LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef,
     LoadBalancerTlsCertificateDomainValidationOptionTypeDef,
     LoadBalancerTlsCertificateSummaryTypeDef,
     NameServersUpdateStateTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PendingModifiedRelationalDatabaseValuesTypeDef,
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
-    RelationalDatabaseParameterTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
     StopGUISessionRequestRequestTypeDef,
@@ -678,24 +644,43 @@
     UpdateRelationalDatabaseRequestRequestTypeDef,
     AccessKeyTypeDef,
     AddOnRequestTypeDef,
     AlarmTypeDef,
     ContactMethodTypeDef,
     OperationTypeDef,
     StaticIpTypeDef,
+    DownloadDefaultKeyPairResultTypeDef,
+    GetActiveNamesResultTypeDef,
+    GetContainerAPIMetadataResultTypeDef,
+    GetDistributionLatestCacheResetResultTypeDef,
+    GetRelationalDatabaseLogStreamsResultTypeDef,
+    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
+    IsVpcPeeredResultTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
+    CreateBucketRequestRequestTypeDef,
+    CreateCertificateRequestRequestTypeDef,
+    CreateDiskSnapshotRequestRequestTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    CreateInstanceSnapshotRequestRequestTypeDef,
+    CreateKeyPairRequestRequestTypeDef,
+    CreateLoadBalancerRequestRequestTypeDef,
+    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    CreateRelationalDatabaseRequestRequestTypeDef,
+    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetBundlesResultTypeDef,
     CacheSettingsOutputTypeDef,
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
@@ -704,57 +689,65 @@
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
-    CreateBucketRequestRequestTypeDef,
-    CreateCertificateRequestRequestTypeDef,
-    CreateDiskSnapshotRequestRequestTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    CreateInstanceSnapshotRequestRequestTypeDef,
-    CreateKeyPairRequestRequestTypeDef,
-    CreateLoadBalancerRequestRequestTypeDef,
-    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    CreateRelationalDatabaseRequestRequestTypeDef,
-    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
+    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
+    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
+    GetBundlesRequestGetBundlesPaginateTypeDef,
+    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
+    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
+    GetDisksRequestGetDisksPaginateTypeDef,
+    GetDomainsRequestGetDomainsPaginateTypeDef,
+    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
+    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
+    GetInstancesRequestGetInstancesPaginateTypeDef,
+    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
+    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
+    GetOperationsRequestGetOperationsPaginateTypeDef,
+    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
+    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
+    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
+    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
+    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetBucketMetricDataResultTypeDef,
     GetContainerServiceMetricDataResultTypeDef,
     GetDistributionMetricDataResultTypeDef,
     GetInstanceMetricDataResultTypeDef,
     GetLoadBalancerMetricDataResultTypeDef,
     GetRelationalDatabaseMetricDataResultTypeDef,
     GetInstancePortStatesResultTypeDef,
     GetInstanceStateResultTypeDef,
     GetLoadBalancerTlsPoliciesResultTypeDef,
     GetRelationalDatabaseBlueprintsResultTypeDef,
     GetRelationalDatabaseBundlesResultTypeDef,
     GetRelationalDatabaseEventsResultTypeDef,
     GetRelationalDatabaseLogEventsResultTypeDef,
     GetRelationalDatabaseParametersResultTypeDef,
+    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     InstanceAccessDetailsTypeDef,
     InstanceNetworkingTypeDef,
     LoadBalancerTlsCertificateDomainValidationRecordTypeDef,
     LoadBalancerTlsCertificateRenewalSummaryTypeDef,
     LoadBalancerTypeDef,
     RegisteredDomainDelegationInfoTypeDef,
     RelationalDatabaseTypeDef,
-    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     GetBucketAccessKeysResultTypeDef,
     CreateDiskFromSnapshotRequestRequestTypeDef,
     CreateDiskRequestRequestTypeDef,
     CreateInstancesFromSnapshotRequestRequestTypeDef,
     CreateInstancesRequestRequestTypeDef,
     EnableAddOnRequestRequestTypeDef,
     GetAlarmsResultTypeDef,
```

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__init__.py` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__init__.pyi` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/__main__.py` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Lightsail 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Lightsail 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
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

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/client.py` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/client.pyi` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/literals.py` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/literals.pyi` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/paginator.py` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 class GetActiveNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getactivenamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetActiveNamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getactivenamespaginator)
         """
 
 
@@ -148,15 +148,15 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getblueprintspaginator)
         """
 
 
@@ -167,195 +167,195 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getbundlespaginator)
         """
 
 
 class GetCloudFormationStackRecordsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getcloudformationstackrecordspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCloudFormationStackRecordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getcloudformationstackrecordspaginator)
         """
 
 
 class GetDiskSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdisksnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDiskSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdisksnapshotspaginator)
         """
 
 
 class GetDisksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdiskspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDisksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdiskspaginator)
         """
 
 
 class GetDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdomainspaginator)
         """
 
 
 class GetExportSnapshotRecordsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getexportsnapshotrecordspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetExportSnapshotRecordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getexportsnapshotrecordspaginator)
         """
 
 
 class GetInstanceSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancesnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInstanceSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancesnapshotspaginator)
         """
 
 
 class GetInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInstancesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancespaginator)
         """
 
 
 class GetKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getkeypairspaginator)
     """
 
     def paginate(
-        self, *, includeDefaultKeyPair: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, includeDefaultKeyPair: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetKeyPairsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getkeypairspaginator)
         """
 
 
 class GetLoadBalancersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetLoadBalancersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getloadbalancerspaginator)
         """
 
 
 class GetOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOperationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getoperationspaginator)
         """
 
 
 class GetRelationalDatabaseBlueprintsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseblueprintspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseblueprintspaginator)
         """
 
 
 class GetRelationalDatabaseBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasebundlespaginator)
     """
 
     def paginate(
-        self, *, includeInactive: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, includeInactive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasebundlespaginator)
         """
 
 
@@ -366,73 +366,73 @@
     """
 
     def paginate(
         self,
         *,
         relationalDatabaseName: str,
         durationInMinutes: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseEventsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseeventspaginator)
         """
 
 
 class GetRelationalDatabaseParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseparameterspaginator)
     """
 
     def paginate(
-        self, *, relationalDatabaseName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, relationalDatabaseName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseparameterspaginator)
         """
 
 
 class GetRelationalDatabaseSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasesnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasesnapshotspaginator)
         """
 
 
 class GetRelationalDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabasesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasespaginator)
         """
 
 
 class GetStaticIpsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getstaticipspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetStaticIpsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getstaticipspaginator)
         """
```

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/paginator.pyi` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 class GetActiveNamesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getactivenamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetActiveNamesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetActiveNames.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getactivenamespaginator)
         """
 
 class GetBlueprintsPaginator(Paginator):
@@ -143,15 +143,15 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getblueprintspaginator)
         """
 
 class GetBundlesPaginator(Paginator):
@@ -161,183 +161,183 @@
     """
 
     def paginate(
         self,
         *,
         includeInactive: bool = ...,
         appCategory: Literal["LfR"] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getbundlespaginator)
         """
 
 class GetCloudFormationStackRecordsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getcloudformationstackrecordspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetCloudFormationStackRecordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetCloudFormationStackRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getcloudformationstackrecordspaginator)
         """
 
 class GetDiskSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdisksnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDiskSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDiskSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdisksnapshotspaginator)
         """
 
 class GetDisksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdiskspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDisksResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDisks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdiskspaginator)
         """
 
 class GetDomainsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetDomains.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getdomainspaginator)
         """
 
 class GetExportSnapshotRecordsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getexportsnapshotrecordspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetExportSnapshotRecordsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetExportSnapshotRecords.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getexportsnapshotrecordspaginator)
         """
 
 class GetInstanceSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancesnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInstanceSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstanceSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancesnapshotspaginator)
         """
 
 class GetInstancesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetInstancesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getinstancespaginator)
         """
 
 class GetKeyPairsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getkeypairspaginator)
     """
 
     def paginate(
-        self, *, includeDefaultKeyPair: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, includeDefaultKeyPair: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetKeyPairsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetKeyPairs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getkeypairspaginator)
         """
 
 class GetLoadBalancersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getloadbalancerspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetLoadBalancersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetLoadBalancers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getloadbalancerspaginator)
         """
 
 class GetOperationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getoperationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetOperationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getoperationspaginator)
         """
 
 class GetRelationalDatabaseBlueprintsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseblueprintspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseBlueprintsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBlueprints.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseblueprintspaginator)
         """
 
 class GetRelationalDatabaseBundlesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasebundlespaginator)
     """
 
     def paginate(
-        self, *, includeInactive: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, includeInactive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseBundlesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseBundles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasebundlespaginator)
         """
 
 class GetRelationalDatabaseEventsPaginator(Paginator):
@@ -347,69 +347,69 @@
     """
 
     def paginate(
         self,
         *,
         relationalDatabaseName: str,
         durationInMinutes: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseEventsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseeventspaginator)
         """
 
 class GetRelationalDatabaseParametersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseparameterspaginator)
     """
 
     def paginate(
-        self, *, relationalDatabaseName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, relationalDatabaseName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseParametersResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseParameters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabaseparameterspaginator)
         """
 
 class GetRelationalDatabaseSnapshotsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasesnapshotspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabaseSnapshotsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabaseSnapshots.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasesnapshotspaginator)
         """
 
 class GetRelationalDatabasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetRelationalDatabasesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetRelationalDatabases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getrelationaldatabasespaginator)
         """
 
 class GetStaticIpsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getstaticipspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetStaticIpsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Paginator.GetStaticIps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/paginators/#getstaticipspaginator)
         """
```

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/type_defs.py` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,40 +99,37 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessKeyLastUsedTypeDef",
-    "AccessRulesOutputTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
     "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
     "MonitoredResourceInfoTypeDef",
     "ResourceLocationTypeDef",
     "AllocateStaticIpRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AttachCertificateToDistributionRequestRequestTypeDef",
     "AttachDiskRequestRequestTypeDef",
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     "AttachLoadBalancerTlsCertificateRequestRequestTypeDef",
     "AttachStaticIpRequestRequestTypeDef",
     "AttachedDiskTypeDef",
     "AvailabilityZoneTypeDef",
     "BlueprintTypeDef",
-    "BucketAccessLogConfigOutputTypeDef",
     "BucketAccessLogConfigTypeDef",
     "BucketBundleTypeDef",
     "BucketStateTypeDef",
     "ResourceReceivingAccessTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "BundleTypeDef",
-    "CacheBehaviorOutputTypeDef",
-    "CacheBehaviorPerPathOutputTypeDef",
     "CacheBehaviorPerPathTypeDef",
     "CacheBehaviorTypeDef",
     "CookieObjectOutputTypeDef",
     "HeaderObjectOutputTypeDef",
     "QueryStringObjectOutputTypeDef",
     "CookieObjectTypeDef",
     "HeaderObjectTypeDef",
@@ -141,23 +138,21 @@
     "CloudFormationStackRecordSourceInfoTypeDef",
     "DestinationInfoTypeDef",
     "ContainerImageTypeDef",
     "ContainerOutputTypeDef",
     "ContainerTypeDef",
     "ContainerServiceECRImagePullerRoleRequestTypeDef",
     "ContainerServiceECRImagePullerRoleTypeDef",
-    "ContainerServiceHealthCheckConfigOutputTypeDef",
     "ContainerServiceHealthCheckConfigTypeDef",
     "ContainerServiceLogEventTypeDef",
     "ContainerServicePowerTypeDef",
     "ContainerServiceRegistryLoginTypeDef",
     "ContainerServiceStateDetailTypeDef",
     "CopySnapshotRequestRequestTypeDef",
     "CreateBucketAccessKeyRequestRequestTypeDef",
-    "TagTypeDef",
     "InstanceEntryTypeDef",
     "CreateContactMethodRequestRequestTypeDef",
     "InputOriginTypeDef",
     "DomainEntryTypeDef",
     "CreateGUISessionAccessDetailsRequestRequestTypeDef",
     "SessionTypeDef",
     "DiskMapTypeDef",
@@ -188,139 +183,110 @@
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
     "DomainEntryOutputTypeDef",
     "ResourceRecordTypeDef",
-    "DownloadDefaultKeyPairResultTypeDef",
     "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
-    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
-    "GetActiveNamesResultTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
-    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBlueprintsRequestRequestTypeDef",
     "GetBucketAccessKeysRequestRequestTypeDef",
     "GetBucketBundlesRequestRequestTypeDef",
     "GetBucketMetricDataRequestRequestTypeDef",
     "MetricDatapointTypeDef",
     "GetBucketsRequestRequestTypeDef",
-    "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetBundlesRequestRequestTypeDef",
     "GetCertificatesRequestRequestTypeDef",
-    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     "GetContactMethodsRequestRequestTypeDef",
-    "GetContainerAPIMetadataResultTypeDef",
     "GetContainerImagesRequestRequestTypeDef",
     "GetContainerLogRequestRequestTypeDef",
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     "GetContainerServiceMetricDataRequestRequestTypeDef",
     "GetContainerServicesRequestRequestTypeDef",
     "GetCostEstimateRequestRequestTypeDef",
     "GetDiskRequestRequestTypeDef",
     "GetDiskSnapshotRequestRequestTypeDef",
-    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
     "GetDiskSnapshotsRequestRequestTypeDef",
-    "GetDisksRequestGetDisksPaginateTypeDef",
     "GetDisksRequestRequestTypeDef",
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
-    "GetDistributionLatestCacheResetResultTypeDef",
     "GetDistributionMetricDataRequestRequestTypeDef",
     "GetDistributionsRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
-    "GetDomainsRequestGetDomainsPaginateTypeDef",
     "GetDomainsRequestRequestTypeDef",
-    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     "GetInstanceAccessDetailsRequestRequestTypeDef",
     "GetInstanceMetricDataRequestRequestTypeDef",
     "GetInstancePortStatesRequestRequestTypeDef",
     "InstancePortStateTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "GetInstanceSnapshotRequestRequestTypeDef",
-    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
     "GetInstanceSnapshotsRequestRequestTypeDef",
     "GetInstanceStateRequestRequestTypeDef",
     "InstanceStateTypeDef",
-    "GetInstancesRequestGetInstancesPaginateTypeDef",
     "GetInstancesRequestRequestTypeDef",
     "GetKeyPairRequestRequestTypeDef",
-    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
     "GetKeyPairsRequestRequestTypeDef",
     "GetLoadBalancerMetricDataRequestRequestTypeDef",
     "GetLoadBalancerRequestRequestTypeDef",
     "GetLoadBalancerTlsCertificatesRequestRequestTypeDef",
     "GetLoadBalancerTlsPoliciesRequestRequestTypeDef",
     "LoadBalancerTlsPolicyTypeDef",
-    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
     "GetLoadBalancersRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "GetOperationsForResourceRequestRequestTypeDef",
-    "GetOperationsRequestGetOperationsPaginateTypeDef",
     "GetOperationsRequestRequestTypeDef",
     "GetRegionsRequestRequestTypeDef",
-    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     "RelationalDatabaseBlueprintTypeDef",
-    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     "RelationalDatabaseBundleTypeDef",
-    "GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
     "GetRelationalDatabaseEventsRequestRequestTypeDef",
     "RelationalDatabaseEventTypeDef",
     "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
     "LogEventTypeDef",
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
-    "GetRelationalDatabaseLogStreamsResultTypeDef",
     "GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
-    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
-    "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
     "GetRelationalDatabaseParametersRequestRequestTypeDef",
-    "RelationalDatabaseParameterOutputTypeDef",
+    "RelationalDatabaseParameterTypeDef",
     "GetRelationalDatabaseRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
-    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
-    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
     "GetRelationalDatabasesRequestRequestTypeDef",
     "GetStaticIpRequestRequestTypeDef",
-    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     "GetStaticIpsRequestRequestTypeDef",
     "HostKeyAttributesTypeDef",
     "ImportKeyPairRequestRequestTypeDef",
     "PasswordDataTypeDef",
     "InstanceHealthSummaryTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstancePortInfoTypeDef",
     "MonthlyTransferTypeDef",
-    "IsVpcPeeredResultTypeDef",
     "OriginTypeDef",
     "LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef",
     "LoadBalancerTlsCertificateDomainValidationOptionTypeDef",
     "LoadBalancerTlsCertificateSummaryTypeDef",
     "NameServersUpdateStateTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PendingModifiedRelationalDatabaseValuesTypeDef",
     "PutAlarmRequestRequestTypeDef",
     "R53HostedZoneDeletionStateTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RebootRelationalDatabaseRequestRequestTypeDef",
     "RegisterContainerImageRequestRequestTypeDef",
     "RelationalDatabaseEndpointTypeDef",
     "RelationalDatabaseHardwareTypeDef",
-    "RelationalDatabaseParameterTypeDef",
     "ReleaseStaticIpRequestRequestTypeDef",
     "ResetDistributionCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SendContactMethodVerificationRequestRequestTypeDef",
     "SetIpAddressTypeRequestRequestTypeDef",
     "SetResourceAccessForBucketRequestRequestTypeDef",
     "StartGUISessionRequestRequestTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartRelationalDatabaseRequestRequestTypeDef",
     "StopGUISessionRequestRequestTypeDef",
@@ -335,24 +301,43 @@
     "UpdateRelationalDatabaseRequestRequestTypeDef",
     "AccessKeyTypeDef",
     "AddOnRequestTypeDef",
     "AlarmTypeDef",
     "ContactMethodTypeDef",
     "OperationTypeDef",
     "StaticIpTypeDef",
+    "DownloadDefaultKeyPairResultTypeDef",
+    "GetActiveNamesResultTypeDef",
+    "GetContainerAPIMetadataResultTypeDef",
+    "GetDistributionLatestCacheResetResultTypeDef",
+    "GetRelationalDatabaseLogStreamsResultTypeDef",
+    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
+    "IsVpcPeeredResultTypeDef",
     "AutoSnapshotDetailsTypeDef",
     "RegionTypeDef",
     "GetBlueprintsResultTypeDef",
     "UpdateBucketRequestRequestTypeDef",
     "GetBucketBundlesResultTypeDef",
     "BucketTypeDef",
+    "CreateBucketRequestRequestTypeDef",
+    "CreateCertificateRequestRequestTypeDef",
+    "CreateDiskSnapshotRequestRequestTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "CreateInstanceSnapshotRequestRequestTypeDef",
+    "CreateKeyPairRequestRequestTypeDef",
+    "CreateLoadBalancerRequestRequestTypeDef",
+    "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
+    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    "CreateRelationalDatabaseRequestRequestTypeDef",
+    "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     "DiskSnapshotTypeDef",
     "DiskTypeDef",
     "KeyPairTypeDef",
     "RelationalDatabaseSnapshotTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "GetBundlesResultTypeDef",
     "CacheSettingsOutputTypeDef",
     "CacheSettingsTypeDef",
     "CloseInstancePublicPortsRequestRequestTypeDef",
     "OpenInstancePublicPortsRequestRequestTypeDef",
     "PutInstancePublicPortsRequestRequestTypeDef",
     "CloudFormationStackRecordTypeDef",
@@ -361,57 +346,65 @@
     "PrivateRegistryAccessRequestTypeDef",
     "PrivateRegistryAccessTypeDef",
     "ContainerServiceEndpointTypeDef",
     "EndpointRequestTypeDef",
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
-    "CreateBucketRequestRequestTypeDef",
-    "CreateCertificateRequestRequestTypeDef",
-    "CreateDiskSnapshotRequestRequestTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "CreateInstanceSnapshotRequestRequestTypeDef",
-    "CreateKeyPairRequestRequestTypeDef",
-    "CreateLoadBalancerRequestRequestTypeDef",
-    "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
-    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
-    "CreateRelationalDatabaseRequestRequestTypeDef",
-    "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateCloudFormationStackRequestRequestTypeDef",
     "CreateDomainEntryRequestRequestTypeDef",
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
     "CreateGUISessionAccessDetailsResultTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
     "DomainValidationRecordTypeDef",
     "EstimateByTimeTypeDef",
+    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
+    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
+    "GetBundlesRequestGetBundlesPaginateTypeDef",
+    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
+    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
+    "GetDisksRequestGetDisksPaginateTypeDef",
+    "GetDomainsRequestGetDomainsPaginateTypeDef",
+    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
+    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
+    "GetInstancesRequestGetInstancesPaginateTypeDef",
+    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
+    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
+    "GetOperationsRequestGetOperationsPaginateTypeDef",
+    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
+    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
+    "GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
+    "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
+    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
+    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
+    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     "GetBucketMetricDataResultTypeDef",
     "GetContainerServiceMetricDataResultTypeDef",
     "GetDistributionMetricDataResultTypeDef",
     "GetInstanceMetricDataResultTypeDef",
     "GetLoadBalancerMetricDataResultTypeDef",
     "GetRelationalDatabaseMetricDataResultTypeDef",
     "GetInstancePortStatesResultTypeDef",
     "GetInstanceStateResultTypeDef",
     "GetLoadBalancerTlsPoliciesResultTypeDef",
     "GetRelationalDatabaseBlueprintsResultTypeDef",
     "GetRelationalDatabaseBundlesResultTypeDef",
     "GetRelationalDatabaseEventsResultTypeDef",
     "GetRelationalDatabaseLogEventsResultTypeDef",
     "GetRelationalDatabaseParametersResultTypeDef",
+    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     "InstanceAccessDetailsTypeDef",
     "InstanceNetworkingTypeDef",
     "LoadBalancerTlsCertificateDomainValidationRecordTypeDef",
     "LoadBalancerTlsCertificateRenewalSummaryTypeDef",
     "LoadBalancerTypeDef",
     "RegisteredDomainDelegationInfoTypeDef",
     "RelationalDatabaseTypeDef",
-    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     "GetBucketAccessKeysResultTypeDef",
     "CreateDiskFromSnapshotRequestRequestTypeDef",
     "CreateDiskRequestRequestTypeDef",
     "CreateInstancesFromSnapshotRequestRequestTypeDef",
     "CreateInstancesRequestRequestTypeDef",
     "EnableAddOnRequestRequestTypeDef",
     "GetAlarmsResultTypeDef",
@@ -568,23 +561,14 @@
         "lastUsedDate": datetime,
         "region": str,
         "serviceName": str,
     },
     total=False,
 )
 
-AccessRulesOutputTypeDef = TypedDict(
-    "AccessRulesOutputTypeDef",
-    {
-        "getObject": AccessTypeType,
-        "allowPublicOverrides": bool,
-    },
-    total=False,
-)
-
 AccessRulesTypeDef = TypedDict(
     "AccessRulesTypeDef",
     {
         "getObject": AccessTypeType,
         "allowPublicOverrides": bool,
     },
     total=False,
@@ -653,14 +637,25 @@
 AllocateStaticIpRequestRequestTypeDef = TypedDict(
     "AllocateStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
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
 AttachCertificateToDistributionRequestRequestTypeDef = TypedDict(
     "AttachCertificateToDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "certificateName": str,
     },
 )
@@ -746,36 +741,14 @@
         "licenseUrl": str,
         "platform": InstancePlatformType,
         "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
-_RequiredBucketAccessLogConfigOutputTypeDef = TypedDict(
-    "_RequiredBucketAccessLogConfigOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalBucketAccessLogConfigOutputTypeDef = TypedDict(
-    "_OptionalBucketAccessLogConfigOutputTypeDef",
-    {
-        "destination": str,
-        "prefix": str,
-    },
-    total=False,
-)
-
-
-class BucketAccessLogConfigOutputTypeDef(
-    _RequiredBucketAccessLogConfigOutputTypeDef, _OptionalBucketAccessLogConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredBucketAccessLogConfigTypeDef = TypedDict(
     "_RequiredBucketAccessLogConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalBucketAccessLogConfigTypeDef = TypedDict(
@@ -821,16 +794,16 @@
     {
         "name": str,
         "resourceType": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
@@ -849,31 +822,14 @@
         "transferPerMonthInGb": int,
         "supportedPlatforms": List[InstancePlatformType],
         "supportedAppCategories": List[Literal["LfR"]],
     },
     total=False,
 )
 
-CacheBehaviorOutputTypeDef = TypedDict(
-    "CacheBehaviorOutputTypeDef",
-    {
-        "behavior": BehaviorEnumType,
-    },
-    total=False,
-)
-
-CacheBehaviorPerPathOutputTypeDef = TypedDict(
-    "CacheBehaviorPerPathOutputTypeDef",
-    {
-        "path": str,
-        "behavior": BehaviorEnumType,
-    },
-    total=False,
-)
-
 CacheBehaviorPerPathTypeDef = TypedDict(
     "CacheBehaviorPerPathTypeDef",
     {
         "path": str,
         "behavior": BehaviorEnumType,
     },
     total=False,
@@ -1018,27 +974,14 @@
     {
         "isActive": bool,
         "principalArn": str,
     },
     total=False,
 )
 
-ContainerServiceHealthCheckConfigOutputTypeDef = TypedDict(
-    "ContainerServiceHealthCheckConfigOutputTypeDef",
-    {
-        "healthyThreshold": int,
-        "unhealthyThreshold": int,
-        "timeoutSeconds": int,
-        "intervalSeconds": int,
-        "path": str,
-        "successCodes": str,
-    },
-    total=False,
-)
-
 ContainerServiceHealthCheckConfigTypeDef = TypedDict(
     "ContainerServiceHealthCheckConfigTypeDef",
     {
         "healthyThreshold": int,
         "unhealthyThreshold": int,
         "timeoutSeconds": int,
         "intervalSeconds": int,
@@ -1118,23 +1061,14 @@
 CreateBucketAccessKeyRequestRequestTypeDef = TypedDict(
     "CreateBucketAccessKeyRequestRequestTypeDef",
     {
         "bucketName": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 _RequiredInstanceEntryTypeDef = TypedDict(
     "_RequiredInstanceEntryTypeDef",
     {
         "sourceName": str,
         "instanceType": str,
         "portInfoSource": PortInfoSourceTypeType,
         "availabilityZone": str,
@@ -1538,24 +1472,14 @@
         "name": str,
         "type": str,
         "value": str,
     },
     total=False,
 )
 
-DownloadDefaultKeyPairResultTypeDef = TypedDict(
-    "DownloadDefaultKeyPairResultTypeDef",
-    {
-        "publicKeyBase64": str,
-        "privateKeyBase64": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimePeriodTypeDef = TypedDict(
     "TimePeriodTypeDef",
     {
         "start": datetime,
         "end": datetime,
     },
     total=False,
@@ -1564,39 +1488,32 @@
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "sourceSnapshotName": str,
     },
 )
 
-GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
-    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
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
 
 GetActiveNamesRequestRequestTypeDef = TypedDict(
     "GetActiveNamesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-GetActiveNamesResultTypeDef = TypedDict(
-    "GetActiveNamesResultTypeDef",
-    {
-        "activeNames": List[str],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAlarmsRequestRequestTypeDef = TypedDict(
     "GetAlarmsRequestRequestTypeDef",
     {
         "alarmName": str,
         "pageToken": str,
         "monitoredResourceName": str,
     },
@@ -1606,24 +1523,14 @@
 GetAutoSnapshotsRequestRequestTypeDef = TypedDict(
     "GetAutoSnapshotsRequestRequestTypeDef",
     {
         "resourceName": str,
     },
 )
 
-GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
-    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "appCategory": Literal["LfR"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBlueprintsRequestRequestTypeDef = TypedDict(
     "GetBlueprintsRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
         "appCategory": Literal["LfR"],
     },
@@ -1678,24 +1585,14 @@
         "bucketName": str,
         "pageToken": str,
         "includeConnectedResources": bool,
     },
     total=False,
 )
 
-GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
-    "GetBundlesRequestGetBundlesPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "appCategory": Literal["LfR"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBundlesRequestRequestTypeDef = TypedDict(
     "GetBundlesRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
         "appCategory": Literal["LfR"],
     },
@@ -1709,22 +1606,14 @@
         "includeCertificateDetails": bool,
         "certificateName": str,
         "pageToken": str,
     },
     total=False,
 )
 
-GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
-    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetCloudFormationStackRecordsRequestRequestTypeDef = TypedDict(
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1733,22 +1622,14 @@
     "GetContactMethodsRequestRequestTypeDef",
     {
         "protocols": Sequence[ContactProtocolType],
     },
     total=False,
 )
 
-GetContainerAPIMetadataResultTypeDef = TypedDict(
-    "GetContainerAPIMetadataResultTypeDef",
-    {
-        "metadata": List[Dict[str, str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContainerImagesRequestRequestTypeDef = TypedDict(
     "GetContainerImagesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
@@ -1823,38 +1704,22 @@
 GetDiskSnapshotRequestRequestTypeDef = TypedDict(
     "GetDiskSnapshotRequestRequestTypeDef",
     {
         "diskSnapshotName": str,
     },
 )
 
-GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = TypedDict(
-    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDiskSnapshotsRequestRequestTypeDef = TypedDict(
     "GetDiskSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-GetDisksRequestGetDisksPaginateTypeDef = TypedDict(
-    "GetDisksRequestGetDisksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDisksRequestRequestTypeDef = TypedDict(
     "GetDisksRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1863,23 +1728,14 @@
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
 )
 
-GetDistributionLatestCacheResetResultTypeDef = TypedDict(
-    "GetDistributionLatestCacheResetResultTypeDef",
-    {
-        "status": str,
-        "createTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDistributionMetricDataRequestRequestTypeDef = TypedDict(
     "GetDistributionMetricDataRequestRequestTypeDef",
     {
         "distributionName": str,
         "metricName": DistributionMetricNameType,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
@@ -1901,38 +1757,22 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 
-GetDomainsRequestGetDomainsPaginateTypeDef = TypedDict(
-    "GetDomainsRequestGetDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDomainsRequestRequestTypeDef = TypedDict(
     "GetDomainsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = TypedDict(
-    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetExportSnapshotRecordsRequestRequestTypeDef = TypedDict(
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2003,22 +1843,14 @@
 GetInstanceSnapshotRequestRequestTypeDef = TypedDict(
     "GetInstanceSnapshotRequestRequestTypeDef",
     {
         "instanceSnapshotName": str,
     },
 )
 
-GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = TypedDict(
-    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInstanceSnapshotsRequestRequestTypeDef = TypedDict(
     "GetInstanceSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2035,22 +1867,14 @@
     {
         "code": int,
         "name": str,
     },
     total=False,
 )
 
-GetInstancesRequestGetInstancesPaginateTypeDef = TypedDict(
-    "GetInstancesRequestGetInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInstancesRequestRequestTypeDef = TypedDict(
     "GetInstancesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2058,23 +1882,14 @@
 GetKeyPairRequestRequestTypeDef = TypedDict(
     "GetKeyPairRequestRequestTypeDef",
     {
         "keyPairName": str,
     },
 )
 
-GetKeyPairsRequestGetKeyPairsPaginateTypeDef = TypedDict(
-    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
-    {
-        "includeDefaultKeyPair": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetKeyPairsRequestRequestTypeDef = TypedDict(
     "GetKeyPairsRequestRequestTypeDef",
     {
         "pageToken": str,
         "includeDefaultKeyPair": bool,
     },
     total=False,
@@ -2123,22 +1938,14 @@
         "description": str,
         "protocols": List[str],
         "ciphers": List[str],
     },
     total=False,
 )
 
-GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = TypedDict(
-    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetLoadBalancersRequestRequestTypeDef = TypedDict(
     "GetLoadBalancersRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2168,22 +1975,14 @@
 class GetOperationsForResourceRequestRequestTypeDef(
     _RequiredGetOperationsForResourceRequestRequestTypeDef,
     _OptionalGetOperationsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-GetOperationsRequestGetOperationsPaginateTypeDef = TypedDict(
-    "GetOperationsRequestGetOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetOperationsRequestRequestTypeDef = TypedDict(
     "GetOperationsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2193,22 +1992,14 @@
     {
         "includeAvailabilityZones": bool,
         "includeRelationalDatabaseAvailabilityZones": bool,
     },
     total=False,
 )
 
-GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRelationalDatabaseBlueprintsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2222,23 +2013,14 @@
         "engineDescription": str,
         "engineVersionDescription": str,
         "isEngineDefault": bool,
     },
     total=False,
 )
 
-GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRelationalDatabaseBundlesRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     {
         "pageToken": str,
         "includeInactive": bool,
     },
     total=False,
@@ -2256,37 +2038,14 @@
         "cpuCount": int,
         "isEncrypted": bool,
         "isActive": bool,
     },
     total=False,
 )
 
-_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    {
-        "durationInMinutes": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef(
-    _RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-    _OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRelationalDatabaseEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseEventsRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseEventsRequestRequestTypeDef = TypedDict(
@@ -2355,22 +2114,14 @@
 GetRelationalDatabaseLogStreamsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 
-GetRelationalDatabaseLogStreamsResultTypeDef = TypedDict(
-    "GetRelationalDatabaseLogStreamsResultTypeDef",
-    {
-        "logStreams": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef = TypedDict(
@@ -2385,58 +2136,27 @@
 class GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
 ):
     pass
 
 
-GetRelationalDatabaseMasterUserPasswordResultTypeDef = TypedDict(
-    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
-    {
-        "masterUserPassword": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRelationalDatabaseMetricDataRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "metricName": RelationalDatabaseMetricNameType,
         "period": int,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "unit": MetricUnitType,
         "statistics": Sequence[MetricStatisticType],
     },
 )
 
-_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef(
-    _RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-    _OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
@@ -2451,16 +2171,16 @@
 class GetRelationalDatabaseParametersRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef,
 ):
     pass
 
 
-RelationalDatabaseParameterOutputTypeDef = TypedDict(
-    "RelationalDatabaseParameterOutputTypeDef",
+RelationalDatabaseParameterTypeDef = TypedDict(
+    "RelationalDatabaseParameterTypeDef",
     {
         "allowedValues": str,
         "applyMethod": str,
         "applyType": str,
         "dataType": str,
         "description": str,
         "isModifiable": bool,
@@ -2480,38 +2200,22 @@
 GetRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseSnapshotName": str,
     },
 )
 
-GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRelationalDatabaseSnapshotsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = TypedDict(
-    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRelationalDatabasesRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabasesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2519,22 +2223,14 @@
 GetStaticIpRequestRequestTypeDef = TypedDict(
     "GetStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
     },
 )
 
-GetStaticIpsRequestGetStaticIpsPaginateTypeDef = TypedDict(
-    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetStaticIpsRequestRequestTypeDef = TypedDict(
     "GetStaticIpsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2613,22 +2309,14 @@
     "MonthlyTransferTypeDef",
     {
         "gbPerMonthAllocated": int,
     },
     total=False,
 )
 
-IsVpcPeeredResultTypeDef = TypedDict(
-    "IsVpcPeeredResultTypeDef",
-    {
-        "isPeered": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OriginTypeDef = TypedDict(
     "OriginTypeDef",
     {
         "name": str,
         "resourceType": ResourceTypeType,
         "regionName": RegionNameType,
         "protocolPolicy": OriginProtocolPolicyEnumType,
@@ -2668,24 +2356,14 @@
     {
         "code": NameServersUpdateStateCodeType,
         "message": str,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "action": str,
         "description": str,
         "currentApplyDate": datetime,
     },
@@ -2779,29 +2457,14 @@
         "cpuCount": int,
         "diskSizeInGb": int,
         "ramSizeInGb": float,
     },
     total=False,
 )
 
-RelationalDatabaseParameterTypeDef = TypedDict(
-    "RelationalDatabaseParameterTypeDef",
-    {
-        "allowedValues": str,
-        "applyMethod": str,
-        "applyType": str,
-        "dataType": str,
-        "description": str,
-        "isModifiable": bool,
-        "parameterName": str,
-        "parameterValue": str,
-    },
-    total=False,
-)
-
 ReleaseStaticIpRequestRequestTypeDef = TypedDict(
     "ReleaseStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
     },
 )
 
@@ -2809,25 +2472,14 @@
     "ResetDistributionCacheRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
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
 SendContactMethodVerificationRequestRequestTypeDef = TypedDict(
     "SendContactMethodVerificationRequestRequestTypeDef",
     {
         "protocol": Literal["Email"],
     },
 )
 
@@ -3137,14 +2789,75 @@
         "ipAddress": str,
         "attachedTo": str,
         "isAttached": bool,
     },
     total=False,
 )
 
+DownloadDefaultKeyPairResultTypeDef = TypedDict(
+    "DownloadDefaultKeyPairResultTypeDef",
+    {
+        "publicKeyBase64": str,
+        "privateKeyBase64": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetActiveNamesResultTypeDef = TypedDict(
+    "GetActiveNamesResultTypeDef",
+    {
+        "activeNames": List[str],
+        "nextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerAPIMetadataResultTypeDef = TypedDict(
+    "GetContainerAPIMetadataResultTypeDef",
+    {
+        "metadata": List[Dict[str, str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDistributionLatestCacheResetResultTypeDef = TypedDict(
+    "GetDistributionLatestCacheResetResultTypeDef",
+    {
+        "status": str,
+        "createTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRelationalDatabaseLogStreamsResultTypeDef = TypedDict(
+    "GetRelationalDatabaseLogStreamsResultTypeDef",
+    {
+        "logStreams": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRelationalDatabaseMasterUserPasswordResultTypeDef = TypedDict(
+    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
+    {
+        "masterUserPassword": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IsVpcPeeredResultTypeDef = TypedDict(
+    "IsVpcPeeredResultTypeDef",
+    {
+        "isPeered": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AutoSnapshotDetailsTypeDef = TypedDict(
     "AutoSnapshotDetailsTypeDef",
     {
         "date": str,
         "createdAt": datetime,
         "status": AutoSnapshotStatusType,
         "fromAttachedDisks": List[AttachedDiskTypeDef],
@@ -3166,15 +2879,15 @@
 )
 
 GetBlueprintsResultTypeDef = TypedDict(
     "GetBlueprintsResultTypeDef",
     {
         "blueprints": List[BlueprintTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBucketRequestRequestTypeDef",
     {
         "bucketName": str,
@@ -3198,290 +2911,41 @@
     pass
 
 
 GetBucketBundlesResultTypeDef = TypedDict(
     "GetBucketBundlesResultTypeDef",
     {
         "bundles": List[BucketBundleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "resourceType": str,
-        "accessRules": AccessRulesOutputTypeDef,
+        "accessRules": AccessRulesTypeDef,
         "arn": str,
         "bundleId": str,
         "createdAt": datetime,
         "url": str,
         "location": ResourceLocationTypeDef,
         "name": str,
         "supportCode": str,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "objectVersioning": str,
         "ableToUpdateBundle": bool,
         "readonlyAccessAccounts": List[str],
         "resourcesReceivingAccess": List[ResourceReceivingAccessTypeDef],
         "state": BucketStateTypeDef,
-        "accessLogConfig": BucketAccessLogConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-DiskSnapshotTypeDef = TypedDict(
-    "DiskSnapshotTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
-        "sizeInGb": int,
-        "state": DiskSnapshotStateType,
-        "progress": str,
-        "fromDiskName": str,
-        "fromDiskArn": str,
-        "fromInstanceName": str,
-        "fromInstanceArn": str,
-        "isFromAutoSnapshot": bool,
-    },
-    total=False,
-)
-
-DiskTypeDef = TypedDict(
-    "DiskTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
-        "addOns": List[AddOnTypeDef],
-        "sizeInGb": int,
-        "isSystemDisk": bool,
-        "iops": int,
-        "path": str,
-        "state": DiskStateType,
-        "attachedTo": str,
-        "isAttached": bool,
-        "attachmentState": str,
-        "gbInUse": int,
-        "autoMountStatus": AutoMountStatusType,
-    },
-    total=False,
-)
-
-KeyPairTypeDef = TypedDict(
-    "KeyPairTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
-        "fingerprint": str,
-    },
-    total=False,
-)
-
-RelationalDatabaseSnapshotTypeDef = TypedDict(
-    "RelationalDatabaseSnapshotTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
-        "engine": str,
-        "engineVersion": str,
-        "sizeInGb": int,
-        "state": str,
-        "fromRelationalDatabaseName": str,
-        "fromRelationalDatabaseArn": str,
-        "fromRelationalDatabaseBundleId": str,
-        "fromRelationalDatabaseBlueprintId": str,
-    },
-    total=False,
-)
-
-GetBundlesResultTypeDef = TypedDict(
-    "GetBundlesResultTypeDef",
-    {
-        "bundles": List[BundleTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CacheSettingsOutputTypeDef = TypedDict(
-    "CacheSettingsOutputTypeDef",
-    {
-        "defaultTTL": int,
-        "minimumTTL": int,
-        "maximumTTL": int,
-        "allowedHTTPMethods": str,
-        "cachedHTTPMethods": str,
-        "forwardedCookies": CookieObjectOutputTypeDef,
-        "forwardedHeaders": HeaderObjectOutputTypeDef,
-        "forwardedQueryStrings": QueryStringObjectOutputTypeDef,
-    },
-    total=False,
-)
-
-CacheSettingsTypeDef = TypedDict(
-    "CacheSettingsTypeDef",
-    {
-        "defaultTTL": int,
-        "minimumTTL": int,
-        "maximumTTL": int,
-        "allowedHTTPMethods": str,
-        "cachedHTTPMethods": str,
-        "forwardedCookies": CookieObjectTypeDef,
-        "forwardedHeaders": HeaderObjectTypeDef,
-        "forwardedQueryStrings": QueryStringObjectTypeDef,
-    },
-    total=False,
-)
-
-CloseInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "CloseInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfo": PortInfoTypeDef,
-        "instanceName": str,
-    },
-)
-
-OpenInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "OpenInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfo": PortInfoTypeDef,
-        "instanceName": str,
-    },
-)
-
-PutInstancePublicPortsRequestRequestTypeDef = TypedDict(
-    "PutInstancePublicPortsRequestRequestTypeDef",
-    {
-        "portInfos": Sequence[PortInfoTypeDef],
-        "instanceName": str,
-    },
-)
-
-CloudFormationStackRecordTypeDef = TypedDict(
-    "CloudFormationStackRecordTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "state": RecordStateType,
-        "sourceInfo": List[CloudFormationStackRecordSourceInfoTypeDef],
-        "destinationInfo": DestinationInfoTypeDef,
-    },
-    total=False,
-)
-
-GetContainerImagesResultTypeDef = TypedDict(
-    "GetContainerImagesResultTypeDef",
-    {
-        "containerImages": List[ContainerImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RegisterContainerImageResultTypeDef = TypedDict(
-    "RegisterContainerImageResultTypeDef",
-    {
-        "containerImage": ContainerImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PrivateRegistryAccessRequestTypeDef = TypedDict(
-    "PrivateRegistryAccessRequestTypeDef",
-    {
-        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
-    },
-    total=False,
-)
-
-PrivateRegistryAccessTypeDef = TypedDict(
-    "PrivateRegistryAccessTypeDef",
-    {
-        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleTypeDef,
-    },
-    total=False,
-)
-
-ContainerServiceEndpointTypeDef = TypedDict(
-    "ContainerServiceEndpointTypeDef",
-    {
-        "containerName": str,
-        "containerPort": int,
-        "healthCheck": ContainerServiceHealthCheckConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-_RequiredEndpointRequestTypeDef = TypedDict(
-    "_RequiredEndpointRequestTypeDef",
-    {
-        "containerName": str,
-        "containerPort": int,
-    },
-)
-_OptionalEndpointRequestTypeDef = TypedDict(
-    "_OptionalEndpointRequestTypeDef",
-    {
-        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
+        "accessLogConfig": BucketAccessLogConfigTypeDef,
     },
     total=False,
 )
 
-
-class EndpointRequestTypeDef(_RequiredEndpointRequestTypeDef, _OptionalEndpointRequestTypeDef):
-    pass
-
-
-GetContainerLogResultTypeDef = TypedDict(
-    "GetContainerLogResultTypeDef",
-    {
-        "logEvents": List[ContainerServiceLogEventTypeDef],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetContainerServicePowersResultTypeDef = TypedDict(
-    "GetContainerServicePowersResultTypeDef",
-    {
-        "powers": List[ContainerServicePowerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
-    "CreateContainerServiceRegistryLoginResultTypeDef",
-    {
-        "registryLogin": ContainerServiceRegistryLoginTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBucketRequestRequestTypeDef",
     {
         "bucketName": str,
         "bundleId": str,
     },
 )
@@ -3746,14 +3210,98 @@
 class CreateRelationalDatabaseSnapshotRequestRequestTypeDef(
     _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     _OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
 ):
     pass
 
 
+DiskSnapshotTypeDef = TypedDict(
+    "DiskSnapshotTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagTypeDef],
+        "sizeInGb": int,
+        "state": DiskSnapshotStateType,
+        "progress": str,
+        "fromDiskName": str,
+        "fromDiskArn": str,
+        "fromInstanceName": str,
+        "fromInstanceArn": str,
+        "isFromAutoSnapshot": bool,
+    },
+    total=False,
+)
+
+DiskTypeDef = TypedDict(
+    "DiskTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagTypeDef],
+        "addOns": List[AddOnTypeDef],
+        "sizeInGb": int,
+        "isSystemDisk": bool,
+        "iops": int,
+        "path": str,
+        "state": DiskStateType,
+        "attachedTo": str,
+        "isAttached": bool,
+        "attachmentState": str,
+        "gbInUse": int,
+        "autoMountStatus": AutoMountStatusType,
+    },
+    total=False,
+)
+
+KeyPairTypeDef = TypedDict(
+    "KeyPairTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagTypeDef],
+        "fingerprint": str,
+    },
+    total=False,
+)
+
+RelationalDatabaseSnapshotTypeDef = TypedDict(
+    "RelationalDatabaseSnapshotTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "tags": List[TagTypeDef],
+        "engine": str,
+        "engineVersion": str,
+        "sizeInGb": int,
+        "state": str,
+        "fromRelationalDatabaseName": str,
+        "fromRelationalDatabaseArn": str,
+        "fromRelationalDatabaseBundleId": str,
+        "fromRelationalDatabaseBlueprintId": str,
+    },
+    total=False,
+)
+
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "resourceName": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -3768,14 +3316,179 @@
 
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
 
+GetBundlesResultTypeDef = TypedDict(
+    "GetBundlesResultTypeDef",
+    {
+        "bundles": List[BundleTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CacheSettingsOutputTypeDef = TypedDict(
+    "CacheSettingsOutputTypeDef",
+    {
+        "defaultTTL": int,
+        "minimumTTL": int,
+        "maximumTTL": int,
+        "allowedHTTPMethods": str,
+        "cachedHTTPMethods": str,
+        "forwardedCookies": CookieObjectOutputTypeDef,
+        "forwardedHeaders": HeaderObjectOutputTypeDef,
+        "forwardedQueryStrings": QueryStringObjectOutputTypeDef,
+    },
+    total=False,
+)
+
+CacheSettingsTypeDef = TypedDict(
+    "CacheSettingsTypeDef",
+    {
+        "defaultTTL": int,
+        "minimumTTL": int,
+        "maximumTTL": int,
+        "allowedHTTPMethods": str,
+        "cachedHTTPMethods": str,
+        "forwardedCookies": CookieObjectTypeDef,
+        "forwardedHeaders": HeaderObjectTypeDef,
+        "forwardedQueryStrings": QueryStringObjectTypeDef,
+    },
+    total=False,
+)
+
+CloseInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "CloseInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfo": PortInfoTypeDef,
+        "instanceName": str,
+    },
+)
+
+OpenInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "OpenInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfo": PortInfoTypeDef,
+        "instanceName": str,
+    },
+)
+
+PutInstancePublicPortsRequestRequestTypeDef = TypedDict(
+    "PutInstancePublicPortsRequestRequestTypeDef",
+    {
+        "portInfos": Sequence[PortInfoTypeDef],
+        "instanceName": str,
+    },
+)
+
+CloudFormationStackRecordTypeDef = TypedDict(
+    "CloudFormationStackRecordTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "state": RecordStateType,
+        "sourceInfo": List[CloudFormationStackRecordSourceInfoTypeDef],
+        "destinationInfo": DestinationInfoTypeDef,
+    },
+    total=False,
+)
+
+GetContainerImagesResultTypeDef = TypedDict(
+    "GetContainerImagesResultTypeDef",
+    {
+        "containerImages": List[ContainerImageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterContainerImageResultTypeDef = TypedDict(
+    "RegisterContainerImageResultTypeDef",
+    {
+        "containerImage": ContainerImageTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PrivateRegistryAccessRequestTypeDef = TypedDict(
+    "PrivateRegistryAccessRequestTypeDef",
+    {
+        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
+    },
+    total=False,
+)
+
+PrivateRegistryAccessTypeDef = TypedDict(
+    "PrivateRegistryAccessTypeDef",
+    {
+        "ecrImagePullerRole": ContainerServiceECRImagePullerRoleTypeDef,
+    },
+    total=False,
+)
+
+ContainerServiceEndpointTypeDef = TypedDict(
+    "ContainerServiceEndpointTypeDef",
+    {
+        "containerName": str,
+        "containerPort": int,
+        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredEndpointRequestTypeDef = TypedDict(
+    "_RequiredEndpointRequestTypeDef",
+    {
+        "containerName": str,
+        "containerPort": int,
+    },
+)
+_OptionalEndpointRequestTypeDef = TypedDict(
+    "_OptionalEndpointRequestTypeDef",
+    {
+        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class EndpointRequestTypeDef(_RequiredEndpointRequestTypeDef, _OptionalEndpointRequestTypeDef):
+    pass
+
+
+GetContainerLogResultTypeDef = TypedDict(
+    "GetContainerLogResultTypeDef",
+    {
+        "logEvents": List[ContainerServiceLogEventTypeDef],
+        "nextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerServicePowersResultTypeDef = TypedDict(
+    "GetContainerServicePowersResultTypeDef",
+    {
+        "powers": List[ContainerServicePowerTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
+    "CreateContainerServiceRegistryLoginResultTypeDef",
+    {
+        "registryLogin": ContainerServiceRegistryLoginTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateCloudFormationStackRequestRequestTypeDef = TypedDict(
     "CreateCloudFormationStackRequestRequestTypeDef",
     {
         "instances": Sequence[InstanceEntryTypeDef],
     },
 )
 
@@ -3807,15 +3520,15 @@
     "CreateGUISessionAccessDetailsResultTypeDef",
     {
         "resourceName": str,
         "status": StatusType,
         "percentageComplete": int,
         "failureReason": str,
         "sessions": List[SessionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceSnapshotInfoTypeDef = TypedDict(
     "InstanceSnapshotInfoTypeDef",
     {
         "fromBundleId": str,
@@ -3825,15 +3538,15 @@
     total=False,
 )
 
 GetDistributionBundlesResultTypeDef = TypedDict(
     "GetDistributionBundlesResultTypeDef",
     {
         "bundles": List[DistributionBundleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainValidationRecordTypeDef = TypedDict(
     "DomainValidationRecordTypeDef",
     {
         "domainName": str,
@@ -3852,136 +3565,339 @@
         "unit": float,
         "currency": Literal["USD"],
         "timePeriod": TimePeriodTypeDef,
     },
     total=False,
 )
 
+GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
+    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
+    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "appCategory": Literal["LfR"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
+    "GetBundlesRequestGetBundlesPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "appCategory": Literal["LfR"],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
+    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = TypedDict(
+    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetDisksRequestGetDisksPaginateTypeDef = TypedDict(
+    "GetDisksRequestGetDisksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetDomainsRequestGetDomainsPaginateTypeDef = TypedDict(
+    "GetDomainsRequestGetDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = TypedDict(
+    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = TypedDict(
+    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetInstancesRequestGetInstancesPaginateTypeDef = TypedDict(
+    "GetInstancesRequestGetInstancesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetKeyPairsRequestGetKeyPairsPaginateTypeDef = TypedDict(
+    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
+    {
+        "includeDefaultKeyPair": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = TypedDict(
+    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetOperationsRequestGetOperationsPaginateTypeDef = TypedDict(
+    "GetOperationsRequestGetOperationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
+    {
+        "includeInactive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
+    {
+        "durationInMinutes": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef(
+    _RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+    _OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef(
+    _RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+    _OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+):
+    pass
+
+
+GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = TypedDict(
+    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetStaticIpsRequestGetStaticIpsPaginateTypeDef = TypedDict(
+    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetBucketMetricDataResultTypeDef = TypedDict(
     "GetBucketMetricDataResultTypeDef",
     {
         "metricName": BucketMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContainerServiceMetricDataResultTypeDef = TypedDict(
     "GetContainerServiceMetricDataResultTypeDef",
     {
         "metricName": ContainerServiceMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionMetricDataResultTypeDef = TypedDict(
     "GetDistributionMetricDataResultTypeDef",
     {
         "metricName": DistributionMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceMetricDataResultTypeDef = TypedDict(
     "GetInstanceMetricDataResultTypeDef",
     {
         "metricName": InstanceMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoadBalancerMetricDataResultTypeDef = TypedDict(
     "GetLoadBalancerMetricDataResultTypeDef",
     {
         "metricName": LoadBalancerMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseMetricDataResultTypeDef = TypedDict(
     "GetRelationalDatabaseMetricDataResultTypeDef",
     {
         "metricName": RelationalDatabaseMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstancePortStatesResultTypeDef = TypedDict(
     "GetInstancePortStatesResultTypeDef",
     {
         "portStates": List[InstancePortStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceStateResultTypeDef = TypedDict(
     "GetInstanceStateResultTypeDef",
     {
         "state": InstanceStateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoadBalancerTlsPoliciesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsPoliciesResultTypeDef",
     {
         "tlsPolicies": List[LoadBalancerTlsPolicyTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseBlueprintsResultTypeDef = TypedDict(
     "GetRelationalDatabaseBlueprintsResultTypeDef",
     {
         "blueprints": List[RelationalDatabaseBlueprintTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseBundlesResultTypeDef = TypedDict(
     "GetRelationalDatabaseBundlesResultTypeDef",
     {
         "bundles": List[RelationalDatabaseBundleTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseEventsResultTypeDef = TypedDict(
     "GetRelationalDatabaseEventsResultTypeDef",
     {
         "relationalDatabaseEvents": List[RelationalDatabaseEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseLogEventsResultTypeDef = TypedDict(
     "GetRelationalDatabaseLogEventsResultTypeDef",
     {
         "resourceLogEvents": List[LogEventTypeDef],
         "nextBackwardToken": str,
         "nextForwardToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseParametersResultTypeDef = TypedDict(
     "GetRelationalDatabaseParametersResultTypeDef",
     {
-        "parameters": List[RelationalDatabaseParameterOutputTypeDef],
+        "parameters": List[RelationalDatabaseParameterTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
+    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "parameters": Sequence[RelationalDatabaseParameterTypeDef],
     },
 )
 
 InstanceAccessDetailsTypeDef = TypedDict(
     "InstanceAccessDetailsTypeDef",
     {
         "certKey": str,
@@ -4034,15 +3950,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "dnsName": str,
         "state": LoadBalancerStateType,
         "protocol": LoadBalancerProtocolType,
         "publicPorts": List[int],
         "healthCheckPath": str,
         "instancePort": int,
         "instanceHealthSummary": List[InstanceHealthSummaryTypeDef],
@@ -4069,15 +3985,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "relationalDatabaseBlueprintId": str,
         "relationalDatabaseBundleId": str,
         "masterDatabaseName": str,
         "hardware": RelationalDatabaseHardwareTypeDef,
         "state": str,
         "secondaryAvailabilityZone": str,
         "backupRetentionEnabled": bool,
@@ -4093,27 +4009,19 @@
         "masterEndpoint": RelationalDatabaseEndpointTypeDef,
         "pendingMaintenanceActions": List[PendingMaintenanceActionTypeDef],
         "caCertificateIdentifier": str,
     },
     total=False,
 )
 
-UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
-    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-        "parameters": Sequence[RelationalDatabaseParameterTypeDef],
-    },
-)
-
 GetBucketAccessKeysResultTypeDef = TypedDict(
     "GetBucketAccessKeysResultTypeDef",
     {
         "accessKeys": List[AccessKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDiskFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDiskFromSnapshotRequestRequestTypeDef",
     {
         "diskName": str,
@@ -4237,790 +4145,790 @@
 )
 
 GetAlarmsResultTypeDef = TypedDict(
     "GetAlarmsResultTypeDef",
     {
         "alarms": List[AlarmTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContactMethodsResultTypeDef = TypedDict(
     "GetContactMethodsResultTypeDef",
     {
         "contactMethods": List[ContactMethodTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocateStaticIpResultTypeDef = TypedDict(
     "AllocateStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachCertificateToDistributionResultTypeDef = TypedDict(
     "AttachCertificateToDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachDiskResultTypeDef = TypedDict(
     "AttachDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachInstancesToLoadBalancerResultTypeDef = TypedDict(
     "AttachInstancesToLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "AttachLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachStaticIpResultTypeDef = TypedDict(
     "AttachStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CloseInstancePublicPortsResultTypeDef = TypedDict(
     "CloseInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBucketAccessKeyResultTypeDef = TypedDict(
     "CreateBucketAccessKeyResultTypeDef",
     {
         "accessKey": AccessKeyTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCloudFormationStackResultTypeDef = TypedDict(
     "CreateCloudFormationStackResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContactMethodResultTypeDef = TypedDict(
     "CreateContactMethodResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDiskFromSnapshotResultTypeDef = TypedDict(
     "CreateDiskFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDiskResultTypeDef = TypedDict(
     "CreateDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDiskSnapshotResultTypeDef = TypedDict(
     "CreateDiskSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainEntryResultTypeDef = TypedDict(
     "CreateDomainEntryResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInstanceSnapshotResultTypeDef = TypedDict(
     "CreateInstanceSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInstancesFromSnapshotResultTypeDef = TypedDict(
     "CreateInstancesFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInstancesResultTypeDef = TypedDict(
     "CreateInstancesResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoadBalancerResultTypeDef = TypedDict(
     "CreateLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "CreateLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRelationalDatabaseFromSnapshotResultTypeDef = TypedDict(
     "CreateRelationalDatabaseFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRelationalDatabaseResultTypeDef = TypedDict(
     "CreateRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "CreateRelationalDatabaseSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAlarmResultTypeDef = TypedDict(
     "DeleteAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAutoSnapshotResultTypeDef = TypedDict(
     "DeleteAutoSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBucketAccessKeyResultTypeDef = TypedDict(
     "DeleteBucketAccessKeyResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBucketResultTypeDef = TypedDict(
     "DeleteBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCertificateResultTypeDef = TypedDict(
     "DeleteCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteContactMethodResultTypeDef = TypedDict(
     "DeleteContactMethodResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDiskResultTypeDef = TypedDict(
     "DeleteDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDiskSnapshotResultTypeDef = TypedDict(
     "DeleteDiskSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDistributionResultTypeDef = TypedDict(
     "DeleteDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainEntryResultTypeDef = TypedDict(
     "DeleteDomainEntryResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInstanceResultTypeDef = TypedDict(
     "DeleteInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInstanceSnapshotResultTypeDef = TypedDict(
     "DeleteInstanceSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKeyPairResultTypeDef = TypedDict(
     "DeleteKeyPairResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKnownHostKeysResultTypeDef = TypedDict(
     "DeleteKnownHostKeysResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteLoadBalancerResultTypeDef = TypedDict(
     "DeleteLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "DeleteLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRelationalDatabaseResultTypeDef = TypedDict(
     "DeleteRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "DeleteRelationalDatabaseSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachCertificateFromDistributionResultTypeDef = TypedDict(
     "DetachCertificateFromDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachDiskResultTypeDef = TypedDict(
     "DetachDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachInstancesFromLoadBalancerResultTypeDef = TypedDict(
     "DetachInstancesFromLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachStaticIpResultTypeDef = TypedDict(
     "DetachStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableAddOnResultTypeDef = TypedDict(
     "DisableAddOnResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableAddOnResultTypeDef = TypedDict(
     "EnableAddOnResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportSnapshotResultTypeDef = TypedDict(
     "ExportSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationResultTypeDef = TypedDict(
     "GetOperationResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationsForResourceResultTypeDef = TypedDict(
     "GetOperationsForResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "nextPageCount": str,
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationsResultTypeDef = TypedDict(
     "GetOperationsResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportKeyPairResultTypeDef = TypedDict(
     "ImportKeyPairResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpenInstancePublicPortsResultTypeDef = TypedDict(
     "OpenInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PeerVpcResultTypeDef = TypedDict(
     "PeerVpcResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAlarmResultTypeDef = TypedDict(
     "PutAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutInstancePublicPortsResultTypeDef = TypedDict(
     "PutInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootInstanceResultTypeDef = TypedDict(
     "RebootInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootRelationalDatabaseResultTypeDef = TypedDict(
     "RebootRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReleaseStaticIpResultTypeDef = TypedDict(
     "ReleaseStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetDistributionCacheResultTypeDef = TypedDict(
     "ResetDistributionCacheResultTypeDef",
     {
         "status": str,
         "createTime": datetime,
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendContactMethodVerificationResultTypeDef = TypedDict(
     "SendContactMethodVerificationResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetIpAddressTypeResultTypeDef = TypedDict(
     "SetIpAddressTypeResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetResourceAccessForBucketResultTypeDef = TypedDict(
     "SetResourceAccessForBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartGUISessionResultTypeDef = TypedDict(
     "StartGUISessionResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartInstanceResultTypeDef = TypedDict(
     "StartInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartRelationalDatabaseResultTypeDef = TypedDict(
     "StartRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopGUISessionResultTypeDef = TypedDict(
     "StopGUISessionResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopInstanceResultTypeDef = TypedDict(
     "StopInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopRelationalDatabaseResultTypeDef = TypedDict(
     "StopRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceResultTypeDef = TypedDict(
     "TagResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestAlarmResultTypeDef = TypedDict(
     "TestAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UnpeerVpcResultTypeDef = TypedDict(
     "UnpeerVpcResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UntagResourceResultTypeDef = TypedDict(
     "UntagResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBucketBundleResultTypeDef = TypedDict(
     "UpdateBucketBundleResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionBundleResultTypeDef = TypedDict(
     "UpdateDistributionBundleResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainEntryResultTypeDef = TypedDict(
     "UpdateDomainEntryResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInstanceMetadataOptionsResultTypeDef = TypedDict(
     "UpdateInstanceMetadataOptionsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLoadBalancerAttributeResultTypeDef = TypedDict(
     "UpdateLoadBalancerAttributeResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRelationalDatabaseParametersResultTypeDef = TypedDict(
     "UpdateRelationalDatabaseParametersResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRelationalDatabaseResultTypeDef = TypedDict(
     "UpdateRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStaticIpResultTypeDef = TypedDict(
     "GetStaticIpResultTypeDef",
     {
         "staticIp": StaticIpTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStaticIpsResultTypeDef = TypedDict(
     "GetStaticIpsResultTypeDef",
     {
         "staticIps": List[StaticIpTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutoSnapshotsResultTypeDef = TypedDict(
     "GetAutoSnapshotsResultTypeDef",
     {
         "resourceName": str,
         "resourceType": ResourceTypeType,
         "autoSnapshots": List[AutoSnapshotDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegionsResultTypeDef = TypedDict(
     "GetRegionsResultTypeDef",
     {
         "regions": List[RegionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBucketResultTypeDef = TypedDict(
     "CreateBucketResultTypeDef",
     {
         "bucket": BucketTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketsResultTypeDef = TypedDict(
     "GetBucketsResultTypeDef",
     {
         "buckets": List[BucketTypeDef],
         "nextPageToken": str,
         "accountLevelBpaSync": AccountLevelBpaSyncTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBucketResultTypeDef = TypedDict(
     "UpdateBucketResultTypeDef",
     {
         "bucket": BucketTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiskSnapshotResultTypeDef = TypedDict(
     "GetDiskSnapshotResultTypeDef",
     {
         "diskSnapshot": DiskSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiskSnapshotsResultTypeDef = TypedDict(
     "GetDiskSnapshotsResultTypeDef",
     {
         "diskSnapshots": List[DiskSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiskResultTypeDef = TypedDict(
     "GetDiskResultTypeDef",
     {
         "disk": DiskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDisksResultTypeDef = TypedDict(
     "GetDisksResultTypeDef",
     {
         "disks": List[DiskTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceHardwareTypeDef = TypedDict(
     "InstanceHardwareTypeDef",
     {
         "cpuCount": int,
@@ -5035,15 +4943,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "state": InstanceSnapshotStateType,
         "progress": str,
         "fromAttachedDisks": List[DiskTypeDef],
         "fromInstanceName": str,
         "fromInstanceArn": str,
         "fromBlueprintId": str,
         "fromBundleId": str,
@@ -5056,49 +4964,49 @@
 CreateKeyPairResultTypeDef = TypedDict(
     "CreateKeyPairResultTypeDef",
     {
         "keyPair": KeyPairTypeDef,
         "publicKeyBase64": str,
         "privateKeyBase64": str,
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKeyPairResultTypeDef = TypedDict(
     "GetKeyPairResultTypeDef",
     {
         "keyPair": KeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKeyPairsResultTypeDef = TypedDict(
     "GetKeyPairsResultTypeDef",
     {
         "keyPairs": List[KeyPairTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotResultTypeDef",
     {
         "relationalDatabaseSnapshot": RelationalDatabaseSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseSnapshotsResultTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotsResultTypeDef",
     {
         "relationalDatabaseSnapshots": List[RelationalDatabaseSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LightsailDistributionTypeDef = TypedDict(
     "LightsailDistributionTypeDef",
     {
         "name": str,
@@ -5111,20 +5019,20 @@
         "status": str,
         "isEnabled": bool,
         "domainName": str,
         "bundleId": str,
         "certificateName": str,
         "origin": OriginTypeDef,
         "originPublicDNS": str,
-        "defaultCacheBehavior": CacheBehaviorOutputTypeDef,
+        "defaultCacheBehavior": CacheBehaviorTypeDef,
         "cacheBehaviorSettings": CacheSettingsOutputTypeDef,
-        "cacheBehaviors": List[CacheBehaviorPerPathOutputTypeDef],
+        "cacheBehaviors": List[CacheBehaviorPerPathTypeDef],
         "ableToUpdateBundle": bool,
         "ipAddressType": IpAddressTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
@@ -5180,15 +5088,15 @@
 
 
 GetCloudFormationStackRecordsResultTypeDef = TypedDict(
     "GetCloudFormationStackRecordsResultTypeDef",
     {
         "cloudFormationStackRecords": List[CloudFormationStackRecordTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateContainerServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerServiceRequestRequestTypeDef",
     {
         "serviceName": str,
@@ -5293,28 +5201,28 @@
     total=False,
 )
 
 GetInstanceAccessDetailsResultTypeDef = TypedDict(
     "GetInstanceAccessDetailsResultTypeDef",
     {
         "accessDetails": InstanceAccessDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoadBalancerTlsCertificateTypeDef = TypedDict(
     "LoadBalancerTlsCertificateTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "loadBalancerName": str,
         "isAttached": bool,
         "status": LoadBalancerTlsCertificateStatusType,
         "domainName": str,
         "domainValidationRecords": List[LoadBalancerTlsCertificateDomainValidationRecordTypeDef],
         "failureReason": LoadBalancerTlsCertificateFailureReasonType,
         "issuedAt": datetime,
@@ -5333,70 +5241,70 @@
     total=False,
 )
 
 GetLoadBalancerResultTypeDef = TypedDict(
     "GetLoadBalancerResultTypeDef",
     {
         "loadBalancer": LoadBalancerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoadBalancersResultTypeDef = TypedDict(
     "GetLoadBalancersResultTypeDef",
     {
         "loadBalancers": List[LoadBalancerTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "domainEntries": List[DomainEntryOutputTypeDef],
         "registeredDomainDelegationInfo": RegisteredDomainDelegationInfoTypeDef,
     },
     total=False,
 )
 
 GetRelationalDatabaseResultTypeDef = TypedDict(
     "GetRelationalDatabaseResultTypeDef",
     {
         "relationalDatabase": RelationalDatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabasesResultTypeDef = TypedDict(
     "GetRelationalDatabasesResultTypeDef",
     {
         "relationalDatabases": List[RelationalDatabaseTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "blueprintId": str,
         "blueprintName": str,
         "bundleId": str,
         "addOns": List[AddOnTypeDef],
         "isStaticIp": bool,
         "privateIpAddress": str,
         "publicIpAddress": str,
@@ -5412,54 +5320,54 @@
     total=False,
 )
 
 GetInstanceSnapshotResultTypeDef = TypedDict(
     "GetInstanceSnapshotResultTypeDef",
     {
         "instanceSnapshot": InstanceSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceSnapshotsResultTypeDef = TypedDict(
     "GetInstanceSnapshotsResultTypeDef",
     {
         "instanceSnapshots": List[InstanceSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "distribution": LightsailDistributionTypeDef,
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionsResultTypeDef = TypedDict(
     "GetDistributionsResultTypeDef",
     {
         "distributions": List[LightsailDistributionTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContainerServiceTypeDef = TypedDict(
     "ContainerServiceTypeDef",
     {
         "containerServiceName": str,
         "arn": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "power": ContainerServicePowerNameType,
         "powerId": str,
         "state": ContainerServiceStateType,
         "stateDetail": ContainerServiceStateDetailTypeDef,
         "scale": int,
         "currentDeployment": ContainerServiceDeploymentTypeDef,
         "nextDeployment": ContainerServiceDeploymentTypeDef,
@@ -5473,15 +5381,15 @@
     total=False,
 )
 
 GetContainerServiceDeploymentsResultTypeDef = TypedDict(
     "GetContainerServiceDeploymentsResultTypeDef",
     {
         "deployments": List[ContainerServiceDeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateContainerServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerServiceRequestRequestTypeDef",
     {
         "serviceName": str,
@@ -5541,15 +5449,15 @@
         "issuerCA": str,
         "notBefore": datetime,
         "notAfter": datetime,
         "eligibleToRenew": str,
         "renewalSummary": RenewalSummaryTypeDef,
         "revokedAt": datetime,
         "revocationReason": str,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "supportCode": str,
     },
     total=False,
 )
 
 ResourceBudgetEstimateTypeDef = TypedDict(
     "ResourceBudgetEstimateTypeDef",
@@ -5563,123 +5471,123 @@
     total=False,
 )
 
 GetLoadBalancerTlsCertificatesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsCertificatesResultTypeDef",
     {
         "tlsCertificates": List[LoadBalancerTlsCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainResultTypeDef = TypedDict(
     "GetDomainResultTypeDef",
     {
         "domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainsResultTypeDef = TypedDict(
     "GetDomainsResultTypeDef",
     {
         "domains": List[DomainTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceResultTypeDef = TypedDict(
     "GetInstanceResultTypeDef",
     {
         "instance": InstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstancesResultTypeDef = TypedDict(
     "GetInstancesResultTypeDef",
     {
         "instances": List[InstanceTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContainerServicesListResultTypeDef = TypedDict(
     "ContainerServicesListResultTypeDef",
     {
         "containerServices": List[ContainerServiceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContainerServiceDeploymentResultTypeDef = TypedDict(
     "CreateContainerServiceDeploymentResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContainerServiceResultTypeDef = TypedDict(
     "CreateContainerServiceResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerServiceResultTypeDef = TypedDict(
     "UpdateContainerServiceResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExportSnapshotRecordsResultTypeDef = TypedDict(
     "GetExportSnapshotRecordsResultTypeDef",
     {
         "exportSnapshotRecords": List[ExportSnapshotRecordTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "certificateArn": str,
         "certificateName": str,
         "domainName": str,
         "certificateDetail": CertificateTypeDef,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 GetCostEstimateResultTypeDef = TypedDict(
     "GetCostEstimateResultTypeDef",
     {
         "resourcesBudgetEstimate": List[ResourceBudgetEstimateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCertificateResultTypeDef = TypedDict(
     "CreateCertificateResultTypeDef",
     {
         "certificate": CertificateSummaryTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCertificatesResultTypeDef = TypedDict(
     "GetCertificatesResultTypeDef",
     {
         "certificates": List[CertificateSummaryTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail/type_defs.pyi` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -98,40 +98,37 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessKeyLastUsedTypeDef",
-    "AccessRulesOutputTypeDef",
     "AccessRulesTypeDef",
     "AccountLevelBpaSyncTypeDef",
     "AutoSnapshotAddOnRequestTypeDef",
     "StopInstanceOnIdleRequestTypeDef",
     "AddOnTypeDef",
     "MonitoredResourceInfoTypeDef",
     "ResourceLocationTypeDef",
     "AllocateStaticIpRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AttachCertificateToDistributionRequestRequestTypeDef",
     "AttachDiskRequestRequestTypeDef",
     "AttachInstancesToLoadBalancerRequestRequestTypeDef",
     "AttachLoadBalancerTlsCertificateRequestRequestTypeDef",
     "AttachStaticIpRequestRequestTypeDef",
     "AttachedDiskTypeDef",
     "AvailabilityZoneTypeDef",
     "BlueprintTypeDef",
-    "BucketAccessLogConfigOutputTypeDef",
     "BucketAccessLogConfigTypeDef",
     "BucketBundleTypeDef",
     "BucketStateTypeDef",
     "ResourceReceivingAccessTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "BundleTypeDef",
-    "CacheBehaviorOutputTypeDef",
-    "CacheBehaviorPerPathOutputTypeDef",
     "CacheBehaviorPerPathTypeDef",
     "CacheBehaviorTypeDef",
     "CookieObjectOutputTypeDef",
     "HeaderObjectOutputTypeDef",
     "QueryStringObjectOutputTypeDef",
     "CookieObjectTypeDef",
     "HeaderObjectTypeDef",
@@ -140,23 +137,21 @@
     "CloudFormationStackRecordSourceInfoTypeDef",
     "DestinationInfoTypeDef",
     "ContainerImageTypeDef",
     "ContainerOutputTypeDef",
     "ContainerTypeDef",
     "ContainerServiceECRImagePullerRoleRequestTypeDef",
     "ContainerServiceECRImagePullerRoleTypeDef",
-    "ContainerServiceHealthCheckConfigOutputTypeDef",
     "ContainerServiceHealthCheckConfigTypeDef",
     "ContainerServiceLogEventTypeDef",
     "ContainerServicePowerTypeDef",
     "ContainerServiceRegistryLoginTypeDef",
     "ContainerServiceStateDetailTypeDef",
     "CopySnapshotRequestRequestTypeDef",
     "CreateBucketAccessKeyRequestRequestTypeDef",
-    "TagTypeDef",
     "InstanceEntryTypeDef",
     "CreateContactMethodRequestRequestTypeDef",
     "InputOriginTypeDef",
     "DomainEntryTypeDef",
     "CreateGUISessionAccessDetailsRequestRequestTypeDef",
     "SessionTypeDef",
     "DiskMapTypeDef",
@@ -187,139 +182,110 @@
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
     "DomainEntryOutputTypeDef",
     "ResourceRecordTypeDef",
-    "DownloadDefaultKeyPairResultTypeDef",
     "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
-    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
-    "GetActiveNamesResultTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
-    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBlueprintsRequestRequestTypeDef",
     "GetBucketAccessKeysRequestRequestTypeDef",
     "GetBucketBundlesRequestRequestTypeDef",
     "GetBucketMetricDataRequestRequestTypeDef",
     "MetricDatapointTypeDef",
     "GetBucketsRequestRequestTypeDef",
-    "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetBundlesRequestRequestTypeDef",
     "GetCertificatesRequestRequestTypeDef",
-    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     "GetContactMethodsRequestRequestTypeDef",
-    "GetContainerAPIMetadataResultTypeDef",
     "GetContainerImagesRequestRequestTypeDef",
     "GetContainerLogRequestRequestTypeDef",
     "GetContainerServiceDeploymentsRequestRequestTypeDef",
     "GetContainerServiceMetricDataRequestRequestTypeDef",
     "GetContainerServicesRequestRequestTypeDef",
     "GetCostEstimateRequestRequestTypeDef",
     "GetDiskRequestRequestTypeDef",
     "GetDiskSnapshotRequestRequestTypeDef",
-    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
     "GetDiskSnapshotsRequestRequestTypeDef",
-    "GetDisksRequestGetDisksPaginateTypeDef",
     "GetDisksRequestRequestTypeDef",
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
-    "GetDistributionLatestCacheResetResultTypeDef",
     "GetDistributionMetricDataRequestRequestTypeDef",
     "GetDistributionsRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
-    "GetDomainsRequestGetDomainsPaginateTypeDef",
     "GetDomainsRequestRequestTypeDef",
-    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     "GetInstanceAccessDetailsRequestRequestTypeDef",
     "GetInstanceMetricDataRequestRequestTypeDef",
     "GetInstancePortStatesRequestRequestTypeDef",
     "InstancePortStateTypeDef",
     "GetInstanceRequestRequestTypeDef",
     "GetInstanceSnapshotRequestRequestTypeDef",
-    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
     "GetInstanceSnapshotsRequestRequestTypeDef",
     "GetInstanceStateRequestRequestTypeDef",
     "InstanceStateTypeDef",
-    "GetInstancesRequestGetInstancesPaginateTypeDef",
     "GetInstancesRequestRequestTypeDef",
     "GetKeyPairRequestRequestTypeDef",
-    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
     "GetKeyPairsRequestRequestTypeDef",
     "GetLoadBalancerMetricDataRequestRequestTypeDef",
     "GetLoadBalancerRequestRequestTypeDef",
     "GetLoadBalancerTlsCertificatesRequestRequestTypeDef",
     "GetLoadBalancerTlsPoliciesRequestRequestTypeDef",
     "LoadBalancerTlsPolicyTypeDef",
-    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
     "GetLoadBalancersRequestRequestTypeDef",
     "GetOperationRequestRequestTypeDef",
     "GetOperationsForResourceRequestRequestTypeDef",
-    "GetOperationsRequestGetOperationsPaginateTypeDef",
     "GetOperationsRequestRequestTypeDef",
     "GetRegionsRequestRequestTypeDef",
-    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     "RelationalDatabaseBlueprintTypeDef",
-    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     "RelationalDatabaseBundleTypeDef",
-    "GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
     "GetRelationalDatabaseEventsRequestRequestTypeDef",
     "RelationalDatabaseEventTypeDef",
     "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
     "LogEventTypeDef",
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
-    "GetRelationalDatabaseLogStreamsResultTypeDef",
     "GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
-    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
-    "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
     "GetRelationalDatabaseParametersRequestRequestTypeDef",
-    "RelationalDatabaseParameterOutputTypeDef",
+    "RelationalDatabaseParameterTypeDef",
     "GetRelationalDatabaseRequestRequestTypeDef",
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
-    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
-    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
     "GetRelationalDatabasesRequestRequestTypeDef",
     "GetStaticIpRequestRequestTypeDef",
-    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     "GetStaticIpsRequestRequestTypeDef",
     "HostKeyAttributesTypeDef",
     "ImportKeyPairRequestRequestTypeDef",
     "PasswordDataTypeDef",
     "InstanceHealthSummaryTypeDef",
     "InstanceMetadataOptionsTypeDef",
     "InstancePortInfoTypeDef",
     "MonthlyTransferTypeDef",
-    "IsVpcPeeredResultTypeDef",
     "OriginTypeDef",
     "LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef",
     "LoadBalancerTlsCertificateDomainValidationOptionTypeDef",
     "LoadBalancerTlsCertificateSummaryTypeDef",
     "NameServersUpdateStateTypeDef",
-    "PaginatorConfigTypeDef",
     "PendingMaintenanceActionTypeDef",
     "PendingModifiedRelationalDatabaseValuesTypeDef",
     "PutAlarmRequestRequestTypeDef",
     "R53HostedZoneDeletionStateTypeDef",
     "RebootInstanceRequestRequestTypeDef",
     "RebootRelationalDatabaseRequestRequestTypeDef",
     "RegisterContainerImageRequestRequestTypeDef",
     "RelationalDatabaseEndpointTypeDef",
     "RelationalDatabaseHardwareTypeDef",
-    "RelationalDatabaseParameterTypeDef",
     "ReleaseStaticIpRequestRequestTypeDef",
     "ResetDistributionCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SendContactMethodVerificationRequestRequestTypeDef",
     "SetIpAddressTypeRequestRequestTypeDef",
     "SetResourceAccessForBucketRequestRequestTypeDef",
     "StartGUISessionRequestRequestTypeDef",
     "StartInstanceRequestRequestTypeDef",
     "StartRelationalDatabaseRequestRequestTypeDef",
     "StopGUISessionRequestRequestTypeDef",
@@ -334,24 +300,43 @@
     "UpdateRelationalDatabaseRequestRequestTypeDef",
     "AccessKeyTypeDef",
     "AddOnRequestTypeDef",
     "AlarmTypeDef",
     "ContactMethodTypeDef",
     "OperationTypeDef",
     "StaticIpTypeDef",
+    "DownloadDefaultKeyPairResultTypeDef",
+    "GetActiveNamesResultTypeDef",
+    "GetContainerAPIMetadataResultTypeDef",
+    "GetDistributionLatestCacheResetResultTypeDef",
+    "GetRelationalDatabaseLogStreamsResultTypeDef",
+    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
+    "IsVpcPeeredResultTypeDef",
     "AutoSnapshotDetailsTypeDef",
     "RegionTypeDef",
     "GetBlueprintsResultTypeDef",
     "UpdateBucketRequestRequestTypeDef",
     "GetBucketBundlesResultTypeDef",
     "BucketTypeDef",
+    "CreateBucketRequestRequestTypeDef",
+    "CreateCertificateRequestRequestTypeDef",
+    "CreateDiskSnapshotRequestRequestTypeDef",
+    "CreateDomainRequestRequestTypeDef",
+    "CreateInstanceSnapshotRequestRequestTypeDef",
+    "CreateKeyPairRequestRequestTypeDef",
+    "CreateLoadBalancerRequestRequestTypeDef",
+    "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
+    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    "CreateRelationalDatabaseRequestRequestTypeDef",
+    "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     "DiskSnapshotTypeDef",
     "DiskTypeDef",
     "KeyPairTypeDef",
     "RelationalDatabaseSnapshotTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "GetBundlesResultTypeDef",
     "CacheSettingsOutputTypeDef",
     "CacheSettingsTypeDef",
     "CloseInstancePublicPortsRequestRequestTypeDef",
     "OpenInstancePublicPortsRequestRequestTypeDef",
     "PutInstancePublicPortsRequestRequestTypeDef",
     "CloudFormationStackRecordTypeDef",
@@ -360,57 +345,65 @@
     "PrivateRegistryAccessRequestTypeDef",
     "PrivateRegistryAccessTypeDef",
     "ContainerServiceEndpointTypeDef",
     "EndpointRequestTypeDef",
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
-    "CreateBucketRequestRequestTypeDef",
-    "CreateCertificateRequestRequestTypeDef",
-    "CreateDiskSnapshotRequestRequestTypeDef",
-    "CreateDomainRequestRequestTypeDef",
-    "CreateInstanceSnapshotRequestRequestTypeDef",
-    "CreateKeyPairRequestRequestTypeDef",
-    "CreateLoadBalancerRequestRequestTypeDef",
-    "CreateLoadBalancerTlsCertificateRequestRequestTypeDef",
-    "CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
-    "CreateRelationalDatabaseRequestRequestTypeDef",
-    "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "CreateCloudFormationStackRequestRequestTypeDef",
     "CreateDomainEntryRequestRequestTypeDef",
     "DeleteDomainEntryRequestRequestTypeDef",
     "UpdateDomainEntryRequestRequestTypeDef",
     "CreateGUISessionAccessDetailsResultTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
     "DomainValidationRecordTypeDef",
     "EstimateByTimeTypeDef",
+    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
+    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
+    "GetBundlesRequestGetBundlesPaginateTypeDef",
+    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
+    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
+    "GetDisksRequestGetDisksPaginateTypeDef",
+    "GetDomainsRequestGetDomainsPaginateTypeDef",
+    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
+    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
+    "GetInstancesRequestGetInstancesPaginateTypeDef",
+    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
+    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
+    "GetOperationsRequestGetOperationsPaginateTypeDef",
+    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
+    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
+    "GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
+    "GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
+    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
+    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
+    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     "GetBucketMetricDataResultTypeDef",
     "GetContainerServiceMetricDataResultTypeDef",
     "GetDistributionMetricDataResultTypeDef",
     "GetInstanceMetricDataResultTypeDef",
     "GetLoadBalancerMetricDataResultTypeDef",
     "GetRelationalDatabaseMetricDataResultTypeDef",
     "GetInstancePortStatesResultTypeDef",
     "GetInstanceStateResultTypeDef",
     "GetLoadBalancerTlsPoliciesResultTypeDef",
     "GetRelationalDatabaseBlueprintsResultTypeDef",
     "GetRelationalDatabaseBundlesResultTypeDef",
     "GetRelationalDatabaseEventsResultTypeDef",
     "GetRelationalDatabaseLogEventsResultTypeDef",
     "GetRelationalDatabaseParametersResultTypeDef",
+    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     "InstanceAccessDetailsTypeDef",
     "InstanceNetworkingTypeDef",
     "LoadBalancerTlsCertificateDomainValidationRecordTypeDef",
     "LoadBalancerTlsCertificateRenewalSummaryTypeDef",
     "LoadBalancerTypeDef",
     "RegisteredDomainDelegationInfoTypeDef",
     "RelationalDatabaseTypeDef",
-    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
     "GetBucketAccessKeysResultTypeDef",
     "CreateDiskFromSnapshotRequestRequestTypeDef",
     "CreateDiskRequestRequestTypeDef",
     "CreateInstancesFromSnapshotRequestRequestTypeDef",
     "CreateInstancesRequestRequestTypeDef",
     "EnableAddOnRequestRequestTypeDef",
     "GetAlarmsResultTypeDef",
@@ -567,23 +560,14 @@
         "lastUsedDate": datetime,
         "region": str,
         "serviceName": str,
     },
     total=False,
 )
 
-AccessRulesOutputTypeDef = TypedDict(
-    "AccessRulesOutputTypeDef",
-    {
-        "getObject": AccessTypeType,
-        "allowPublicOverrides": bool,
-    },
-    total=False,
-)
-
 AccessRulesTypeDef = TypedDict(
     "AccessRulesTypeDef",
     {
         "getObject": AccessTypeType,
         "allowPublicOverrides": bool,
     },
     total=False,
@@ -652,14 +636,25 @@
 AllocateStaticIpRequestRequestTypeDef = TypedDict(
     "AllocateStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
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
 AttachCertificateToDistributionRequestRequestTypeDef = TypedDict(
     "AttachCertificateToDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "certificateName": str,
     },
 )
@@ -743,34 +738,14 @@
         "licenseUrl": str,
         "platform": InstancePlatformType,
         "appCategory": Literal["LfR"],
     },
     total=False,
 )
 
-_RequiredBucketAccessLogConfigOutputTypeDef = TypedDict(
-    "_RequiredBucketAccessLogConfigOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-)
-_OptionalBucketAccessLogConfigOutputTypeDef = TypedDict(
-    "_OptionalBucketAccessLogConfigOutputTypeDef",
-    {
-        "destination": str,
-        "prefix": str,
-    },
-    total=False,
-)
-
-class BucketAccessLogConfigOutputTypeDef(
-    _RequiredBucketAccessLogConfigOutputTypeDef, _OptionalBucketAccessLogConfigOutputTypeDef
-):
-    pass
-
 _RequiredBucketAccessLogConfigTypeDef = TypedDict(
     "_RequiredBucketAccessLogConfigTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalBucketAccessLogConfigTypeDef = TypedDict(
@@ -814,16 +789,16 @@
     {
         "name": str,
         "resourceType": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
@@ -842,31 +817,14 @@
         "transferPerMonthInGb": int,
         "supportedPlatforms": List[InstancePlatformType],
         "supportedAppCategories": List[Literal["LfR"]],
     },
     total=False,
 )
 
-CacheBehaviorOutputTypeDef = TypedDict(
-    "CacheBehaviorOutputTypeDef",
-    {
-        "behavior": BehaviorEnumType,
-    },
-    total=False,
-)
-
-CacheBehaviorPerPathOutputTypeDef = TypedDict(
-    "CacheBehaviorPerPathOutputTypeDef",
-    {
-        "path": str,
-        "behavior": BehaviorEnumType,
-    },
-    total=False,
-)
-
 CacheBehaviorPerPathTypeDef = TypedDict(
     "CacheBehaviorPerPathTypeDef",
     {
         "path": str,
         "behavior": BehaviorEnumType,
     },
     total=False,
@@ -1011,27 +969,14 @@
     {
         "isActive": bool,
         "principalArn": str,
     },
     total=False,
 )
 
-ContainerServiceHealthCheckConfigOutputTypeDef = TypedDict(
-    "ContainerServiceHealthCheckConfigOutputTypeDef",
-    {
-        "healthyThreshold": int,
-        "unhealthyThreshold": int,
-        "timeoutSeconds": int,
-        "intervalSeconds": int,
-        "path": str,
-        "successCodes": str,
-    },
-    total=False,
-)
-
 ContainerServiceHealthCheckConfigTypeDef = TypedDict(
     "ContainerServiceHealthCheckConfigTypeDef",
     {
         "healthyThreshold": int,
         "unhealthyThreshold": int,
         "timeoutSeconds": int,
         "intervalSeconds": int,
@@ -1109,23 +1054,14 @@
 CreateBucketAccessKeyRequestRequestTypeDef = TypedDict(
     "CreateBucketAccessKeyRequestRequestTypeDef",
     {
         "bucketName": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-    total=False,
-)
-
 _RequiredInstanceEntryTypeDef = TypedDict(
     "_RequiredInstanceEntryTypeDef",
     {
         "sourceName": str,
         "instanceType": str,
         "portInfoSource": PortInfoSourceTypeType,
         "availabilityZone": str,
@@ -1515,24 +1451,14 @@
         "name": str,
         "type": str,
         "value": str,
     },
     total=False,
 )
 
-DownloadDefaultKeyPairResultTypeDef = TypedDict(
-    "DownloadDefaultKeyPairResultTypeDef",
-    {
-        "publicKeyBase64": str,
-        "privateKeyBase64": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TimePeriodTypeDef = TypedDict(
     "TimePeriodTypeDef",
     {
         "start": datetime,
         "end": datetime,
     },
     total=False,
@@ -1541,39 +1467,32 @@
 ExportSnapshotRequestRequestTypeDef = TypedDict(
     "ExportSnapshotRequestRequestTypeDef",
     {
         "sourceSnapshotName": str,
     },
 )
 
-GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
-    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
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
 
 GetActiveNamesRequestRequestTypeDef = TypedDict(
     "GetActiveNamesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-GetActiveNamesResultTypeDef = TypedDict(
-    "GetActiveNamesResultTypeDef",
-    {
-        "activeNames": List[str],
-        "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAlarmsRequestRequestTypeDef = TypedDict(
     "GetAlarmsRequestRequestTypeDef",
     {
         "alarmName": str,
         "pageToken": str,
         "monitoredResourceName": str,
     },
@@ -1583,24 +1502,14 @@
 GetAutoSnapshotsRequestRequestTypeDef = TypedDict(
     "GetAutoSnapshotsRequestRequestTypeDef",
     {
         "resourceName": str,
     },
 )
 
-GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
-    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "appCategory": Literal["LfR"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBlueprintsRequestRequestTypeDef = TypedDict(
     "GetBlueprintsRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
         "appCategory": Literal["LfR"],
     },
@@ -1655,24 +1564,14 @@
         "bucketName": str,
         "pageToken": str,
         "includeConnectedResources": bool,
     },
     total=False,
 )
 
-GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
-    "GetBundlesRequestGetBundlesPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "appCategory": Literal["LfR"],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetBundlesRequestRequestTypeDef = TypedDict(
     "GetBundlesRequestRequestTypeDef",
     {
         "includeInactive": bool,
         "pageToken": str,
         "appCategory": Literal["LfR"],
     },
@@ -1686,22 +1585,14 @@
         "includeCertificateDetails": bool,
         "certificateName": str,
         "pageToken": str,
     },
     total=False,
 )
 
-GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
-    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetCloudFormationStackRecordsRequestRequestTypeDef = TypedDict(
     "GetCloudFormationStackRecordsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1710,22 +1601,14 @@
     "GetContactMethodsRequestRequestTypeDef",
     {
         "protocols": Sequence[ContactProtocolType],
     },
     total=False,
 )
 
-GetContainerAPIMetadataResultTypeDef = TypedDict(
-    "GetContainerAPIMetadataResultTypeDef",
-    {
-        "metadata": List[Dict[str, str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetContainerImagesRequestRequestTypeDef = TypedDict(
     "GetContainerImagesRequestRequestTypeDef",
     {
         "serviceName": str,
     },
 )
 
@@ -1798,38 +1681,22 @@
 GetDiskSnapshotRequestRequestTypeDef = TypedDict(
     "GetDiskSnapshotRequestRequestTypeDef",
     {
         "diskSnapshotName": str,
     },
 )
 
-GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = TypedDict(
-    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDiskSnapshotsRequestRequestTypeDef = TypedDict(
     "GetDiskSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-GetDisksRequestGetDisksPaginateTypeDef = TypedDict(
-    "GetDisksRequestGetDisksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDisksRequestRequestTypeDef = TypedDict(
     "GetDisksRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1838,23 +1705,14 @@
     "GetDistributionLatestCacheResetRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
 )
 
-GetDistributionLatestCacheResetResultTypeDef = TypedDict(
-    "GetDistributionLatestCacheResetResultTypeDef",
-    {
-        "status": str,
-        "createTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDistributionMetricDataRequestRequestTypeDef = TypedDict(
     "GetDistributionMetricDataRequestRequestTypeDef",
     {
         "distributionName": str,
         "metricName": DistributionMetricNameType,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
@@ -1876,38 +1734,22 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainName": str,
     },
 )
 
-GetDomainsRequestGetDomainsPaginateTypeDef = TypedDict(
-    "GetDomainsRequestGetDomainsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDomainsRequestRequestTypeDef = TypedDict(
     "GetDomainsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = TypedDict(
-    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetExportSnapshotRecordsRequestRequestTypeDef = TypedDict(
     "GetExportSnapshotRecordsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -1976,22 +1818,14 @@
 GetInstanceSnapshotRequestRequestTypeDef = TypedDict(
     "GetInstanceSnapshotRequestRequestTypeDef",
     {
         "instanceSnapshotName": str,
     },
 )
 
-GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = TypedDict(
-    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInstanceSnapshotsRequestRequestTypeDef = TypedDict(
     "GetInstanceSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2008,22 +1842,14 @@
     {
         "code": int,
         "name": str,
     },
     total=False,
 )
 
-GetInstancesRequestGetInstancesPaginateTypeDef = TypedDict(
-    "GetInstancesRequestGetInstancesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetInstancesRequestRequestTypeDef = TypedDict(
     "GetInstancesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2031,23 +1857,14 @@
 GetKeyPairRequestRequestTypeDef = TypedDict(
     "GetKeyPairRequestRequestTypeDef",
     {
         "keyPairName": str,
     },
 )
 
-GetKeyPairsRequestGetKeyPairsPaginateTypeDef = TypedDict(
-    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
-    {
-        "includeDefaultKeyPair": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetKeyPairsRequestRequestTypeDef = TypedDict(
     "GetKeyPairsRequestRequestTypeDef",
     {
         "pageToken": str,
         "includeDefaultKeyPair": bool,
     },
     total=False,
@@ -2096,22 +1913,14 @@
         "description": str,
         "protocols": List[str],
         "ciphers": List[str],
     },
     total=False,
 )
 
-GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = TypedDict(
-    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetLoadBalancersRequestRequestTypeDef = TypedDict(
     "GetLoadBalancersRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2139,22 +1948,14 @@
 
 class GetOperationsForResourceRequestRequestTypeDef(
     _RequiredGetOperationsForResourceRequestRequestTypeDef,
     _OptionalGetOperationsForResourceRequestRequestTypeDef,
 ):
     pass
 
-GetOperationsRequestGetOperationsPaginateTypeDef = TypedDict(
-    "GetOperationsRequestGetOperationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetOperationsRequestRequestTypeDef = TypedDict(
     "GetOperationsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2164,22 +1965,14 @@
     {
         "includeAvailabilityZones": bool,
         "includeRelationalDatabaseAvailabilityZones": bool,
     },
     total=False,
 )
 
-GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRelationalDatabaseBlueprintsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseBlueprintsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2193,23 +1986,14 @@
         "engineDescription": str,
         "engineVersionDescription": str,
         "isEngineDefault": bool,
     },
     total=False,
 )
 
-GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
-    {
-        "includeInactive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRelationalDatabaseBundlesRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseBundlesRequestRequestTypeDef",
     {
         "pageToken": str,
         "includeInactive": bool,
     },
     total=False,
@@ -2227,35 +2011,14 @@
         "cpuCount": int,
         "isEncrypted": bool,
         "isActive": bool,
     },
     total=False,
 )
 
-_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
-    {
-        "durationInMinutes": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef(
-    _RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-    _OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRelationalDatabaseEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseEventsRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseEventsRequestRequestTypeDef = TypedDict(
@@ -2320,22 +2083,14 @@
 GetRelationalDatabaseLogStreamsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseLogStreamsRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 
-GetRelationalDatabaseLogStreamsResultTypeDef = TypedDict(
-    "GetRelationalDatabaseLogStreamsResultTypeDef",
-    {
-        "logStreams": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef = TypedDict(
@@ -2348,56 +2103,27 @@
 
 class GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
 ):
     pass
 
-GetRelationalDatabaseMasterUserPasswordResultTypeDef = TypedDict(
-    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
-    {
-        "masterUserPassword": str,
-        "createdAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRelationalDatabaseMetricDataRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
         "metricName": RelationalDatabaseMetricNameType,
         "period": int,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "unit": MetricUnitType,
         "statistics": Sequence[MetricStatisticType],
     },
 )
 
-_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
-    "_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    {
-        "relationalDatabaseName": str,
-    },
-)
-_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
-    "_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef(
-    _RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-    _OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
     "_RequiredGetRelationalDatabaseParametersRequestRequestTypeDef",
     {
         "relationalDatabaseName": str,
     },
 )
 _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
@@ -2410,16 +2136,16 @@
 
 class GetRelationalDatabaseParametersRequestRequestTypeDef(
     _RequiredGetRelationalDatabaseParametersRequestRequestTypeDef,
     _OptionalGetRelationalDatabaseParametersRequestRequestTypeDef,
 ):
     pass
 
-RelationalDatabaseParameterOutputTypeDef = TypedDict(
-    "RelationalDatabaseParameterOutputTypeDef",
+RelationalDatabaseParameterTypeDef = TypedDict(
+    "RelationalDatabaseParameterTypeDef",
     {
         "allowedValues": str,
         "applyMethod": str,
         "applyType": str,
         "dataType": str,
         "description": str,
         "isModifiable": bool,
@@ -2439,38 +2165,22 @@
 GetRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotRequestRequestTypeDef",
     {
         "relationalDatabaseSnapshotName": str,
     },
 )
 
-GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = TypedDict(
-    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRelationalDatabaseSnapshotsRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
 
-GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = TypedDict(
-    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRelationalDatabasesRequestRequestTypeDef = TypedDict(
     "GetRelationalDatabasesRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2478,22 +2188,14 @@
 GetStaticIpRequestRequestTypeDef = TypedDict(
     "GetStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
     },
 )
 
-GetStaticIpsRequestGetStaticIpsPaginateTypeDef = TypedDict(
-    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetStaticIpsRequestRequestTypeDef = TypedDict(
     "GetStaticIpsRequestRequestTypeDef",
     {
         "pageToken": str,
     },
     total=False,
 )
@@ -2572,22 +2274,14 @@
     "MonthlyTransferTypeDef",
     {
         "gbPerMonthAllocated": int,
     },
     total=False,
 )
 
-IsVpcPeeredResultTypeDef = TypedDict(
-    "IsVpcPeeredResultTypeDef",
-    {
-        "isPeered": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 OriginTypeDef = TypedDict(
     "OriginTypeDef",
     {
         "name": str,
         "resourceType": ResourceTypeType,
         "regionName": RegionNameType,
         "protocolPolicy": OriginProtocolPolicyEnumType,
@@ -2627,24 +2321,14 @@
     {
         "code": NameServersUpdateStateCodeType,
         "message": str,
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
 PendingMaintenanceActionTypeDef = TypedDict(
     "PendingMaintenanceActionTypeDef",
     {
         "action": str,
         "description": str,
         "currentApplyDate": datetime,
     },
@@ -2736,29 +2420,14 @@
         "cpuCount": int,
         "diskSizeInGb": int,
         "ramSizeInGb": float,
     },
     total=False,
 )
 
-RelationalDatabaseParameterTypeDef = TypedDict(
-    "RelationalDatabaseParameterTypeDef",
-    {
-        "allowedValues": str,
-        "applyMethod": str,
-        "applyType": str,
-        "dataType": str,
-        "description": str,
-        "isModifiable": bool,
-        "parameterName": str,
-        "parameterValue": str,
-    },
-    total=False,
-)
-
 ReleaseStaticIpRequestRequestTypeDef = TypedDict(
     "ReleaseStaticIpRequestRequestTypeDef",
     {
         "staticIpName": str,
     },
 )
 
@@ -2766,25 +2435,14 @@
     "ResetDistributionCacheRequestRequestTypeDef",
     {
         "distributionName": str,
     },
     total=False,
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
 SendContactMethodVerificationRequestRequestTypeDef = TypedDict(
     "SendContactMethodVerificationRequestRequestTypeDef",
     {
         "protocol": Literal["Email"],
     },
 )
 
@@ -3082,14 +2740,75 @@
         "ipAddress": str,
         "attachedTo": str,
         "isAttached": bool,
     },
     total=False,
 )
 
+DownloadDefaultKeyPairResultTypeDef = TypedDict(
+    "DownloadDefaultKeyPairResultTypeDef",
+    {
+        "publicKeyBase64": str,
+        "privateKeyBase64": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetActiveNamesResultTypeDef = TypedDict(
+    "GetActiveNamesResultTypeDef",
+    {
+        "activeNames": List[str],
+        "nextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetContainerAPIMetadataResultTypeDef = TypedDict(
+    "GetContainerAPIMetadataResultTypeDef",
+    {
+        "metadata": List[Dict[str, str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDistributionLatestCacheResetResultTypeDef = TypedDict(
+    "GetDistributionLatestCacheResetResultTypeDef",
+    {
+        "status": str,
+        "createTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRelationalDatabaseLogStreamsResultTypeDef = TypedDict(
+    "GetRelationalDatabaseLogStreamsResultTypeDef",
+    {
+        "logStreams": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRelationalDatabaseMasterUserPasswordResultTypeDef = TypedDict(
+    "GetRelationalDatabaseMasterUserPasswordResultTypeDef",
+    {
+        "masterUserPassword": str,
+        "createdAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+IsVpcPeeredResultTypeDef = TypedDict(
+    "IsVpcPeeredResultTypeDef",
+    {
+        "isPeered": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AutoSnapshotDetailsTypeDef = TypedDict(
     "AutoSnapshotDetailsTypeDef",
     {
         "date": str,
         "createdAt": datetime,
         "status": AutoSnapshotStatusType,
         "fromAttachedDisks": List[AttachedDiskTypeDef],
@@ -3111,15 +2830,15 @@
 )
 
 GetBlueprintsResultTypeDef = TypedDict(
     "GetBlueprintsResultTypeDef",
     {
         "blueprints": List[BlueprintTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBucketRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBucketRequestRequestTypeDef",
     {
         "bucketName": str,
@@ -3141,51 +2860,301 @@
 ):
     pass
 
 GetBucketBundlesResultTypeDef = TypedDict(
     "GetBucketBundlesResultTypeDef",
     {
         "bundles": List[BucketBundleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketTypeDef = TypedDict(
     "BucketTypeDef",
     {
         "resourceType": str,
-        "accessRules": AccessRulesOutputTypeDef,
+        "accessRules": AccessRulesTypeDef,
         "arn": str,
         "bundleId": str,
         "createdAt": datetime,
         "url": str,
         "location": ResourceLocationTypeDef,
         "name": str,
         "supportCode": str,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "objectVersioning": str,
         "ableToUpdateBundle": bool,
         "readonlyAccessAccounts": List[str],
         "resourcesReceivingAccess": List[ResourceReceivingAccessTypeDef],
         "state": BucketStateTypeDef,
-        "accessLogConfig": BucketAccessLogConfigOutputTypeDef,
+        "accessLogConfig": BucketAccessLogConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredCreateBucketRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateBucketRequestRequestTypeDef",
+    {
+        "bucketName": str,
+        "bundleId": str,
+    },
+)
+_OptionalCreateBucketRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateBucketRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+        "enableObjectVersioning": bool,
+    },
+    total=False,
+)
+
+class CreateBucketRequestRequestTypeDef(
+    _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCertificateRequestRequestTypeDef",
+    {
+        "certificateName": str,
+        "domainName": str,
+    },
+)
+_OptionalCreateCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCertificateRequestRequestTypeDef",
+    {
+        "subjectAlternativeNames": Sequence[str],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateCertificateRequestRequestTypeDef(
+    _RequiredCreateCertificateRequestRequestTypeDef, _OptionalCreateCertificateRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateDiskSnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDiskSnapshotRequestRequestTypeDef",
+    {
+        "diskSnapshotName": str,
+    },
+)
+_OptionalCreateDiskSnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDiskSnapshotRequestRequestTypeDef",
+    {
+        "diskName": str,
+        "instanceName": str,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDiskSnapshotRequestRequestTypeDef(
+    _RequiredCreateDiskSnapshotRequestRequestTypeDef,
+    _OptionalCreateDiskSnapshotRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDomainRequestRequestTypeDef",
+    {
+        "domainName": str,
+    },
+)
+_OptionalCreateDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDomainRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateDomainRequestRequestTypeDef(
+    _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateInstanceSnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceSnapshotRequestRequestTypeDef",
+    {
+        "instanceSnapshotName": str,
+        "instanceName": str,
+    },
+)
+_OptionalCreateInstanceSnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceSnapshotRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateInstanceSnapshotRequestRequestTypeDef(
+    _RequiredCreateInstanceSnapshotRequestRequestTypeDef,
+    _OptionalCreateInstanceSnapshotRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateKeyPairRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyPairRequestRequestTypeDef",
+    {
+        "keyPairName": str,
+    },
+)
+_OptionalCreateKeyPairRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyPairRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateKeyPairRequestRequestTypeDef(
+    _RequiredCreateKeyPairRequestRequestTypeDef, _OptionalCreateKeyPairRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateLoadBalancerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLoadBalancerRequestRequestTypeDef",
+    {
+        "loadBalancerName": str,
+        "instancePort": int,
+    },
+)
+_OptionalCreateLoadBalancerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLoadBalancerRequestRequestTypeDef",
+    {
+        "healthCheckPath": str,
+        "certificateName": str,
+        "certificateDomainName": str,
+        "certificateAlternativeNames": Sequence[str],
+        "tags": Sequence[TagTypeDef],
+        "ipAddressType": IpAddressTypeType,
+        "tlsPolicyName": str,
+    },
+    total=False,
+)
+
+class CreateLoadBalancerRequestRequestTypeDef(
+    _RequiredCreateLoadBalancerRequestRequestTypeDef,
+    _OptionalCreateLoadBalancerRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef",
+    {
+        "loadBalancerName": str,
+        "certificateName": str,
+        "certificateDomainName": str,
+    },
+)
+_OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef",
+    {
+        "certificateAlternativeNames": Sequence[str],
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateLoadBalancerTlsCertificateRequestRequestTypeDef(
+    _RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
+    _OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+    },
+)
+_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+    {
+        "availabilityZone": str,
+        "publiclyAccessible": bool,
+        "relationalDatabaseSnapshotName": str,
+        "relationalDatabaseBundleId": str,
+        "sourceRelationalDatabaseName": str,
+        "restoreTime": Union[datetime, str],
+        "useLatestRestorableTime": bool,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(
+    _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateRelationalDatabaseRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRelationalDatabaseRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "relationalDatabaseBlueprintId": str,
+        "relationalDatabaseBundleId": str,
+        "masterDatabaseName": str,
+        "masterUsername": str,
+    },
+)
+_OptionalCreateRelationalDatabaseRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRelationalDatabaseRequestRequestTypeDef",
+    {
+        "availabilityZone": str,
+        "masterUserPassword": str,
+        "preferredBackupWindow": str,
+        "preferredMaintenanceWindow": str,
+        "publiclyAccessible": bool,
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateRelationalDatabaseRequestRequestTypeDef(
+    _RequiredCreateRelationalDatabaseRequestRequestTypeDef,
+    _OptionalCreateRelationalDatabaseRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "relationalDatabaseSnapshotName": str,
+    },
+)
+_OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef",
+    {
+        "tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateRelationalDatabaseSnapshotRequestRequestTypeDef(
+    _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
+    _OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
+):
+    pass
+
 DiskSnapshotTypeDef = TypedDict(
     "DiskSnapshotTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "sizeInGb": int,
         "state": DiskSnapshotStateType,
         "progress": str,
         "fromDiskName": str,
         "fromDiskArn": str,
         "fromInstanceName": str,
         "fromInstanceArn": str,
@@ -3199,15 +3168,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "addOns": List[AddOnTypeDef],
         "sizeInGb": int,
         "isSystemDisk": bool,
         "iops": int,
         "path": str,
         "state": DiskStateType,
         "attachedTo": str,
@@ -3224,48 +3193,68 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "fingerprint": str,
     },
     total=False,
 )
 
 RelationalDatabaseSnapshotTypeDef = TypedDict(
     "RelationalDatabaseSnapshotTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "engine": str,
         "engineVersion": str,
         "sizeInGb": int,
         "state": str,
         "fromRelationalDatabaseName": str,
         "fromRelationalDatabaseArn": str,
         "fromRelationalDatabaseBundleId": str,
         "fromRelationalDatabaseBlueprintId": str,
     },
     total=False,
 )
 
+_RequiredTagResourceRequestRequestTypeDef = TypedDict(
+    "_RequiredTagResourceRequestRequestTypeDef",
+    {
+        "resourceName": str,
+        "tags": Sequence[TagTypeDef],
+    },
+)
+_OptionalTagResourceRequestRequestTypeDef = TypedDict(
+    "_OptionalTagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+    },
+    total=False,
+)
+
+class TagResourceRequestRequestTypeDef(
+    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
+):
+    pass
+
 GetBundlesResultTypeDef = TypedDict(
     "GetBundlesResultTypeDef",
     {
         "bundles": List[BundleTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CacheSettingsOutputTypeDef = TypedDict(
     "CacheSettingsOutputTypeDef",
     {
         "defaultTTL": int,
@@ -3334,23 +3323,23 @@
     total=False,
 )
 
 GetContainerImagesResultTypeDef = TypedDict(
     "GetContainerImagesResultTypeDef",
     {
         "containerImages": List[ContainerImageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterContainerImageResultTypeDef = TypedDict(
     "RegisterContainerImageResultTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PrivateRegistryAccessRequestTypeDef = TypedDict(
     "PrivateRegistryAccessRequestTypeDef",
     {
         "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
@@ -3367,15 +3356,15 @@
 )
 
 ContainerServiceEndpointTypeDef = TypedDict(
     "ContainerServiceEndpointTypeDef",
     {
         "containerName": str,
         "containerPort": int,
-        "healthCheck": ContainerServiceHealthCheckConfigOutputTypeDef,
+        "healthCheck": ContainerServiceHealthCheckConfigTypeDef,
     },
     total=False,
 )
 
 _RequiredEndpointRequestTypeDef = TypedDict(
     "_RequiredEndpointRequestTypeDef",
     {
@@ -3395,510 +3384,439 @@
     pass
 
 GetContainerLogResultTypeDef = TypedDict(
     "GetContainerLogResultTypeDef",
     {
         "logEvents": List[ContainerServiceLogEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContainerServicePowersResultTypeDef = TypedDict(
     "GetContainerServicePowersResultTypeDef",
     {
         "powers": List[ContainerServicePowerTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContainerServiceRegistryLoginResultTypeDef = TypedDict(
     "CreateContainerServiceRegistryLoginResultTypeDef",
     {
         "registryLogin": ContainerServiceRegistryLoginTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateBucketRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateBucketRequestRequestTypeDef",
+CreateCloudFormationStackRequestRequestTypeDef = TypedDict(
+    "CreateCloudFormationStackRequestRequestTypeDef",
     {
-        "bucketName": str,
-        "bundleId": str,
+        "instances": Sequence[InstanceEntryTypeDef],
     },
 )
-_OptionalCreateBucketRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateBucketRequestRequestTypeDef",
+
+CreateDomainEntryRequestRequestTypeDef = TypedDict(
+    "CreateDomainEntryRequestRequestTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
-        "enableObjectVersioning": bool,
+        "domainName": str,
+        "domainEntry": DomainEntryTypeDef,
     },
-    total=False,
 )
 
-class CreateBucketRequestRequestTypeDef(
-    _RequiredCreateBucketRequestRequestTypeDef, _OptionalCreateBucketRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCertificateRequestRequestTypeDef",
+DeleteDomainEntryRequestRequestTypeDef = TypedDict(
+    "DeleteDomainEntryRequestRequestTypeDef",
     {
-        "certificateName": str,
         "domainName": str,
+        "domainEntry": DomainEntryTypeDef,
     },
 )
-_OptionalCreateCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCertificateRequestRequestTypeDef",
+
+UpdateDomainEntryRequestRequestTypeDef = TypedDict(
+    "UpdateDomainEntryRequestRequestTypeDef",
     {
-        "subjectAlternativeNames": Sequence[str],
-        "tags": Sequence[TagTypeDef],
+        "domainName": str,
+        "domainEntry": DomainEntryTypeDef,
     },
-    total=False,
 )
 
-class CreateCertificateRequestRequestTypeDef(
-    _RequiredCreateCertificateRequestRequestTypeDef, _OptionalCreateCertificateRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateDiskSnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDiskSnapshotRequestRequestTypeDef",
+CreateGUISessionAccessDetailsResultTypeDef = TypedDict(
+    "CreateGUISessionAccessDetailsResultTypeDef",
     {
-        "diskSnapshotName": str,
+        "resourceName": str,
+        "status": StatusType,
+        "percentageComplete": int,
+        "failureReason": str,
+        "sessions": List[SessionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateDiskSnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDiskSnapshotRequestRequestTypeDef",
+
+InstanceSnapshotInfoTypeDef = TypedDict(
+    "InstanceSnapshotInfoTypeDef",
     {
-        "diskName": str,
-        "instanceName": str,
-        "tags": Sequence[TagTypeDef],
+        "fromBundleId": str,
+        "fromBlueprintId": str,
+        "fromDiskInfo": List[DiskInfoTypeDef],
     },
     total=False,
 )
 
-class CreateDiskSnapshotRequestRequestTypeDef(
-    _RequiredCreateDiskSnapshotRequestRequestTypeDef,
-    _OptionalCreateDiskSnapshotRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateDomainRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDomainRequestRequestTypeDef",
+GetDistributionBundlesResultTypeDef = TypedDict(
+    "GetDistributionBundlesResultTypeDef",
     {
-        "domainName": str,
+        "bundles": List[DistributionBundleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalCreateDomainRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDomainRequestRequestTypeDef",
+
+DomainValidationRecordTypeDef = TypedDict(
+    "DomainValidationRecordTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "domainName": str,
+        "resourceRecord": ResourceRecordTypeDef,
+        "dnsRecordCreationState": DnsRecordCreationStateTypeDef,
+        "validationStatus": CertificateDomainValidationStatusType,
     },
     total=False,
 )
 
-class CreateDomainRequestRequestTypeDef(
-    _RequiredCreateDomainRequestRequestTypeDef, _OptionalCreateDomainRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateInstanceSnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceSnapshotRequestRequestTypeDef",
-    {
-        "instanceSnapshotName": str,
-        "instanceName": str,
-    },
-)
-_OptionalCreateInstanceSnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceSnapshotRequestRequestTypeDef",
+EstimateByTimeTypeDef = TypedDict(
+    "EstimateByTimeTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "usageCost": float,
+        "pricingUnit": PricingUnitType,
+        "unit": float,
+        "currency": Literal["USD"],
+        "timePeriod": TimePeriodTypeDef,
     },
     total=False,
 )
 
-class CreateInstanceSnapshotRequestRequestTypeDef(
-    _RequiredCreateInstanceSnapshotRequestRequestTypeDef,
-    _OptionalCreateInstanceSnapshotRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateKeyPairRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyPairRequestRequestTypeDef",
-    {
-        "keyPairName": str,
-    },
-)
-_OptionalCreateKeyPairRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyPairRequestRequestTypeDef",
+GetActiveNamesRequestGetActiveNamesPaginateTypeDef = TypedDict(
+    "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateKeyPairRequestRequestTypeDef(
-    _RequiredCreateKeyPairRequestRequestTypeDef, _OptionalCreateKeyPairRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateLoadBalancerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLoadBalancerRequestRequestTypeDef",
+GetBlueprintsRequestGetBlueprintsPaginateTypeDef = TypedDict(
+    "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     {
-        "loadBalancerName": str,
-        "instancePort": int,
+        "includeInactive": bool,
+        "appCategory": Literal["LfR"],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateLoadBalancerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLoadBalancerRequestRequestTypeDef",
+
+GetBundlesRequestGetBundlesPaginateTypeDef = TypedDict(
+    "GetBundlesRequestGetBundlesPaginateTypeDef",
     {
-        "healthCheckPath": str,
-        "certificateName": str,
-        "certificateDomainName": str,
-        "certificateAlternativeNames": Sequence[str],
-        "tags": Sequence[TagTypeDef],
-        "ipAddressType": IpAddressTypeType,
-        "tlsPolicyName": str,
+        "includeInactive": bool,
+        "appCategory": Literal["LfR"],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateLoadBalancerRequestRequestTypeDef(
-    _RequiredCreateLoadBalancerRequestRequestTypeDef,
-    _OptionalCreateLoadBalancerRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef",
+GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef = TypedDict(
+    "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     {
-        "loadBalancerName": str,
-        "certificateName": str,
-        "certificateDomainName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef",
+
+GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef = TypedDict(
+    "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
     {
-        "certificateAlternativeNames": Sequence[str],
-        "tags": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateLoadBalancerTlsCertificateRequestRequestTypeDef(
-    _RequiredCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    _OptionalCreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+GetDisksRequestGetDisksPaginateTypeDef = TypedDict(
+    "GetDisksRequestGetDisksPaginateTypeDef",
     {
-        "relationalDatabaseName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef",
+
+GetDomainsRequestGetDomainsPaginateTypeDef = TypedDict(
+    "GetDomainsRequestGetDomainsPaginateTypeDef",
     {
-        "availabilityZone": str,
-        "publiclyAccessible": bool,
-        "relationalDatabaseSnapshotName": str,
-        "relationalDatabaseBundleId": str,
-        "sourceRelationalDatabaseName": str,
-        "restoreTime": Union[datetime, str],
-        "useLatestRestorableTime": bool,
-        "tags": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef(
-    _RequiredCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    _OptionalCreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateRelationalDatabaseRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRelationalDatabaseRequestRequestTypeDef",
+GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef = TypedDict(
+    "GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef",
     {
-        "relationalDatabaseName": str,
-        "relationalDatabaseBlueprintId": str,
-        "relationalDatabaseBundleId": str,
-        "masterDatabaseName": str,
-        "masterUsername": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateRelationalDatabaseRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRelationalDatabaseRequestRequestTypeDef",
+
+GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef = TypedDict(
+    "GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef",
     {
-        "availabilityZone": str,
-        "masterUserPassword": str,
-        "preferredBackupWindow": str,
-        "preferredMaintenanceWindow": str,
-        "publiclyAccessible": bool,
-        "tags": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateRelationalDatabaseRequestRequestTypeDef(
-    _RequiredCreateRelationalDatabaseRequestRequestTypeDef,
-    _OptionalCreateRelationalDatabaseRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef",
+GetInstancesRequestGetInstancesPaginateTypeDef = TypedDict(
+    "GetInstancesRequestGetInstancesPaginateTypeDef",
     {
-        "relationalDatabaseName": str,
-        "relationalDatabaseSnapshotName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef",
+
+GetKeyPairsRequestGetKeyPairsPaginateTypeDef = TypedDict(
+    "GetKeyPairsRequestGetKeyPairsPaginateTypeDef",
     {
-        "tags": Sequence[TagTypeDef],
+        "includeDefaultKeyPair": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class CreateRelationalDatabaseSnapshotRequestRequestTypeDef(
-    _RequiredCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
-    _OptionalCreateRelationalDatabaseSnapshotRequestRequestTypeDef,
-):
-    pass
-
-_RequiredTagResourceRequestRequestTypeDef = TypedDict(
-    "_RequiredTagResourceRequestRequestTypeDef",
+GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef = TypedDict(
+    "GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef",
     {
-        "resourceName": str,
-        "tags": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalTagResourceRequestRequestTypeDef = TypedDict(
-    "_OptionalTagResourceRequestRequestTypeDef",
+
+GetOperationsRequestGetOperationsPaginateTypeDef = TypedDict(
+    "GetOperationsRequestGetOperationsPaginateTypeDef",
     {
-        "resourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class TagResourceRequestRequestTypeDef(
-    _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
-):
-    pass
-
-CreateCloudFormationStackRequestRequestTypeDef = TypedDict(
-    "CreateCloudFormationStackRequestRequestTypeDef",
+GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef",
     {
-        "instances": Sequence[InstanceEntryTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-CreateDomainEntryRequestRequestTypeDef = TypedDict(
-    "CreateDomainEntryRequestRequestTypeDef",
+GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef",
     {
-        "domainName": str,
-        "domainEntry": DomainEntryTypeDef,
+        "includeInactive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DeleteDomainEntryRequestRequestTypeDef = TypedDict(
-    "DeleteDomainEntryRequestRequestTypeDef",
+_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
     {
-        "domainName": str,
-        "domainEntry": DomainEntryTypeDef,
+        "relationalDatabaseName": str,
     },
 )
-
-UpdateDomainEntryRequestRequestTypeDef = TypedDict(
-    "UpdateDomainEntryRequestRequestTypeDef",
+_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef",
     {
-        "domainName": str,
-        "domainEntry": DomainEntryTypeDef,
+        "durationInMinutes": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-CreateGUISessionAccessDetailsResultTypeDef = TypedDict(
-    "CreateGUISessionAccessDetailsResultTypeDef",
+class GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef(
+    _RequiredGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+    _OptionalGetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
+    "_RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
     {
-        "resourceName": str,
-        "status": StatusType,
-        "percentageComplete": int,
-        "failureReason": str,
-        "sessions": List[SessionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "relationalDatabaseName": str,
     },
 )
-
-InstanceSnapshotInfoTypeDef = TypedDict(
-    "InstanceSnapshotInfoTypeDef",
+_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef = TypedDict(
+    "_OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef",
     {
-        "fromBundleId": str,
-        "fromBlueprintId": str,
-        "fromDiskInfo": List[DiskInfoTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GetDistributionBundlesResultTypeDef = TypedDict(
-    "GetDistributionBundlesResultTypeDef",
+class GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef(
+    _RequiredGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+    _OptionalGetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+):
+    pass
+
+GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef = TypedDict(
+    "GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef",
     {
-        "bundles": List[DistributionBundleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DomainValidationRecordTypeDef = TypedDict(
-    "DomainValidationRecordTypeDef",
+GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef = TypedDict(
+    "GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef",
     {
-        "domainName": str,
-        "resourceRecord": ResourceRecordTypeDef,
-        "dnsRecordCreationState": DnsRecordCreationStateTypeDef,
-        "validationStatus": CertificateDomainValidationStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-EstimateByTimeTypeDef = TypedDict(
-    "EstimateByTimeTypeDef",
+GetStaticIpsRequestGetStaticIpsPaginateTypeDef = TypedDict(
+    "GetStaticIpsRequestGetStaticIpsPaginateTypeDef",
     {
-        "usageCost": float,
-        "pricingUnit": PricingUnitType,
-        "unit": float,
-        "currency": Literal["USD"],
-        "timePeriod": TimePeriodTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetBucketMetricDataResultTypeDef = TypedDict(
     "GetBucketMetricDataResultTypeDef",
     {
         "metricName": BucketMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContainerServiceMetricDataResultTypeDef = TypedDict(
     "GetContainerServiceMetricDataResultTypeDef",
     {
         "metricName": ContainerServiceMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionMetricDataResultTypeDef = TypedDict(
     "GetDistributionMetricDataResultTypeDef",
     {
         "metricName": DistributionMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceMetricDataResultTypeDef = TypedDict(
     "GetInstanceMetricDataResultTypeDef",
     {
         "metricName": InstanceMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoadBalancerMetricDataResultTypeDef = TypedDict(
     "GetLoadBalancerMetricDataResultTypeDef",
     {
         "metricName": LoadBalancerMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseMetricDataResultTypeDef = TypedDict(
     "GetRelationalDatabaseMetricDataResultTypeDef",
     {
         "metricName": RelationalDatabaseMetricNameType,
         "metricData": List[MetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstancePortStatesResultTypeDef = TypedDict(
     "GetInstancePortStatesResultTypeDef",
     {
         "portStates": List[InstancePortStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceStateResultTypeDef = TypedDict(
     "GetInstanceStateResultTypeDef",
     {
         "state": InstanceStateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoadBalancerTlsPoliciesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsPoliciesResultTypeDef",
     {
         "tlsPolicies": List[LoadBalancerTlsPolicyTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseBlueprintsResultTypeDef = TypedDict(
     "GetRelationalDatabaseBlueprintsResultTypeDef",
     {
         "blueprints": List[RelationalDatabaseBlueprintTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseBundlesResultTypeDef = TypedDict(
     "GetRelationalDatabaseBundlesResultTypeDef",
     {
         "bundles": List[RelationalDatabaseBundleTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseEventsResultTypeDef = TypedDict(
     "GetRelationalDatabaseEventsResultTypeDef",
     {
         "relationalDatabaseEvents": List[RelationalDatabaseEventTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseLogEventsResultTypeDef = TypedDict(
     "GetRelationalDatabaseLogEventsResultTypeDef",
     {
         "resourceLogEvents": List[LogEventTypeDef],
         "nextBackwardToken": str,
         "nextForwardToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseParametersResultTypeDef = TypedDict(
     "GetRelationalDatabaseParametersResultTypeDef",
     {
-        "parameters": List[RelationalDatabaseParameterOutputTypeDef],
+        "parameters": List[RelationalDatabaseParameterTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
+    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
+    {
+        "relationalDatabaseName": str,
+        "parameters": Sequence[RelationalDatabaseParameterTypeDef],
     },
 )
 
 InstanceAccessDetailsTypeDef = TypedDict(
     "InstanceAccessDetailsTypeDef",
     {
         "certKey": str,
@@ -3951,15 +3869,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "dnsName": str,
         "state": LoadBalancerStateType,
         "protocol": LoadBalancerProtocolType,
         "publicPorts": List[int],
         "healthCheckPath": str,
         "instancePort": int,
         "instanceHealthSummary": List[InstanceHealthSummaryTypeDef],
@@ -3986,15 +3904,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "relationalDatabaseBlueprintId": str,
         "relationalDatabaseBundleId": str,
         "masterDatabaseName": str,
         "hardware": RelationalDatabaseHardwareTypeDef,
         "state": str,
         "secondaryAvailabilityZone": str,
         "backupRetentionEnabled": bool,
@@ -4010,27 +3928,19 @@
         "masterEndpoint": RelationalDatabaseEndpointTypeDef,
         "pendingMaintenanceActions": List[PendingMaintenanceActionTypeDef],
         "caCertificateIdentifier": str,
     },
     total=False,
 )
 
-UpdateRelationalDatabaseParametersRequestRequestTypeDef = TypedDict(
-    "UpdateRelationalDatabaseParametersRequestRequestTypeDef",
-    {
-        "relationalDatabaseName": str,
-        "parameters": Sequence[RelationalDatabaseParameterTypeDef],
-    },
-)
-
 GetBucketAccessKeysResultTypeDef = TypedDict(
     "GetBucketAccessKeysResultTypeDef",
     {
         "accessKeys": List[AccessKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDiskFromSnapshotRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDiskFromSnapshotRequestRequestTypeDef",
     {
         "diskName": str,
@@ -4146,790 +4056,790 @@
 )
 
 GetAlarmsResultTypeDef = TypedDict(
     "GetAlarmsResultTypeDef",
     {
         "alarms": List[AlarmTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetContactMethodsResultTypeDef = TypedDict(
     "GetContactMethodsResultTypeDef",
     {
         "contactMethods": List[ContactMethodTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocateStaticIpResultTypeDef = TypedDict(
     "AllocateStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachCertificateToDistributionResultTypeDef = TypedDict(
     "AttachCertificateToDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachDiskResultTypeDef = TypedDict(
     "AttachDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachInstancesToLoadBalancerResultTypeDef = TypedDict(
     "AttachInstancesToLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "AttachLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AttachStaticIpResultTypeDef = TypedDict(
     "AttachStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CloseInstancePublicPortsResultTypeDef = TypedDict(
     "CloseInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CopySnapshotResultTypeDef = TypedDict(
     "CopySnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBucketAccessKeyResultTypeDef = TypedDict(
     "CreateBucketAccessKeyResultTypeDef",
     {
         "accessKey": AccessKeyTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCloudFormationStackResultTypeDef = TypedDict(
     "CreateCloudFormationStackResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContactMethodResultTypeDef = TypedDict(
     "CreateContactMethodResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDiskFromSnapshotResultTypeDef = TypedDict(
     "CreateDiskFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDiskResultTypeDef = TypedDict(
     "CreateDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDiskSnapshotResultTypeDef = TypedDict(
     "CreateDiskSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainEntryResultTypeDef = TypedDict(
     "CreateDomainEntryResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDomainResultTypeDef = TypedDict(
     "CreateDomainResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInstanceSnapshotResultTypeDef = TypedDict(
     "CreateInstanceSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInstancesFromSnapshotResultTypeDef = TypedDict(
     "CreateInstancesFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInstancesResultTypeDef = TypedDict(
     "CreateInstancesResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoadBalancerResultTypeDef = TypedDict(
     "CreateLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "CreateLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRelationalDatabaseFromSnapshotResultTypeDef = TypedDict(
     "CreateRelationalDatabaseFromSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRelationalDatabaseResultTypeDef = TypedDict(
     "CreateRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "CreateRelationalDatabaseSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAlarmResultTypeDef = TypedDict(
     "DeleteAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteAutoSnapshotResultTypeDef = TypedDict(
     "DeleteAutoSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBucketAccessKeyResultTypeDef = TypedDict(
     "DeleteBucketAccessKeyResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBucketResultTypeDef = TypedDict(
     "DeleteBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCertificateResultTypeDef = TypedDict(
     "DeleteCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteContactMethodResultTypeDef = TypedDict(
     "DeleteContactMethodResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDiskResultTypeDef = TypedDict(
     "DeleteDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDiskSnapshotResultTypeDef = TypedDict(
     "DeleteDiskSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDistributionResultTypeDef = TypedDict(
     "DeleteDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainEntryResultTypeDef = TypedDict(
     "DeleteDomainEntryResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDomainResultTypeDef = TypedDict(
     "DeleteDomainResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInstanceResultTypeDef = TypedDict(
     "DeleteInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInstanceSnapshotResultTypeDef = TypedDict(
     "DeleteInstanceSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKeyPairResultTypeDef = TypedDict(
     "DeleteKeyPairResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKnownHostKeysResultTypeDef = TypedDict(
     "DeleteKnownHostKeysResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteLoadBalancerResultTypeDef = TypedDict(
     "DeleteLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteLoadBalancerTlsCertificateResultTypeDef = TypedDict(
     "DeleteLoadBalancerTlsCertificateResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRelationalDatabaseResultTypeDef = TypedDict(
     "DeleteRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "DeleteRelationalDatabaseSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachCertificateFromDistributionResultTypeDef = TypedDict(
     "DetachCertificateFromDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachDiskResultTypeDef = TypedDict(
     "DetachDiskResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachInstancesFromLoadBalancerResultTypeDef = TypedDict(
     "DetachInstancesFromLoadBalancerResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetachStaticIpResultTypeDef = TypedDict(
     "DetachStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableAddOnResultTypeDef = TypedDict(
     "DisableAddOnResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableAddOnResultTypeDef = TypedDict(
     "EnableAddOnResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportSnapshotResultTypeDef = TypedDict(
     "ExportSnapshotResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationResultTypeDef = TypedDict(
     "GetOperationResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationsForResourceResultTypeDef = TypedDict(
     "GetOperationsForResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "nextPageCount": str,
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetOperationsResultTypeDef = TypedDict(
     "GetOperationsResultTypeDef",
     {
         "operations": List[OperationTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportKeyPairResultTypeDef = TypedDict(
     "ImportKeyPairResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpenInstancePublicPortsResultTypeDef = TypedDict(
     "OpenInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PeerVpcResultTypeDef = TypedDict(
     "PeerVpcResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAlarmResultTypeDef = TypedDict(
     "PutAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutInstancePublicPortsResultTypeDef = TypedDict(
     "PutInstancePublicPortsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootInstanceResultTypeDef = TypedDict(
     "RebootInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RebootRelationalDatabaseResultTypeDef = TypedDict(
     "RebootRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReleaseStaticIpResultTypeDef = TypedDict(
     "ReleaseStaticIpResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResetDistributionCacheResultTypeDef = TypedDict(
     "ResetDistributionCacheResultTypeDef",
     {
         "status": str,
         "createTime": datetime,
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SendContactMethodVerificationResultTypeDef = TypedDict(
     "SendContactMethodVerificationResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetIpAddressTypeResultTypeDef = TypedDict(
     "SetIpAddressTypeResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetResourceAccessForBucketResultTypeDef = TypedDict(
     "SetResourceAccessForBucketResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartGUISessionResultTypeDef = TypedDict(
     "StartGUISessionResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartInstanceResultTypeDef = TypedDict(
     "StartInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartRelationalDatabaseResultTypeDef = TypedDict(
     "StartRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopGUISessionResultTypeDef = TypedDict(
     "StopGUISessionResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopInstanceResultTypeDef = TypedDict(
     "StopInstanceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopRelationalDatabaseResultTypeDef = TypedDict(
     "StopRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceResultTypeDef = TypedDict(
     "TagResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestAlarmResultTypeDef = TypedDict(
     "TestAlarmResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UnpeerVpcResultTypeDef = TypedDict(
     "UnpeerVpcResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UntagResourceResultTypeDef = TypedDict(
     "UntagResourceResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBucketBundleResultTypeDef = TypedDict(
     "UpdateBucketBundleResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionBundleResultTypeDef = TypedDict(
     "UpdateDistributionBundleResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDistributionResultTypeDef = TypedDict(
     "UpdateDistributionResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainEntryResultTypeDef = TypedDict(
     "UpdateDomainEntryResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateInstanceMetadataOptionsResultTypeDef = TypedDict(
     "UpdateInstanceMetadataOptionsResultTypeDef",
     {
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLoadBalancerAttributeResultTypeDef = TypedDict(
     "UpdateLoadBalancerAttributeResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRelationalDatabaseParametersResultTypeDef = TypedDict(
     "UpdateRelationalDatabaseParametersResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRelationalDatabaseResultTypeDef = TypedDict(
     "UpdateRelationalDatabaseResultTypeDef",
     {
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStaticIpResultTypeDef = TypedDict(
     "GetStaticIpResultTypeDef",
     {
         "staticIp": StaticIpTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStaticIpsResultTypeDef = TypedDict(
     "GetStaticIpsResultTypeDef",
     {
         "staticIps": List[StaticIpTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutoSnapshotsResultTypeDef = TypedDict(
     "GetAutoSnapshotsResultTypeDef",
     {
         "resourceName": str,
         "resourceType": ResourceTypeType,
         "autoSnapshots": List[AutoSnapshotDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRegionsResultTypeDef = TypedDict(
     "GetRegionsResultTypeDef",
     {
         "regions": List[RegionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBucketResultTypeDef = TypedDict(
     "CreateBucketResultTypeDef",
     {
         "bucket": BucketTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetBucketsResultTypeDef = TypedDict(
     "GetBucketsResultTypeDef",
     {
         "buckets": List[BucketTypeDef],
         "nextPageToken": str,
         "accountLevelBpaSync": AccountLevelBpaSyncTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateBucketResultTypeDef = TypedDict(
     "UpdateBucketResultTypeDef",
     {
         "bucket": BucketTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiskSnapshotResultTypeDef = TypedDict(
     "GetDiskSnapshotResultTypeDef",
     {
         "diskSnapshot": DiskSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiskSnapshotsResultTypeDef = TypedDict(
     "GetDiskSnapshotsResultTypeDef",
     {
         "diskSnapshots": List[DiskSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiskResultTypeDef = TypedDict(
     "GetDiskResultTypeDef",
     {
         "disk": DiskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDisksResultTypeDef = TypedDict(
     "GetDisksResultTypeDef",
     {
         "disks": List[DiskTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceHardwareTypeDef = TypedDict(
     "InstanceHardwareTypeDef",
     {
         "cpuCount": int,
@@ -4944,15 +4854,15 @@
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "state": InstanceSnapshotStateType,
         "progress": str,
         "fromAttachedDisks": List[DiskTypeDef],
         "fromInstanceName": str,
         "fromInstanceArn": str,
         "fromBlueprintId": str,
         "fromBundleId": str,
@@ -4965,49 +4875,49 @@
 CreateKeyPairResultTypeDef = TypedDict(
     "CreateKeyPairResultTypeDef",
     {
         "keyPair": KeyPairTypeDef,
         "publicKeyBase64": str,
         "privateKeyBase64": str,
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKeyPairResultTypeDef = TypedDict(
     "GetKeyPairResultTypeDef",
     {
         "keyPair": KeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetKeyPairsResultTypeDef = TypedDict(
     "GetKeyPairsResultTypeDef",
     {
         "keyPairs": List[KeyPairTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseSnapshotResultTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotResultTypeDef",
     {
         "relationalDatabaseSnapshot": RelationalDatabaseSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabaseSnapshotsResultTypeDef = TypedDict(
     "GetRelationalDatabaseSnapshotsResultTypeDef",
     {
         "relationalDatabaseSnapshots": List[RelationalDatabaseSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LightsailDistributionTypeDef = TypedDict(
     "LightsailDistributionTypeDef",
     {
         "name": str,
@@ -5020,20 +4930,20 @@
         "status": str,
         "isEnabled": bool,
         "domainName": str,
         "bundleId": str,
         "certificateName": str,
         "origin": OriginTypeDef,
         "originPublicDNS": str,
-        "defaultCacheBehavior": CacheBehaviorOutputTypeDef,
+        "defaultCacheBehavior": CacheBehaviorTypeDef,
         "cacheBehaviorSettings": CacheSettingsOutputTypeDef,
-        "cacheBehaviors": List[CacheBehaviorPerPathOutputTypeDef],
+        "cacheBehaviors": List[CacheBehaviorPerPathTypeDef],
         "ableToUpdateBundle": bool,
         "ipAddressType": IpAddressTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
@@ -5085,15 +4995,15 @@
     pass
 
 GetCloudFormationStackRecordsResultTypeDef = TypedDict(
     "GetCloudFormationStackRecordsResultTypeDef",
     {
         "cloudFormationStackRecords": List[CloudFormationStackRecordTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateContainerServiceRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateContainerServiceRequestRequestTypeDef",
     {
         "serviceName": str,
@@ -5194,28 +5104,28 @@
     total=False,
 )
 
 GetInstanceAccessDetailsResultTypeDef = TypedDict(
     "GetInstanceAccessDetailsResultTypeDef",
     {
         "accessDetails": InstanceAccessDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LoadBalancerTlsCertificateTypeDef = TypedDict(
     "LoadBalancerTlsCertificateTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "loadBalancerName": str,
         "isAttached": bool,
         "status": LoadBalancerTlsCertificateStatusType,
         "domainName": str,
         "domainValidationRecords": List[LoadBalancerTlsCertificateDomainValidationRecordTypeDef],
         "failureReason": LoadBalancerTlsCertificateFailureReasonType,
         "issuedAt": datetime,
@@ -5234,70 +5144,70 @@
     total=False,
 )
 
 GetLoadBalancerResultTypeDef = TypedDict(
     "GetLoadBalancerResultTypeDef",
     {
         "loadBalancer": LoadBalancerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLoadBalancersResultTypeDef = TypedDict(
     "GetLoadBalancersResultTypeDef",
     {
         "loadBalancers": List[LoadBalancerTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DomainTypeDef = TypedDict(
     "DomainTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "domainEntries": List[DomainEntryOutputTypeDef],
         "registeredDomainDelegationInfo": RegisteredDomainDelegationInfoTypeDef,
     },
     total=False,
 )
 
 GetRelationalDatabaseResultTypeDef = TypedDict(
     "GetRelationalDatabaseResultTypeDef",
     {
         "relationalDatabase": RelationalDatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRelationalDatabasesResultTypeDef = TypedDict(
     "GetRelationalDatabasesResultTypeDef",
     {
         "relationalDatabases": List[RelationalDatabaseTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceTypeDef = TypedDict(
     "InstanceTypeDef",
     {
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "blueprintId": str,
         "blueprintName": str,
         "bundleId": str,
         "addOns": List[AddOnTypeDef],
         "isStaticIp": bool,
         "privateIpAddress": str,
         "publicIpAddress": str,
@@ -5313,54 +5223,54 @@
     total=False,
 )
 
 GetInstanceSnapshotResultTypeDef = TypedDict(
     "GetInstanceSnapshotResultTypeDef",
     {
         "instanceSnapshot": InstanceSnapshotTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceSnapshotsResultTypeDef = TypedDict(
     "GetInstanceSnapshotsResultTypeDef",
     {
         "instanceSnapshots": List[InstanceSnapshotTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDistributionResultTypeDef = TypedDict(
     "CreateDistributionResultTypeDef",
     {
         "distribution": LightsailDistributionTypeDef,
         "operation": OperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDistributionsResultTypeDef = TypedDict(
     "GetDistributionsResultTypeDef",
     {
         "distributions": List[LightsailDistributionTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContainerServiceTypeDef = TypedDict(
     "ContainerServiceTypeDef",
     {
         "containerServiceName": str,
         "arn": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "power": ContainerServicePowerNameType,
         "powerId": str,
         "state": ContainerServiceStateType,
         "stateDetail": ContainerServiceStateDetailTypeDef,
         "scale": int,
         "currentDeployment": ContainerServiceDeploymentTypeDef,
         "nextDeployment": ContainerServiceDeploymentTypeDef,
@@ -5374,15 +5284,15 @@
     total=False,
 )
 
 GetContainerServiceDeploymentsResultTypeDef = TypedDict(
     "GetContainerServiceDeploymentsResultTypeDef",
     {
         "deployments": List[ContainerServiceDeploymentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateContainerServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateContainerServiceRequestRequestTypeDef",
     {
         "serviceName": str,
@@ -5440,15 +5350,15 @@
         "issuerCA": str,
         "notBefore": datetime,
         "notAfter": datetime,
         "eligibleToRenew": str,
         "renewalSummary": RenewalSummaryTypeDef,
         "revokedAt": datetime,
         "revocationReason": str,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
         "supportCode": str,
     },
     total=False,
 )
 
 ResourceBudgetEstimateTypeDef = TypedDict(
     "ResourceBudgetEstimateTypeDef",
@@ -5462,123 +5372,123 @@
     total=False,
 )
 
 GetLoadBalancerTlsCertificatesResultTypeDef = TypedDict(
     "GetLoadBalancerTlsCertificatesResultTypeDef",
     {
         "tlsCertificates": List[LoadBalancerTlsCertificateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainResultTypeDef = TypedDict(
     "GetDomainResultTypeDef",
     {
         "domain": DomainTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainsResultTypeDef = TypedDict(
     "GetDomainsResultTypeDef",
     {
         "domains": List[DomainTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstanceResultTypeDef = TypedDict(
     "GetInstanceResultTypeDef",
     {
         "instance": InstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInstancesResultTypeDef = TypedDict(
     "GetInstancesResultTypeDef",
     {
         "instances": List[InstanceTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ContainerServicesListResultTypeDef = TypedDict(
     "ContainerServicesListResultTypeDef",
     {
         "containerServices": List[ContainerServiceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContainerServiceDeploymentResultTypeDef = TypedDict(
     "CreateContainerServiceDeploymentResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateContainerServiceResultTypeDef = TypedDict(
     "CreateContainerServiceResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateContainerServiceResultTypeDef = TypedDict(
     "UpdateContainerServiceResultTypeDef",
     {
         "containerService": ContainerServiceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetExportSnapshotRecordsResultTypeDef = TypedDict(
     "GetExportSnapshotRecordsResultTypeDef",
     {
         "exportSnapshotRecords": List[ExportSnapshotRecordTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateSummaryTypeDef = TypedDict(
     "CertificateSummaryTypeDef",
     {
         "certificateArn": str,
         "certificateName": str,
         "domainName": str,
         "certificateDetail": CertificateTypeDef,
-        "tags": List[TagOutputTypeDef],
+        "tags": List[TagTypeDef],
     },
     total=False,
 )
 
 GetCostEstimateResultTypeDef = TypedDict(
     "GetCostEstimateResultTypeDef",
     {
         "resourcesBudgetEstimate": List[ResourceBudgetEstimateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCertificateResultTypeDef = TypedDict(
     "CreateCertificateResultTypeDef",
     {
         "certificate": CertificateSummaryTypeDef,
         "operations": List[OperationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCertificatesResultTypeDef = TypedDict(
     "GetCertificatesResultTypeDef",
     {
         "certificates": List[CertificateSummaryTypeDef],
         "nextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/PKG-INFO` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-lightsail
-Version: 1.28.12
-Summary: Type annotations for boto3.Lightsail 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-lightsail.svg?color=blue)](https://pypi.org/project/mypy-boto3-lightsail)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-lightsail)](https://pepy.tech/project/mypy-boto3-lightsail)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Lightsail 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
+[boto3.Lightsail 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail)
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
 [mypy-boto3-lightsail docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_lightsail/).
 
 See how it helps to find and fix potential bugs:
 
@@ -474,40 +474,37 @@
 
 `mypy_boto3_lightsail.type_defs` module contains structures and shapes
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_lightsail.type_defs import (
     AccessKeyLastUsedTypeDef,
-    AccessRulesOutputTypeDef,
     AccessRulesTypeDef,
     AccountLevelBpaSyncTypeDef,
     AutoSnapshotAddOnRequestTypeDef,
     StopInstanceOnIdleRequestTypeDef,
     AddOnTypeDef,
     MonitoredResourceInfoTypeDef,
     ResourceLocationTypeDef,
     AllocateStaticIpRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AttachCertificateToDistributionRequestRequestTypeDef,
     AttachDiskRequestRequestTypeDef,
     AttachInstancesToLoadBalancerRequestRequestTypeDef,
     AttachLoadBalancerTlsCertificateRequestRequestTypeDef,
     AttachStaticIpRequestRequestTypeDef,
     AttachedDiskTypeDef,
     AvailabilityZoneTypeDef,
     BlueprintTypeDef,
-    BucketAccessLogConfigOutputTypeDef,
     BucketAccessLogConfigTypeDef,
     BucketBundleTypeDef,
     BucketStateTypeDef,
     ResourceReceivingAccessTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     BundleTypeDef,
-    CacheBehaviorOutputTypeDef,
-    CacheBehaviorPerPathOutputTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
     CookieObjectOutputTypeDef,
     HeaderObjectOutputTypeDef,
     QueryStringObjectOutputTypeDef,
     CookieObjectTypeDef,
     HeaderObjectTypeDef,
@@ -516,23 +513,21 @@
     CloudFormationStackRecordSourceInfoTypeDef,
     DestinationInfoTypeDef,
     ContainerImageTypeDef,
     ContainerOutputTypeDef,
     ContainerTypeDef,
     ContainerServiceECRImagePullerRoleRequestTypeDef,
     ContainerServiceECRImagePullerRoleTypeDef,
-    ContainerServiceHealthCheckConfigOutputTypeDef,
     ContainerServiceHealthCheckConfigTypeDef,
     ContainerServiceLogEventTypeDef,
     ContainerServicePowerTypeDef,
     ContainerServiceRegistryLoginTypeDef,
     ContainerServiceStateDetailTypeDef,
     CopySnapshotRequestRequestTypeDef,
     CreateBucketAccessKeyRequestRequestTypeDef,
-    TagTypeDef,
     InstanceEntryTypeDef,
     CreateContactMethodRequestRequestTypeDef,
     InputOriginTypeDef,
     DomainEntryTypeDef,
     CreateGUISessionAccessDetailsRequestRequestTypeDef,
     SessionTypeDef,
     DiskMapTypeDef,
@@ -563,139 +558,110 @@
     DisableAddOnRequestRequestTypeDef,
     DiskInfoTypeDef,
     DiskSnapshotInfoTypeDef,
     DistributionBundleTypeDef,
     DnsRecordCreationStateTypeDef,
     DomainEntryOutputTypeDef,
     ResourceRecordTypeDef,
-    DownloadDefaultKeyPairResultTypeDef,
     TimePeriodTypeDef,
     ExportSnapshotRequestRequestTypeDef,
-    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetActiveNamesRequestRequestTypeDef,
-    GetActiveNamesResultTypeDef,
     GetAlarmsRequestRequestTypeDef,
     GetAutoSnapshotsRequestRequestTypeDef,
-    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
     GetBlueprintsRequestRequestTypeDef,
     GetBucketAccessKeysRequestRequestTypeDef,
     GetBucketBundlesRequestRequestTypeDef,
     GetBucketMetricDataRequestRequestTypeDef,
     MetricDatapointTypeDef,
     GetBucketsRequestRequestTypeDef,
-    GetBundlesRequestGetBundlesPaginateTypeDef,
     GetBundlesRequestRequestTypeDef,
     GetCertificatesRequestRequestTypeDef,
-    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
     GetCloudFormationStackRecordsRequestRequestTypeDef,
     GetContactMethodsRequestRequestTypeDef,
-    GetContainerAPIMetadataResultTypeDef,
     GetContainerImagesRequestRequestTypeDef,
     GetContainerLogRequestRequestTypeDef,
     GetContainerServiceDeploymentsRequestRequestTypeDef,
     GetContainerServiceMetricDataRequestRequestTypeDef,
     GetContainerServicesRequestRequestTypeDef,
     GetCostEstimateRequestRequestTypeDef,
     GetDiskRequestRequestTypeDef,
     GetDiskSnapshotRequestRequestTypeDef,
-    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
     GetDiskSnapshotsRequestRequestTypeDef,
-    GetDisksRequestGetDisksPaginateTypeDef,
     GetDisksRequestRequestTypeDef,
     GetDistributionLatestCacheResetRequestRequestTypeDef,
-    GetDistributionLatestCacheResetResultTypeDef,
     GetDistributionMetricDataRequestRequestTypeDef,
     GetDistributionsRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainsRequestGetDomainsPaginateTypeDef,
     GetDomainsRequestRequestTypeDef,
-    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
     GetExportSnapshotRecordsRequestRequestTypeDef,
     GetInstanceAccessDetailsRequestRequestTypeDef,
     GetInstanceMetricDataRequestRequestTypeDef,
     GetInstancePortStatesRequestRequestTypeDef,
     InstancePortStateTypeDef,
     GetInstanceRequestRequestTypeDef,
     GetInstanceSnapshotRequestRequestTypeDef,
-    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
     GetInstanceSnapshotsRequestRequestTypeDef,
     GetInstanceStateRequestRequestTypeDef,
     InstanceStateTypeDef,
-    GetInstancesRequestGetInstancesPaginateTypeDef,
     GetInstancesRequestRequestTypeDef,
     GetKeyPairRequestRequestTypeDef,
-    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
     GetKeyPairsRequestRequestTypeDef,
     GetLoadBalancerMetricDataRequestRequestTypeDef,
     GetLoadBalancerRequestRequestTypeDef,
     GetLoadBalancerTlsCertificatesRequestRequestTypeDef,
     GetLoadBalancerTlsPoliciesRequestRequestTypeDef,
     LoadBalancerTlsPolicyTypeDef,
-    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
     GetLoadBalancersRequestRequestTypeDef,
     GetOperationRequestRequestTypeDef,
     GetOperationsForResourceRequestRequestTypeDef,
-    GetOperationsRequestGetOperationsPaginateTypeDef,
     GetOperationsRequestRequestTypeDef,
     GetRegionsRequestRequestTypeDef,
-    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
     GetRelationalDatabaseBlueprintsRequestRequestTypeDef,
     RelationalDatabaseBlueprintTypeDef,
-    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
     GetRelationalDatabaseBundlesRequestRequestTypeDef,
     RelationalDatabaseBundleTypeDef,
-    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
     GetRelationalDatabaseEventsRequestRequestTypeDef,
     RelationalDatabaseEventTypeDef,
     GetRelationalDatabaseLogEventsRequestRequestTypeDef,
     LogEventTypeDef,
     GetRelationalDatabaseLogStreamsRequestRequestTypeDef,
-    GetRelationalDatabaseLogStreamsResultTypeDef,
     GetRelationalDatabaseMasterUserPasswordRequestRequestTypeDef,
-    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
     GetRelationalDatabaseMetricDataRequestRequestTypeDef,
-    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
     GetRelationalDatabaseParametersRequestRequestTypeDef,
-    RelationalDatabaseParameterOutputTypeDef,
+    RelationalDatabaseParameterTypeDef,
     GetRelationalDatabaseRequestRequestTypeDef,
     GetRelationalDatabaseSnapshotRequestRequestTypeDef,
-    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
     GetRelationalDatabaseSnapshotsRequestRequestTypeDef,
-    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
     GetRelationalDatabasesRequestRequestTypeDef,
     GetStaticIpRequestRequestTypeDef,
-    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetStaticIpsRequestRequestTypeDef,
     HostKeyAttributesTypeDef,
     ImportKeyPairRequestRequestTypeDef,
     PasswordDataTypeDef,
     InstanceHealthSummaryTypeDef,
     InstanceMetadataOptionsTypeDef,
     InstancePortInfoTypeDef,
     MonthlyTransferTypeDef,
-    IsVpcPeeredResultTypeDef,
     OriginTypeDef,
     LoadBalancerTlsCertificateDnsRecordCreationStateTypeDef,
     LoadBalancerTlsCertificateDomainValidationOptionTypeDef,
     LoadBalancerTlsCertificateSummaryTypeDef,
     NameServersUpdateStateTypeDef,
-    PaginatorConfigTypeDef,
     PendingMaintenanceActionTypeDef,
     PendingModifiedRelationalDatabaseValuesTypeDef,
     PutAlarmRequestRequestTypeDef,
     R53HostedZoneDeletionStateTypeDef,
     RebootInstanceRequestRequestTypeDef,
     RebootRelationalDatabaseRequestRequestTypeDef,
     RegisterContainerImageRequestRequestTypeDef,
     RelationalDatabaseEndpointTypeDef,
     RelationalDatabaseHardwareTypeDef,
-    RelationalDatabaseParameterTypeDef,
     ReleaseStaticIpRequestRequestTypeDef,
     ResetDistributionCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SendContactMethodVerificationRequestRequestTypeDef,
     SetIpAddressTypeRequestRequestTypeDef,
     SetResourceAccessForBucketRequestRequestTypeDef,
     StartGUISessionRequestRequestTypeDef,
     StartInstanceRequestRequestTypeDef,
     StartRelationalDatabaseRequestRequestTypeDef,
     StopGUISessionRequestRequestTypeDef,
@@ -710,24 +676,43 @@
     UpdateRelationalDatabaseRequestRequestTypeDef,
     AccessKeyTypeDef,
     AddOnRequestTypeDef,
     AlarmTypeDef,
     ContactMethodTypeDef,
     OperationTypeDef,
     StaticIpTypeDef,
+    DownloadDefaultKeyPairResultTypeDef,
+    GetActiveNamesResultTypeDef,
+    GetContainerAPIMetadataResultTypeDef,
+    GetDistributionLatestCacheResetResultTypeDef,
+    GetRelationalDatabaseLogStreamsResultTypeDef,
+    GetRelationalDatabaseMasterUserPasswordResultTypeDef,
+    IsVpcPeeredResultTypeDef,
     AutoSnapshotDetailsTypeDef,
     RegionTypeDef,
     GetBlueprintsResultTypeDef,
     UpdateBucketRequestRequestTypeDef,
     GetBucketBundlesResultTypeDef,
     BucketTypeDef,
+    CreateBucketRequestRequestTypeDef,
+    CreateCertificateRequestRequestTypeDef,
+    CreateDiskSnapshotRequestRequestTypeDef,
+    CreateDomainRequestRequestTypeDef,
+    CreateInstanceSnapshotRequestRequestTypeDef,
+    CreateKeyPairRequestRequestTypeDef,
+    CreateLoadBalancerRequestRequestTypeDef,
+    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
+    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
+    CreateRelationalDatabaseRequestRequestTypeDef,
+    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
     DiskSnapshotTypeDef,
     DiskTypeDef,
     KeyPairTypeDef,
     RelationalDatabaseSnapshotTypeDef,
+    TagResourceRequestRequestTypeDef,
     GetBundlesResultTypeDef,
     CacheSettingsOutputTypeDef,
     CacheSettingsTypeDef,
     CloseInstancePublicPortsRequestRequestTypeDef,
     OpenInstancePublicPortsRequestRequestTypeDef,
     PutInstancePublicPortsRequestRequestTypeDef,
     CloudFormationStackRecordTypeDef,
@@ -736,57 +721,65 @@
     PrivateRegistryAccessRequestTypeDef,
     PrivateRegistryAccessTypeDef,
     ContainerServiceEndpointTypeDef,
     EndpointRequestTypeDef,
     GetContainerLogResultTypeDef,
     GetContainerServicePowersResultTypeDef,
     CreateContainerServiceRegistryLoginResultTypeDef,
-    CreateBucketRequestRequestTypeDef,
-    CreateCertificateRequestRequestTypeDef,
-    CreateDiskSnapshotRequestRequestTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    CreateInstanceSnapshotRequestRequestTypeDef,
-    CreateKeyPairRequestRequestTypeDef,
-    CreateLoadBalancerRequestRequestTypeDef,
-    CreateLoadBalancerTlsCertificateRequestRequestTypeDef,
-    CreateRelationalDatabaseFromSnapshotRequestRequestTypeDef,
-    CreateRelationalDatabaseRequestRequestTypeDef,
-    CreateRelationalDatabaseSnapshotRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     CreateCloudFormationStackRequestRequestTypeDef,
     CreateDomainEntryRequestRequestTypeDef,
     DeleteDomainEntryRequestRequestTypeDef,
     UpdateDomainEntryRequestRequestTypeDef,
     CreateGUISessionAccessDetailsResultTypeDef,
     InstanceSnapshotInfoTypeDef,
     GetDistributionBundlesResultTypeDef,
     DomainValidationRecordTypeDef,
     EstimateByTimeTypeDef,
+    GetActiveNamesRequestGetActiveNamesPaginateTypeDef,
+    GetBlueprintsRequestGetBlueprintsPaginateTypeDef,
+    GetBundlesRequestGetBundlesPaginateTypeDef,
+    GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef,
+    GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef,
+    GetDisksRequestGetDisksPaginateTypeDef,
+    GetDomainsRequestGetDomainsPaginateTypeDef,
+    GetExportSnapshotRecordsRequestGetExportSnapshotRecordsPaginateTypeDef,
+    GetInstanceSnapshotsRequestGetInstanceSnapshotsPaginateTypeDef,
+    GetInstancesRequestGetInstancesPaginateTypeDef,
+    GetKeyPairsRequestGetKeyPairsPaginateTypeDef,
+    GetLoadBalancersRequestGetLoadBalancersPaginateTypeDef,
+    GetOperationsRequestGetOperationsPaginateTypeDef,
+    GetRelationalDatabaseBlueprintsRequestGetRelationalDatabaseBlueprintsPaginateTypeDef,
+    GetRelationalDatabaseBundlesRequestGetRelationalDatabaseBundlesPaginateTypeDef,
+    GetRelationalDatabaseEventsRequestGetRelationalDatabaseEventsPaginateTypeDef,
+    GetRelationalDatabaseParametersRequestGetRelationalDatabaseParametersPaginateTypeDef,
+    GetRelationalDatabaseSnapshotsRequestGetRelationalDatabaseSnapshotsPaginateTypeDef,
+    GetRelationalDatabasesRequestGetRelationalDatabasesPaginateTypeDef,
+    GetStaticIpsRequestGetStaticIpsPaginateTypeDef,
     GetBucketMetricDataResultTypeDef,
     GetContainerServiceMetricDataResultTypeDef,
     GetDistributionMetricDataResultTypeDef,
     GetInstanceMetricDataResultTypeDef,
     GetLoadBalancerMetricDataResultTypeDef,
     GetRelationalDatabaseMetricDataResultTypeDef,
     GetInstancePortStatesResultTypeDef,
     GetInstanceStateResultTypeDef,
     GetLoadBalancerTlsPoliciesResultTypeDef,
     GetRelationalDatabaseBlueprintsResultTypeDef,
     GetRelationalDatabaseBundlesResultTypeDef,
     GetRelationalDatabaseEventsResultTypeDef,
     GetRelationalDatabaseLogEventsResultTypeDef,
     GetRelationalDatabaseParametersResultTypeDef,
+    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     InstanceAccessDetailsTypeDef,
     InstanceNetworkingTypeDef,
     LoadBalancerTlsCertificateDomainValidationRecordTypeDef,
     LoadBalancerTlsCertificateRenewalSummaryTypeDef,
     LoadBalancerTypeDef,
     RegisteredDomainDelegationInfoTypeDef,
     RelationalDatabaseTypeDef,
-    UpdateRelationalDatabaseParametersRequestRequestTypeDef,
     GetBucketAccessKeysResultTypeDef,
     CreateDiskFromSnapshotRequestRequestTypeDef,
     CreateDiskRequestRequestTypeDef,
     CreateInstancesFromSnapshotRequestRequestTypeDef,
     CreateInstancesRequestRequestTypeDef,
     EnableAddOnRequestRequestTypeDef,
     GetAlarmsResultTypeDef,
```

### Comparing `mypy-boto3-lightsail-1.28.12/mypy_boto3_lightsail.egg-info/SOURCES.txt` & `mypy-boto3-lightsail-1.28.15/mypy_boto3_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-lightsail-1.28.12/setup.py` & `mypy-boto3-lightsail-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-lightsail",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Lightsail 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Lightsail 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

