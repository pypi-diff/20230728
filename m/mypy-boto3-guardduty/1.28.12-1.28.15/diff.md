# Comparing `tmp/mypy-boto3-guardduty-1.28.12.tar.gz` & `tmp/mypy-boto3-guardduty-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-guardduty-1.28.12.tar", last modified: Thu Jul 27 05:34:45 2023, max compression
+gzip compressed data, was "mypy-boto3-guardduty-1.28.15.tar", last modified: Fri Jul 28 20:42:53 2023, max compression
```

## Comparing `mypy-boto3-guardduty-1.28.12.tar` & `mypy-boto3-guardduty-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.324497 mypy-boto3-guardduty-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-07-27 05:34:45.320497 mypy-boto3-guardduty-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.316497 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49732 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49647 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11970 2023-07-27 05:23:13.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    94960 2023-07-27 05:23:16.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    94871 2023-07-27 05:23:14.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:45.320497 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-27 05:34:45.000000 mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:45.324497 mypy-boto3-guardduty-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-27 05:23:12.000000 mypy-boto3-guardduty-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.257171 mypy-boto3-guardduty-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25967 2023-07-28 20:42:53.257171 mypy-boto3-guardduty-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24472 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.245171 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49732 2023-07-28 20:27:13.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49647 2023-07-28 20:27:13.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-07-28 20:27:14.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14088 2023-07-28 20:27:14.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-07-28 20:27:13.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-07-28 20:27:13.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94150 2023-07-28 20:27:16.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94063 2023-07-28 20:27:15.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:53.257171 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25967 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-28 20:42:53.000000 mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:53.257171 mypy-boto3-guardduty-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-07-28 20:27:11.000000 mypy-boto3-guardduty-1.28.15/setup.py
```

### Comparing `mypy-boto3-guardduty-1.28.12/LICENSE` & `mypy-boto3-guardduty-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.12/PKG-INFO` & `mypy-boto3-guardduty-1.28.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.28.12
-Summary: Type annotations for boto3.GuardDuty 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,41 +415,38 @@
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
-    CreateFilterResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
-    DestinationPropertiesOutputTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
@@ -461,58 +458,42 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
-    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
     LineageObjectTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
     MemberAdditionalConfigurationResultTypeDef,
     MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
@@ -524,64 +505,81 @@
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
-    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    ScanConditionPairOutputTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
     StartMalwareScanRequestRequestTypeDef,
-    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateIPSetResponseTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetThreatIntelSetResponseTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
+    StartMalwareScanResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
+    DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
-    DescribePublishingDestinationResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.28.12/README.md` & `mypy-boto3-guardduty-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -383,41 +383,38 @@
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
-    CreateFilterResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
-    DestinationPropertiesOutputTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
@@ -429,58 +426,42 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
-    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
     LineageObjectTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
     MemberAdditionalConfigurationResultTypeDef,
     MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
@@ -492,64 +473,81 @@
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
-    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    ScanConditionPairOutputTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
     StartMalwareScanRequestRequestTypeDef,
-    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateIPSetResponseTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetThreatIntelSetResponseTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
+    StartMalwareScanResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
+    DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
-    DescribePublishingDestinationResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__init__.py` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__init__.pyi` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/__main__.py` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.GuardDuty 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.GuardDuty 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
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

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/client.py` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/client.pyi` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/literals.py` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/literals.pyi` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/paginator.py` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -69,185 +69,173 @@
     "ListIPSetsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
     "ListThreatIntelSetsPaginator",
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
 class DescribeMalwareScansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#describemalwarescanspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: FilterCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMalwareScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#describemalwarescanspaginator)
         """
 
-
 class ListCoveragePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
         SortCriteria: CoverageSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listcoveragepaginator)
         """
 
-
 class ListDetectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listdetectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listdetectorspaginator)
         """
 
-
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfilterspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfilterspaginator)
         """
 
-
 class ListFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
         """
 
-
 class ListIPSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listipsetspaginator)
         """
 
-
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listinvitationspaginator)
         """
 
-
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listmemberspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         OnlyAssociated: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listmemberspaginator)
         """
 
-
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listorganizationadminaccountspaginator)
         """
 
-
 class ListThreatIntelSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listthreatintelsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThreatIntelSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listthreatintelsetspaginator)
         """
```

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/paginator.pyi` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/paginator.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,173 +69,185 @@
     "ListIPSetsPaginator",
     "ListInvitationsPaginator",
     "ListMembersPaginator",
     "ListOrganizationAdminAccountsPaginator",
     "ListThreatIntelSetsPaginator",
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
 class DescribeMalwareScansPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#describemalwarescanspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: FilterCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[DescribeMalwareScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#describemalwarescanspaginator)
         """
 
+
 class ListCoveragePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
         SortCriteria: CoverageSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listcoveragepaginator)
         """
 
+
 class ListDetectorsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listdetectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listdetectorspaginator)
         """
 
+
 class ListFiltersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfilterspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfilterspaginator)
         """
 
+
 class ListFindingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FindingCriteria: FindingCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listfindingspaginator)
         """
 
+
 class ListIPSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listipsetspaginator)
         """
 
+
 class ListInvitationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listinvitationspaginator)
         """
 
+
 class ListMembersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listmemberspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         OnlyAssociated: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listmemberspaginator)
         """
 
+
 class ListOrganizationAdminAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listorganizationadminaccountspaginator)
         """
 
+
 class ListThreatIntelSetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listthreatintelsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThreatIntelSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/paginators/#listthreatintelsetspaginator)
         """
```

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/type_defs.py` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,41 +81,38 @@
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
     "CoverageFilterConditionTypeDef",
     "CoverageSortCriteriaTypeDef",
     "CoverageStatisticsTypeDef",
-    "CreateFilterResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateIPSetRequestRequestTypeDef",
-    "CreateIPSetResponseTypeDef",
     "UnprocessedAccountTypeDef",
     "DestinationPropertiesTypeDef",
-    "CreatePublishingDestinationResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
     "CreateThreatIntelSetRequestRequestTypeDef",
-    "CreateThreatIntelSetResponseTypeDef",
     "DNSLogsConfigurationResultTypeDef",
     "FlowLogsConfigurationResultTypeDef",
     "S3LogsConfigurationResultTypeDef",
     "S3LogsConfigurationTypeDef",
     "DataSourceFreeTrialTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DefaultServerSideEncryptionTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DeletePublishingDestinationRequestRequestTypeDef",
     "DeleteThreatIntelSetRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "SortCriteriaTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
     "DescribePublishingDestinationRequestRequestTypeDef",
