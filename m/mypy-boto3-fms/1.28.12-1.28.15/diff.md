# Comparing `tmp/mypy-boto3-fms-1.28.12.tar.gz` & `tmp/mypy-boto3-fms-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-fms-1.28.12.tar", last modified: Thu Jul 27 05:34:42 2023, max compression
+gzip compressed data, was "mypy-boto3-fms-1.28.15.tar", last modified: Fri Jul 28 20:42:49 2023, max compression
```

## Comparing `mypy-boto3-fms-1.28.12.tar` & `mypy-boto3-fms-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19881 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/mypy_boto3_fms/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30820 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30763 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-27 05:22:22.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-27 05:22:22.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9694 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65998 2023-07-27 05:22:23.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65919 2023-07-27 05:22:22.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:42.000000 mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:42.476507 mypy-boto3-fms-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:22:21.000000 mypy-boto3-fms-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.965126 mypy-boto3-fms-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-07-28 20:42:49.965126 mypy-boto3-fms-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19649 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.961126 mypy-boto3-fms-1.28.15/mypy_boto3_fms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30820 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30763 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-28 20:25:58.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13072 2023-07-28 20:25:58.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63794 2023-07-28 20:26:01.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63719 2023-07-28 20:26:00.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:49.961126 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21120 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:49.000000 mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:49.965126 mypy-boto3-fms-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:25:57.000000 mypy-boto3-fms-1.28.15/setup.py
```

### Comparing `mypy-boto3-fms-1.28.12/LICENSE` & `mypy-boto3-fms-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.12/PKG-INFO` & `mypy-boto3-fms-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.28.12
-Summary: Type annotations for boto3.FMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -381,162 +381,155 @@
     AdminAccountSummaryTypeDef,
     OrganizationalUnitScopeOutputTypeDef,
     PolicyTypeScopeOutputTypeDef,
     RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
-    AppOutputTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
-    GetAdminAccountResponseTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
-    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
-    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
-    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
-    ListAdminsManagingAccountResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
-    ListMemberAccountsResponseTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    TagTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
-    NetworkFirewallPolicyOutputTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
-    PaginatorConfigTypeDef,
-    ThirdPartyFirewallPolicyOutputTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
-    ResourceTagOutputTypeDef,
     ResourceTagTypeDef,
     ProtocolsListDataTypeDef,
-    TagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
-    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
-    ListAdminAccountsForOrganizationResponseTypeDef,
     AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
     AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetNotificationChannelResponseTypeDef,
+    GetProtectionStatusResponseTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
-    PolicyOptionOutputTypeDef,
     PolicyOptionTypeDef,
     PutProtocolsListRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
     PutAdminAccountRequestRequestTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListResponseTypeDef,
     ListAppsListsResponseTypeDef,
     PutAppsListRequestRequestTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
-    SecurityServicePolicyDataOutputTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
     PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
```

### Comparing `mypy-boto3-fms-1.28.12/README.md` & `mypy-boto3-fms-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -349,162 +349,155 @@
     AdminAccountSummaryTypeDef,
     OrganizationalUnitScopeOutputTypeDef,
     PolicyTypeScopeOutputTypeDef,
     RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
-    AppOutputTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
-    GetAdminAccountResponseTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
-    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
-    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
-    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
-    ListAdminsManagingAccountResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
-    ListMemberAccountsResponseTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    TagTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
-    NetworkFirewallPolicyOutputTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
-    PaginatorConfigTypeDef,
-    ThirdPartyFirewallPolicyOutputTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
-    ResourceTagOutputTypeDef,
     ResourceTagTypeDef,
     ProtocolsListDataTypeDef,
-    TagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
-    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
-    ListAdminAccountsForOrganizationResponseTypeDef,
     AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
     AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetNotificationChannelResponseTypeDef,
+    GetProtectionStatusResponseTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
-    PolicyOptionOutputTypeDef,
     PolicyOptionTypeDef,
     PutProtocolsListRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
     PutAdminAccountRequestRequestTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListResponseTypeDef,
     ListAppsListsResponseTypeDef,
     PutAppsListRequestRequestTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
-    SecurityServicePolicyDataOutputTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
     PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
```

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/__init__.py` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/__init__.pyi` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/__main__.py` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.FMS 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.FMS 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
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

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/client.py` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/client.pyi` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/literals.py` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/literals.pyi` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/paginator.py` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,105 +75,105 @@
 class ListAdminAccountsForOrganizationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAdminAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminaccountsfororganizationpaginator)
         """
 
 
 class ListAdminsManagingAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminsmanagingaccountpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAdminsManagingAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminsmanagingaccountpaginator)
         """
 
 
 class ListAppsListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listappslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listappslistspaginator)
         """
 
 
 class ListComplianceStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listcompliancestatuspaginator)
     """
 
     def paginate(
-        self, *, PolicyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PolicyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComplianceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listcompliancestatuspaginator)
         """
 
 
 class ListMemberAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMemberAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listmemberaccountspaginator)
         """
 
 
 class ListPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listpoliciespaginator)
         """
 
 
 class ListProtocolsListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listprotocolslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProtocolsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listprotocolslistspaginator)
         """
 
 
@@ -183,13 +183,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ThirdPartyFirewall: ThirdPartyFirewallType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/paginator.pyi` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -72,99 +72,99 @@
 class ListAdminAccountsForOrganizationPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAdminAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminaccountsfororganizationpaginator)
         """
 
 class ListAdminsManagingAccountPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminsmanagingaccountpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAdminsManagingAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listadminsmanagingaccountpaginator)
         """
 
 class ListAppsListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listappslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAppsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listappslistspaginator)
         """
 
 class ListComplianceStatusPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listcompliancestatuspaginator)
     """
 
     def paginate(
-        self, *, PolicyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PolicyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListComplianceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listcompliancestatuspaginator)
         """
 
 class ListMemberAccountsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMemberAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listmemberaccountspaginator)
         """
 
 class ListPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listpoliciespaginator)
         """
 
 class ListProtocolsListsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listprotocolslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProtocolsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listprotocolslistspaginator)
         """
 
 class ListThirdPartyFirewallFirewallPoliciesPaginator(Paginator):
