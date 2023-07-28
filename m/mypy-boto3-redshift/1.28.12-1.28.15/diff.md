# Comparing `tmp/mypy-boto3-redshift-1.28.12.tar.gz` & `tmp/mypy-boto3-redshift-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-redshift-1.28.12.tar", last modified: Thu Jul 27 11:49:27 2023, max compression
+gzip compressed data, was "mypy-boto3-redshift-1.28.15.tar", last modified: Fri Jul 28 20:43:33 2023, max compression
```

## Comparing `mypy-boto3-redshift-1.28.12.tar` & `mypy-boto3-redshift-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.825190 mypy-boto3-redshift-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-07-27 11:49:27.825190 mypy-boto3-redshift-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35679 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.821190 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   115402 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   115235 2023-07-27 11:44:16.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-07-27 11:44:19.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-07-27 11:44:19.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    43550 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43515 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   136230 2023-07-27 11:44:22.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   136109 2023-07-27 11:44:20.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-27 11:44:17.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:27.825190 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 11:49:27.000000 mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:27.825190 mypy-boto3-redshift-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 11:44:15.000000 mypy-boto3-redshift-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.457723 mypy-boto3-redshift-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36918 2023-07-28 20:43:33.457723 mypy-boto3-redshift-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    35427 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.449723 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115226 2023-07-28 20:36:34.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115059 2023-07-28 20:36:34.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17351 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17349 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    43550 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43515 2023-07-28 20:36:34.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   134047 2023-07-28 20:36:39.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   133928 2023-07-28 20:36:37.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5320 2023-07-28 20:36:35.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:33.457723 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36918 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-28 20:43:33.000000 mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:33.457723 mypy-boto3-redshift-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-28 20:36:33.000000 mypy-boto3-redshift-1.28.15/setup.py
```

### Comparing `mypy-boto3-redshift-1.28.12/LICENSE` & `mypy-boto3-redshift-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/PKG-INFO` & `mypy-boto3-redshift-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.28.12
-Summary: Type annotations for boto3.Redshift 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -558,32 +558,31 @@
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
     RevisionTargetTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
-    ParameterOutputTypeDef,
+    ParameterTypeDef,
     ClusterParameterStatusTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
     HsmStatusTypeDef,
     PendingModifiedValuesTypeDef,
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    TagTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
@@ -654,41 +653,37 @@
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
-    ParameterTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PauseClusterMessageOutputTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
-    ResizeClusterMessageOutputTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
-    ResumeClusterMessageOutputTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
@@ -697,15 +692,15 @@
     ClusterExtendedCredentialsTypeDef,
     ClusterParameterGroupNameMessageTypeDef,
     CreateAuthenticationProfileResultTypeDef,
     CreateCustomDomainAssociationResultTypeDef,
     CustomerStorageMessageTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
     LoggingStatusTypeDef,
     ModifyAuthenticationProfileResultTypeDef,
     ModifyCustomDomainAssociationResultTypeDef,
     PartnerIntegrationOutputMessageTypeDef,
     ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
@@ -714,43 +709,45 @@
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
     DefaultClusterParametersTypeDef,
+    ModifyClusterParameterGroupMessageRequestTypeDef,
+    ResetClusterParameterGroupMessageRequestTypeDef,
     ClusterParameterGroupStatusTypeDef,
     ClusterParameterGroupTypeDef,
-    EC2SecurityGroupTypeDef,
-    EventSubscriptionTypeDef,
-    HsmClientCertificateTypeDef,
-    HsmConfigurationTypeDef,
-    IPRangeTypeDef,
-    SnapshotCopyGrantTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
-    SnapshotScheduleTypeDef,
-    SnapshotTypeDef,
-    TaggedResourceTypeDef,
-    UsageLimitResponseMetadataTypeDef,
-    UsageLimitTypeDef,
-    DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
-    ClusterVersionsMessageTypeDef,
     CreateClusterMessageRequestTypeDef,
     CreateClusterParameterGroupMessageRequestTypeDef,
     CreateClusterSecurityGroupMessageRequestTypeDef,
     CreateClusterSnapshotMessageRequestTypeDef,
     CreateClusterSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateHsmClientCertificateMessageRequestTypeDef,
     CreateHsmConfigurationMessageRequestTypeDef,
     CreateSnapshotCopyGrantMessageRequestTypeDef,
     CreateSnapshotScheduleMessageRequestTypeDef,
     CreateTagsMessageRequestTypeDef,
     CreateUsageLimitMessageRequestTypeDef,
-    DataShareResponseMetadataTypeDef,
+    EC2SecurityGroupTypeDef,
+    EventSubscriptionTypeDef,
+    HsmClientCertificateTypeDef,
+    HsmConfigurationTypeDef,
+    IPRangeTypeDef,
+    SnapshotCopyGrantTypeDef,
+    SnapshotScheduleResponseTypeDef,
+    SnapshotScheduleTypeDef,
+    SnapshotTypeDef,
+    TaggedResourceTypeDef,
+    UsageLimitResponseTypeDef,
+    UsageLimitTypeDef,
+    DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
+    ClusterVersionsMessageTypeDef,
+    DataShareResponseTypeDef,
     DataShareTypeDef,
     DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
@@ -788,23 +785,20 @@
     DescribeNodeConfigurationOptionsMessageRequestTypeDef,
     DescribePartnersOutputMessageTypeDef,
     DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsMessageRequestTypeDef,
     EndpointAuthorizationListTypeDef,
     EventCategoriesMapTypeDef,
     EventsMessageTypeDef,
-    ModifyClusterParameterGroupMessageRequestTypeDef,
-    ResetClusterParameterGroupMessageRequestTypeDef,
     VpcEndpointTypeDef,
     NodeConfigurationOptionsMessageTypeDef,
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
-    ScheduledActionTypeOutputTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
@@ -831,27 +825,27 @@
     SnapshotMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     UsageLimitListTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
     DescribeDataSharesResultTypeDef,
     EventCategoriesMessageTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
-    ScheduledActionTypeDef,
     CreateScheduledActionMessageRequestTypeDef,
     ModifyScheduledActionMessageRequestTypeDef,
+    ScheduledActionResponseTypeDef,
+    ScheduledActionTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
```

### Comparing `mypy-boto3-redshift-1.28.12/README.md` & `mypy-boto3-redshift-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -526,32 +526,31 @@
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
     RevisionTargetTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
-    ParameterOutputTypeDef,
+    ParameterTypeDef,
     ClusterParameterStatusTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
     HsmStatusTypeDef,
     PendingModifiedValuesTypeDef,
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    TagTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
@@ -622,41 +621,37 @@
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
-    ParameterTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PauseClusterMessageOutputTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
-    ResizeClusterMessageOutputTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
-    ResumeClusterMessageOutputTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
@@ -665,15 +660,15 @@
     ClusterExtendedCredentialsTypeDef,
     ClusterParameterGroupNameMessageTypeDef,
     CreateAuthenticationProfileResultTypeDef,
     CreateCustomDomainAssociationResultTypeDef,
     CustomerStorageMessageTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
     LoggingStatusTypeDef,
     ModifyAuthenticationProfileResultTypeDef,
     ModifyCustomDomainAssociationResultTypeDef,
     PartnerIntegrationOutputMessageTypeDef,
     ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
@@ -682,43 +677,45 @@
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
     DefaultClusterParametersTypeDef,
+    ModifyClusterParameterGroupMessageRequestTypeDef,
+    ResetClusterParameterGroupMessageRequestTypeDef,
     ClusterParameterGroupStatusTypeDef,
     ClusterParameterGroupTypeDef,
-    EC2SecurityGroupTypeDef,
-    EventSubscriptionTypeDef,
-    HsmClientCertificateTypeDef,
-    HsmConfigurationTypeDef,
-    IPRangeTypeDef,
-    SnapshotCopyGrantTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
-    SnapshotScheduleTypeDef,
-    SnapshotTypeDef,
-    TaggedResourceTypeDef,
-    UsageLimitResponseMetadataTypeDef,
-    UsageLimitTypeDef,
-    DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
-    ClusterVersionsMessageTypeDef,
     CreateClusterMessageRequestTypeDef,
     CreateClusterParameterGroupMessageRequestTypeDef,
     CreateClusterSecurityGroupMessageRequestTypeDef,
     CreateClusterSnapshotMessageRequestTypeDef,
     CreateClusterSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateHsmClientCertificateMessageRequestTypeDef,
     CreateHsmConfigurationMessageRequestTypeDef,
     CreateSnapshotCopyGrantMessageRequestTypeDef,
     CreateSnapshotScheduleMessageRequestTypeDef,
     CreateTagsMessageRequestTypeDef,
     CreateUsageLimitMessageRequestTypeDef,
-    DataShareResponseMetadataTypeDef,
+    EC2SecurityGroupTypeDef,
+    EventSubscriptionTypeDef,
+    HsmClientCertificateTypeDef,
+    HsmConfigurationTypeDef,
+    IPRangeTypeDef,
+    SnapshotCopyGrantTypeDef,
+    SnapshotScheduleResponseTypeDef,
+    SnapshotScheduleTypeDef,
+    SnapshotTypeDef,
+    TaggedResourceTypeDef,
+    UsageLimitResponseTypeDef,
+    UsageLimitTypeDef,
+    DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
+    ClusterVersionsMessageTypeDef,
+    DataShareResponseTypeDef,
     DataShareTypeDef,
     DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
@@ -756,23 +753,20 @@
     DescribeNodeConfigurationOptionsMessageRequestTypeDef,
     DescribePartnersOutputMessageTypeDef,
     DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsMessageRequestTypeDef,
     EndpointAuthorizationListTypeDef,
     EventCategoriesMapTypeDef,
     EventsMessageTypeDef,
-    ModifyClusterParameterGroupMessageRequestTypeDef,
-    ResetClusterParameterGroupMessageRequestTypeDef,
     VpcEndpointTypeDef,
     NodeConfigurationOptionsMessageTypeDef,
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
-    ScheduledActionTypeOutputTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
@@ -799,27 +793,27 @@
     SnapshotMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     UsageLimitListTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
     DescribeDataSharesResultTypeDef,
     EventCategoriesMessageTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
-    ScheduledActionTypeDef,
     CreateScheduledActionMessageRequestTypeDef,
     ModifyScheduledActionMessageRequestTypeDef,