-    "DestinationPropertiesOutputTypeDef",
     "DestinationTypeDef",
     "DetectorAdditionalConfigurationResultTypeDef",
     "DetectorAdditionalConfigurationTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateFromAdministratorAccountRequestRequestTypeDef",
     "DisassociateFromMasterAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
@@ -127,58 +124,42 @@
     "FilterConditionTypeDef",
     "FindingStatisticsTypeDef",
     "GeoLocationTypeDef",
     "GetAdministratorAccountRequestRequestTypeDef",
     "GetDetectorRequestRequestTypeDef",
     "GetFilterRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
-    "GetIPSetResponseTypeDef",
-    "GetInvitationsCountResponseTypeDef",
     "GetMalwareScanSettingsRequestRequestTypeDef",
     "GetMasterAccountRequestRequestTypeDef",
     "MasterTypeDef",
     "GetMemberDetectorsRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "GetRemainingFreeTrialDaysRequestRequestTypeDef",
     "GetThreatIntelSetRequestRequestTypeDef",
-    "GetThreatIntelSetResponseTypeDef",
     "UsageCriteriaTypeDef",
     "HighestSeverityThreatDetailsTypeDef",
     "HostPathTypeDef",
     "IamInstanceProfileTypeDef",
     "ProductCodeTypeDef",
     "InvitationTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "KubernetesAuditLogsConfigurationResultTypeDef",
     "KubernetesAuditLogsConfigurationTypeDef",
     "KubernetesUserDetailsTypeDef",
     "LineageObjectTypeDef",
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
     "ListDetectorsRequestRequestTypeDef",
-    "ListDetectorsResponseTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
-    "ListFiltersResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
-    "ListIPSetsResponseTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListPublishingDestinationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "ListThreatIntelSetsRequestRequestTypeDef",
-    "ListThreatIntelSetsResponseTypeDef",
     "LocalIpDetailsTypeDef",
     "LocalPortDetailsTypeDef",
     "LoginAttributeTypeDef",
     "ScanEc2InstanceWithFindingsTypeDef",
     "MemberAdditionalConfigurationResultTypeDef",
     "MemberAdditionalConfigurationTypeDef",
     "RemotePortDetailsTypeDef",
@@ -190,64 +171,81 @@
     "OrganizationS3LogsConfigurationTypeDef",
     "OrganizationEbsVolumesResultTypeDef",
     "OrganizationEbsVolumesTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationResultTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationTypeDef",
     "OrganizationTypeDef",
     "OwnerTypeDef",
-    "PaginatorConfigTypeDef",
     "RdsDbUserDetailsTypeDef",
     "ResourceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
-    "ScanConditionPairOutputTypeDef",
     "ScanConditionPairTypeDef",
     "ScannedItemCountTypeDef",
     "ThreatsDetectedItemCountTypeDef",
     "ScanFilePathTypeDef",
     "ScanResultDetailsTypeDef",
     "TriggerDetailsTypeDef",
     "ServiceAdditionalInfoTypeDef",
     "StartMalwareScanRequestRequestTypeDef",
-    "StartMalwareScanResponseTypeDef",
     "StartMonitoringMembersRequestRequestTypeDef",
     "StopMonitoringMembersRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TotalTypeDef",
     "UnarchiveFindingsRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateFilterResponseTypeDef",
     "UpdateFindingsFeedbackRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "CoverageEksClusterDetailsTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "GetAdministratorAccountResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
     "CoverageFilterCriterionTypeDef",
+    "CreateFilterResponseTypeDef",
+    "CreateIPSetResponseTypeDef",
+    "CreatePublishingDestinationResponseTypeDef",
+    "CreateThreatIntelSetResponseTypeDef",
+    "GetAdministratorAccountResponseTypeDef",
     "GetCoverageStatisticsResponseTypeDef",
+    "GetIPSetResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "GetThreatIntelSetResponseTypeDef",
+    "ListDetectorsResponseTypeDef",
+    "ListFiltersResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListIPSetsResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListThreatIntelSetsResponseTypeDef",
+    "StartMalwareScanResponseTypeDef",
+    "UpdateFilterResponseTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DisassociateMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "StartMonitoringMembersResponseTypeDef",
     "StopMonitoringMembersResponseTypeDef",
     "UpdateMemberDetectorsResponseTypeDef",
     "CreatePublishingDestinationRequestRequestTypeDef",
+    "DescribePublishingDestinationResponseTypeDef",
     "UpdatePublishingDestinationRequestRequestTypeDef",
     "KubernetesDataSourceFreeTrialTypeDef",
     "MalwareProtectionDataSourceFreeTrialTypeDef",
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "DescribePublishingDestinationResponseTypeDef",
     "ListPublishingDestinationsResponseTypeDef",
     "DetectorFeatureConfigurationResultTypeDef",
     "DetectorFeatureConfigurationTypeDef",
     "EbsVolumeDetailsTypeDef",
     "ScanEc2InstanceWithFindingsResultTypeDef",
     "EksClusterDetailsTypeDef",
     "RdsDbInstanceDetailsTypeDef",
@@ -594,19 +592,22 @@
     {
         "CountByResourceType": Dict[Literal["EKS"], int],
         "CountByCoverageStatus": Dict[CoverageStatusType, int],
     },
     total=False,
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateIPSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -628,22 +629,14 @@
 
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
 