@@ -173,13 +173,13 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ThirdPartyFirewall: ThirdPartyFirewallType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/type_defs.py` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -41,174 +41,166 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
     "OrganizationalUnitScopeOutputTypeDef",
     "PolicyTypeScopeOutputTypeDef",
     "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
-    "AppOutputTypeDef",
     "AppTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
-    "AssociateThirdPartyFirewallResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
     "BatchDisassociateResourceRequestRequestTypeDef",
     "ComplianceViolatorTypeDef",
     "DeleteAppsListRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "DeleteProtocolsListRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
-    "DisassociateThirdPartyFirewallResponseTypeDef",
     "DiscoveredResourceTypeDef",
     "DnsDuplicateRuleGroupViolationTypeDef",
     "DnsRuleGroupLimitExceededViolationTypeDef",
     "DnsRuleGroupPriorityConflictViolationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluationResultTypeDef",
     "ExpectedRouteTypeDef",
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
-    "GetAdminAccountResponseTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
-    "GetNotificationChannelResponseTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProtectionStatusRequestRequestTypeDef",
-    "GetProtectionStatusResponseTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
     "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
     "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
-    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
-    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
-    "ListAdminsManagingAccountResponseTypeDef",
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
     "ListAppsListsRequestRequestTypeDef",
-    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
-    "ListMemberAccountsResponseTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "PolicySummaryTypeDef",
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListProtocolsListsRequestRequestTypeDef",
     "ProtocolsListDataSummaryTypeDef",
     "ListResourceSetResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    "TagTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
-    "NetworkFirewallPolicyOutputTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
-    "PaginatorConfigTypeDef",
-    "ThirdPartyFirewallPolicyOutputTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
-    "ResourceTagOutputTypeDef",
     "ResourceTagTypeDef",
     "ProtocolsListDataTypeDef",
-    "TagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
     "ResourceSetTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
-    "ResponseMetadataTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
-    "ListAdminAccountsForOrganizationResponseTypeDef",
     "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
     "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
+    "AssociateThirdPartyFirewallResponseTypeDef",
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAdminAccountResponseTypeDef",
+    "GetNotificationChannelResponseTypeDef",
+    "GetProtectionStatusResponseTypeDef",
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    "ListAdminsManagingAccountResponseTypeDef",
+    "ListMemberAccountsResponseTypeDef",
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
+    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
-    "PolicyOptionOutputTypeDef",
     "PolicyOptionTypeDef",
     "PutProtocolsListRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "PutResourceSetRequestRequestTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
     "GetAppsListResponseTypeDef",
     "PutAppsListResponseTypeDef",
     "ListAppsListsResponseTypeDef",
     "PutAppsListRequestRequestTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
-    "SecurityServicePolicyDataOutputTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
     "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
@@ -312,23 +304,14 @@
     {
         "Regions": Sequence[str],
         "AllRegionsEnabled": bool,
     },
     total=False,
 )
 
-AppOutputTypeDef = TypedDict(
-    "AppOutputTypeDef",
-    {
-        "AppName": str,
-        "Protocol": str,
-        "Port": int,
-    },
-)
-
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
@@ -344,19 +327,22 @@
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "AssociateThirdPartyFirewallResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AwsEc2NetworkInterfaceViolationTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -427,21 +413,19 @@
     "_OptionalDeletePolicyRequestRequestTypeDef",
     {
         "DeleteAllPolicyResources": bool,
     },
     total=False,
 )
 
-
 class DeletePolicyRequestRequestTypeDef(
     _RequiredDeletePolicyRequestRequestTypeDef, _OptionalDeletePolicyRequestRequestTypeDef
 ):
     pass
 
-
 DeleteProtocolsListRequestRequestTypeDef = TypedDict(
     "DeleteProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 
@@ -455,22 +439,14 @@
 DisassociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "DisassociateThirdPartyFirewallResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiscoveredResourceTypeDef = TypedDict(
     "DiscoveredResourceTypeDef",
     {
         "URI": str,
         "AccountId": str,
         "Type": str,
         "Name": str,
@@ -505,21 +481,14 @@
         "ConflictingPriority": int,
         "ConflictingPolicyId": str,
         "UnavailablePriorities": List[int],
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
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "ComplianceStatus": PolicyComplianceStatusTypeType,
         "ViolatorCount": int,
         "EvaluationLimitExceeded": bool,
     },
@@ -567,23 +536,14 @@
         "VpcId": str,
         "SubnetAvailabilityZone": str,
         "SubnetAvailabilityZoneId": str,
     },
     total=False,
 )
 
-GetAdminAccountResponseTypeDef = TypedDict(
-    "GetAdminAccountResponseTypeDef",
-    {
-        "AdminAccount": str,
-        "RoleStatus": AccountRoleStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAdminScopeRequestRequestTypeDef = TypedDict(
     "GetAdminScopeRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
@@ -597,38 +557,27 @@
     "_OptionalGetAppsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
-
 class GetAppsListRequestRequestTypeDef(
     _RequiredGetAppsListRequestRequestTypeDef, _OptionalGetAppsListRequestRequestTypeDef
 ):
     pass
 
-
 GetComplianceDetailRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
 
-GetNotificationChannelResponseTypeDef = TypedDict(
-    "GetNotificationChannelResponseTypeDef",
-    {
-        "SnsTopicArn": str,
-        "SnsRoleName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
@@ -646,54 +595,39 @@
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetProtectionStatusRequestRequestTypeDef(
     _RequiredGetProtectionStatusRequestRequestTypeDef,
     _OptionalGetProtectionStatusRequestRequestTypeDef,
 ):
     pass
 
-
-GetProtectionStatusResponseTypeDef = TypedDict(
-    "GetProtectionStatusResponseTypeDef",
-    {
-        "AdminAccountId": str,
-        "ServiceType": SecurityServiceTypeType,
-        "Data": str,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_OptionalGetProtocolsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
-
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredProtocolsListDataOutputTypeDef = TypedDict(
     "_RequiredProtocolsListDataOutputTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
@@ -705,21 +639,19 @@
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
-
 class ProtocolsListDataOutputTypeDef(
     _RequiredProtocolsListDataOutputTypeDef, _OptionalProtocolsListDataOutputTypeDef
 ):
     pass
 
-
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -738,99 +670,64 @@
         "UpdateToken": str,
         "LastUpdateTime": datetime,
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
-
 class ResourceSetOutputTypeDef(
     _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
 ):
     pass
 
-
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetViolationDetailsRequestRequestTypeDef = TypedDict(
     "GetViolationDetailsRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
         "ResourceId": str,
         "ResourceType": str,
     },
 )
 
-ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
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
 
 ListAdminAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
-    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAdminsManagingAccountRequestRequestTypeDef = TypedDict(
     "ListAdminsManagingAccountRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListAdminsManagingAccountResponseTypeDef = TypedDict(
-    "ListAdminsManagingAccountResponseTypeDef",
-    {
-        "AdminAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListAppsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppsListsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListAppsListsRequestRequestTypeDef = TypedDict(
@@ -838,43 +735,19 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
-    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestRequestTypeDef = TypedDict(
@@ -882,22 +755,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListComplianceStatusRequestRequestTypeDef(
     _RequiredListComplianceStatusRequestRequestTypeDef,
     _OptionalListComplianceStatusRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "MemberAccountIds": Sequence[str],
         "ResourceType": str,
     },
 )
@@ -906,56 +777,29 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListMemberAccountsResponseTypeDef = TypedDict(
-    "ListMemberAccountsResponseTypeDef",
-    {
-        "MemberAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -972,23 +816,14 @@
         "RemediationEnabled": bool,
         "DeleteUnusedFMManagedResources": bool,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
-ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListProtocolsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListProtocolsListsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListProtocolsListsRequestRequestTypeDef = TypedDict(
@@ -996,22 +831,20 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProtocolsListsRequestRequestTypeDef(
     _RequiredListProtocolsListsRequestRequestTypeDef,
     _OptionalListProtocolsListsRequestRequestTypeDef,
 ):
     pass
 
-
 ProtocolsListDataSummaryTypeDef = TypedDict(
     "ProtocolsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "ProtocolsList": List[str],
@@ -1030,41 +863,37 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListResourceSetResourcesRequestRequestTypeDef(
     _RequiredListResourceSetResourcesRequestRequestTypeDef,
     _OptionalListResourceSetResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "URI": str,
     },
 )
 _OptionalResourceTypeDef = TypedDict(
     "_OptionalResourceTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
-
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1085,44 +914,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
-    },
-)
-_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
-    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
         "MaxResults": int,
     },
 )
@@ -1130,22 +937,20 @@
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
     },
     total=False,
@@ -1210,22 +1015,14 @@
         "RuleGroupName": str,
         "ResourceId": str,
         "Priority": int,
     },
     total=False,
 )
 
-NetworkFirewallPolicyOutputTypeDef = TypedDict(
-    "NetworkFirewallPolicyOutputTypeDef",
-    {
-        "FirewallDeploymentModel": FirewallDeploymentModelType,
-    },
-    total=False,
-)
-
 NetworkFirewallPolicyTypeDef = TypedDict(
     "NetworkFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
@@ -1234,80 +1031,39 @@
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
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
-ThirdPartyFirewallPolicyOutputTypeDef = TypedDict(
-    "ThirdPartyFirewallPolicyOutputTypeDef",
-    {
-        "FirewallDeploymentModel": FirewallDeploymentModelType,
-    },
-    total=False,
-)
-
 ThirdPartyFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
 
-_RequiredResourceTagOutputTypeDef = TypedDict(
-    "_RequiredResourceTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalResourceTagOutputTypeDef = TypedDict(
-    "_OptionalResourceTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class ResourceTagOutputTypeDef(
-    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
-):
-    pass
-
-
 _RequiredResourceTagTypeDef = TypedDict(
     "_RequiredResourceTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalResourceTagTypeDef = TypedDict(
     "_OptionalResourceTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
-
 _RequiredProtocolsListDataTypeDef = TypedDict(
     "_RequiredProtocolsListDataTypeDef",
     {
         "ListName": str,
         "ProtocolsList": Sequence[str],
     },
 )
@@ -1319,29 +1075,19 @@
         "CreateTime": Union[datetime, str],
         "LastUpdateTime": Union[datetime, str],
         "PreviousProtocolsList": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class ProtocolsListDataTypeDef(
     _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
 ):
     pass
 
-
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
@@ -1361,19 +1107,17 @@
         "UpdateToken": str,
         "LastUpdateTime": Union[datetime, str],
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
-
 class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
     pass
 
-
 ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef = TypedDict(
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     {
         "ViolationTarget": str,
         "VPC": str,
         "AvailabilityZone": str,
         "CurrentRouteTable": str,
@@ -1400,25 +1144,14 @@
         "VPC": str,
         "AvailabilityZone": str,
         "TargetViolationReason": str,
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
 SecurityGroupRuleDescriptionTypeDef = TypedDict(
     "SecurityGroupRuleDescriptionTypeDef",
     {
         "IPV4Range": str,
         "IPV6Range": str,
         "PrefixListId": str,
         "Protocol": str,
@@ -1448,21 +1181,19 @@
         "Description": str,
         "SubnetId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2AssociateRouteTableActionTypeDef(
     _RequiredEC2AssociateRouteTableActionTypeDef, _OptionalEC2AssociateRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CopyRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CopyRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1470,21 +1201,19 @@
     "_OptionalEC2CopyRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2CopyRouteTableActionTypeDef(
     _RequiredEC2CopyRouteTableActionTypeDef, _OptionalEC2CopyRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CreateRouteActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteActionTypeDef = TypedDict(
@@ -1496,42 +1225,38 @@
         "DestinationIpv6CidrBlock": str,
         "VpcEndpointId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2CreateRouteActionTypeDef(
     _RequiredEC2CreateRouteActionTypeDef, _OptionalEC2CreateRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CreateRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteTableActionTypeDef = TypedDict(
     "_OptionalEC2CreateRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2CreateRouteTableActionTypeDef(
     _RequiredEC2CreateRouteTableActionTypeDef, _OptionalEC2CreateRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2DeleteRouteActionTypeDef = TypedDict(
     "_RequiredEC2DeleteRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2DeleteRouteActionTypeDef = TypedDict(
@@ -1541,21 +1266,19 @@
         "DestinationCidrBlock": str,
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
     },
     total=False,
 )
 
-
 class EC2DeleteRouteActionTypeDef(
     _RequiredEC2DeleteRouteActionTypeDef, _OptionalEC2DeleteRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2ReplaceRouteActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2ReplaceRouteActionTypeDef = TypedDict(
@@ -1566,21 +1289,19 @@
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2ReplaceRouteActionTypeDef(
     _RequiredEC2ReplaceRouteActionTypeDef, _OptionalEC2ReplaceRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2ReplaceRouteTableAssociationActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1588,31 +1309,20 @@
     "_OptionalEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
-
-ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
-    "ListAdminAccountsForOrganizationResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AdminScopeOutputTypeDef = TypedDict(
     "AdminScopeOutputTypeDef",
     {
         "AccountScope": AccountScopeOutputTypeDef,
         "OrganizationalUnitScope": OrganizationalUnitScopeOutputTypeDef,
         "RegionScope": RegionScopeOutputTypeDef,
         "PolicyTypeScope": PolicyTypeScopeOutputTypeDef,
@@ -1631,43 +1341,41 @@
     total=False,
 )
 
 _RequiredAppsListDataOutputTypeDef = TypedDict(
     "_RequiredAppsListDataOutputTypeDef",
     {
         "ListName": str,
-        "AppsList": List[AppOutputTypeDef],
+        "AppsList": List[AppTypeDef],
     },
 )
 _OptionalAppsListDataOutputTypeDef = TypedDict(
     "_OptionalAppsListDataOutputTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
-        "PreviousAppsList": Dict[str, List[AppOutputTypeDef]],
+        "PreviousAppsList": Dict[str, List[AppTypeDef]],
     },
     total=False,
 )
 
-
 class AppsListDataOutputTypeDef(
     _RequiredAppsListDataOutputTypeDef, _OptionalAppsListDataOutputTypeDef
 ):
     pass
 
-
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
-        "AppsList": List[AppOutputTypeDef],
+        "AppsList": List[AppTypeDef],
     },
     total=False,
 )
 
 _RequiredAppsListDataTypeDef = TypedDict(
     "_RequiredAppsListDataTypeDef",
     {
@@ -1683,18 +1391,104 @@
         "CreateTime": Union[datetime, str],
         "LastUpdateTime": Union[datetime, str],
         "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
     },
     total=False,
 )
 
-
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
+AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "AssociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
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
+GetAdminAccountResponseTypeDef = TypedDict(
+    "GetAdminAccountResponseTypeDef",
+    {
+        "AdminAccount": str,
+        "RoleStatus": AccountRoleStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNotificationChannelResponseTypeDef = TypedDict(
+    "GetNotificationChannelResponseTypeDef",
+    {
+        "SnsTopicArn": str,
+        "SnsRoleName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProtectionStatusResponseTypeDef = TypedDict(
+    "GetProtectionStatusResponseTypeDef",
+    {
+        "AdminAccountId": str,
+        "ServiceType": SecurityServiceTypeType,
+        "Data": str,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminsManagingAccountResponseTypeDef = TypedDict(
+    "ListAdminsManagingAccountResponseTypeDef",
+    {
+        "AdminAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListMemberAccountsResponseTypeDef = TypedDict(
+    "ListMemberAccountsResponseTypeDef",
+    {
+        "MemberAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": str,
         "AwsEc2NetworkInterfaceViolations": List[AwsEc2NetworkInterfaceViolationTypeDef],
     },
@@ -1702,24 +1496,24 @@
 )
 
 BatchAssociateResourceResponseTypeDef = TypedDict(
     "BatchAssociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateResourceResponseTypeDef = TypedDict(
     "BatchDisassociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyComplianceDetailTypeDef = TypedDict(
     "PolicyComplianceDetailTypeDef",
     {
         "PolicyOwner": str,
@@ -1734,15 +1528,15 @@
 )
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "Items": List[DiscoveredResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyComplianceStatusTypeDef = TypedDict(
     "PolicyComplianceStatusTypeDef",
     {
         "PolicyOwner": str,
@@ -1767,95 +1561,193 @@
 )
 
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
         "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
         "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
         "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
+    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+):
+    pass
+
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
+    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+):
+    pass
+
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "PolicyList": List[PolicySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtocolsListsResponseTypeDef = TypedDict(
     "ListProtocolsListsResponseTypeDef",
     {
         "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceSetResourcesResponseTypeDef = TypedDict(
     "ListResourceSetResourcesResponseTypeDef",
     {
         "Items": List[ResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "ResourceSets": List[ResourceSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
     },
 )
 
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFirewallBlackHoleRouteDetectedViolationTypeDef = TypedDict(
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -1960,23 +1852,14 @@
         "ResourceId": str,
         "Priority": int,
         "Override": NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     },
     total=False,
 )
 
-PolicyOptionOutputTypeDef = TypedDict(
-    "PolicyOptionOutputTypeDef",
-    {
-        "NetworkFirewallPolicy": NetworkFirewallPolicyOutputTypeDef,
-        "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 PolicyOptionTypeDef = TypedDict(
     "PolicyOptionTypeDef",
     {
         "NetworkFirewallPolicy": NetworkFirewallPolicyTypeDef,
         "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyTypeDef,
     },
     total=False,
@@ -1992,50 +1875,38 @@
     "_OptionalPutProtocolsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutProtocolsListRequestRequestTypeDef(
     _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
 ):
     pass
 
-
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
-    },
-)
-
 _RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceSetRequestRequestTypeDef",
     {
         "ResourceSet": ResourceSetTypeDef,
     },
 )
 _OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
     "_OptionalPutResourceSetRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutResourceSetRequestRequestTypeDef(
     _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
 ):
     pass
 
-
 SecurityGroupRemediationActionTypeDef = TypedDict(
     "SecurityGroupRemediationActionTypeDef",
     {
         "RemediationActionType": RemediationActionTypeType,
         "Description": str,
         "RemediationResult": SecurityGroupRuleDescriptionTypeDef,
         "IsDefaultAction": bool,
@@ -2062,15 +1933,15 @@
 )
 
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
         "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
@@ -2080,45 +1951,43 @@
     "_OptionalPutAdminAccountRequestRequestTypeDef",
     {
         "AdminScope": AdminScopeTypeDef,
     },
     total=False,
 )
 
-
 class PutAdminAccountRequestRequestTypeDef(
     _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
 ):
     pass
 
-
 GetAppsListResponseTypeDef = TypedDict(
     "GetAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAppsListResponseTypeDef = TypedDict(
     "PutAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppsListsResponseTypeDef = TypedDict(
     "ListAppsListsResponseTypeDef",
     {
         "AppsLists": List[AppsListDataSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
@@ -2128,35 +1997,33 @@
     "_OptionalPutAppsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
-
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComplianceStatusResponseTypeDef = TypedDict(
     "ListComplianceStatusResponseTypeDef",
     {
         "PolicyComplianceStatusList": List[PolicyComplianceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFirewallPolicyDescriptionTypeDef = TypedDict(
     "NetworkFirewallPolicyDescriptionTypeDef",
     {
         "StatelessRuleGroups": List[StatelessRuleGroupTypeDef],
@@ -2166,36 +2033,14 @@
         "StatefulRuleGroups": List[StatefulRuleGroupTypeDef],
         "StatefulDefaultActions": List[str],
         "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredSecurityServicePolicyDataOutputTypeDef = TypedDict(
-    "_RequiredSecurityServicePolicyDataOutputTypeDef",
-    {
-        "Type": SecurityServiceTypeType,
-    },
-)
-_OptionalSecurityServicePolicyDataOutputTypeDef = TypedDict(
-    "_OptionalSecurityServicePolicyDataOutputTypeDef",
-    {
-        "ManagedServiceData": str,
-        "PolicyOption": PolicyOptionOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class SecurityServicePolicyDataOutputTypeDef(
-    _RequiredSecurityServicePolicyDataOutputTypeDef, _OptionalSecurityServicePolicyDataOutputTypeDef
-):
-    pass
-
-
 _RequiredSecurityServicePolicyDataTypeDef = TypedDict(
     "_RequiredSecurityServicePolicyDataTypeDef",
     {
         "Type": SecurityServiceTypeType,
     },
 )
 _OptionalSecurityServicePolicyDataTypeDef = TypedDict(
@@ -2203,21 +2048,19 @@
     {
         "ManagedServiceData": str,
         "PolicyOption": PolicyOptionTypeDef,
     },
     total=False,
 )
 
-
 class SecurityServicePolicyDataTypeDef(
     _RequiredSecurityServicePolicyDataTypeDef, _OptionalSecurityServicePolicyDataTypeDef
 ):
     pass
 
-
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": str,
         "ViolationTargetDescription": str,
         "PartialMatches": List[PartialMatchTypeDef],
         "PossibleSecurityGroupRemediationActions": List[SecurityGroupRemediationActionTypeDef],
@@ -2244,42 +2087,40 @@
     total=False,
 )
 
 _RequiredPolicyOutputTypeDef = TypedDict(
     "_RequiredPolicyOutputTypeDef",
     {
         "PolicyName": str,
-        "SecurityServicePolicyData": SecurityServicePolicyDataOutputTypeDef,
+        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
     },
 )
 _OptionalPolicyOutputTypeDef = TypedDict(
     "_OptionalPolicyOutputTypeDef",
     {
         "PolicyId": str,
         "PolicyUpdateToken": str,
         "ResourceTypeList": List[str],
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "ResourceTags": List[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
-
 class PolicyOutputTypeDef(_RequiredPolicyOutputTypeDef, _OptionalPolicyOutputTypeDef):
     pass
 
-
 _RequiredPolicyTypeDef = TypedDict(
     "_RequiredPolicyTypeDef",
     {
         "PolicyName": str,
         "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
@@ -2299,19 +2140,17 @@
         "ResourceSetIds": Sequence[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
-
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
-
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
     },
 )
 _OptionalPossibleRemediationActionTypeDef = TypedDict(
@@ -2319,36 +2158,34 @@
     {
         "Description": str,
         "IsDefaultAction": bool,
     },
     total=False,
 )
 
-
 class PossibleRemediationActionTypeDef(
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
-
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
@@ -2358,21 +2195,19 @@
     "_OptionalPutPolicyRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
-
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
         "Actions": List[PossibleRemediationActionTypeDef],
     },
     total=False,
@@ -2437,25 +2272,23 @@
         "ResourceType": str,
         "ResourceViolations": List[ResourceViolationTypeDef],
     },
 )
 _OptionalViolationDetailTypeDef = TypedDict(
     "_OptionalViolationDetailTypeDef",
     {
-        "ResourceTags": List[TagOutputTypeDef],
+        "ResourceTags": List[TagTypeDef],
         "ResourceDescription": str,
     },
     total=False,
 )
 
-
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
-
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms/type_defs.pyi` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,173 +41,167 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
     "OrganizationalUnitScopeOutputTypeDef",
     "PolicyTypeScopeOutputTypeDef",
     "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