+    ScheduledActionResponseTypeDef,
+    ScheduledActionTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
```

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__init__.py` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__init__.pyi` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/__main__.py` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Redshift 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.Redshift 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift\nOther"
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

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/client.py` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     CreateCustomDomainAssociationResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateHsmClientCertificateResultTypeDef,
     CreateHsmConfigurationResultTypeDef,
     CreateSnapshotCopyGrantResultTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     CustomerStorageMessageTypeDef,
-    DataShareResponseMetadataTypeDef,
+    DataShareResponseTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterResultTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     DeleteClusterSnapshotResultTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
@@ -113,17 +113,17 @@
     DescribePartnersOutputMessageTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     DescribeSnapshotSchedulesOutputMessageTypeDef,
     DisableSnapshotCopyResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableSnapshotCopyResultTypeDef,
     EndpointAccessListTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAuthorizationListTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     HsmClientCertificateMessageTypeDef,
     HsmConfigurationMessageTypeDef,
@@ -154,27 +154,27 @@
     RestoreFromClusterSnapshotResultTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
     RevokeSnapshotAccessResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
     ScheduledActionFilterTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
+    ScheduledActionResponseTypeDef,
     ScheduledActionsMessageTypeDef,
     ScheduledActionTypeTypeDef,
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
+    SnapshotScheduleResponseTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     TagTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
-    UsageLimitResponseMetadataTypeDef,
+    UsageLimitResponseTypeDef,
 )
 from .waiter import (
     ClusterAvailableWaiter,
     ClusterDeletedWaiter,
     ClusterRestoredWaiter,
     SnapshotAvailableWaiter,
 )
@@ -369,15 +369,15 @@
     def associate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         AssociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, associates a datashare with the account
         (AssociateEntireAccount) or the specified namespace (ConsumerArn).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.associate_data_share_consumer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#associate_data_share_consumer)
         """
@@ -395,26 +395,26 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_cluster_security_group_ingress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#authorize_cluster_security_group_ingress)
         """
 
     def authorize_data_share(
         self, *, DataShareArn: str, ConsumerIdentifier: str
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a data producer account, authorizes the sharing of a datashare with one or
         more consumer accounts or managing entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_data_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#authorize_data_share)
         """
 
     def authorize_endpoint_access(
         self, *, Account: str, ClusterIdentifier: str = ..., VpcIds: Sequence[str] = ...
-    ) -> EndpointAuthorizationResponseMetadataTypeDef:
+    ) -> EndpointAuthorizationResponseTypeDef:
         """
         Grants access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#authorize_endpoint_access)
         """
 
@@ -622,15 +622,15 @@
         self,
         *,
         EndpointName: str,
         SubnetGroupName: str,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    ) -> EndpointAccessResponseTypeDef:
         """
         Creates a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_endpoint_access)
         """
 
@@ -692,15 +692,15 @@
         TargetAction: ScheduledActionTypeTypeDef,
         Schedule: str,
         IamRole: str,
         ScheduledActionDescription: str = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Enable: bool = ...
-    ) -> ScheduledActionResponseMetadataTypeDef:
+    ) -> ScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_scheduled_action)
         """
 
@@ -721,15 +721,15 @@
         *,
         ScheduleDefinitions: Sequence[str] = ...,
         ScheduleIdentifier: str = ...,
         ScheduleDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         NextInvocations: int = ...
-    ) -> SnapshotScheduleResponseMetadataTypeDef:
+    ) -> SnapshotScheduleResponseTypeDef:
         """
         Create a snapshot schedule that can be associated to a cluster and which
         overrides the default system backup schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_snapshot_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_snapshot_schedule)
         """
@@ -750,25 +750,25 @@
         ClusterIdentifier: str,
         FeatureType: UsageLimitFeatureTypeType,
         LimitType: UsageLimitLimitTypeType,
         Amount: int,
         Period: UsageLimitPeriodType = ...,
         BreachAction: UsageLimitBreachActionType = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UsageLimitResponseMetadataTypeDef:
+    ) -> UsageLimitResponseTypeDef:
         """
         Creates a usage limit for a specified Amazon Redshift feature on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_usage_limit)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_usage_limit)
         """
 
     def deauthorize_data_share(
         self, *, DataShareArn: str, ConsumerIdentifier: str
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare producer account, removes authorization from the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.deauthorize_data_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#deauthorize_data_share)
         """
@@ -845,15 +845,15 @@
         """
         Contains information about deleting a custom domain association for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_custom_domain_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_custom_domain_association)
         """
 
-    def delete_endpoint_access(self, *, EndpointName: str) -> EndpointAccessResponseMetadataTypeDef:
+    def delete_endpoint_access(self, *, EndpointName: str) -> EndpointAccessResponseTypeDef:
         """
         Deletes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_endpoint_access)
         """
 
@@ -1520,15 +1520,15 @@
     def disassociate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         DisassociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, remove association for the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disassociate_data_share_consumer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#disassociate_data_share_consumer)
         """
@@ -1802,15 +1802,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_custom_domain_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_custom_domain_association)
         """
 
     def modify_endpoint_access(
         self, *, EndpointName: str, VpcSecurityGroupIds: Sequence[str] = ...
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    ) -> EndpointAccessResponseTypeDef:
         """
         Modifies a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_endpoint_access)
         """
 
@@ -1839,15 +1839,15 @@
         TargetAction: ScheduledActionTypeTypeDef = ...,
         Schedule: str = ...,
         IamRole: str = ...,
         ScheduledActionDescription: str = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Enable: bool = ...
-    ) -> ScheduledActionResponseMetadataTypeDef:
+    ) -> ScheduledActionResponseTypeDef:
         """
         Modifies a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_scheduled_action)
         """
 
@@ -1861,29 +1861,29 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_snapshot_copy_retention_period)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_snapshot_copy_retention_period)
         """
 
     def modify_snapshot_schedule(
         self, *, ScheduleIdentifier: str, ScheduleDefinitions: Sequence[str]
-    ) -> SnapshotScheduleResponseMetadataTypeDef:
+    ) -> SnapshotScheduleResponseTypeDef:
         """
         Modifies a snapshot schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_snapshot_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_snapshot_schedule)
         """
 
     def modify_usage_limit(
         self,
         *,
         UsageLimitId: str,
         Amount: int = ...,
         BreachAction: UsageLimitBreachActionType = ...
-    ) -> UsageLimitResponseMetadataTypeDef:
+    ) -> UsageLimitResponseTypeDef:
         """
         Modifies a usage limit in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_usage_limit)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_usage_limit)
         """
 
@@ -1909,15 +1909,15 @@
         """
         Reboots a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reboot_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#reboot_cluster)
         """
 
-    def reject_data_share(self, *, DataShareArn: str) -> DataShareResponseMetadataTypeDef:
+    def reject_data_share(self, *, DataShareArn: str) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, rejects the specified datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reject_data_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#reject_data_share)
         """
 
@@ -2045,15 +2045,15 @@
     def revoke_endpoint_access(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         VpcIds: Sequence[str] = ...,
         Force: bool = ...
-    ) -> EndpointAuthorizationResponseMetadataTypeDef:
+    ) -> EndpointAuthorizationResponseTypeDef:
         """
         Revokes access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#revoke_endpoint_access)
         """
```

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/client.pyi` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     CreateCustomDomainAssociationResultTypeDef,
     CreateEventSubscriptionResultTypeDef,
     CreateHsmClientCertificateResultTypeDef,
     CreateHsmConfigurationResultTypeDef,
     CreateSnapshotCopyGrantResultTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     CustomerStorageMessageTypeDef,
-    DataShareResponseMetadataTypeDef,
+    DataShareResponseTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     DeleteClusterResultTypeDef,
     DeleteClusterSnapshotMessageTypeDef,
     DeleteClusterSnapshotResultTypeDef,
     DescribeAuthenticationProfilesResultTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
@@ -113,17 +113,17 @@
     DescribePartnersOutputMessageTypeDef,
     DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
     DescribeSnapshotSchedulesOutputMessageTypeDef,
     DisableSnapshotCopyResultTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableSnapshotCopyResultTypeDef,
     EndpointAccessListTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAuthorizationListTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
     EventCategoriesMessageTypeDef,
     EventsMessageTypeDef,
     EventSubscriptionsMessageTypeDef,
     GetReservedNodeExchangeConfigurationOptionsOutputMessageTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     HsmClientCertificateMessageTypeDef,
     HsmConfigurationMessageTypeDef,
@@ -154,27 +154,27 @@
     RestoreFromClusterSnapshotResultTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     ResumeClusterResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
     RevokeSnapshotAccessResultTypeDef,
     RotateEncryptionKeyResultTypeDef,
     ScheduledActionFilterTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
+    ScheduledActionResponseTypeDef,
     ScheduledActionsMessageTypeDef,
     ScheduledActionTypeTypeDef,
     SnapshotCopyGrantMessageTypeDef,
     SnapshotMessageTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
+    SnapshotScheduleResponseTypeDef,
     SnapshotSortingEntityTypeDef,
     TableRestoreStatusMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     TagTypeDef,
     TrackListMessageTypeDef,
     UsageLimitListTypeDef,
-    UsageLimitResponseMetadataTypeDef,
+    UsageLimitResponseTypeDef,
 )
 from .waiter import (
     ClusterAvailableWaiter,
     ClusterDeletedWaiter,
     ClusterRestoredWaiter,
     SnapshotAvailableWaiter,
 )
@@ -362,15 +362,15 @@
     def associate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         AssociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, associates a datashare with the account
         (AssociateEntireAccount) or the specified namespace (ConsumerArn).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.associate_data_share_consumer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#associate_data_share_consumer)
         """
@@ -386,25 +386,25 @@
         Adds an inbound (ingress) rule to an Amazon Redshift security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_cluster_security_group_ingress)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#authorize_cluster_security_group_ingress)
         """
     def authorize_data_share(
         self, *, DataShareArn: str, ConsumerIdentifier: str
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a data producer account, authorizes the sharing of a datashare with one or
         more consumer accounts or managing entities.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_data_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#authorize_data_share)
         """
     def authorize_endpoint_access(
         self, *, Account: str, ClusterIdentifier: str = ..., VpcIds: Sequence[str] = ...
-    ) -> EndpointAuthorizationResponseMetadataTypeDef:
+    ) -> EndpointAuthorizationResponseTypeDef:
         """
         Grants access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.authorize_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#authorize_endpoint_access)
         """
     def authorize_snapshot_access(
@@ -597,15 +597,15 @@
         self,
         *,
         EndpointName: str,
         SubnetGroupName: str,
         ClusterIdentifier: str = ...,
         ResourceOwner: str = ...,
         VpcSecurityGroupIds: Sequence[str] = ...
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    ) -> EndpointAccessResponseTypeDef:
         """
         Creates a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_endpoint_access)
         """
     def create_event_subscription(
@@ -663,15 +663,15 @@
         TargetAction: ScheduledActionTypeTypeDef,
         Schedule: str,
         IamRole: str,
         ScheduledActionDescription: str = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Enable: bool = ...
-    ) -> ScheduledActionResponseMetadataTypeDef:
+    ) -> ScheduledActionResponseTypeDef:
         """
         Creates a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_scheduled_action)
         """
     def create_snapshot_copy_grant(
@@ -690,15 +690,15 @@
         *,
         ScheduleDefinitions: Sequence[str] = ...,
         ScheduleIdentifier: str = ...,
         ScheduleDescription: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DryRun: bool = ...,
         NextInvocations: int = ...
-    ) -> SnapshotScheduleResponseMetadataTypeDef:
+    ) -> SnapshotScheduleResponseTypeDef:
         """
         Create a snapshot schedule that can be associated to a cluster and which
         overrides the default system backup schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_snapshot_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_snapshot_schedule)
         """
@@ -717,24 +717,24 @@
         ClusterIdentifier: str,
         FeatureType: UsageLimitFeatureTypeType,
         LimitType: UsageLimitLimitTypeType,
         Amount: int,
         Period: UsageLimitPeriodType = ...,
         BreachAction: UsageLimitBreachActionType = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> UsageLimitResponseMetadataTypeDef:
+    ) -> UsageLimitResponseTypeDef:
         """
         Creates a usage limit for a specified Amazon Redshift feature on a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.create_usage_limit)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#create_usage_limit)
         """
     def deauthorize_data_share(
         self, *, DataShareArn: str, ConsumerIdentifier: str
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare producer account, removes authorization from the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.deauthorize_data_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#deauthorize_data_share)
         """
@@ -803,15 +803,15 @@
     ) -> EmptyResponseMetadataTypeDef:
         """
         Contains information about deleting a custom domain association for a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_custom_domain_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_custom_domain_association)
         """
-    def delete_endpoint_access(self, *, EndpointName: str) -> EndpointAccessResponseMetadataTypeDef:
+    def delete_endpoint_access(self, *, EndpointName: str) -> EndpointAccessResponseTypeDef:
         """
         Deletes a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.delete_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#delete_endpoint_access)
         """
     def delete_event_subscription(self, *, SubscriptionName: str) -> EmptyResponseMetadataTypeDef:
@@ -1428,15 +1428,15 @@
     def disassociate_data_share_consumer(
         self,
         *,
         DataShareArn: str,
         DisassociateEntireAccount: bool = ...,
         ConsumerArn: str = ...,
         ConsumerRegion: str = ...
-    ) -> DataShareResponseMetadataTypeDef:
+    ) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, remove association for the specified
         datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.disassociate_data_share_consumer)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#disassociate_data_share_consumer)
         """
@@ -1691,15 +1691,15 @@
         Contains information for changing a custom domain association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_custom_domain_association)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_custom_domain_association)
         """
     def modify_endpoint_access(
         self, *, EndpointName: str, VpcSecurityGroupIds: Sequence[str] = ...
-    ) -> EndpointAccessResponseMetadataTypeDef:
+    ) -> EndpointAccessResponseTypeDef:
         """
         Modifies a Redshift-managed VPC endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_endpoint_access)
         """
     def modify_event_subscription(
@@ -1726,15 +1726,15 @@
         TargetAction: ScheduledActionTypeTypeDef = ...,
         Schedule: str = ...,
         IamRole: str = ...,
         ScheduledActionDescription: str = ...,
         StartTime: Union[datetime, str] = ...,
         EndTime: Union[datetime, str] = ...,
         Enable: bool = ...
-    ) -> ScheduledActionResponseMetadataTypeDef:
+    ) -> ScheduledActionResponseTypeDef:
         """
         Modifies a scheduled action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_scheduled_action)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_scheduled_action)
         """
     def modify_snapshot_copy_retention_period(
@@ -1746,28 +1746,28 @@
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_snapshot_copy_retention_period)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_snapshot_copy_retention_period)
         """
     def modify_snapshot_schedule(
         self, *, ScheduleIdentifier: str, ScheduleDefinitions: Sequence[str]
-    ) -> SnapshotScheduleResponseMetadataTypeDef:
+    ) -> SnapshotScheduleResponseTypeDef:
         """
         Modifies a snapshot schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_snapshot_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_snapshot_schedule)
         """
     def modify_usage_limit(
         self,
         *,
         UsageLimitId: str,
         Amount: int = ...,
         BreachAction: UsageLimitBreachActionType = ...
-    ) -> UsageLimitResponseMetadataTypeDef:
+    ) -> UsageLimitResponseTypeDef:
         """
         Modifies a usage limit in a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.modify_usage_limit)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#modify_usage_limit)
         """
     def pause_cluster(self, *, ClusterIdentifier: str) -> PauseClusterResultTypeDef:
@@ -1789,15 +1789,15 @@
     def reboot_cluster(self, *, ClusterIdentifier: str) -> RebootClusterResultTypeDef:
         """
         Reboots a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reboot_cluster)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#reboot_cluster)
         """
-    def reject_data_share(self, *, DataShareArn: str) -> DataShareResponseMetadataTypeDef:
+    def reject_data_share(self, *, DataShareArn: str) -> DataShareResponseTypeDef:
         """
         From a datashare consumer account, rejects the specified datashare.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.reject_data_share)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#reject_data_share)
         """
     def reset_cluster_parameter_group(
@@ -1918,15 +1918,15 @@
     def revoke_endpoint_access(
         self,
         *,
         ClusterIdentifier: str = ...,
         Account: str = ...,
         VpcIds: Sequence[str] = ...,
         Force: bool = ...
-    ) -> EndpointAuthorizationResponseMetadataTypeDef:
+    ) -> EndpointAuthorizationResponseTypeDef:
         """
         Revokes access to a cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift.Client.revoke_endpoint_access)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/client/#revoke_endpoint_access)
         """
     def revoke_snapshot_access(
```

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/literals.py` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/literals.pyi` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/paginator.py` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/paginator.pyi` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/type_defs.py` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,32 +70,31 @@
     "SnapshotErrorMessageTypeDef",
     "BatchModifyClusterSnapshotsMessageRequestTypeDef",
     "CancelResizeMessageRequestTypeDef",
     "ClusterAssociatedToScheduleTypeDef",
     "RevisionTargetTypeDef",
     "ClusterIamRoleTypeDef",
     "ClusterNodeTypeDef",
-    "ParameterOutputTypeDef",
+    "ParameterTypeDef",
     "ClusterParameterStatusTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ClusterSecurityGroupMembershipTypeDef",
     "ClusterSnapshotCopyStatusTypeDef",
     "DataTransferProgressTypeDef",
     "DeferredMaintenanceWindowTypeDef",
     "ElasticIpStatusTypeDef",
     "HsmStatusTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReservedNodeExchangeStatusTypeDef",
     "ResizeInfoTypeDef",
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
-    "TagTypeDef",
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
@@ -166,41 +165,37 @@
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
     "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
-    "ParameterTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
     "ModifyCustomDomainAssociationMessageRequestTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     "ModifySnapshotScheduleMessageRequestTypeDef",
     "ModifyUsageLimitMessageRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeConfigurationOptionTypeDef",
     "PartnerIntegrationInputMessageRequestTypeDef",
-    "PauseClusterMessageOutputTypeDef",
     "PauseClusterMessageRequestTypeDef",
     "PauseClusterMessageTypeDef",
     "PurchaseReservedNodeOfferingMessageRequestTypeDef",
     "RebootClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectDataShareMessageRequestTypeDef",
-    "ResizeClusterMessageOutputTypeDef",
     "ResizeClusterMessageRequestTypeDef",
     "ResizeClusterMessageTypeDef",
     "RestoreFromClusterSnapshotMessageRequestTypeDef",
     "RestoreTableFromClusterSnapshotMessageRequestTypeDef",
     "TableRestoreStatusTypeDef",
-    "ResumeClusterMessageOutputTypeDef",
     "ResumeClusterMessageRequestTypeDef",
     "ResumeClusterMessageTypeDef",
     "RevokeClusterSecurityGroupIngressMessageRequestTypeDef",
     "RevokeEndpointAccessMessageRequestTypeDef",
     "RevokeSnapshotAccessMessageRequestTypeDef",
     "RotateEncryptionKeyMessageRequestTypeDef",
     "SupportedOperationTypeDef",
@@ -209,15 +204,15 @@
     "ClusterExtendedCredentialsTypeDef",
     "ClusterParameterGroupNameMessageTypeDef",
     "CreateAuthenticationProfileResultTypeDef",
     "CreateCustomDomainAssociationResultTypeDef",
     "CustomerStorageMessageTypeDef",
     "DeleteAuthenticationProfileResultTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "EndpointAuthorizationResponseMetadataTypeDef",
+    "EndpointAuthorizationResponseTypeDef",
     "LoggingStatusTypeDef",
     "ModifyAuthenticationProfileResultTypeDef",
     "ModifyCustomDomainAssociationResultTypeDef",
     "PartnerIntegrationOutputMessageTypeDef",
     "ResizeProgressMessageTypeDef",
     "AccountAttributeTypeDef",
     "ModifyAquaOutputMessageTypeDef",
@@ -226,43 +221,45 @@
     "AvailabilityZoneTypeDef",
     "BatchDeleteClusterSnapshotsRequestRequestTypeDef",
     "BatchDeleteClusterSnapshotsResultTypeDef",
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     "ClusterDbRevisionTypeDef",
     "ClusterParameterGroupDetailsTypeDef",
     "DefaultClusterParametersTypeDef",
+    "ModifyClusterParameterGroupMessageRequestTypeDef",
+    "ResetClusterParameterGroupMessageRequestTypeDef",
     "ClusterParameterGroupStatusTypeDef",
     "ClusterParameterGroupTypeDef",
-    "EC2SecurityGroupTypeDef",
-    "EventSubscriptionTypeDef",
-    "HsmClientCertificateTypeDef",
-    "HsmConfigurationTypeDef",
-    "IPRangeTypeDef",
-    "SnapshotCopyGrantTypeDef",
-    "SnapshotScheduleResponseMetadataTypeDef",
-    "SnapshotScheduleTypeDef",
-    "SnapshotTypeDef",
-    "TaggedResourceTypeDef",
-    "UsageLimitResponseMetadataTypeDef",
-    "UsageLimitTypeDef",
-    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
-    "ClusterVersionsMessageTypeDef",
     "CreateClusterMessageRequestTypeDef",
     "CreateClusterParameterGroupMessageRequestTypeDef",
     "CreateClusterSecurityGroupMessageRequestTypeDef",
     "CreateClusterSnapshotMessageRequestTypeDef",
     "CreateClusterSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateHsmClientCertificateMessageRequestTypeDef",
     "CreateHsmConfigurationMessageRequestTypeDef",
     "CreateSnapshotCopyGrantMessageRequestTypeDef",
     "CreateSnapshotScheduleMessageRequestTypeDef",
     "CreateTagsMessageRequestTypeDef",
     "CreateUsageLimitMessageRequestTypeDef",
-    "DataShareResponseMetadataTypeDef",
+    "EC2SecurityGroupTypeDef",
+    "EventSubscriptionTypeDef",
+    "HsmClientCertificateTypeDef",
+    "HsmConfigurationTypeDef",
+    "IPRangeTypeDef",
+    "SnapshotCopyGrantTypeDef",
+    "SnapshotScheduleResponseTypeDef",
+    "SnapshotScheduleTypeDef",
+    "SnapshotTypeDef",
+    "TaggedResourceTypeDef",
+    "UsageLimitResponseTypeDef",
+    "UsageLimitTypeDef",
+    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
+    "ClusterVersionsMessageTypeDef",
+    "DataShareResponseTypeDef",
     "DataShareTypeDef",
     "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
@@ -300,23 +297,20 @@
     "DescribeNodeConfigurationOptionsMessageRequestTypeDef",
     "DescribePartnersOutputMessageTypeDef",
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsMessageRequestTypeDef",
     "EndpointAuthorizationListTypeDef",
     "EventCategoriesMapTypeDef",
     "EventsMessageTypeDef",
-    "ModifyClusterParameterGroupMessageRequestTypeDef",
-    "ResetClusterParameterGroupMessageRequestTypeDef",
     "VpcEndpointTypeDef",
     "NodeConfigurationOptionsMessageTypeDef",
     "ReservedNodeOfferingTypeDef",
     "ReservedNodeTypeDef",
     "RestoreTableFromClusterSnapshotResultTypeDef",
     "TableRestoreStatusMessageTypeDef",
-    "ScheduledActionTypeOutputTypeDef",
     "ScheduledActionTypeTypeDef",
     "UpdateTargetTypeDef",
     "AccountAttributeListTypeDef",
     "CustomDomainAssociationsMessageTypeDef",
     "OrderableClusterOptionTypeDef",
     "SubnetTypeDef",
     "ClusterDbRevisionsMessageTypeDef",
@@ -343,27 +337,27 @@
     "SnapshotMessageTypeDef",
     "TaggedResourceListMessageTypeDef",
     "UsageLimitListTypeDef",
     "DescribeDataSharesForConsumerResultTypeDef",
     "DescribeDataSharesForProducerResultTypeDef",
     "DescribeDataSharesResultTypeDef",
     "EventCategoriesMessageTypeDef",
-    "EndpointAccessResponseMetadataTypeDef",
+    "EndpointAccessResponseTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     "ReservedNodeOfferingsMessageTypeDef",
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     "PurchaseReservedNodeOfferingResultTypeDef",
     "ReservedNodeConfigurationOptionTypeDef",
     "ReservedNodesMessageTypeDef",
-    "ScheduledActionResponseMetadataTypeDef",
-    "ScheduledActionTypeDef",
     "CreateScheduledActionMessageRequestTypeDef",
     "ModifyScheduledActionMessageRequestTypeDef",
+    "ScheduledActionResponseTypeDef",
+    "ScheduledActionTypeDef",
     "MaintenanceTrackTypeDef",
     "OrderableClusterOptionsMessageTypeDef",
     "ClusterSubnetGroupTypeDef",
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     "ClusterSecurityGroupMessageTypeDef",
     "CreateClusterSecurityGroupResultTypeDef",
     "RevokeClusterSecurityGroupIngressResultTypeDef",
@@ -663,16 +657,16 @@
         "NodeRole": str,
         "PrivateIPAddress": str,
         "PublicIPAddress": str,
     },
     total=False,
 )
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "DataType": str,
         "AllowedValues": str,
@@ -689,16 +683,16 @@
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -867,23 +861,14 @@
     "CreateAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 CreateCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "ClusterIdentifier": str,
     },
@@ -1901,30 +1886,14 @@
 
 class ModifyClusterMessageRequestTypeDef(
     _RequiredModifyClusterMessageRequestTypeDef, _OptionalModifyClusterMessageRequestTypeDef
 ):
     pass
 
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-        "Description": str,
-        "Source": str,
-        "DataType": str,
-        "AllowedValues": str,
-        "ApplyType": ParameterApplyTypeType,
-        "IsModifiable": bool,
-        "MinimumEngineVersion": str,
-    },
-    total=False,
-)
-
 _RequiredModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2143,21 +2112,14 @@
         "AccountId": str,
         "ClusterIdentifier": str,
         "DatabaseName": str,
         "PartnerName": str,
     },
 )
 
-PauseClusterMessageOutputTypeDef = TypedDict(
-    "PauseClusterMessageOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-
 PauseClusterMessageRequestTypeDef = TypedDict(
     "PauseClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2209,40 +2171,14 @@
 RejectDataShareMessageRequestTypeDef = TypedDict(
     "RejectDataShareMessageRequestTypeDef",
     {
         "DataShareArn": str,
     },
 )
 
-_RequiredResizeClusterMessageOutputTypeDef = TypedDict(
-    "_RequiredResizeClusterMessageOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-_OptionalResizeClusterMessageOutputTypeDef = TypedDict(
-    "_OptionalResizeClusterMessageOutputTypeDef",
-    {
-        "ClusterType": str,
-        "NodeType": str,
-        "NumberOfNodes": int,
-        "Classic": bool,
-        "ReservedNodeId": str,
-        "TargetReservedNodeOfferingId": str,
-    },
-    total=False,
-)
-
-
-class ResizeClusterMessageOutputTypeDef(
-    _RequiredResizeClusterMessageOutputTypeDef, _OptionalResizeClusterMessageOutputTypeDef
-):
-    pass
-
-
 _RequiredResizeClusterMessageRequestTypeDef = TypedDict(
     "_RequiredResizeClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalResizeClusterMessageRequestTypeDef = TypedDict(
@@ -2390,21 +2326,14 @@
         "TargetDatabaseName": str,
         "TargetSchemaName": str,
         "NewTableName": str,
     },
     total=False,
 )
 
-ResumeClusterMessageOutputTypeDef = TypedDict(
-    "ResumeClusterMessageOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-
 ResumeClusterMessageRequestTypeDef = TypedDict(
     "ResumeClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2585,16 +2514,16 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
-    "EndpointAuthorizationResponseMetadataTypeDef",
+EndpointAuthorizationResponseTypeDef = TypedDict(
+    "EndpointAuthorizationResponseTypeDef",
     {
         "Grantor": str,
         "Grantee": str,
         "ClusterIdentifier": str,
         "AuthorizeTime": datetime,
         "ClusterStatus": str,
         "Status": AuthorizationStatusType,
@@ -2751,249 +2680,82 @@
     },
     total=False,
 )
 
 ClusterParameterGroupDetailsTypeDef = TypedDict(
     "ClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefaultClusterParametersTypeDef = TypedDict(
     "DefaultClusterParametersTypeDef",
     {
         "ParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
     },
     total=False,
 )
 
-ClusterParameterGroupStatusTypeDef = TypedDict(
-    "ClusterParameterGroupStatusTypeDef",
+ModifyClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
-        "ParameterApplyStatus": str,
-        "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
+        "Parameters": Sequence[ParameterTypeDef],
     },
-    total=False,
 )
 
-ClusterParameterGroupTypeDef = TypedDict(
-    "ClusterParameterGroupTypeDef",
+_RequiredResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
-        "ParameterGroupFamily": str,
-        "Description": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-EC2SecurityGroupTypeDef = TypedDict(
-    "EC2SecurityGroupTypeDef",
-    {
-        "Status": str,
-        "EC2SecurityGroupName": str,
-        "EC2SecurityGroupOwnerId": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-EventSubscriptionTypeDef = TypedDict(
-    "EventSubscriptionTypeDef",
-    {
-        "CustomerAwsId": str,
-        "CustSubscriptionId": str,
-        "SnsTopicArn": str,
-        "Status": str,
-        "SubscriptionCreationTime": datetime,
-        "SourceType": str,
-        "SourceIdsList": List[str],
-        "EventCategoriesList": List[str],
-        "Severity": str,
-        "Enabled": bool,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-HsmClientCertificateTypeDef = TypedDict(
-    "HsmClientCertificateTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "HsmClientCertificatePublicKey": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-HsmConfigurationTypeDef = TypedDict(
-    "HsmConfigurationTypeDef",
-    {
-        "HsmConfigurationIdentifier": str,
-        "Description": str,
-        "HsmIpAddress": str,
-        "HsmPartitionName": str,
-        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
-
-IPRangeTypeDef = TypedDict(
-    "IPRangeTypeDef",
+_OptionalResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetClusterParameterGroupMessageRequestTypeDef",
     {
-        "Status": str,
-        "CIDRIP": str,
-        "Tags": List[TagOutputTypeDef],
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
     },
     total=False,
 )
 
-SnapshotCopyGrantTypeDef = TypedDict(
-    "SnapshotCopyGrantTypeDef",
-    {
-        "SnapshotCopyGrantName": str,
-        "KmsKeyId": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
 
-SnapshotScheduleResponseMetadataTypeDef = TypedDict(
-    "SnapshotScheduleResponseMetadataTypeDef",
-    {
-        "ScheduleDefinitions": List[str],
-        "ScheduleIdentifier": str,
-        "ScheduleDescription": str,
-        "Tags": List[TagOutputTypeDef],
-        "NextInvocations": List[datetime],
-        "AssociatedClusterCount": int,
-        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SnapshotScheduleTypeDef = TypedDict(
-    "SnapshotScheduleTypeDef",
-    {
-        "ScheduleDefinitions": List[str],
-        "ScheduleIdentifier": str,
-        "ScheduleDescription": str,
-        "Tags": List[TagOutputTypeDef],
-        "NextInvocations": List[datetime],
-        "AssociatedClusterCount": int,
-        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-    },
-    total=False,
-)
+class ResetClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
 
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotIdentifier": str,
-        "ClusterIdentifier": str,
-        "SnapshotCreateTime": datetime,
-        "Status": str,
-        "Port": int,
-        "AvailabilityZone": str,
-        "ClusterCreateTime": datetime,
-        "MasterUsername": str,
-        "ClusterVersion": str,
-        "EngineFullVersion": str,
-        "SnapshotType": str,
-        "NodeType": str,
-        "NumberOfNodes": int,
-        "DBName": str,
-        "VpcId": str,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "EncryptedWithHSM": bool,
-        "AccountsWithRestoreAccess": List[AccountWithRestoreAccessTypeDef],
-        "OwnerAccount": str,
-        "TotalBackupSizeInMegaBytes": float,
-        "ActualIncrementalBackupSizeInMegaBytes": float,
-        "BackupProgressInMegaBytes": float,
-        "CurrentBackupRateInMegaBytesPerSecond": float,
-        "EstimatedSecondsToCompletion": int,
-        "ElapsedTimeInSeconds": int,
-        "SourceRegion": str,
-        "Tags": List[TagOutputTypeDef],
-        "RestorableNodeTypes": List[str],
-        "EnhancedVpcRouting": bool,
-        "MaintenanceTrackName": str,
-        "ManualSnapshotRetentionPeriod": int,
-        "ManualSnapshotRemainingDays": int,
-        "SnapshotRetentionStartTime": datetime,
-    },
-    total=False,
-)
 
-TaggedResourceTypeDef = TypedDict(
-    "TaggedResourceTypeDef",
+ClusterParameterGroupStatusTypeDef = TypedDict(
+    "ClusterParameterGroupStatusTypeDef",
     {
-        "Tag": TagOutputTypeDef,
-        "ResourceName": str,
-        "ResourceType": str,
+        "ParameterGroupName": str,
+        "ParameterApplyStatus": str,
+        "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
     },
     total=False,
 )
 
-UsageLimitResponseMetadataTypeDef = TypedDict(
-    "UsageLimitResponseMetadataTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "LimitType": UsageLimitLimitTypeType,
-        "Amount": int,
-        "Period": UsageLimitPeriodType,
-        "BreachAction": UsageLimitBreachActionType,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UsageLimitTypeDef = TypedDict(
-    "UsageLimitTypeDef",
+ClusterParameterGroupTypeDef = TypedDict(
+    "ClusterParameterGroupTypeDef",
     {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "LimitType": UsageLimitLimitTypeType,
-        "Amount": int,
-        "Period": UsageLimitPeriodType,
-        "BreachAction": UsageLimitBreachActionType,
-        "Tags": List[TagOutputTypeDef],
+        "ParameterGroupName": str,
+        "ParameterGroupFamily": str,
+        "Description": str,
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
-    {
-        "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ClusterVersionsMessageTypeDef = TypedDict(
-    "ClusterVersionsMessageTypeDef",
-    {
-        "Marker": str,
-        "ClusterVersions": List[ClusterVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "NodeType": str,
         "MasterUsername": str,
         "MasterUserPassword": str,
@@ -3281,16 +3043,214 @@
 
 class CreateUsageLimitMessageRequestTypeDef(
     _RequiredCreateUsageLimitMessageRequestTypeDef, _OptionalCreateUsageLimitMessageRequestTypeDef
 ):
     pass
 
 
-DataShareResponseMetadataTypeDef = TypedDict(
-    "DataShareResponseMetadataTypeDef",
+EC2SecurityGroupTypeDef = TypedDict(
+    "EC2SecurityGroupTypeDef",
+    {
+        "Status": str,
+        "EC2SecurityGroupName": str,
+        "EC2SecurityGroupOwnerId": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+EventSubscriptionTypeDef = TypedDict(
+    "EventSubscriptionTypeDef",
+    {
+        "CustomerAwsId": str,
+        "CustSubscriptionId": str,
+        "SnsTopicArn": str,
+        "Status": str,
+        "SubscriptionCreationTime": datetime,
+        "SourceType": str,
+        "SourceIdsList": List[str],
+        "EventCategoriesList": List[str],
+        "Severity": str,
+        "Enabled": bool,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+HsmClientCertificateTypeDef = TypedDict(
+    "HsmClientCertificateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "HsmClientCertificatePublicKey": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+HsmConfigurationTypeDef = TypedDict(
+    "HsmConfigurationTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "Description": str,
+        "HsmIpAddress": str,
+        "HsmPartitionName": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+IPRangeTypeDef = TypedDict(
+    "IPRangeTypeDef",
+    {
+        "Status": str,
+        "CIDRIP": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+SnapshotCopyGrantTypeDef = TypedDict(
+    "SnapshotCopyGrantTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "KmsKeyId": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+SnapshotScheduleResponseTypeDef = TypedDict(
+    "SnapshotScheduleResponseTypeDef",
+    {
+        "ScheduleDefinitions": List[str],
+        "ScheduleIdentifier": str,
+        "ScheduleDescription": str,
+        "Tags": List[TagTypeDef],
+        "NextInvocations": List[datetime],
+        "AssociatedClusterCount": int,
+        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SnapshotScheduleTypeDef = TypedDict(
+    "SnapshotScheduleTypeDef",
+    {
+        "ScheduleDefinitions": List[str],
+        "ScheduleIdentifier": str,
+        "ScheduleDescription": str,
+        "Tags": List[TagTypeDef],
+        "NextInvocations": List[datetime],
+        "AssociatedClusterCount": int,
+        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+    },
+    total=False,
+)
+
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotIdentifier": str,
+        "ClusterIdentifier": str,
+        "SnapshotCreateTime": datetime,
+        "Status": str,
+        "Port": int,
+        "AvailabilityZone": str,
+        "ClusterCreateTime": datetime,
+        "MasterUsername": str,
+        "ClusterVersion": str,
+        "EngineFullVersion": str,
+        "SnapshotType": str,
+        "NodeType": str,
+        "NumberOfNodes": int,
+        "DBName": str,
+        "VpcId": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "EncryptedWithHSM": bool,
+        "AccountsWithRestoreAccess": List[AccountWithRestoreAccessTypeDef],
+        "OwnerAccount": str,
+        "TotalBackupSizeInMegaBytes": float,
+        "ActualIncrementalBackupSizeInMegaBytes": float,
+        "BackupProgressInMegaBytes": float,
+        "CurrentBackupRateInMegaBytesPerSecond": float,
+        "EstimatedSecondsToCompletion": int,
+        "ElapsedTimeInSeconds": int,
+        "SourceRegion": str,
+        "Tags": List[TagTypeDef],
+        "RestorableNodeTypes": List[str],
+        "EnhancedVpcRouting": bool,
+        "MaintenanceTrackName": str,
+        "ManualSnapshotRetentionPeriod": int,
+        "ManualSnapshotRemainingDays": int,
+        "SnapshotRetentionStartTime": datetime,
+    },
+    total=False,
+)
+
+TaggedResourceTypeDef = TypedDict(
+    "TaggedResourceTypeDef",
+    {
+        "Tag": TagTypeDef,
+        "ResourceName": str,
+        "ResourceType": str,
+    },
+    total=False,
+)
+
+UsageLimitResponseTypeDef = TypedDict(
+    "UsageLimitResponseTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "LimitType": UsageLimitLimitTypeType,
+        "Amount": int,
+        "Period": UsageLimitPeriodType,
+        "BreachAction": UsageLimitBreachActionType,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UsageLimitTypeDef = TypedDict(
+    "UsageLimitTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "LimitType": UsageLimitLimitTypeType,
+        "Amount": int,
+        "Period": UsageLimitPeriodType,
+        "BreachAction": UsageLimitBreachActionType,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
+    {
+        "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterVersionsMessageTypeDef = TypedDict(
+    "ClusterVersionsMessageTypeDef",
+    {
+        "Marker": str,
+        "ClusterVersions": List[ClusterVersionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DataShareResponseTypeDef = TypedDict(
+    "DataShareResponseTypeDef",
     {
         "DataShareArn": str,
         "ProducerArn": str,
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3890,45 +3850,14 @@
     {
         "Marker": str,
         "Events": List[EventTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-
-_RequiredResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-    total=False,
-)
-
-
-class ResetClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
-
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": str,
         "VpcId": str,
         "NetworkInterfaces": List[NetworkInterfaceTypeDef],
     },
@@ -3993,24 +3922,14 @@
     {
         "TableRestoreStatusDetails": List[TableRestoreStatusTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScheduledActionTypeOutputTypeDef = TypedDict(
-    "ScheduledActionTypeOutputTypeDef",
-    {
-        "ResizeCluster": ResizeClusterMessageOutputTypeDef,
-        "PauseCluster": PauseClusterMessageOutputTypeDef,
-        "ResumeCluster": ResumeClusterMessageOutputTypeDef,
-    },
-    total=False,
-)
-
 ScheduledActionTypeTypeDef = TypedDict(
     "ScheduledActionTypeTypeDef",
     {
         "ResizeCluster": ResizeClusterMessageTypeDef,
         "PauseCluster": PauseClusterMessageTypeDef,
         "ResumeCluster": ResumeClusterMessageTypeDef,
     },
@@ -4161,15 +4080,15 @@
 ClusterSecurityGroupTypeDef = TypedDict(
     "ClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Description": str,
         "EC2SecurityGroups": List[EC2SecurityGroupTypeDef],
         "IPRanges": List[IPRangeTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 CreateSnapshotCopyGrantResultTypeDef = TypedDict(
     "CreateSnapshotCopyGrantResultTypeDef",
     {
@@ -4302,16 +4221,16 @@
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointAccessResponseMetadataTypeDef = TypedDict(
-    "EndpointAccessResponseMetadataTypeDef",
+EndpointAccessResponseTypeDef = TypedDict(
+    "EndpointAccessResponseTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "SubnetGroupName": str,
         "EndpointStatus": str,
         "EndpointName": str,
         "EndpointCreateTime": datetime,
@@ -4399,46 +4318,14 @@
     {
         "Marker": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScheduledActionResponseMetadataTypeDef = TypedDict(
-    "ScheduledActionResponseMetadataTypeDef",
-    {
-        "ScheduledActionName": str,
-        "TargetAction": ScheduledActionTypeOutputTypeDef,
-        "Schedule": str,
-        "IamRole": str,
-        "ScheduledActionDescription": str,
-        "State": ScheduledActionStateType,
-        "NextInvocations": List[datetime],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ScheduledActionTypeDef = TypedDict(
-    "ScheduledActionTypeDef",
-    {
-        "ScheduledActionName": str,
-        "TargetAction": ScheduledActionTypeOutputTypeDef,
-        "Schedule": str,
-        "IamRole": str,
-        "ScheduledActionDescription": str,
-        "State": ScheduledActionStateType,
-        "NextInvocations": List[datetime],
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
@@ -4487,14 +4374,46 @@
 class ModifyScheduledActionMessageRequestTypeDef(
     _RequiredModifyScheduledActionMessageRequestTypeDef,
     _OptionalModifyScheduledActionMessageRequestTypeDef,
 ):
     pass
 
 
+ScheduledActionResponseTypeDef = TypedDict(
+    "ScheduledActionResponseTypeDef",
+    {
+        "ScheduledActionName": str,
+        "TargetAction": ScheduledActionTypeTypeDef,
+        "Schedule": str,
+        "IamRole": str,
+        "ScheduledActionDescription": str,
+        "State": ScheduledActionStateType,
+        "NextInvocations": List[datetime],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduledActionTypeDef = TypedDict(
+    "ScheduledActionTypeDef",
+    {
+        "ScheduledActionName": str,
+        "TargetAction": ScheduledActionTypeTypeDef,
+        "Schedule": str,
+        "IamRole": str,
+        "ScheduledActionDescription": str,
+        "State": ScheduledActionStateType,
+        "NextInvocations": List[datetime],
+        "StartTime": datetime,
+        "EndTime": datetime,
+    },
+    total=False,
+)
+
 MaintenanceTrackTypeDef = TypedDict(
     "MaintenanceTrackTypeDef",
     {
         "MaintenanceTrackName": str,
         "DatabaseVersion": str,
         "UpdateTargets": List[UpdateTargetTypeDef],
     },
@@ -4514,15 +4433,15 @@
     "ClusterSubnetGroupTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "Description": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 AuthorizeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     {
@@ -4596,15 +4515,15 @@
         "DataTransferProgress": DataTransferProgressTypeDef,
         "HsmStatus": HsmStatusTypeDef,
         "ClusterSnapshotCopyStatus": ClusterSnapshotCopyStatusTypeDef,
         "ClusterPublicKey": str,
         "ClusterNodes": List[ClusterNodeTypeDef],
         "ElasticIpStatus": ElasticIpStatusTypeDef,
         "ClusterRevisionNumber": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "KmsKeyId": str,
         "EnhancedVpcRouting": bool,
         "IamRoles": List[ClusterIamRoleTypeDef],
         "PendingActions": List[str],
         "MaintenanceTrackName": str,
         "ElasticResizeNumberOfNodeOptions": str,
         "DeferredMaintenanceWindows": List[DeferredMaintenanceWindowTypeDef],
```

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/type_defs.pyi` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -69,32 +69,31 @@
     "SnapshotErrorMessageTypeDef",
     "BatchModifyClusterSnapshotsMessageRequestTypeDef",
     "CancelResizeMessageRequestTypeDef",
     "ClusterAssociatedToScheduleTypeDef",
     "RevisionTargetTypeDef",
     "ClusterIamRoleTypeDef",
     "ClusterNodeTypeDef",
-    "ParameterOutputTypeDef",
+    "ParameterTypeDef",
     "ClusterParameterStatusTypeDef",
-    "TagOutputTypeDef",
+    "TagTypeDef",
     "ClusterSecurityGroupMembershipTypeDef",
     "ClusterSnapshotCopyStatusTypeDef",
     "DataTransferProgressTypeDef",
     "DeferredMaintenanceWindowTypeDef",
     "ElasticIpStatusTypeDef",
     "HsmStatusTypeDef",
     "PendingModifiedValuesTypeDef",
     "ReservedNodeExchangeStatusTypeDef",
     "ResizeInfoTypeDef",
     "RestoreStatusTypeDef",
     "VpcSecurityGroupMembershipTypeDef",
     "ClusterVersionTypeDef",
     "CopyClusterSnapshotMessageRequestTypeDef",
     "CreateAuthenticationProfileMessageRequestTypeDef",
-    "TagTypeDef",
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     "CreateEndpointAccessMessageRequestTypeDef",
     "DataShareAssociationTypeDef",
     "DeauthorizeDataShareMessageRequestTypeDef",
     "DeleteAuthenticationProfileMessageRequestTypeDef",
     "DeleteClusterMessageRequestTypeDef",
     "DeleteClusterParameterGroupMessageRequestTypeDef",
@@ -165,41 +164,37 @@
     "GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef",
     "ModifyAquaInputMessageRequestTypeDef",
     "ModifyAuthenticationProfileMessageRequestTypeDef",
     "ModifyClusterDbRevisionMessageRequestTypeDef",
     "ModifyClusterIamRolesMessageRequestTypeDef",
     "ModifyClusterMaintenanceMessageRequestTypeDef",
     "ModifyClusterMessageRequestTypeDef",
-    "ParameterTypeDef",
     "ModifyClusterSnapshotMessageRequestTypeDef",
     "ModifyClusterSnapshotScheduleMessageRequestTypeDef",
     "ModifyClusterSubnetGroupMessageRequestTypeDef",
     "ModifyCustomDomainAssociationMessageRequestTypeDef",
     "ModifyEndpointAccessMessageRequestTypeDef",
     "ModifyEventSubscriptionMessageRequestTypeDef",
     "ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef",
     "ModifySnapshotScheduleMessageRequestTypeDef",
     "ModifyUsageLimitMessageRequestTypeDef",
     "NetworkInterfaceTypeDef",
     "NodeConfigurationOptionTypeDef",
     "PartnerIntegrationInputMessageRequestTypeDef",
-    "PauseClusterMessageOutputTypeDef",
     "PauseClusterMessageRequestTypeDef",
     "PauseClusterMessageTypeDef",
     "PurchaseReservedNodeOfferingMessageRequestTypeDef",
     "RebootClusterMessageRequestTypeDef",
     "RecurringChargeTypeDef",
     "RejectDataShareMessageRequestTypeDef",
-    "ResizeClusterMessageOutputTypeDef",
     "ResizeClusterMessageRequestTypeDef",
     "ResizeClusterMessageTypeDef",
     "RestoreFromClusterSnapshotMessageRequestTypeDef",
     "RestoreTableFromClusterSnapshotMessageRequestTypeDef",
     "TableRestoreStatusTypeDef",
-    "ResumeClusterMessageOutputTypeDef",
     "ResumeClusterMessageRequestTypeDef",
     "ResumeClusterMessageTypeDef",
     "RevokeClusterSecurityGroupIngressMessageRequestTypeDef",
     "RevokeEndpointAccessMessageRequestTypeDef",
     "RevokeSnapshotAccessMessageRequestTypeDef",
     "RotateEncryptionKeyMessageRequestTypeDef",
     "SupportedOperationTypeDef",
@@ -208,15 +203,15 @@
     "ClusterExtendedCredentialsTypeDef",
     "ClusterParameterGroupNameMessageTypeDef",
     "CreateAuthenticationProfileResultTypeDef",
     "CreateCustomDomainAssociationResultTypeDef",
     "CustomerStorageMessageTypeDef",
     "DeleteAuthenticationProfileResultTypeDef",
     "EmptyResponseMetadataTypeDef",
-    "EndpointAuthorizationResponseMetadataTypeDef",
+    "EndpointAuthorizationResponseTypeDef",
     "LoggingStatusTypeDef",
     "ModifyAuthenticationProfileResultTypeDef",
     "ModifyCustomDomainAssociationResultTypeDef",
     "PartnerIntegrationOutputMessageTypeDef",
     "ResizeProgressMessageTypeDef",
     "AccountAttributeTypeDef",
     "ModifyAquaOutputMessageTypeDef",
@@ -225,43 +220,45 @@
     "AvailabilityZoneTypeDef",
     "BatchDeleteClusterSnapshotsRequestRequestTypeDef",
     "BatchDeleteClusterSnapshotsResultTypeDef",
     "BatchModifyClusterSnapshotsOutputMessageTypeDef",
     "ClusterDbRevisionTypeDef",
     "ClusterParameterGroupDetailsTypeDef",
     "DefaultClusterParametersTypeDef",
+    "ModifyClusterParameterGroupMessageRequestTypeDef",
+    "ResetClusterParameterGroupMessageRequestTypeDef",
     "ClusterParameterGroupStatusTypeDef",
     "ClusterParameterGroupTypeDef",
-    "EC2SecurityGroupTypeDef",
-    "EventSubscriptionTypeDef",
-    "HsmClientCertificateTypeDef",
-    "HsmConfigurationTypeDef",
-    "IPRangeTypeDef",
-    "SnapshotCopyGrantTypeDef",
-    "SnapshotScheduleResponseMetadataTypeDef",
-    "SnapshotScheduleTypeDef",
-    "SnapshotTypeDef",
-    "TaggedResourceTypeDef",
-    "UsageLimitResponseMetadataTypeDef",
-    "UsageLimitTypeDef",
-    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
-    "ClusterVersionsMessageTypeDef",
     "CreateClusterMessageRequestTypeDef",
     "CreateClusterParameterGroupMessageRequestTypeDef",
     "CreateClusterSecurityGroupMessageRequestTypeDef",
     "CreateClusterSnapshotMessageRequestTypeDef",
     "CreateClusterSubnetGroupMessageRequestTypeDef",
     "CreateEventSubscriptionMessageRequestTypeDef",
     "CreateHsmClientCertificateMessageRequestTypeDef",
     "CreateHsmConfigurationMessageRequestTypeDef",
     "CreateSnapshotCopyGrantMessageRequestTypeDef",
     "CreateSnapshotScheduleMessageRequestTypeDef",
     "CreateTagsMessageRequestTypeDef",
     "CreateUsageLimitMessageRequestTypeDef",
-    "DataShareResponseMetadataTypeDef",
+    "EC2SecurityGroupTypeDef",
+    "EventSubscriptionTypeDef",
+    "HsmClientCertificateTypeDef",
+    "HsmConfigurationTypeDef",
+    "IPRangeTypeDef",
+    "SnapshotCopyGrantTypeDef",
+    "SnapshotScheduleResponseTypeDef",
+    "SnapshotScheduleTypeDef",
+    "SnapshotTypeDef",
+    "TaggedResourceTypeDef",
+    "UsageLimitResponseTypeDef",
+    "UsageLimitTypeDef",
+    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
+    "ClusterVersionsMessageTypeDef",
+    "DataShareResponseTypeDef",
     "DataShareTypeDef",
     "DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef",
     "DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef",
     "DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef",
     "DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef",
     "DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef",
     "DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef",
@@ -299,23 +296,20 @@
     "DescribeNodeConfigurationOptionsMessageRequestTypeDef",
     "DescribePartnersOutputMessageTypeDef",
     "DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef",
     "DescribeScheduledActionsMessageRequestTypeDef",
     "EndpointAuthorizationListTypeDef",
     "EventCategoriesMapTypeDef",
     "EventsMessageTypeDef",
-    "ModifyClusterParameterGroupMessageRequestTypeDef",
-    "ResetClusterParameterGroupMessageRequestTypeDef",
     "VpcEndpointTypeDef",
     "NodeConfigurationOptionsMessageTypeDef",
     "ReservedNodeOfferingTypeDef",
     "ReservedNodeTypeDef",
     "RestoreTableFromClusterSnapshotResultTypeDef",
     "TableRestoreStatusMessageTypeDef",
-    "ScheduledActionTypeOutputTypeDef",
     "ScheduledActionTypeTypeDef",
     "UpdateTargetTypeDef",
     "AccountAttributeListTypeDef",
     "CustomDomainAssociationsMessageTypeDef",
     "OrderableClusterOptionTypeDef",
     "SubnetTypeDef",
     "ClusterDbRevisionsMessageTypeDef",
@@ -342,27 +336,27 @@
     "SnapshotMessageTypeDef",
     "TaggedResourceListMessageTypeDef",
     "UsageLimitListTypeDef",
     "DescribeDataSharesForConsumerResultTypeDef",
     "DescribeDataSharesForProducerResultTypeDef",
     "DescribeDataSharesResultTypeDef",
     "EventCategoriesMessageTypeDef",
-    "EndpointAccessResponseMetadataTypeDef",
+    "EndpointAccessResponseTypeDef",
     "EndpointAccessTypeDef",
     "EndpointTypeDef",
     "GetReservedNodeExchangeOfferingsOutputMessageTypeDef",
     "ReservedNodeOfferingsMessageTypeDef",
     "AcceptReservedNodeExchangeOutputMessageTypeDef",
     "PurchaseReservedNodeOfferingResultTypeDef",
     "ReservedNodeConfigurationOptionTypeDef",
     "ReservedNodesMessageTypeDef",
-    "ScheduledActionResponseMetadataTypeDef",
-    "ScheduledActionTypeDef",
     "CreateScheduledActionMessageRequestTypeDef",
     "ModifyScheduledActionMessageRequestTypeDef",
+    "ScheduledActionResponseTypeDef",
+    "ScheduledActionTypeDef",
     "MaintenanceTrackTypeDef",
     "OrderableClusterOptionsMessageTypeDef",
     "ClusterSubnetGroupTypeDef",
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     "ClusterSecurityGroupMessageTypeDef",
     "CreateClusterSecurityGroupResultTypeDef",
     "RevokeClusterSecurityGroupIngressResultTypeDef",
@@ -650,16 +644,16 @@
         "NodeRole": str,
         "PrivateIPAddress": str,
         "PublicIPAddress": str,
     },
     total=False,
 )
 
-ParameterOutputTypeDef = TypedDict(
-    "ParameterOutputTypeDef",
+ParameterTypeDef = TypedDict(
+    "ParameterTypeDef",
     {
         "ParameterName": str,
         "ParameterValue": str,
         "Description": str,
         "Source": str,
         "DataType": str,
         "AllowedValues": str,
@@ -676,16 +670,16 @@
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
+TagTypeDef = TypedDict(
+    "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
@@ -852,23 +846,14 @@
     "CreateAuthenticationProfileMessageRequestTypeDef",
     {
         "AuthenticationProfileName": str,
         "AuthenticationProfileContent": str,
     },
 )
 
-TagTypeDef = TypedDict(
-    "TagTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 CreateCustomDomainAssociationMessageRequestTypeDef = TypedDict(
     "CreateCustomDomainAssociationMessageRequestTypeDef",
     {
         "CustomDomainName": str,
         "CustomDomainCertificateArn": str,
         "ClusterIdentifier": str,
     },
@@ -1852,30 +1837,14 @@
 )
 
 class ModifyClusterMessageRequestTypeDef(
     _RequiredModifyClusterMessageRequestTypeDef, _OptionalModifyClusterMessageRequestTypeDef
 ):
     pass
 
-ParameterTypeDef = TypedDict(
-    "ParameterTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterValue": str,
-        "Description": str,
-        "Source": str,
-        "DataType": str,
-        "AllowedValues": str,
-        "ApplyType": ParameterApplyTypeType,
-        "IsModifiable": bool,
-        "MinimumEngineVersion": str,
-    },
-    total=False,
-)
-
 _RequiredModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
     "_RequiredModifyClusterSnapshotMessageRequestTypeDef",
     {
         "SnapshotIdentifier": str,
     },
 )
 _OptionalModifyClusterSnapshotMessageRequestTypeDef = TypedDict(
@@ -2078,21 +2047,14 @@
         "AccountId": str,
         "ClusterIdentifier": str,
         "DatabaseName": str,
         "PartnerName": str,
     },
 )
 
-PauseClusterMessageOutputTypeDef = TypedDict(
-    "PauseClusterMessageOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-
 PauseClusterMessageRequestTypeDef = TypedDict(
     "PauseClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2142,38 +2104,14 @@
 RejectDataShareMessageRequestTypeDef = TypedDict(
     "RejectDataShareMessageRequestTypeDef",
     {
         "DataShareArn": str,
     },
 )
 
-_RequiredResizeClusterMessageOutputTypeDef = TypedDict(
-    "_RequiredResizeClusterMessageOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-_OptionalResizeClusterMessageOutputTypeDef = TypedDict(
-    "_OptionalResizeClusterMessageOutputTypeDef",
-    {
-        "ClusterType": str,
-        "NodeType": str,
-        "NumberOfNodes": int,
-        "Classic": bool,
-        "ReservedNodeId": str,
-        "TargetReservedNodeOfferingId": str,
-    },
-    total=False,
-)
-
-class ResizeClusterMessageOutputTypeDef(
-    _RequiredResizeClusterMessageOutputTypeDef, _OptionalResizeClusterMessageOutputTypeDef
-):
-    pass
-
 _RequiredResizeClusterMessageRequestTypeDef = TypedDict(
     "_RequiredResizeClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 _OptionalResizeClusterMessageRequestTypeDef = TypedDict(
@@ -2313,21 +2251,14 @@
         "TargetDatabaseName": str,
         "TargetSchemaName": str,
         "NewTableName": str,
     },
     total=False,
 )
 
-ResumeClusterMessageOutputTypeDef = TypedDict(
-    "ResumeClusterMessageOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-    },
-)
-
 ResumeClusterMessageRequestTypeDef = TypedDict(
     "ResumeClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
     },
 )
 
@@ -2502,16 +2433,16 @@
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointAuthorizationResponseMetadataTypeDef = TypedDict(
-    "EndpointAuthorizationResponseMetadataTypeDef",
+EndpointAuthorizationResponseTypeDef = TypedDict(
+    "EndpointAuthorizationResponseTypeDef",
     {
         "Grantor": str,
         "Grantee": str,
         "ClusterIdentifier": str,
         "AuthorizeTime": datetime,
         "ClusterStatus": str,
         "Status": AuthorizationStatusType,
@@ -2668,249 +2599,80 @@
     },
     total=False,
 )
 
 ClusterParameterGroupDetailsTypeDef = TypedDict(
     "ClusterParameterGroupDetailsTypeDef",
     {
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DefaultClusterParametersTypeDef = TypedDict(
     "DefaultClusterParametersTypeDef",
     {
         "ParameterGroupFamily": str,
         "Marker": str,
-        "Parameters": List[ParameterOutputTypeDef],
+        "Parameters": List[ParameterTypeDef],
     },
     total=False,
 )
 
-ClusterParameterGroupStatusTypeDef = TypedDict(
-    "ClusterParameterGroupStatusTypeDef",
+ModifyClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "ModifyClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
-        "ParameterApplyStatus": str,
-        "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
+        "Parameters": Sequence[ParameterTypeDef],
     },
-    total=False,
 )
 
-ClusterParameterGroupTypeDef = TypedDict(
-    "ClusterParameterGroupTypeDef",
+_RequiredResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_RequiredResetClusterParameterGroupMessageRequestTypeDef",
     {
         "ParameterGroupName": str,
-        "ParameterGroupFamily": str,
-        "Description": str,
-        "Tags": List[TagOutputTypeDef],
     },
-    total=False,
 )
-
-EC2SecurityGroupTypeDef = TypedDict(
-    "EC2SecurityGroupTypeDef",
+_OptionalResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
+    "_OptionalResetClusterParameterGroupMessageRequestTypeDef",
     {
-        "Status": str,
-        "EC2SecurityGroupName": str,
-        "EC2SecurityGroupOwnerId": str,
-        "Tags": List[TagOutputTypeDef],
+        "ResetAllParameters": bool,
+        "Parameters": Sequence[ParameterTypeDef],
     },
     total=False,
 )
 
-EventSubscriptionTypeDef = TypedDict(
-    "EventSubscriptionTypeDef",
-    {
-        "CustomerAwsId": str,
-        "CustSubscriptionId": str,
-        "SnsTopicArn": str,
-        "Status": str,
-        "SubscriptionCreationTime": datetime,
-        "SourceType": str,
-        "SourceIdsList": List[str],
-        "EventCategoriesList": List[str],
-        "Severity": str,
-        "Enabled": bool,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
+class ResetClusterParameterGroupMessageRequestTypeDef(
+    _RequiredResetClusterParameterGroupMessageRequestTypeDef,
+    _OptionalResetClusterParameterGroupMessageRequestTypeDef,
+):
+    pass
 
-HsmClientCertificateTypeDef = TypedDict(
-    "HsmClientCertificateTypeDef",
+ClusterParameterGroupStatusTypeDef = TypedDict(
+    "ClusterParameterGroupStatusTypeDef",
     {
-        "HsmClientCertificateIdentifier": str,
-        "HsmClientCertificatePublicKey": str,
-        "Tags": List[TagOutputTypeDef],
+        "ParameterGroupName": str,
+        "ParameterApplyStatus": str,
+        "ClusterParameterStatusList": List[ClusterParameterStatusTypeDef],
     },
     total=False,
 )
 
-HsmConfigurationTypeDef = TypedDict(
-    "HsmConfigurationTypeDef",
+ClusterParameterGroupTypeDef = TypedDict(
+    "ClusterParameterGroupTypeDef",
     {
-        "HsmConfigurationIdentifier": str,
+        "ParameterGroupName": str,
+        "ParameterGroupFamily": str,
         "Description": str,
-        "HsmIpAddress": str,
-        "HsmPartitionName": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-IPRangeTypeDef = TypedDict(
-    "IPRangeTypeDef",
-    {
-        "Status": str,
-        "CIDRIP": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-SnapshotCopyGrantTypeDef = TypedDict(
-    "SnapshotCopyGrantTypeDef",
-    {
-        "SnapshotCopyGrantName": str,
-        "KmsKeyId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-SnapshotScheduleResponseMetadataTypeDef = TypedDict(
-    "SnapshotScheduleResponseMetadataTypeDef",
-    {
-        "ScheduleDefinitions": List[str],
-        "ScheduleIdentifier": str,
-        "ScheduleDescription": str,
-        "Tags": List[TagOutputTypeDef],
-        "NextInvocations": List[datetime],
-        "AssociatedClusterCount": int,
-        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-SnapshotScheduleTypeDef = TypedDict(
-    "SnapshotScheduleTypeDef",
-    {
-        "ScheduleDefinitions": List[str],
-        "ScheduleIdentifier": str,
-        "ScheduleDescription": str,
-        "Tags": List[TagOutputTypeDef],
-        "NextInvocations": List[datetime],
-        "AssociatedClusterCount": int,
-        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
-    },
-    total=False,
-)
-
-SnapshotTypeDef = TypedDict(
-    "SnapshotTypeDef",
-    {
-        "SnapshotIdentifier": str,
-        "ClusterIdentifier": str,
-        "SnapshotCreateTime": datetime,
-        "Status": str,
-        "Port": int,
-        "AvailabilityZone": str,
-        "ClusterCreateTime": datetime,
-        "MasterUsername": str,
-        "ClusterVersion": str,
-        "EngineFullVersion": str,
-        "SnapshotType": str,
-        "NodeType": str,
-        "NumberOfNodes": int,
-        "DBName": str,
-        "VpcId": str,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "EncryptedWithHSM": bool,
-        "AccountsWithRestoreAccess": List[AccountWithRestoreAccessTypeDef],
-        "OwnerAccount": str,
-        "TotalBackupSizeInMegaBytes": float,
-        "ActualIncrementalBackupSizeInMegaBytes": float,
-        "BackupProgressInMegaBytes": float,
-        "CurrentBackupRateInMegaBytesPerSecond": float,
-        "EstimatedSecondsToCompletion": int,
-        "ElapsedTimeInSeconds": int,
-        "SourceRegion": str,
-        "Tags": List[TagOutputTypeDef],
-        "RestorableNodeTypes": List[str],
-        "EnhancedVpcRouting": bool,
-        "MaintenanceTrackName": str,
-        "ManualSnapshotRetentionPeriod": int,
-        "ManualSnapshotRemainingDays": int,
-        "SnapshotRetentionStartTime": datetime,
-    },
-    total=False,
-)
-
-TaggedResourceTypeDef = TypedDict(
-    "TaggedResourceTypeDef",
-    {
-        "Tag": TagOutputTypeDef,
-        "ResourceName": str,
-        "ResourceType": str,
-    },
-    total=False,
-)
-
-UsageLimitResponseMetadataTypeDef = TypedDict(
-    "UsageLimitResponseMetadataTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "LimitType": UsageLimitLimitTypeType,
-        "Amount": int,
-        "Period": UsageLimitPeriodType,
-        "BreachAction": UsageLimitBreachActionType,
-        "Tags": List[TagOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-UsageLimitTypeDef = TypedDict(
-    "UsageLimitTypeDef",
-    {
-        "UsageLimitId": str,
-        "ClusterIdentifier": str,
-        "FeatureType": UsageLimitFeatureTypeType,
-        "LimitType": UsageLimitLimitTypeType,
-        "Amount": int,
-        "Period": UsageLimitPeriodType,
-        "BreachAction": UsageLimitBreachActionType,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
-DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
-    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
-    {
-        "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
-        "Marker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ClusterVersionsMessageTypeDef = TypedDict(
-    "ClusterVersionsMessageTypeDef",
-    {
-        "Marker": str,
-        "ClusterVersions": List[ClusterVersionTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredCreateClusterMessageRequestTypeDef = TypedDict(
     "_RequiredCreateClusterMessageRequestTypeDef",
     {
         "ClusterIdentifier": str,
         "NodeType": str,
         "MasterUsername": str,
         "MasterUserPassword": str,
@@ -3178,16 +2940,214 @@
 )
 
 class CreateUsageLimitMessageRequestTypeDef(
     _RequiredCreateUsageLimitMessageRequestTypeDef, _OptionalCreateUsageLimitMessageRequestTypeDef
 ):
     pass
 
-DataShareResponseMetadataTypeDef = TypedDict(
-    "DataShareResponseMetadataTypeDef",
+EC2SecurityGroupTypeDef = TypedDict(
+    "EC2SecurityGroupTypeDef",
+    {
+        "Status": str,
+        "EC2SecurityGroupName": str,
+        "EC2SecurityGroupOwnerId": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+EventSubscriptionTypeDef = TypedDict(
+    "EventSubscriptionTypeDef",
+    {
+        "CustomerAwsId": str,
+        "CustSubscriptionId": str,
+        "SnsTopicArn": str,
+        "Status": str,
+        "SubscriptionCreationTime": datetime,
+        "SourceType": str,
+        "SourceIdsList": List[str],
+        "EventCategoriesList": List[str],
+        "Severity": str,
+        "Enabled": bool,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+HsmClientCertificateTypeDef = TypedDict(
+    "HsmClientCertificateTypeDef",
+    {
+        "HsmClientCertificateIdentifier": str,
+        "HsmClientCertificatePublicKey": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+HsmConfigurationTypeDef = TypedDict(
+    "HsmConfigurationTypeDef",
+    {
+        "HsmConfigurationIdentifier": str,
+        "Description": str,
+        "HsmIpAddress": str,
+        "HsmPartitionName": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+IPRangeTypeDef = TypedDict(
+    "IPRangeTypeDef",
+    {
+        "Status": str,
+        "CIDRIP": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+SnapshotCopyGrantTypeDef = TypedDict(
+    "SnapshotCopyGrantTypeDef",
+    {
+        "SnapshotCopyGrantName": str,
+        "KmsKeyId": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+SnapshotScheduleResponseTypeDef = TypedDict(
+    "SnapshotScheduleResponseTypeDef",
+    {
+        "ScheduleDefinitions": List[str],
+        "ScheduleIdentifier": str,
+        "ScheduleDescription": str,
+        "Tags": List[TagTypeDef],
+        "NextInvocations": List[datetime],
+        "AssociatedClusterCount": int,
+        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SnapshotScheduleTypeDef = TypedDict(
+    "SnapshotScheduleTypeDef",
+    {
+        "ScheduleDefinitions": List[str],
+        "ScheduleIdentifier": str,
+        "ScheduleDescription": str,
+        "Tags": List[TagTypeDef],
+        "NextInvocations": List[datetime],
+        "AssociatedClusterCount": int,
+        "AssociatedClusters": List[ClusterAssociatedToScheduleTypeDef],
+    },
+    total=False,
+)
+
+SnapshotTypeDef = TypedDict(
+    "SnapshotTypeDef",
+    {
+        "SnapshotIdentifier": str,
+        "ClusterIdentifier": str,
+        "SnapshotCreateTime": datetime,
+        "Status": str,
+        "Port": int,
+        "AvailabilityZone": str,
+        "ClusterCreateTime": datetime,
+        "MasterUsername": str,
+        "ClusterVersion": str,
+        "EngineFullVersion": str,
+        "SnapshotType": str,
+        "NodeType": str,
+        "NumberOfNodes": int,
+        "DBName": str,
+        "VpcId": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "EncryptedWithHSM": bool,
+        "AccountsWithRestoreAccess": List[AccountWithRestoreAccessTypeDef],
+        "OwnerAccount": str,
+        "TotalBackupSizeInMegaBytes": float,
+        "ActualIncrementalBackupSizeInMegaBytes": float,
+        "BackupProgressInMegaBytes": float,
+        "CurrentBackupRateInMegaBytesPerSecond": float,
+        "EstimatedSecondsToCompletion": int,
+        "ElapsedTimeInSeconds": int,
+        "SourceRegion": str,
+        "Tags": List[TagTypeDef],
+        "RestorableNodeTypes": List[str],
+        "EnhancedVpcRouting": bool,
+        "MaintenanceTrackName": str,
+        "ManualSnapshotRetentionPeriod": int,
+        "ManualSnapshotRemainingDays": int,
+        "SnapshotRetentionStartTime": datetime,
+    },
+    total=False,
+)
+
+TaggedResourceTypeDef = TypedDict(
+    "TaggedResourceTypeDef",
+    {
+        "Tag": TagTypeDef,
+        "ResourceName": str,
+        "ResourceType": str,
+    },
+    total=False,
+)
+
+UsageLimitResponseTypeDef = TypedDict(
+    "UsageLimitResponseTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "LimitType": UsageLimitLimitTypeType,
+        "Amount": int,
+        "Period": UsageLimitPeriodType,
+        "BreachAction": UsageLimitBreachActionType,
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UsageLimitTypeDef = TypedDict(
+    "UsageLimitTypeDef",
+    {
+        "UsageLimitId": str,
+        "ClusterIdentifier": str,
+        "FeatureType": UsageLimitFeatureTypeType,
+        "LimitType": UsageLimitLimitTypeType,
+        "Amount": int,
+        "Period": UsageLimitPeriodType,
+        "BreachAction": UsageLimitBreachActionType,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
+DescribeReservedNodeExchangeStatusOutputMessageTypeDef = TypedDict(
+    "DescribeReservedNodeExchangeStatusOutputMessageTypeDef",
+    {
+        "ReservedNodeExchangeStatusDetails": List[ReservedNodeExchangeStatusTypeDef],
+        "Marker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ClusterVersionsMessageTypeDef = TypedDict(
+    "ClusterVersionsMessageTypeDef",
+    {
+        "Marker": str,
+        "ClusterVersions": List[ClusterVersionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DataShareResponseTypeDef = TypedDict(
+    "DataShareResponseTypeDef",
     {
         "DataShareArn": str,
         "ProducerArn": str,
         "AllowPubliclyAccessibleConsumers": bool,
         "DataShareAssociations": List[DataShareAssociationTypeDef],
         "ManagedBy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -3775,43 +3735,14 @@
     {
         "Marker": str,
         "Events": List[EventTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "ModifyClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ParameterGroupName": str,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-)
-
-_RequiredResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_RequiredResetClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ParameterGroupName": str,
-    },
-)
-_OptionalResetClusterParameterGroupMessageRequestTypeDef = TypedDict(
-    "_OptionalResetClusterParameterGroupMessageRequestTypeDef",
-    {
-        "ResetAllParameters": bool,
-        "Parameters": Sequence[ParameterTypeDef],
-    },
-    total=False,
-)
-
-class ResetClusterParameterGroupMessageRequestTypeDef(
-    _RequiredResetClusterParameterGroupMessageRequestTypeDef,
-    _OptionalResetClusterParameterGroupMessageRequestTypeDef,
-):
-    pass
-
 VpcEndpointTypeDef = TypedDict(
     "VpcEndpointTypeDef",
     {
         "VpcEndpointId": str,
         "VpcId": str,
         "NetworkInterfaces": List[NetworkInterfaceTypeDef],
     },
@@ -3876,24 +3807,14 @@
     {
         "TableRestoreStatusDetails": List[TableRestoreStatusTypeDef],
         "Marker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScheduledActionTypeOutputTypeDef = TypedDict(
-    "ScheduledActionTypeOutputTypeDef",
-    {
-        "ResizeCluster": ResizeClusterMessageOutputTypeDef,
-        "PauseCluster": PauseClusterMessageOutputTypeDef,
-        "ResumeCluster": ResumeClusterMessageOutputTypeDef,
-    },
-    total=False,
-)
-
 ScheduledActionTypeTypeDef = TypedDict(
     "ScheduledActionTypeTypeDef",
     {
         "ResizeCluster": ResizeClusterMessageTypeDef,
         "PauseCluster": PauseClusterMessageTypeDef,
         "ResumeCluster": ResumeClusterMessageTypeDef,
     },
@@ -4044,15 +3965,15 @@
 ClusterSecurityGroupTypeDef = TypedDict(
     "ClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Description": str,
         "EC2SecurityGroups": List[EC2SecurityGroupTypeDef],
         "IPRanges": List[IPRangeTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 CreateSnapshotCopyGrantResultTypeDef = TypedDict(
     "CreateSnapshotCopyGrantResultTypeDef",
     {
@@ -4185,16 +4106,16 @@
     "EventCategoriesMessageTypeDef",
     {
         "EventCategoriesMapList": List[EventCategoriesMapTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EndpointAccessResponseMetadataTypeDef = TypedDict(
-    "EndpointAccessResponseMetadataTypeDef",
+EndpointAccessResponseTypeDef = TypedDict(
+    "EndpointAccessResponseTypeDef",
     {
         "ClusterIdentifier": str,
         "ResourceOwner": str,
         "SubnetGroupName": str,
         "EndpointStatus": str,
         "EndpointName": str,
         "EndpointCreateTime": datetime,
@@ -4282,46 +4203,14 @@
     {
         "Marker": str,
         "ReservedNodes": List[ReservedNodeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ScheduledActionResponseMetadataTypeDef = TypedDict(
-    "ScheduledActionResponseMetadataTypeDef",
-    {
-        "ScheduledActionName": str,
-        "TargetAction": ScheduledActionTypeOutputTypeDef,
-        "Schedule": str,
-        "IamRole": str,
-        "ScheduledActionDescription": str,
-        "State": ScheduledActionStateType,
-        "NextInvocations": List[datetime],
-        "StartTime": datetime,
-        "EndTime": datetime,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ScheduledActionTypeDef = TypedDict(
-    "ScheduledActionTypeDef",
-    {
-        "ScheduledActionName": str,
-        "TargetAction": ScheduledActionTypeOutputTypeDef,
-        "Schedule": str,
-        "IamRole": str,
-        "ScheduledActionDescription": str,
-        "State": ScheduledActionStateType,
-        "NextInvocations": List[datetime],
-        "StartTime": datetime,
-        "EndTime": datetime,
-    },
-    total=False,
-)
-
 _RequiredCreateScheduledActionMessageRequestTypeDef = TypedDict(
     "_RequiredCreateScheduledActionMessageRequestTypeDef",
     {
         "ScheduledActionName": str,
         "TargetAction": ScheduledActionTypeTypeDef,
         "Schedule": str,
         "IamRole": str,
@@ -4366,14 +4255,46 @@
 
 class ModifyScheduledActionMessageRequestTypeDef(
     _RequiredModifyScheduledActionMessageRequestTypeDef,
     _OptionalModifyScheduledActionMessageRequestTypeDef,
 ):
     pass
 
+ScheduledActionResponseTypeDef = TypedDict(
+    "ScheduledActionResponseTypeDef",
+    {
+        "ScheduledActionName": str,
+        "TargetAction": ScheduledActionTypeTypeDef,
+        "Schedule": str,
+        "IamRole": str,
+        "ScheduledActionDescription": str,
+        "State": ScheduledActionStateType,
+        "NextInvocations": List[datetime],
+        "StartTime": datetime,
+        "EndTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ScheduledActionTypeDef = TypedDict(
+    "ScheduledActionTypeDef",
+    {
+        "ScheduledActionName": str,
+        "TargetAction": ScheduledActionTypeTypeDef,
+        "Schedule": str,
+        "IamRole": str,
+        "ScheduledActionDescription": str,
+        "State": ScheduledActionStateType,
+        "NextInvocations": List[datetime],
+        "StartTime": datetime,
+        "EndTime": datetime,
+    },
+    total=False,
+)
+
 MaintenanceTrackTypeDef = TypedDict(
     "MaintenanceTrackTypeDef",
     {
         "MaintenanceTrackName": str,
         "DatabaseVersion": str,
         "UpdateTargets": List[UpdateTargetTypeDef],
     },
@@ -4393,15 +4314,15 @@
     "ClusterSubnetGroupTypeDef",
     {
         "ClusterSubnetGroupName": str,
         "Description": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
         "Subnets": List[SubnetTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 AuthorizeClusterSecurityGroupIngressResultTypeDef = TypedDict(
     "AuthorizeClusterSecurityGroupIngressResultTypeDef",
     {
@@ -4475,15 +4396,15 @@
         "DataTransferProgress": DataTransferProgressTypeDef,
         "HsmStatus": HsmStatusTypeDef,
         "ClusterSnapshotCopyStatus": ClusterSnapshotCopyStatusTypeDef,
         "ClusterPublicKey": str,
         "ClusterNodes": List[ClusterNodeTypeDef],
         "ElasticIpStatus": ElasticIpStatusTypeDef,
         "ClusterRevisionNumber": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "KmsKeyId": str,
         "EnhancedVpcRouting": bool,
         "IamRoles": List[ClusterIamRoleTypeDef],
         "PendingActions": List[str],
         "MaintenanceTrackName": str,
         "ElasticResizeNumberOfNodeOptions": str,
         "DeferredMaintenanceWindows": List[DeferredMaintenanceWindowTypeDef],
```

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/waiter.py` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift/waiter.pyi` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/PKG-INFO` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-redshift
-Version: 1.28.12
-Summary: Type annotations for boto3.Redshift 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-redshift.svg?color=blue)](https://pypi.org/project/mypy-boto3-redshift)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-redshift)](https://pepy.tech/project/mypy-boto3-redshift)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Redshift 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
+[boto3.Redshift 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift.html#Redshift)
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
 [mypy-boto3-redshift docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_redshift/).
 
 See how it helps to find and fix potential bugs:
 
@@ -558,32 +558,31 @@
     SnapshotErrorMessageTypeDef,
     BatchModifyClusterSnapshotsMessageRequestTypeDef,
     CancelResizeMessageRequestTypeDef,
     ClusterAssociatedToScheduleTypeDef,
     RevisionTargetTypeDef,
     ClusterIamRoleTypeDef,
     ClusterNodeTypeDef,
-    ParameterOutputTypeDef,
+    ParameterTypeDef,
     ClusterParameterStatusTypeDef,
-    TagOutputTypeDef,
+    TagTypeDef,
     ClusterSecurityGroupMembershipTypeDef,
     ClusterSnapshotCopyStatusTypeDef,
     DataTransferProgressTypeDef,
     DeferredMaintenanceWindowTypeDef,
     ElasticIpStatusTypeDef,
     HsmStatusTypeDef,
     PendingModifiedValuesTypeDef,
     ReservedNodeExchangeStatusTypeDef,
     ResizeInfoTypeDef,
     RestoreStatusTypeDef,
     VpcSecurityGroupMembershipTypeDef,
     ClusterVersionTypeDef,
     CopyClusterSnapshotMessageRequestTypeDef,
     CreateAuthenticationProfileMessageRequestTypeDef,
-    TagTypeDef,
     CreateCustomDomainAssociationMessageRequestTypeDef,
     CreateEndpointAccessMessageRequestTypeDef,
     DataShareAssociationTypeDef,
     DeauthorizeDataShareMessageRequestTypeDef,
     DeleteAuthenticationProfileMessageRequestTypeDef,
     DeleteClusterMessageRequestTypeDef,
     DeleteClusterParameterGroupMessageRequestTypeDef,
@@ -654,41 +653,37 @@
     GetReservedNodeExchangeOfferingsInputMessageRequestTypeDef,
     ModifyAquaInputMessageRequestTypeDef,
     ModifyAuthenticationProfileMessageRequestTypeDef,
     ModifyClusterDbRevisionMessageRequestTypeDef,
     ModifyClusterIamRolesMessageRequestTypeDef,
     ModifyClusterMaintenanceMessageRequestTypeDef,
     ModifyClusterMessageRequestTypeDef,
-    ParameterTypeDef,
     ModifyClusterSnapshotMessageRequestTypeDef,
     ModifyClusterSnapshotScheduleMessageRequestTypeDef,
     ModifyClusterSubnetGroupMessageRequestTypeDef,
     ModifyCustomDomainAssociationMessageRequestTypeDef,
     ModifyEndpointAccessMessageRequestTypeDef,
     ModifyEventSubscriptionMessageRequestTypeDef,
     ModifySnapshotCopyRetentionPeriodMessageRequestTypeDef,
     ModifySnapshotScheduleMessageRequestTypeDef,
     ModifyUsageLimitMessageRequestTypeDef,
     NetworkInterfaceTypeDef,
     NodeConfigurationOptionTypeDef,
     PartnerIntegrationInputMessageRequestTypeDef,
-    PauseClusterMessageOutputTypeDef,
     PauseClusterMessageRequestTypeDef,
     PauseClusterMessageTypeDef,
     PurchaseReservedNodeOfferingMessageRequestTypeDef,
     RebootClusterMessageRequestTypeDef,
     RecurringChargeTypeDef,
     RejectDataShareMessageRequestTypeDef,
-    ResizeClusterMessageOutputTypeDef,
     ResizeClusterMessageRequestTypeDef,
     ResizeClusterMessageTypeDef,
     RestoreFromClusterSnapshotMessageRequestTypeDef,
     RestoreTableFromClusterSnapshotMessageRequestTypeDef,
     TableRestoreStatusTypeDef,
-    ResumeClusterMessageOutputTypeDef,
     ResumeClusterMessageRequestTypeDef,
     ResumeClusterMessageTypeDef,
     RevokeClusterSecurityGroupIngressMessageRequestTypeDef,
     RevokeEndpointAccessMessageRequestTypeDef,
     RevokeSnapshotAccessMessageRequestTypeDef,
     RotateEncryptionKeyMessageRequestTypeDef,
     SupportedOperationTypeDef,
@@ -697,15 +692,15 @@
     ClusterExtendedCredentialsTypeDef,
     ClusterParameterGroupNameMessageTypeDef,
     CreateAuthenticationProfileResultTypeDef,
     CreateCustomDomainAssociationResultTypeDef,
     CustomerStorageMessageTypeDef,
     DeleteAuthenticationProfileResultTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointAuthorizationResponseMetadataTypeDef,
+    EndpointAuthorizationResponseTypeDef,
     LoggingStatusTypeDef,
     ModifyAuthenticationProfileResultTypeDef,
     ModifyCustomDomainAssociationResultTypeDef,
     PartnerIntegrationOutputMessageTypeDef,
     ResizeProgressMessageTypeDef,
     AccountAttributeTypeDef,
     ModifyAquaOutputMessageTypeDef,
@@ -714,43 +709,45 @@
     AvailabilityZoneTypeDef,
     BatchDeleteClusterSnapshotsRequestRequestTypeDef,
     BatchDeleteClusterSnapshotsResultTypeDef,
     BatchModifyClusterSnapshotsOutputMessageTypeDef,
     ClusterDbRevisionTypeDef,
     ClusterParameterGroupDetailsTypeDef,
     DefaultClusterParametersTypeDef,
+    ModifyClusterParameterGroupMessageRequestTypeDef,
+    ResetClusterParameterGroupMessageRequestTypeDef,
     ClusterParameterGroupStatusTypeDef,
     ClusterParameterGroupTypeDef,
-    EC2SecurityGroupTypeDef,
-    EventSubscriptionTypeDef,
-    HsmClientCertificateTypeDef,
-    HsmConfigurationTypeDef,
-    IPRangeTypeDef,
-    SnapshotCopyGrantTypeDef,
-    SnapshotScheduleResponseMetadataTypeDef,
-    SnapshotScheduleTypeDef,
-    SnapshotTypeDef,
-    TaggedResourceTypeDef,
-    UsageLimitResponseMetadataTypeDef,
-    UsageLimitTypeDef,
-    DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
-    ClusterVersionsMessageTypeDef,
     CreateClusterMessageRequestTypeDef,
     CreateClusterParameterGroupMessageRequestTypeDef,
     CreateClusterSecurityGroupMessageRequestTypeDef,
     CreateClusterSnapshotMessageRequestTypeDef,
     CreateClusterSubnetGroupMessageRequestTypeDef,
     CreateEventSubscriptionMessageRequestTypeDef,
     CreateHsmClientCertificateMessageRequestTypeDef,
     CreateHsmConfigurationMessageRequestTypeDef,
     CreateSnapshotCopyGrantMessageRequestTypeDef,
     CreateSnapshotScheduleMessageRequestTypeDef,
     CreateTagsMessageRequestTypeDef,
     CreateUsageLimitMessageRequestTypeDef,
-    DataShareResponseMetadataTypeDef,
+    EC2SecurityGroupTypeDef,
+    EventSubscriptionTypeDef,
+    HsmClientCertificateTypeDef,
+    HsmConfigurationTypeDef,
+    IPRangeTypeDef,
+    SnapshotCopyGrantTypeDef,
+    SnapshotScheduleResponseTypeDef,
+    SnapshotScheduleTypeDef,
+    SnapshotTypeDef,
+    TaggedResourceTypeDef,
+    UsageLimitResponseTypeDef,
+    UsageLimitTypeDef,
+    DescribeReservedNodeExchangeStatusOutputMessageTypeDef,
+    ClusterVersionsMessageTypeDef,
+    DataShareResponseTypeDef,
     DataShareTypeDef,
     DescribeClusterDbRevisionsMessageDescribeClusterDbRevisionsPaginateTypeDef,
     DescribeClusterParameterGroupsMessageDescribeClusterParameterGroupsPaginateTypeDef,
     DescribeClusterParametersMessageDescribeClusterParametersPaginateTypeDef,
     DescribeClusterSecurityGroupsMessageDescribeClusterSecurityGroupsPaginateTypeDef,
     DescribeClusterSubnetGroupsMessageDescribeClusterSubnetGroupsPaginateTypeDef,
     DescribeClusterTracksMessageDescribeClusterTracksPaginateTypeDef,
@@ -788,23 +785,20 @@
     DescribeNodeConfigurationOptionsMessageRequestTypeDef,
     DescribePartnersOutputMessageTypeDef,
     DescribeScheduledActionsMessageDescribeScheduledActionsPaginateTypeDef,
     DescribeScheduledActionsMessageRequestTypeDef,
     EndpointAuthorizationListTypeDef,
     EventCategoriesMapTypeDef,
     EventsMessageTypeDef,
-    ModifyClusterParameterGroupMessageRequestTypeDef,
-    ResetClusterParameterGroupMessageRequestTypeDef,
     VpcEndpointTypeDef,
     NodeConfigurationOptionsMessageTypeDef,
     ReservedNodeOfferingTypeDef,
     ReservedNodeTypeDef,
     RestoreTableFromClusterSnapshotResultTypeDef,
     TableRestoreStatusMessageTypeDef,
-    ScheduledActionTypeOutputTypeDef,
     ScheduledActionTypeTypeDef,
     UpdateTargetTypeDef,
     AccountAttributeListTypeDef,
     CustomDomainAssociationsMessageTypeDef,
     OrderableClusterOptionTypeDef,
     SubnetTypeDef,
     ClusterDbRevisionsMessageTypeDef,
@@ -831,27 +825,27 @@
     SnapshotMessageTypeDef,
     TaggedResourceListMessageTypeDef,
     UsageLimitListTypeDef,
     DescribeDataSharesForConsumerResultTypeDef,
     DescribeDataSharesForProducerResultTypeDef,
     DescribeDataSharesResultTypeDef,
     EventCategoriesMessageTypeDef,
-    EndpointAccessResponseMetadataTypeDef,
+    EndpointAccessResponseTypeDef,
     EndpointAccessTypeDef,
     EndpointTypeDef,
     GetReservedNodeExchangeOfferingsOutputMessageTypeDef,
     ReservedNodeOfferingsMessageTypeDef,
     AcceptReservedNodeExchangeOutputMessageTypeDef,
     PurchaseReservedNodeOfferingResultTypeDef,
     ReservedNodeConfigurationOptionTypeDef,
     ReservedNodesMessageTypeDef,
-    ScheduledActionResponseMetadataTypeDef,
-    ScheduledActionTypeDef,
     CreateScheduledActionMessageRequestTypeDef,
     ModifyScheduledActionMessageRequestTypeDef,
+    ScheduledActionResponseTypeDef,
+    ScheduledActionTypeDef,
     MaintenanceTrackTypeDef,
     OrderableClusterOptionsMessageTypeDef,
     ClusterSubnetGroupTypeDef,
     AuthorizeClusterSecurityGroupIngressResultTypeDef,
     ClusterSecurityGroupMessageTypeDef,
     CreateClusterSecurityGroupResultTypeDef,
     RevokeClusterSecurityGroupIngressResultTypeDef,
```

### Comparing `mypy-boto3-redshift-1.28.12/mypy_boto3_redshift.egg-info/SOURCES.txt` & `mypy-boto3-redshift-1.28.15/mypy_boto3_redshift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-redshift-1.28.12/setup.py` & `mypy-boto3-redshift-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-redshift",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_redshift"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.Redshift 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.Redshift 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