-CreateIPSetResponseTypeDef = TypedDict(
-    "CreateIPSetResponseTypeDef",
-    {
-        "IpSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnprocessedAccountTypeDef = TypedDict(
     "UnprocessedAccountTypeDef",
     {
         "AccountId": str,
         "Result": str,
     },
 )
@@ -653,22 +646,14 @@
     {
         "DestinationArn": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-CreatePublishingDestinationResponseTypeDef = TypedDict(
-    "CreatePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSampleFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalCreateSampleFindingsRequestRequestTypeDef = TypedDict(
@@ -710,22 +695,14 @@
 class CreateThreatIntelSetRequestRequestTypeDef(
     _RequiredCreateThreatIntelSetRequestRequestTypeDef,
     _OptionalCreateThreatIntelSetRequestRequestTypeDef,
 ):
     pass
 
 
-CreateThreatIntelSetResponseTypeDef = TypedDict(
-    "CreateThreatIntelSetResponseTypeDef",
-    {
-        "ThreatIntelSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DNSLogsConfigurationResultTypeDef = TypedDict(
     "DNSLogsConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
@@ -824,14 +801,24 @@
     "DeleteThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 SortCriteriaTypeDef = TypedDict(
     "SortCriteriaTypeDef",
     {
         "AttributeName": str,
         "OrderBy": OrderByType,
     },
     total=False,
@@ -864,23 +851,14 @@
     "DescribePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
 
-DestinationPropertiesOutputTypeDef = TypedDict(
-    "DestinationPropertiesOutputTypeDef",
-    {
-        "DestinationArn": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
     },
@@ -1035,34 +1013,14 @@
     "GetIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "IpSetId": str,
     },
 )
 
-GetIPSetResponseTypeDef = TypedDict(
-    "GetIPSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": IpSetFormatType,
-        "Location": str,
-        "Status": IpSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "InvitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "GetMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 
@@ -1151,26 +1109,14 @@
     "GetThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
-GetThreatIntelSetResponseTypeDef = TypedDict(
-    "GetThreatIntelSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": ThreatIntelSetFormatType,
-        "Location": str,
-        "Status": ThreatIntelSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UsageCriteriaTypeDef = TypedDict(
     "UsageCriteriaTypeDef",
     {
         "AccountIds": Sequence[str],
         "DataSources": Sequence[DataSourceType],
         "Resources": Sequence[str],
         "Features": Sequence[UsageFeatureType],
@@ -1285,62 +1231,23 @@
         "ExecutablePath": str,
         "Euid": int,
         "ParentUuid": str,
     },
     total=False,
 )
 
-ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDetectorsRequestRequestTypeDef = TypedDict(
     "ListDetectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListDetectorsResponseTypeDef = TypedDict(
-    "ListDetectorsResponseTypeDef",
-    {
-        "DetectorIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFiltersRequestListFiltersPaginateTypeDef(
-    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
-    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredListFiltersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFiltersRequestRequestTypeDef = TypedDict(
@@ -1355,54 +1262,14 @@
 
 class ListFiltersRequestRequestTypeDef(
     _RequiredListFiltersRequestRequestTypeDef, _OptionalListFiltersRequestRequestTypeDef
 ):
     pass
 
 
-ListFiltersResponseTypeDef = TypedDict(
-    "ListFiltersResponseTypeDef",
-    {
-        "FilterNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "FindingIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIPSetsRequestListIPSetsPaginateTypeDef(
-    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
-    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIPSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListIPSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListIPSetsRequestRequestTypeDef = TypedDict(
@@ -1417,63 +1284,23 @@
 
 class ListIPSetsRequestRequestTypeDef(
     _RequiredListIPSetsRequestRequestTypeDef, _OptionalListIPSetsRequestRequestTypeDef
 ):
     pass
 
 
-ListIPSetsResponseTypeDef = TypedDict(
-    "ListIPSetsResponseTypeDef",
-    {
-        "IpSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersRequestListMembersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMembersRequestListMembersPaginateTypeDef(
-    _RequiredListMembersRequestListMembersPaginateTypeDef,
-    _OptionalListMembersRequestListMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListMembersRequestRequestTypeDef = TypedDict(
@@ -1489,22 +1316,14 @@
 
 class ListMembersRequestRequestTypeDef(
     _RequiredListMembersRequestRequestTypeDef, _OptionalListMembersRequestRequestTypeDef
 ):
     pass
 
 
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1536,44 +1355,14 @@
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
-_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
-    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThreatIntelSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListThreatIntelSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListThreatIntelSetsRequestRequestTypeDef = TypedDict(
@@ -1589,23 +1378,14 @@
 class ListThreatIntelSetsRequestRequestTypeDef(
     _RequiredListThreatIntelSetsRequestRequestTypeDef,
     _OptionalListThreatIntelSetsRequestRequestTypeDef,
 ):
     pass
 
 
-ListThreatIntelSetsResponseTypeDef = TypedDict(
-    "ListThreatIntelSetsResponseTypeDef",
-    {
-        "ThreatIntelSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LocalIpDetailsTypeDef = TypedDict(
     "LocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
@@ -1761,24 +1541,14 @@
     "OwnerTypeDef",
     {
         "Id": str,
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
 RdsDbUserDetailsTypeDef = TypedDict(
     "RdsDbUserDetailsTypeDef",
     {
         "User": str,
         "Application": str,
         "Database": str,
         "Ssl": str,
@@ -1791,46 +1561,14 @@
     "ResourceDetailsTypeDef",
     {
         "InstanceArn": str,
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
-_RequiredScanConditionPairOutputTypeDef = TypedDict(
-    "_RequiredScanConditionPairOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalScanConditionPairOutputTypeDef = TypedDict(
-    "_OptionalScanConditionPairOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class ScanConditionPairOutputTypeDef(
-    _RequiredScanConditionPairOutputTypeDef, _OptionalScanConditionPairOutputTypeDef
-):
-    pass
-
-
 _RequiredScanConditionPairTypeDef = TypedDict(
     "_RequiredScanConditionPairTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalScanConditionPairTypeDef = TypedDict(
@@ -1906,22 +1644,14 @@
 StartMalwareScanRequestRequestTypeDef = TypedDict(
     "StartMalwareScanRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-StartMalwareScanResponseTypeDef = TypedDict(
-    "StartMalwareScanResponseTypeDef",
-    {
-        "ScanId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartMonitoringMembersRequestRequestTypeDef = TypedDict(
     "StartMonitoringMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountIds": Sequence[str],
     },
 )
@@ -1963,22 +1693,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFindingsFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingsFeedbackRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
         "Feedback": FeedbackType,
     },
@@ -2071,31 +1793,14 @@
         "CoveredNodes": int,
         "CompatibleNodes": int,
         "AddonDetails": AddonDetailsTypeDef,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAdministratorAccountResponseTypeDef = TypedDict(
-    "GetAdministratorAccountResponseTypeDef",
-    {
-        "Administrator": AdministratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
@@ -2137,91 +1842,241 @@
     {
         "CriterionKey": CoverageFilterCriterionKeyType,
         "FilterCondition": CoverageFilterConditionTypeDef,
     },
     total=False,
 )
 
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIPSetResponseTypeDef = TypedDict(
+    "CreateIPSetResponseTypeDef",
+    {
+        "IpSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePublishingDestinationResponseTypeDef = TypedDict(
+    "CreatePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThreatIntelSetResponseTypeDef = TypedDict(
+    "CreateThreatIntelSetResponseTypeDef",
+    {
+        "ThreatIntelSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAdministratorAccountResponseTypeDef = TypedDict(
+    "GetAdministratorAccountResponseTypeDef",
+    {
+        "Administrator": AdministratorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCoverageStatisticsResponseTypeDef = TypedDict(
     "GetCoverageStatisticsResponseTypeDef",
     {
         "CoverageStatistics": CoverageStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIPSetResponseTypeDef = TypedDict(
+    "GetIPSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": IpSetFormatType,
+        "Location": str,
+        "Status": IpSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetThreatIntelSetResponseTypeDef = TypedDict(
+    "GetThreatIntelSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": ThreatIntelSetFormatType,
+        "Location": str,
+        "Status": ThreatIntelSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDetectorsResponseTypeDef = TypedDict(
+    "ListDetectorsResponseTypeDef",
+    {
+        "DetectorIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFiltersResponseTypeDef = TypedDict(
+    "ListFiltersResponseTypeDef",
+    {
+        "FilterNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "FindingIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIPSetsResponseTypeDef = TypedDict(
+    "ListIPSetsResponseTypeDef",
+    {
+        "IpSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
+        "NextToken": str,
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
+ListThreatIntelSetsResponseTypeDef = TypedDict(
+    "ListThreatIntelSetsResponseTypeDef",
+    {
+        "ThreatIntelSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMalwareScanResponseTypeDef = TypedDict(
+    "StartMalwareScanResponseTypeDef",
+    {
+        "ScanId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateMembersResponseTypeDef = TypedDict(
     "DisassociateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMonitoringMembersResponseTypeDef = TypedDict(
     "StartMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopMonitoringMembersResponseTypeDef = TypedDict(
     "StopMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMemberDetectorsResponseTypeDef = TypedDict(
     "UpdateMemberDetectorsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2241,14 +2096,26 @@
 class CreatePublishingDestinationRequestRequestTypeDef(
     _RequiredCreatePublishingDestinationRequestRequestTypeDef,
     _OptionalCreatePublishingDestinationRequestRequestTypeDef,
 ):
     pass
 
 
+DescribePublishingDestinationResponseTypeDef = TypedDict(
+    "DescribePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "DestinationType": Literal["S3"],
+        "Status": PublishingStatusType,
+        "PublishingFailureStartTimestamp": int,
+        "DestinationProperties": DestinationPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
@@ -2280,14 +2147,127 @@
     "MalwareProtectionDataSourceFreeTrialTypeDef",
     {
         "ScanEc2InstanceWithFindings": DataSourceFreeTrialTypeDef,
     },
     total=False,
 )
 
+ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFiltersRequestListFiltersPaginateTypeDef(
+    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
+    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIPSetsRequestListIPSetsPaginateTypeDef(
+    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
+    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
+):
+    pass
+
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersRequestListMembersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMembersRequestListMembersPaginateTypeDef(
+    _RequiredListMembersRequestListMembersPaginateTypeDef,
+    _OptionalListMembersRequestListMembersPaginateTypeDef,
+):
+    pass
+
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
+    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
     },
 )
@@ -2302,32 +2282,20 @@
 
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
 
-DescribePublishingDestinationResponseTypeDef = TypedDict(
-    "DescribePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "DestinationType": Literal["S3"],
-        "Status": PublishingStatusType,
-        "PublishingFailureStartTimestamp": int,
-        "DestinationProperties": DestinationPropertiesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPublishingDestinationsResponseTypeDef = TypedDict(
     "ListPublishingDestinationsResponseTypeDef",
     {
         "Destinations": List[DestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectorFeatureConfigurationResultTypeDef = TypedDict(
     "DetectorFeatureConfigurationResultTypeDef",
     {
         "Name": DetectorFeatureResultType,
@@ -2408,41 +2376,41 @@
     total=False,
 )
 
 GetFindingsStatisticsResponseTypeDef = TypedDict(
     "GetFindingsStatisticsResponseTypeDef",
     {
         "FindingStatistics": FindingStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": MasterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2478,15 +2446,15 @@
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KubernetesConfigurationResultTypeDef = TypedDict(
     "KubernetesConfigurationResultTypeDef",
     {
         "AuditLogs": KubernetesAuditLogsConfigurationResultTypeDef,
@@ -2637,15 +2605,15 @@
     },
     total=False,
 )
 
 ScanConditionOutputTypeDef = TypedDict(
     "ScanConditionOutputTypeDef",
     {
-        "MapEquals": List[ScanConditionPairOutputTypeDef],
+        "MapEquals": List[ScanConditionPairTypeDef],
     },
 )
 
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
         "MapEquals": Sequence[ScanConditionPairTypeDef],
@@ -2744,15 +2712,15 @@
     {
         "Name": str,
         "Description": str,
         "Action": FilterActionType,
         "Rank": int,
         "FindingCriteria": FindingCriteriaOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2809,15 +2777,15 @@
     },
 )
 _OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
     {
         "FindingCriteria": FindingCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListFindingsRequestListFindingsPaginateTypeDef(
     _RequiredListFindingsRequestListFindingsPaginateTypeDef,
@@ -3126,15 +3094,15 @@
 )
 
 DescribeMalwareScansResponseTypeDef = TypedDict(
     "DescribeMalwareScansResponseTypeDef",
     {
         "Scans": List[ScanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageStatisticsTypeDef = TypedDict(
     "UsageStatisticsTypeDef",
     {
         "SumByAccount": List[UsageAccountResultTypeDef],
@@ -3199,15 +3167,15 @@
     },
 )
 _OptionalListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
     "_OptionalListCoverageRequestListCoveragePaginateTypeDef",
     {
         "FilterCriteria": CoverageFilterCriteriaTypeDef,
         "SortCriteria": CoverageSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListCoverageRequestListCoveragePaginateTypeDef(
     _RequiredListCoverageRequestListCoveragePaginateTypeDef,
@@ -3290,15 +3258,15 @@
     },
 )
 _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef = TypedDict(
     "_OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef",
     {
         "FilterCriteria": FilterCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef(
     _RequiredDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
@@ -3481,15 +3449,15 @@
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
         "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3524,24 +3492,24 @@
 )
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "UsageStatistics": UsageStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "Resources": List[CoverageResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3BucketDetailTypeDef = TypedDict(
     "S3BucketDetailTypeDef",
     {
         "Arn": str,
@@ -3557,30 +3525,30 @@
 )
 
 GetRemainingFreeTrialDaysResponseTypeDef = TypedDict(
     "GetRemainingFreeTrialDaysResponseTypeDef",
     {
         "Accounts": List[AccountFreeTrialInfoTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDetectorResponseTypeDef = TypedDict(
     "GetDetectorResponseTypeDef",
     {
         "CreatedAt": str,
         "FindingPublishingFrequency": FindingPublishingFrequencyType,
         "ServiceRole": str,
         "Status": DetectorStatusType,
         "UpdatedAt": str,
         "DataSources": DataSourceConfigurationsResultTypeDef,
         "Tags": Dict[str, str],
         "Features": List[DetectorFeatureConfigurationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMemberDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredMemberDataSourceConfigurationTypeDef",
     {
         "AccountId": str,
@@ -3603,28 +3571,28 @@
 
 
 CreateDetectorResponseTypeDef = TypedDict(
     "CreateDetectorResponseTypeDef",
     {
         "DetectorId": str,
         "UnprocessedDataSources": UnprocessedDataSourcesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "AutoEnable": bool,
         "MemberAccountLimitReached": bool,
         "DataSources": OrganizationDataSourceConfigurationsResultTypeDef,
         "Features": List[OrganizationFeatureConfigurationResultTypeDef],
         "NextToken": str,
         "AutoEnableOrganizationMembers": AutoEnableMembersType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3697,15 +3665,15 @@
 )
 
 GetMemberDetectorsResponseTypeDef = TypedDict(
     "GetMemberDetectorsResponseTypeDef",
     {
         "MemberDataSourceConfigurations": List[MemberDataSourceConfigurationTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "Action": ActionTypeDef,
@@ -3758,10 +3726,10 @@
     pass
 
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "Findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty/type_defs.pyi` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -80,41 +80,38 @@
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
     "CoverageFilterConditionTypeDef",
     "CoverageSortCriteriaTypeDef",
     "CoverageStatisticsTypeDef",
-    "CreateFilterResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateIPSetRequestRequestTypeDef",
-    "CreateIPSetResponseTypeDef",
     "UnprocessedAccountTypeDef",
     "DestinationPropertiesTypeDef",
-    "CreatePublishingDestinationResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
     "CreateThreatIntelSetRequestRequestTypeDef",
-    "CreateThreatIntelSetResponseTypeDef",
     "DNSLogsConfigurationResultTypeDef",
     "FlowLogsConfigurationResultTypeDef",
     "S3LogsConfigurationResultTypeDef",
     "S3LogsConfigurationTypeDef",
     "DataSourceFreeTrialTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DefaultServerSideEncryptionTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DeletePublishingDestinationRequestRequestTypeDef",
     "DeleteThreatIntelSetRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "SortCriteriaTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
     "DescribePublishingDestinationRequestRequestTypeDef",
-    "DestinationPropertiesOutputTypeDef",
     "DestinationTypeDef",
     "DetectorAdditionalConfigurationResultTypeDef",
     "DetectorAdditionalConfigurationTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateFromAdministratorAccountRequestRequestTypeDef",
     "DisassociateFromMasterAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
@@ -126,58 +123,42 @@
     "FilterConditionTypeDef",
     "FindingStatisticsTypeDef",
     "GeoLocationTypeDef",
     "GetAdministratorAccountRequestRequestTypeDef",
     "GetDetectorRequestRequestTypeDef",
     "GetFilterRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
-    "GetIPSetResponseTypeDef",
-    "GetInvitationsCountResponseTypeDef",
     "GetMalwareScanSettingsRequestRequestTypeDef",
     "GetMasterAccountRequestRequestTypeDef",
     "MasterTypeDef",
     "GetMemberDetectorsRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "GetRemainingFreeTrialDaysRequestRequestTypeDef",
     "GetThreatIntelSetRequestRequestTypeDef",
-    "GetThreatIntelSetResponseTypeDef",
     "UsageCriteriaTypeDef",
     "HighestSeverityThreatDetailsTypeDef",
     "HostPathTypeDef",
     "IamInstanceProfileTypeDef",
     "ProductCodeTypeDef",
     "InvitationTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "KubernetesAuditLogsConfigurationResultTypeDef",
     "KubernetesAuditLogsConfigurationTypeDef",
     "KubernetesUserDetailsTypeDef",
     "LineageObjectTypeDef",
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
     "ListDetectorsRequestRequestTypeDef",
-    "ListDetectorsResponseTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
-    "ListFiltersResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
-    "ListIPSetsResponseTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListPublishingDestinationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "ListThreatIntelSetsRequestRequestTypeDef",
-    "ListThreatIntelSetsResponseTypeDef",
     "LocalIpDetailsTypeDef",
     "LocalPortDetailsTypeDef",
     "LoginAttributeTypeDef",
     "ScanEc2InstanceWithFindingsTypeDef",
     "MemberAdditionalConfigurationResultTypeDef",
     "MemberAdditionalConfigurationTypeDef",
     "RemotePortDetailsTypeDef",
@@ -189,64 +170,81 @@
     "OrganizationS3LogsConfigurationTypeDef",
     "OrganizationEbsVolumesResultTypeDef",
     "OrganizationEbsVolumesTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationResultTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationTypeDef",
     "OrganizationTypeDef",
     "OwnerTypeDef",
-    "PaginatorConfigTypeDef",
     "RdsDbUserDetailsTypeDef",
     "ResourceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
-    "ScanConditionPairOutputTypeDef",
     "ScanConditionPairTypeDef",
     "ScannedItemCountTypeDef",
     "ThreatsDetectedItemCountTypeDef",
     "ScanFilePathTypeDef",
     "ScanResultDetailsTypeDef",
     "TriggerDetailsTypeDef",
     "ServiceAdditionalInfoTypeDef",
     "StartMalwareScanRequestRequestTypeDef",
-    "StartMalwareScanResponseTypeDef",
     "StartMonitoringMembersRequestRequestTypeDef",
     "StopMonitoringMembersRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TotalTypeDef",
     "UnarchiveFindingsRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateFilterResponseTypeDef",
     "UpdateFindingsFeedbackRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "CoverageEksClusterDetailsTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "GetAdministratorAccountResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
     "CoverageFilterCriterionTypeDef",
+    "CreateFilterResponseTypeDef",
+    "CreateIPSetResponseTypeDef",
+    "CreatePublishingDestinationResponseTypeDef",
+    "CreateThreatIntelSetResponseTypeDef",
+    "GetAdministratorAccountResponseTypeDef",
     "GetCoverageStatisticsResponseTypeDef",
+    "GetIPSetResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "GetThreatIntelSetResponseTypeDef",
+    "ListDetectorsResponseTypeDef",
+    "ListFiltersResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListIPSetsResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListThreatIntelSetsResponseTypeDef",
+    "StartMalwareScanResponseTypeDef",
+    "UpdateFilterResponseTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DisassociateMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "StartMonitoringMembersResponseTypeDef",
     "StopMonitoringMembersResponseTypeDef",
     "UpdateMemberDetectorsResponseTypeDef",
     "CreatePublishingDestinationRequestRequestTypeDef",
+    "DescribePublishingDestinationResponseTypeDef",
     "UpdatePublishingDestinationRequestRequestTypeDef",
     "KubernetesDataSourceFreeTrialTypeDef",
     "MalwareProtectionDataSourceFreeTrialTypeDef",
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
-    "DescribePublishingDestinationResponseTypeDef",
     "ListPublishingDestinationsResponseTypeDef",
     "DetectorFeatureConfigurationResultTypeDef",
     "DetectorFeatureConfigurationTypeDef",
     "EbsVolumeDetailsTypeDef",
     "ScanEc2InstanceWithFindingsResultTypeDef",
     "EksClusterDetailsTypeDef",
     "RdsDbInstanceDetailsTypeDef",
@@ -593,19 +591,22 @@
     {
         "CountByResourceType": Dict[Literal["EKS"], int],
         "CountByCoverageStatus": Dict[CoverageStatusType, int],
     },
     total=False,
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateIPSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -625,22 +626,14 @@
 )
 
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
-CreateIPSetResponseTypeDef = TypedDict(
-    "CreateIPSetResponseTypeDef",
-    {
-        "IpSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnprocessedAccountTypeDef = TypedDict(
     "UnprocessedAccountTypeDef",
     {
         "AccountId": str,
         "Result": str,
     },
 )
@@ -650,22 +643,14 @@
     {
         "DestinationArn": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-CreatePublishingDestinationResponseTypeDef = TypedDict(
-    "CreatePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSampleFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalCreateSampleFindingsRequestRequestTypeDef = TypedDict(
@@ -703,22 +688,14 @@
 
 class CreateThreatIntelSetRequestRequestTypeDef(
     _RequiredCreateThreatIntelSetRequestRequestTypeDef,
     _OptionalCreateThreatIntelSetRequestRequestTypeDef,
 ):
     pass
 
-CreateThreatIntelSetResponseTypeDef = TypedDict(
-    "CreateThreatIntelSetResponseTypeDef",
-    {
-        "ThreatIntelSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DNSLogsConfigurationResultTypeDef = TypedDict(
     "DNSLogsConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
@@ -817,14 +794,24 @@
     "DeleteThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
+
 SortCriteriaTypeDef = TypedDict(
     "SortCriteriaTypeDef",
     {
         "AttributeName": str,
         "OrderBy": OrderByType,
     },
     total=False,
@@ -855,23 +842,14 @@
     "DescribePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
 
-DestinationPropertiesOutputTypeDef = TypedDict(
-    "DestinationPropertiesOutputTypeDef",
-    {
-        "DestinationArn": str,
-        "KmsKeyArn": str,
-    },
-    total=False,
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
     },
@@ -1026,34 +1004,14 @@
     "GetIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "IpSetId": str,
     },
 )
 
-GetIPSetResponseTypeDef = TypedDict(
-    "GetIPSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": IpSetFormatType,
-        "Location": str,
-        "Status": IpSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "InvitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "GetMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 
@@ -1138,26 +1096,14 @@
     "GetThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
-GetThreatIntelSetResponseTypeDef = TypedDict(
-    "GetThreatIntelSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": ThreatIntelSetFormatType,
-        "Location": str,
-        "Status": ThreatIntelSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UsageCriteriaTypeDef = TypedDict(
     "UsageCriteriaTypeDef",
     {
         "AccountIds": Sequence[str],
         "DataSources": Sequence[DataSourceType],
         "Resources": Sequence[str],
         "Features": Sequence[UsageFeatureType],
@@ -1270,60 +1216,23 @@
         "ExecutablePath": str,
         "Euid": int,
         "ParentUuid": str,
     },
     total=False,
 )
 
-ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDetectorsRequestRequestTypeDef = TypedDict(
     "ListDetectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListDetectorsResponseTypeDef = TypedDict(
-    "ListDetectorsResponseTypeDef",
-    {
-        "DetectorIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFiltersRequestListFiltersPaginateTypeDef(
-    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
-    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
-):
-    pass
-
 _RequiredListFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredListFiltersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFiltersRequestRequestTypeDef = TypedDict(
@@ -1336,52 +1245,14 @@
 )
 
 class ListFiltersRequestRequestTypeDef(
     _RequiredListFiltersRequestRequestTypeDef, _OptionalListFiltersRequestRequestTypeDef
 ):
     pass
 
-ListFiltersResponseTypeDef = TypedDict(
-    "ListFiltersResponseTypeDef",
-    {
-        "FilterNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "FindingIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIPSetsRequestListIPSetsPaginateTypeDef(
-    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
-    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListIPSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListIPSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListIPSetsRequestRequestTypeDef = TypedDict(
@@ -1394,61 +1265,23 @@
 )
 
 class ListIPSetsRequestRequestTypeDef(
     _RequiredListIPSetsRequestRequestTypeDef, _OptionalListIPSetsRequestRequestTypeDef
 ):
     pass
 
-ListIPSetsResponseTypeDef = TypedDict(
-    "ListIPSetsResponseTypeDef",
-    {
-        "IpSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersRequestListMembersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMembersRequestListMembersPaginateTypeDef(
-    _RequiredListMembersRequestListMembersPaginateTypeDef,
-    _OptionalListMembersRequestListMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListMembersRequestRequestTypeDef = TypedDict(
@@ -1462,22 +1295,14 @@
 )
 
 class ListMembersRequestRequestTypeDef(
     _RequiredListMembersRequestRequestTypeDef, _OptionalListMembersRequestRequestTypeDef
 ):
     pass
 
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1507,42 +1332,14 @@
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
-_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
-    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListThreatIntelSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListThreatIntelSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListThreatIntelSetsRequestRequestTypeDef = TypedDict(
@@ -1556,23 +1353,14 @@
 
 class ListThreatIntelSetsRequestRequestTypeDef(
     _RequiredListThreatIntelSetsRequestRequestTypeDef,
     _OptionalListThreatIntelSetsRequestRequestTypeDef,
 ):
     pass
 
-ListThreatIntelSetsResponseTypeDef = TypedDict(
-    "ListThreatIntelSetsResponseTypeDef",
-    {
-        "ThreatIntelSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LocalIpDetailsTypeDef = TypedDict(
     "LocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
@@ -1728,24 +1516,14 @@
     "OwnerTypeDef",
     {
         "Id": str,
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
 RdsDbUserDetailsTypeDef = TypedDict(
     "RdsDbUserDetailsTypeDef",
     {
         "User": str,
         "Application": str,
         "Database": str,
         "Ssl": str,
@@ -1758,44 +1536,14 @@
     "ResourceDetailsTypeDef",
     {
         "InstanceArn": str,
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
-_RequiredScanConditionPairOutputTypeDef = TypedDict(
-    "_RequiredScanConditionPairOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalScanConditionPairOutputTypeDef = TypedDict(
-    "_OptionalScanConditionPairOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class ScanConditionPairOutputTypeDef(
-    _RequiredScanConditionPairOutputTypeDef, _OptionalScanConditionPairOutputTypeDef
-):
-    pass
-
 _RequiredScanConditionPairTypeDef = TypedDict(
     "_RequiredScanConditionPairTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalScanConditionPairTypeDef = TypedDict(
@@ -1869,22 +1617,14 @@
 StartMalwareScanRequestRequestTypeDef = TypedDict(
     "StartMalwareScanRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-StartMalwareScanResponseTypeDef = TypedDict(
-    "StartMalwareScanResponseTypeDef",
-    {
-        "ScanId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartMonitoringMembersRequestRequestTypeDef = TypedDict(
     "StartMonitoringMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountIds": Sequence[str],
     },
 )
@@ -1926,22 +1666,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFindingsFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingsFeedbackRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
         "Feedback": FeedbackType,
     },
@@ -2028,31 +1760,14 @@
         "CoveredNodes": int,
         "CompatibleNodes": int,
         "AddonDetails": AddonDetailsTypeDef,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAdministratorAccountResponseTypeDef = TypedDict(
-    "GetAdministratorAccountResponseTypeDef",
-    {
-        "Administrator": AdministratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
@@ -2094,91 +1809,241 @@
     {
         "CriterionKey": CoverageFilterCriterionKeyType,
         "FilterCondition": CoverageFilterConditionTypeDef,
     },
     total=False,
 )
 
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIPSetResponseTypeDef = TypedDict(
+    "CreateIPSetResponseTypeDef",
+    {
+        "IpSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePublishingDestinationResponseTypeDef = TypedDict(
+    "CreatePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThreatIntelSetResponseTypeDef = TypedDict(
+    "CreateThreatIntelSetResponseTypeDef",
+    {
+        "ThreatIntelSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAdministratorAccountResponseTypeDef = TypedDict(
+    "GetAdministratorAccountResponseTypeDef",
+    {
+        "Administrator": AdministratorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCoverageStatisticsResponseTypeDef = TypedDict(
     "GetCoverageStatisticsResponseTypeDef",
     {
         "CoverageStatistics": CoverageStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIPSetResponseTypeDef = TypedDict(
+    "GetIPSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": IpSetFormatType,
+        "Location": str,
+        "Status": IpSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetThreatIntelSetResponseTypeDef = TypedDict(
+    "GetThreatIntelSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": ThreatIntelSetFormatType,
+        "Location": str,
+        "Status": ThreatIntelSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDetectorsResponseTypeDef = TypedDict(
+    "ListDetectorsResponseTypeDef",
+    {
+        "DetectorIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFiltersResponseTypeDef = TypedDict(
+    "ListFiltersResponseTypeDef",
+    {
+        "FilterNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "FindingIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIPSetsResponseTypeDef = TypedDict(
+    "ListIPSetsResponseTypeDef",
+    {
+        "IpSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
+        "NextToken": str,
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
+ListThreatIntelSetsResponseTypeDef = TypedDict(
+    "ListThreatIntelSetsResponseTypeDef",
+    {
+        "ThreatIntelSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMalwareScanResponseTypeDef = TypedDict(
+    "StartMalwareScanResponseTypeDef",
+    {
+        "ScanId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateMembersResponseTypeDef = TypedDict(
     "DisassociateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMonitoringMembersResponseTypeDef = TypedDict(
     "StartMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopMonitoringMembersResponseTypeDef = TypedDict(
     "StopMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMemberDetectorsResponseTypeDef = TypedDict(
     "UpdateMemberDetectorsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2196,14 +2061,26 @@
 
 class CreatePublishingDestinationRequestRequestTypeDef(
     _RequiredCreatePublishingDestinationRequestRequestTypeDef,
     _OptionalCreatePublishingDestinationRequestRequestTypeDef,
 ):
     pass
 
+DescribePublishingDestinationResponseTypeDef = TypedDict(
+    "DescribePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "DestinationType": Literal["S3"],
+        "Status": PublishingStatusType,
+        "PublishingFailureStartTimestamp": int,
+        "DestinationProperties": DestinationPropertiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
         "DestinationId": str,
     },
 )
@@ -2233,14 +2110,119 @@
     "MalwareProtectionDataSourceFreeTrialTypeDef",
     {
         "ScanEc2InstanceWithFindings": DataSourceFreeTrialTypeDef,
     },
     total=False,
 )
 
+ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFiltersRequestListFiltersPaginateTypeDef(
+    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
+    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
+):
+    pass
+
+_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIPSetsRequestListIPSetsPaginateTypeDef(
+    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
+    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
+):
+    pass
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersRequestListMembersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMembersRequestListMembersPaginateTypeDef(
+    _RequiredListMembersRequestListMembersPaginateTypeDef,
+    _OptionalListMembersRequestListMembersPaginateTypeDef,
+):
+    pass
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
+    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
     },
 )
@@ -2253,32 +2235,20 @@
 )
 
 class GetFindingsRequestRequestTypeDef(
     _RequiredGetFindingsRequestRequestTypeDef, _OptionalGetFindingsRequestRequestTypeDef
 ):
     pass
 
-DescribePublishingDestinationResponseTypeDef = TypedDict(
-    "DescribePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "DestinationType": Literal["S3"],
-        "Status": PublishingStatusType,
-        "PublishingFailureStartTimestamp": int,
-        "DestinationProperties": DestinationPropertiesOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPublishingDestinationsResponseTypeDef = TypedDict(
     "ListPublishingDestinationsResponseTypeDef",
     {
         "Destinations": List[DestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectorFeatureConfigurationResultTypeDef = TypedDict(
     "DetectorFeatureConfigurationResultTypeDef",
     {
         "Name": DetectorFeatureResultType,
@@ -2359,41 +2329,41 @@
     total=False,
 )
 
 GetFindingsStatisticsResponseTypeDef = TypedDict(
     "GetFindingsStatisticsResponseTypeDef",
     {
         "FindingStatistics": FindingStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": MasterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2427,15 +2397,15 @@
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KubernetesConfigurationResultTypeDef = TypedDict(
     "KubernetesConfigurationResultTypeDef",
     {
         "AuditLogs": KubernetesAuditLogsConfigurationResultTypeDef,
@@ -2586,15 +2556,15 @@
     },
     total=False,
 )
 
 ScanConditionOutputTypeDef = TypedDict(
     "ScanConditionOutputTypeDef",
     {
-        "MapEquals": List[ScanConditionPairOutputTypeDef],
+        "MapEquals": List[ScanConditionPairTypeDef],
     },
 )
 
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
         "MapEquals": Sequence[ScanConditionPairTypeDef],
@@ -2693,15 +2663,15 @@
     {
         "Name": str,
         "Description": str,
         "Action": FilterActionType,
         "Rank": int,
         "FindingCriteria": FindingCriteriaOutputTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2754,15 +2724,15 @@
     },
 )
 _OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
     {
         "FindingCriteria": FindingCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListFindingsRequestListFindingsPaginateTypeDef(
     _RequiredListFindingsRequestListFindingsPaginateTypeDef,
     _OptionalListFindingsRequestListFindingsPaginateTypeDef,
@@ -3065,15 +3035,15 @@
 )
 
 DescribeMalwareScansResponseTypeDef = TypedDict(
     "DescribeMalwareScansResponseTypeDef",
     {
         "Scans": List[ScanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageStatisticsTypeDef = TypedDict(
     "UsageStatisticsTypeDef",
     {
         "SumByAccount": List[UsageAccountResultTypeDef],
@@ -3136,15 +3106,15 @@
     },
 )
 _OptionalListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
     "_OptionalListCoverageRequestListCoveragePaginateTypeDef",
     {
         "FilterCriteria": CoverageFilterCriteriaTypeDef,
         "SortCriteria": CoverageSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListCoverageRequestListCoveragePaginateTypeDef(
     _RequiredListCoverageRequestListCoveragePaginateTypeDef,
     _OptionalListCoverageRequestListCoveragePaginateTypeDef,
@@ -3221,15 +3191,15 @@
     },
 )
 _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef = TypedDict(
     "_OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef",
     {
         "FilterCriteria": FilterCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef(
     _RequiredDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
     _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
@@ -3400,15 +3370,15 @@
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
         "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3441,24 +3411,24 @@
 )
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "UsageStatistics": UsageStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "Resources": List[CoverageResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3BucketDetailTypeDef = TypedDict(
     "S3BucketDetailTypeDef",
     {
         "Arn": str,
@@ -3474,30 +3444,30 @@
 )
 
 GetRemainingFreeTrialDaysResponseTypeDef = TypedDict(
     "GetRemainingFreeTrialDaysResponseTypeDef",
     {
         "Accounts": List[AccountFreeTrialInfoTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDetectorResponseTypeDef = TypedDict(
     "GetDetectorResponseTypeDef",
     {
         "CreatedAt": str,
         "FindingPublishingFrequency": FindingPublishingFrequencyType,
         "ServiceRole": str,
         "Status": DetectorStatusType,
         "UpdatedAt": str,
         "DataSources": DataSourceConfigurationsResultTypeDef,
         "Tags": Dict[str, str],
         "Features": List[DetectorFeatureConfigurationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMemberDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredMemberDataSourceConfigurationTypeDef",
     {
         "AccountId": str,
@@ -3518,28 +3488,28 @@
     pass
 
 CreateDetectorResponseTypeDef = TypedDict(
     "CreateDetectorResponseTypeDef",
     {
         "DetectorId": str,
         "UnprocessedDataSources": UnprocessedDataSourcesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "AutoEnable": bool,
         "MemberAccountLimitReached": bool,
         "DataSources": OrganizationDataSourceConfigurationsResultTypeDef,
         "Features": List[OrganizationFeatureConfigurationResultTypeDef],
         "NextToken": str,
         "AutoEnableOrganizationMembers": AutoEnableMembersType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3610,15 +3580,15 @@
 )
 
 GetMemberDetectorsResponseTypeDef = TypedDict(
     "GetMemberDetectorsResponseTypeDef",
     {
         "MemberDataSourceConfigurations": List[MemberDataSourceConfigurationTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "Action": ActionTypeDef,
@@ -3669,10 +3639,10 @@
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "Findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/PKG-INFO` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-guardduty
-Version: 1.28.12
-Summary: Type annotations for boto3.GuardDuty 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-guardduty.svg?color=blue)](https://pypi.org/project/mypy-boto3-guardduty)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-guardduty)](https://pepy.tech/project/mypy-boto3-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.GuardDuty 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
+[boto3.GuardDuty 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [mypy-boto3-guardduty docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_guardduty/).
 
 See how it helps to find and fix potential bugs:
 
@@ -415,41 +415,38 @@
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
-    CreateFilterResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
-    DestinationPropertiesOutputTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateFromAdministratorAccountRequestRequestTypeDef,
     DisassociateFromMasterAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
@@ -461,58 +458,42 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
-    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
     LineageObjectTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
     MemberAdditionalConfigurationResultTypeDef,
     MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
@@ -524,64 +505,81 @@
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
-    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    ScanConditionPairOutputTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
     StartMalwareScanRequestRequestTypeDef,
-    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateIPSetResponseTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetThreatIntelSetResponseTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
+    StartMalwareScanResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
+    DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
-    DescribePublishingDestinationResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
     RdsDbInstanceDetailsTypeDef,
```

### Comparing `mypy-boto3-guardduty-1.28.12/mypy_boto3_guardduty.egg-info/SOURCES.txt` & `mypy-boto3-guardduty-1.28.15/mypy_boto3_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-guardduty-1.28.12/setup.py` & `mypy-boto3-guardduty-1.28.15/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-guardduty",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.GuardDuty 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.GuardDuty 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