-    "AppOutputTypeDef",
     "AppTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
-    "AssociateThirdPartyFirewallResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
     "BatchDisassociateResourceRequestRequestTypeDef",
     "ComplianceViolatorTypeDef",
     "DeleteAppsListRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "DeleteProtocolsListRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
-    "DisassociateThirdPartyFirewallResponseTypeDef",
     "DiscoveredResourceTypeDef",
     "DnsDuplicateRuleGroupViolationTypeDef",
     "DnsRuleGroupLimitExceededViolationTypeDef",
     "DnsRuleGroupPriorityConflictViolationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluationResultTypeDef",
     "ExpectedRouteTypeDef",
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
-    "GetAdminAccountResponseTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
-    "GetNotificationChannelResponseTypeDef",
     "GetPolicyRequestRequestTypeDef",
     "GetProtectionStatusRequestRequestTypeDef",
-    "GetProtectionStatusResponseTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
     "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
     "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
-    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
-    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
-    "ListAdminsManagingAccountResponseTypeDef",
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
     "ListAppsListsRequestRequestTypeDef",
-    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
-    "ListMemberAccountsResponseTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "PolicySummaryTypeDef",
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListProtocolsListsRequestRequestTypeDef",
     "ProtocolsListDataSummaryTypeDef",
     "ListResourceSetResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    "TagTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
-    "NetworkFirewallPolicyOutputTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
-    "PaginatorConfigTypeDef",
-    "ThirdPartyFirewallPolicyOutputTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
-    "ResourceTagOutputTypeDef",
     "ResourceTagTypeDef",
     "ProtocolsListDataTypeDef",
-    "TagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
     "ResourceSetTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
-    "ResponseMetadataTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
-    "ListAdminAccountsForOrganizationResponseTypeDef",
     "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
     "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
+    "AssociateThirdPartyFirewallResponseTypeDef",
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAdminAccountResponseTypeDef",
+    "GetNotificationChannelResponseTypeDef",
+    "GetProtectionStatusResponseTypeDef",
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    "ListAdminsManagingAccountResponseTypeDef",
+    "ListMemberAccountsResponseTypeDef",
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
+    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
-    "PolicyOptionOutputTypeDef",
     "PolicyOptionTypeDef",
     "PutProtocolsListRequestRequestTypeDef",
-    "TagResourceRequestRequestTypeDef",
     "PutResourceSetRequestRequestTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
     "GetAppsListResponseTypeDef",
     "PutAppsListResponseTypeDef",
     "ListAppsListsResponseTypeDef",
     "PutAppsListRequestRequestTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
-    "SecurityServicePolicyDataOutputTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
     "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
@@ -311,23 +305,14 @@
     {
         "Regions": Sequence[str],
         "AllRegionsEnabled": bool,
     },
     total=False,
 )
 
-AppOutputTypeDef = TypedDict(
-    "AppOutputTypeDef",
-    {
-        "AppName": str,
-        "Protocol": str,
-        "Port": int,
-    },
-)
-
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
@@ -343,19 +328,22 @@
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "AssociateThirdPartyFirewallResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AwsEc2NetworkInterfaceViolationTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -426,19 +414,21 @@
     "_OptionalDeletePolicyRequestRequestTypeDef",
     {
         "DeleteAllPolicyResources": bool,
     },
     total=False,
 )
 
+
 class DeletePolicyRequestRequestTypeDef(
     _RequiredDeletePolicyRequestRequestTypeDef, _OptionalDeletePolicyRequestRequestTypeDef
 ):
     pass
 
+
 DeleteProtocolsListRequestRequestTypeDef = TypedDict(
     "DeleteProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 
@@ -452,22 +442,14 @@
 DisassociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "DisassociateThirdPartyFirewallResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiscoveredResourceTypeDef = TypedDict(
     "DiscoveredResourceTypeDef",
     {
         "URI": str,
         "AccountId": str,
         "Type": str,
         "Name": str,
@@ -502,21 +484,14 @@
         "ConflictingPriority": int,
         "ConflictingPolicyId": str,
         "UnavailablePriorities": List[int],
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
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "ComplianceStatus": PolicyComplianceStatusTypeType,
         "ViolatorCount": int,
         "EvaluationLimitExceeded": bool,
     },
@@ -564,23 +539,14 @@
         "VpcId": str,
         "SubnetAvailabilityZone": str,
         "SubnetAvailabilityZoneId": str,
     },
     total=False,
 )
 
-GetAdminAccountResponseTypeDef = TypedDict(
-    "GetAdminAccountResponseTypeDef",
-    {
-        "AdminAccount": str,
-        "RoleStatus": AccountRoleStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAdminScopeRequestRequestTypeDef = TypedDict(
     "GetAdminScopeRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
@@ -594,36 +560,29 @@
     "_OptionalGetAppsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
+
 class GetAppsListRequestRequestTypeDef(
     _RequiredGetAppsListRequestRequestTypeDef, _OptionalGetAppsListRequestRequestTypeDef
 ):
     pass
 
+
 GetComplianceDetailRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
 
-GetNotificationChannelResponseTypeDef = TypedDict(
-    "GetNotificationChannelResponseTypeDef",
-    {
-        "SnsTopicArn": str,
-        "SnsRoleName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
@@ -641,30 +600,21 @@
         "EndTime": Union[datetime, str],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetProtectionStatusRequestRequestTypeDef(
     _RequiredGetProtectionStatusRequestRequestTypeDef,
     _OptionalGetProtectionStatusRequestRequestTypeDef,
 ):
     pass
 
-GetProtectionStatusResponseTypeDef = TypedDict(
-    "GetProtectionStatusResponseTypeDef",
-    {
-        "AdminAccountId": str,
-        "ServiceType": SecurityServiceTypeType,
-        "Data": str,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
@@ -672,19 +622,21 @@
     "_OptionalGetProtocolsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
+
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredProtocolsListDataOutputTypeDef = TypedDict(
     "_RequiredProtocolsListDataOutputTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
@@ -696,19 +648,21 @@
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
+
 class ProtocolsListDataOutputTypeDef(
     _RequiredProtocolsListDataOutputTypeDef, _OptionalProtocolsListDataOutputTypeDef
 ):
     pass
 
+
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -727,97 +681,66 @@
         "UpdateToken": str,
         "LastUpdateTime": datetime,
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
+
 class ResourceSetOutputTypeDef(
     _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
 ):
     pass
 
+
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetViolationDetailsRequestRequestTypeDef = TypedDict(
     "GetViolationDetailsRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
         "ResourceId": str,
         "ResourceType": str,
     },
 )
 
-ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
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
 
 ListAdminAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
-    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAdminsManagingAccountRequestRequestTypeDef = TypedDict(
     "ListAdminsManagingAccountRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListAdminsManagingAccountResponseTypeDef = TypedDict(
-    "ListAdminsManagingAccountResponseTypeDef",
-    {
-        "AdminAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListAppsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppsListsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListAppsListsRequestRequestTypeDef = TypedDict(
@@ -825,38 +748,20 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
-    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-):
-    pass
 
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
@@ -865,20 +770,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListComplianceStatusRequestRequestTypeDef(
     _RequiredListComplianceStatusRequestRequestTypeDef,
     _OptionalListComplianceStatusRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "MemberAccountIds": Sequence[str],
         "ResourceType": str,
     },
 )
@@ -887,54 +794,31 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListMemberAccountsResponseTypeDef = TypedDict(
-    "ListMemberAccountsResponseTypeDef",
-    {
-        "MemberAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -951,23 +835,14 @@
         "RemediationEnabled": bool,
         "DeleteUnusedFMManagedResources": bool,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
-ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListProtocolsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListProtocolsListsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListProtocolsListsRequestRequestTypeDef = TypedDict(
@@ -975,20 +850,22 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProtocolsListsRequestRequestTypeDef(
     _RequiredListProtocolsListsRequestRequestTypeDef,
     _OptionalListProtocolsListsRequestRequestTypeDef,
 ):
     pass
 
+
 ProtocolsListDataSummaryTypeDef = TypedDict(
     "ProtocolsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "ProtocolsList": List[str],
@@ -1007,37 +884,41 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListResourceSetResourcesRequestRequestTypeDef(
     _RequiredListResourceSetResourcesRequestRequestTypeDef,
     _OptionalListResourceSetResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "URI": str,
     },
 )
 _OptionalResourceTypeDef = TypedDict(
     "_OptionalResourceTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
+
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1058,42 +939,22 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
-    },
-)
-_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
-    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
         "MaxResults": int,
     },
 )
@@ -1101,20 +962,22 @@
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
     },
     total=False,
@@ -1179,22 +1042,14 @@
         "RuleGroupName": str,
         "ResourceId": str,
         "Priority": int,
     },
     total=False,
 )
 
-NetworkFirewallPolicyOutputTypeDef = TypedDict(
-    "NetworkFirewallPolicyOutputTypeDef",
-    {
-        "FirewallDeploymentModel": FirewallDeploymentModelType,
-    },
-    total=False,
-)
-
 NetworkFirewallPolicyTypeDef = TypedDict(
     "NetworkFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
@@ -1203,76 +1058,41 @@
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
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
-ThirdPartyFirewallPolicyOutputTypeDef = TypedDict(
-    "ThirdPartyFirewallPolicyOutputTypeDef",
-    {
-        "FirewallDeploymentModel": FirewallDeploymentModelType,
-    },
-    total=False,
-)
-
 ThirdPartyFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
 
-_RequiredResourceTagOutputTypeDef = TypedDict(
-    "_RequiredResourceTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalResourceTagOutputTypeDef = TypedDict(
-    "_OptionalResourceTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class ResourceTagOutputTypeDef(
-    _RequiredResourceTagOutputTypeDef, _OptionalResourceTagOutputTypeDef
-):
-    pass
-
 _RequiredResourceTagTypeDef = TypedDict(
     "_RequiredResourceTagTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalResourceTagTypeDef = TypedDict(
     "_OptionalResourceTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
+
 _RequiredProtocolsListDataTypeDef = TypedDict(
     "_RequiredProtocolsListDataTypeDef",
     {
         "ListName": str,
         "ProtocolsList": Sequence[str],
     },
 )
@@ -1284,26 +1104,20 @@
         "CreateTime": Union[datetime, str],
         "LastUpdateTime": Union[datetime, str],
         "PreviousProtocolsList": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class ProtocolsListDataTypeDef(
     _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
 ):
     pass
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
 
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
@@ -1324,17 +1138,19 @@
         "UpdateToken": str,
         "LastUpdateTime": Union[datetime, str],
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
+
 class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
     pass
 
+
 ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef = TypedDict(
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     {
         "ViolationTarget": str,
         "VPC": str,
         "AvailabilityZone": str,
         "CurrentRouteTable": str,
@@ -1361,25 +1177,14 @@
         "VPC": str,
         "AvailabilityZone": str,
         "TargetViolationReason": str,
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
 SecurityGroupRuleDescriptionTypeDef = TypedDict(
     "SecurityGroupRuleDescriptionTypeDef",
     {
         "IPV4Range": str,
         "IPV6Range": str,
         "PrefixListId": str,
         "Protocol": str,
@@ -1409,19 +1214,21 @@
         "Description": str,
         "SubnetId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2AssociateRouteTableActionTypeDef(
     _RequiredEC2AssociateRouteTableActionTypeDef, _OptionalEC2AssociateRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CopyRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CopyRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1429,19 +1236,21 @@
     "_OptionalEC2CopyRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2CopyRouteTableActionTypeDef(
     _RequiredEC2CopyRouteTableActionTypeDef, _OptionalEC2CopyRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CreateRouteActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteActionTypeDef = TypedDict(
@@ -1453,38 +1262,42 @@
         "DestinationIpv6CidrBlock": str,
         "VpcEndpointId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2CreateRouteActionTypeDef(
     _RequiredEC2CreateRouteActionTypeDef, _OptionalEC2CreateRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CreateRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteTableActionTypeDef = TypedDict(
     "_OptionalEC2CreateRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2CreateRouteTableActionTypeDef(
     _RequiredEC2CreateRouteTableActionTypeDef, _OptionalEC2CreateRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2DeleteRouteActionTypeDef = TypedDict(
     "_RequiredEC2DeleteRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2DeleteRouteActionTypeDef = TypedDict(
@@ -1494,19 +1307,21 @@
         "DestinationCidrBlock": str,
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
     },
     total=False,
 )
 
+
 class EC2DeleteRouteActionTypeDef(
     _RequiredEC2DeleteRouteActionTypeDef, _OptionalEC2DeleteRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2ReplaceRouteActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2ReplaceRouteActionTypeDef = TypedDict(
@@ -1517,19 +1332,21 @@
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2ReplaceRouteActionTypeDef(
     _RequiredEC2ReplaceRouteActionTypeDef, _OptionalEC2ReplaceRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2ReplaceRouteTableAssociationActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1537,28 +1354,21 @@
     "_OptionalEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
-ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
-    "ListAdminAccountsForOrganizationResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 AdminScopeOutputTypeDef = TypedDict(
     "AdminScopeOutputTypeDef",
     {
         "AccountScope": AccountScopeOutputTypeDef,
         "OrganizationalUnitScope": OrganizationalUnitScopeOutputTypeDef,
         "RegionScope": RegionScopeOutputTypeDef,
@@ -1578,41 +1388,43 @@
     total=False,
 )
 
 _RequiredAppsListDataOutputTypeDef = TypedDict(
     "_RequiredAppsListDataOutputTypeDef",
     {
         "ListName": str,
-        "AppsList": List[AppOutputTypeDef],
+        "AppsList": List[AppTypeDef],
     },
 )
 _OptionalAppsListDataOutputTypeDef = TypedDict(
     "_OptionalAppsListDataOutputTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
-        "PreviousAppsList": Dict[str, List[AppOutputTypeDef]],
+        "PreviousAppsList": Dict[str, List[AppTypeDef]],
     },
     total=False,
 )
 
+
 class AppsListDataOutputTypeDef(
     _RequiredAppsListDataOutputTypeDef, _OptionalAppsListDataOutputTypeDef
 ):
     pass
 
+
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
-        "AppsList": List[AppOutputTypeDef],
+        "AppsList": List[AppTypeDef],
     },
     total=False,
 )
 
 _RequiredAppsListDataTypeDef = TypedDict(
     "_RequiredAppsListDataTypeDef",
     {
@@ -1628,41 +1440,131 @@
         "CreateTime": Union[datetime, str],
         "LastUpdateTime": Union[datetime, str],
         "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
     },
     total=False,
 )
 
+
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
+
+AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "AssociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
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
+GetAdminAccountResponseTypeDef = TypedDict(
+    "GetAdminAccountResponseTypeDef",
+    {
+        "AdminAccount": str,
+        "RoleStatus": AccountRoleStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNotificationChannelResponseTypeDef = TypedDict(
+    "GetNotificationChannelResponseTypeDef",
+    {
+        "SnsTopicArn": str,
+        "SnsRoleName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProtectionStatusResponseTypeDef = TypedDict(
+    "GetProtectionStatusResponseTypeDef",
+    {
+        "AdminAccountId": str,
+        "ServiceType": SecurityServiceTypeType,
+        "Data": str,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminsManagingAccountResponseTypeDef = TypedDict(
+    "ListAdminsManagingAccountResponseTypeDef",
+    {
+        "AdminAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListMemberAccountsResponseTypeDef = TypedDict(
+    "ListMemberAccountsResponseTypeDef",
+    {
+        "MemberAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": str,
         "AwsEc2NetworkInterfaceViolations": List[AwsEc2NetworkInterfaceViolationTypeDef],
     },
     total=False,
 )
 
 BatchAssociateResourceResponseTypeDef = TypedDict(
     "BatchAssociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateResourceResponseTypeDef = TypedDict(
     "BatchDisassociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyComplianceDetailTypeDef = TypedDict(
     "PolicyComplianceDetailTypeDef",
     {
         "PolicyOwner": str,
@@ -1677,15 +1579,15 @@
 )
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "Items": List[DiscoveredResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyComplianceStatusTypeDef = TypedDict(
     "PolicyComplianceStatusTypeDef",
     {
         "PolicyOwner": str,
@@ -1710,95 +1612,197 @@
 )
 
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
         "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
         "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
         "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
         "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
+    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+):
+    pass
+
+
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
+    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+):
+    pass
+
+
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "PolicyList": List[PolicySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProtocolsListsResponseTypeDef = TypedDict(
     "ListProtocolsListsResponseTypeDef",
     {
         "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceSetResourcesResponseTypeDef = TypedDict(
     "ListResourceSetResourcesResponseTypeDef",
     {
         "Items": List[ResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceSetsResponseTypeDef = TypedDict(
     "ListResourceSetsResponseTypeDef",
     {
         "ResourceSets": List[ResourceSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
-        "TagList": List[TagOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
     },
 )
 
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFirewallBlackHoleRouteDetectedViolationTypeDef = TypedDict(
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -1903,23 +1907,14 @@
         "ResourceId": str,
         "Priority": int,
         "Override": NetworkFirewallStatefulRuleGroupOverrideTypeDef,
     },
     total=False,
 )
 
-PolicyOptionOutputTypeDef = TypedDict(
-    "PolicyOptionOutputTypeDef",
-    {
-        "NetworkFirewallPolicy": NetworkFirewallPolicyOutputTypeDef,
-        "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyOutputTypeDef,
-    },
-    total=False,
-)
-
 PolicyOptionTypeDef = TypedDict(
     "PolicyOptionTypeDef",
     {
         "NetworkFirewallPolicy": NetworkFirewallPolicyTypeDef,
         "ThirdPartyFirewallPolicy": ThirdPartyFirewallPolicyTypeDef,
     },
     total=False,
@@ -1935,26 +1930,20 @@
     "_OptionalPutProtocolsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutProtocolsListRequestRequestTypeDef(
     _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
 ):
     pass
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
-    {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
-    },
-)
 
 _RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceSetRequestRequestTypeDef",
     {
         "ResourceSet": ResourceSetTypeDef,
     },
 )
@@ -1962,19 +1951,21 @@
     "_OptionalPutResourceSetRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutResourceSetRequestRequestTypeDef(
     _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
 ):
     pass
 
+
 SecurityGroupRemediationActionTypeDef = TypedDict(
     "SecurityGroupRemediationActionTypeDef",
     {
         "RemediationActionType": RemediationActionTypeType,
         "Description": str,
         "RemediationResult": SecurityGroupRuleDescriptionTypeDef,
         "IsDefaultAction": bool,
@@ -2001,15 +1992,15 @@
 )
 
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
         "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
@@ -2019,43 +2010,45 @@
     "_OptionalPutAdminAccountRequestRequestTypeDef",
     {
         "AdminScope": AdminScopeTypeDef,
     },
     total=False,
 )
 
+
 class PutAdminAccountRequestRequestTypeDef(
     _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
 ):
     pass
 
+
 GetAppsListResponseTypeDef = TypedDict(
     "GetAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAppsListResponseTypeDef = TypedDict(
     "PutAppsListResponseTypeDef",
     {
         "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAppsListsResponseTypeDef = TypedDict(
     "ListAppsListsResponseTypeDef",
     {
         "AppsLists": List[AppsListDataSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
@@ -2065,33 +2058,35 @@
     "_OptionalPutAppsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
+
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComplianceStatusResponseTypeDef = TypedDict(
     "ListComplianceStatusResponseTypeDef",
     {
         "PolicyComplianceStatusList": List[PolicyComplianceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFirewallPolicyDescriptionTypeDef = TypedDict(
     "NetworkFirewallPolicyDescriptionTypeDef",
     {
         "StatelessRuleGroups": List[StatelessRuleGroupTypeDef],
@@ -2101,34 +2096,14 @@
         "StatefulRuleGroups": List[StatefulRuleGroupTypeDef],
         "StatefulDefaultActions": List[str],
         "StatefulEngineOptions": StatefulEngineOptionsTypeDef,
     },
     total=False,
 )
 
-_RequiredSecurityServicePolicyDataOutputTypeDef = TypedDict(
-    "_RequiredSecurityServicePolicyDataOutputTypeDef",
-    {
-        "Type": SecurityServiceTypeType,
-    },
-)
-_OptionalSecurityServicePolicyDataOutputTypeDef = TypedDict(
-    "_OptionalSecurityServicePolicyDataOutputTypeDef",
-    {
-        "ManagedServiceData": str,
-        "PolicyOption": PolicyOptionOutputTypeDef,
-    },
-    total=False,
-)
-
-class SecurityServicePolicyDataOutputTypeDef(
-    _RequiredSecurityServicePolicyDataOutputTypeDef, _OptionalSecurityServicePolicyDataOutputTypeDef
-):
-    pass
-
 _RequiredSecurityServicePolicyDataTypeDef = TypedDict(
     "_RequiredSecurityServicePolicyDataTypeDef",
     {
         "Type": SecurityServiceTypeType,
     },
 )
 _OptionalSecurityServicePolicyDataTypeDef = TypedDict(
@@ -2136,19 +2111,21 @@
     {
         "ManagedServiceData": str,
         "PolicyOption": PolicyOptionTypeDef,
     },
     total=False,
 )
 
+
 class SecurityServicePolicyDataTypeDef(
     _RequiredSecurityServicePolicyDataTypeDef, _OptionalSecurityServicePolicyDataTypeDef
 ):
     pass
 
+
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": str,
         "ViolationTargetDescription": str,
         "PartialMatches": List[PartialMatchTypeDef],
         "PossibleSecurityGroupRemediationActions": List[SecurityGroupRemediationActionTypeDef],
@@ -2175,40 +2152,42 @@
     total=False,
 )
 
 _RequiredPolicyOutputTypeDef = TypedDict(
     "_RequiredPolicyOutputTypeDef",
     {
         "PolicyName": str,
-        "SecurityServicePolicyData": SecurityServicePolicyDataOutputTypeDef,
+        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
     },
 )
 _OptionalPolicyOutputTypeDef = TypedDict(
     "_OptionalPolicyOutputTypeDef",
     {
         "PolicyId": str,
         "PolicyUpdateToken": str,
         "ResourceTypeList": List[str],
-        "ResourceTags": List[ResourceTagOutputTypeDef],
+        "ResourceTags": List[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ExcludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
+
 class PolicyOutputTypeDef(_RequiredPolicyOutputTypeDef, _OptionalPolicyOutputTypeDef):
     pass
 
+
 _RequiredPolicyTypeDef = TypedDict(
     "_RequiredPolicyTypeDef",
     {
         "PolicyName": str,
         "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
@@ -2228,17 +2207,19 @@
         "ResourceSetIds": Sequence[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
+
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
+
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
     },
 )
 _OptionalPossibleRemediationActionTypeDef = TypedDict(
@@ -2246,34 +2227,36 @@
     {
         "Description": str,
         "IsDefaultAction": bool,
     },
     total=False,
 )
 
+
 class PossibleRemediationActionTypeDef(
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
+
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
         "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutPolicyResponseTypeDef = TypedDict(
     "PutPolicyResponseTypeDef",
     {
         "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
@@ -2283,19 +2266,21 @@
     "_OptionalPutPolicyRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
+
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
         "Actions": List[PossibleRemediationActionTypeDef],
     },
     total=False,
@@ -2360,23 +2345,25 @@
         "ResourceType": str,
         "ResourceViolations": List[ResourceViolationTypeDef],
     },
 )
 _OptionalViolationDetailTypeDef = TypedDict(
     "_OptionalViolationDetailTypeDef",
     {
-        "ResourceTags": List[TagOutputTypeDef],
+        "ResourceTags": List[TagTypeDef],
         "ResourceDescription": str,
     },
     total=False,
 )
 
+
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
+
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/PKG-INFO` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-fms
-Version: 1.28.12
-Summary: Type annotations for boto3.FMS 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-fms.svg?color=blue)](https://pypi.org/project/mypy-boto3-fms)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-fms)](https://pepy.tech/project/mypy-boto3-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.FMS 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
+[boto3.FMS 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [mypy-boto3-fms docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_fms/).
 
 See how it helps to find and fix potential bugs:
 
@@ -381,162 +381,155 @@
     AdminAccountSummaryTypeDef,
     OrganizationalUnitScopeOutputTypeDef,
     PolicyTypeScopeOutputTypeDef,
     RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
-    AppOutputTypeDef,
     AppTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
-    GetAdminAccountResponseTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
-    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
     GetProtectionStatusRequestRequestTypeDef,
-    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
     ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
     ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
-    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
-    ListAdminsManagingAccountResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
-    ListMemberAccountsResponseTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    TagTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
-    NetworkFirewallPolicyOutputTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
-    PaginatorConfigTypeDef,
-    ThirdPartyFirewallPolicyOutputTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
-    ResourceTagOutputTypeDef,
     ResourceTagTypeDef,
     ProtocolsListDataTypeDef,
-    TagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ResourceSetTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
-    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
-    ListAdminAccountsForOrganizationResponseTypeDef,
     AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
     AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetNotificationChannelResponseTypeDef,
+    GetProtectionStatusResponseTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
-    PolicyOptionOutputTypeDef,
     PolicyOptionTypeDef,
     PutProtocolsListRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
     PutResourceSetRequestRequestTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
     PutAdminAccountRequestRequestTypeDef,
     GetAppsListResponseTypeDef,
     PutAppsListResponseTypeDef,
     ListAppsListsResponseTypeDef,
     PutAppsListRequestRequestTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
-    SecurityServicePolicyDataOutputTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
     PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
```

### Comparing `mypy-boto3-fms-1.28.12/mypy_boto3_fms.egg-info/SOURCES.txt` & `mypy-boto3-fms-1.28.15/mypy_boto3_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-fms-1.28.12/setup.py` & `mypy-boto3-fms-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-fms",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.FMS 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.FMS 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

