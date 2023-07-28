# Comparing `tmp/mypy-boto3-securityhub-1.28.12.tar.gz` & `tmp/mypy-boto3-securityhub-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-securityhub-1.28.12.tar", last modified: Thu Jul 27 11:49:36 2023, max compression
+gzip compressed data, was "mypy-boto3-securityhub-1.28.15.tar", last modified: Fri Jul 28 20:43:42 2023, max compression
```

## Comparing `mypy-boto3-securityhub-1.28.12.tar` & `mypy-boto3-securityhub-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.653272 mypy-boto3-securityhub-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    82510 2023-07-27 11:49:36.653272 mypy-boto3-securityhub-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    81007 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.641272 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:46:17.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   522233 2023-07-27 11:46:33.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   522150 2023-07-27 11:46:25.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:36.653272 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    82510 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 11:49:36.000000 mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:36.653272 mypy-boto3-securityhub-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-27 11:46:16.000000 mypy-boto3-securityhub-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:42.957853 mypy-boto3-securityhub-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    61539 2023-07-28 20:43:42.957853 mypy-boto3-securityhub-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60036 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:42.953853 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51872 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51783 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14205 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18316 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18299 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:38:49.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   402725 2023-07-28 20:39:03.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   402652 2023-07-28 20:38:58.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:42.957853 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    61539 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 20:43:42.000000 mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:42.957853 mypy-boto3-securityhub-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-28 20:38:48.000000 mypy-boto3-securityhub-1.28.15/setup.py
```

### Comparing `mypy-boto3-securityhub-1.28.12/LICENSE` & `mypy-boto3-securityhub-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/PKG-INFO` & `mypy-boto3-securityhub-1.28.15/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-securityhub
-Version: 1.28.12
-Summary: Type annotations for boto3.SecurityHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -418,682 +386,388 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    ActionLocalIpDetailsOutputTypeDef,
     ActionLocalIpDetailsTypeDef,
-    ActionLocalPortDetailsOutputTypeDef,
     ActionLocalPortDetailsTypeDef,
-    DnsRequestActionOutputTypeDef,
-    CityOutputTypeDef,
-    CountryOutputTypeDef,
-    GeoLocationOutputTypeDef,
-    IpOrganizationDetailsOutputTypeDef,
+    DnsRequestActionTypeDef,
     CityTypeDef,
     CountryTypeDef,
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
-    ActionRemotePortDetailsOutputTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
-    DnsRequestActionTypeDef,
-    AdjustmentOutputTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
-    AssociatedStandardOutputTypeDef,
     AssociatedStandardTypeDef,
-    AssociationStateDetailsOutputTypeDef,
     AssociationStateDetailsTypeDef,
-    NoteUpdateOutputTypeDef,
-    RelatedFindingOutputTypeDef,
-    SeverityUpdateOutputTypeDef,
-    WorkflowUpdateOutputTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
-    MapFilterOutputTypeDef,
-    NumberFilterOutputTypeDef,
-    StringFilterOutputTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
     AutomationRulesMetadataTypeDef,
-    AvailabilityZoneOutputTypeDef,
     AvailabilityZoneTypeDef,
-    AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
-    AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef,
-    AwsAmazonMqBrokerUsersDetailsOutputTypeDef,
     AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
     AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
     AwsAmazonMqBrokerUsersDetailsTypeDef,
-    AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
     AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
-    AwsApiCallActionDomainDetailsOutputTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
-    AwsApiGatewayAccessLogSettingsOutputTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsOutputTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationOutputTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
-    AwsApiGatewayMethodSettingsOutputTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationOutputTypeDef,
     AwsCorsConfigurationTypeDef,
-    AwsApiGatewayV2RouteSettingsOutputTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
-    AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
-    AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
-    AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
-    AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef,
-    AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef,
-    AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
     AwsBackupBackupPlanLifecycleDetailsTypeDef,
     AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
     AwsBackupBackupVaultNotificationsDetailsTypeDef,
-    AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef,
     AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef,
-    AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef,
     AwsBackupRecoveryPointCreatedByDetailsTypeDef,
-    AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef,
     AwsBackupRecoveryPointLifecycleDetailsTypeDef,
-    AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef,
-    AwsCertificateManagerCertificateKeyUsageOutputTypeDef,
-    AwsCertificateManagerCertificateOptionsOutputTypeDef,
     AwsCertificateManagerCertificateExtendedKeyUsageTypeDef,
     AwsCertificateManagerCertificateKeyUsageTypeDef,
     AwsCertificateManagerCertificateOptionsTypeDef,
-    AwsCertificateManagerCertificateResourceRecordOutputTypeDef,
     AwsCertificateManagerCertificateResourceRecordTypeDef,
-    AwsCloudFormationStackDriftInformationDetailsOutputTypeDef,
-    AwsCloudFormationStackOutputsDetailsOutputTypeDef,
     AwsCloudFormationStackDriftInformationDetailsTypeDef,
     AwsCloudFormationStackOutputsDetailsTypeDef,
-    AwsCloudFrontDistributionCacheBehaviorOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorTypeDef,
-    AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef,
     AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
-    AwsCloudFrontDistributionLoggingOutputTypeDef,
-    AwsCloudFrontDistributionViewerCertificateOutputTypeDef,
     AwsCloudFrontDistributionLoggingTypeDef,
     AwsCloudFrontDistributionViewerCertificateTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
-    AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef,
     AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
-    AwsCloudTrailTrailDetailsOutputTypeDef,
     AwsCloudTrailTrailDetailsTypeDef,
-    AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef,
     AwsCloudWatchAlarmDimensionsDetailsTypeDef,
-    AwsCodeBuildProjectArtifactsDetailsOutputTypeDef,
     AwsCodeBuildProjectArtifactsDetailsTypeDef,
-    AwsCodeBuildProjectSourceOutputTypeDef,
-    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectSourceTypeDef,
+    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectVpcConfigTypeDef,
-    AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef,
     AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef,
-    AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef,
     AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
-    AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
-    AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
-    AwsDynamoDbTableAttributeDefinitionOutputTypeDef,
     AwsDynamoDbTableAttributeDefinitionTypeDef,
-    AwsDynamoDbTableBillingModeSummaryOutputTypeDef,
     AwsDynamoDbTableBillingModeSummaryTypeDef,
-    AwsDynamoDbTableKeySchemaOutputTypeDef,
-    AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
-    AwsDynamoDbTableRestoreSummaryOutputTypeDef,
-    AwsDynamoDbTableSseDescriptionOutputTypeDef,
-    AwsDynamoDbTableStreamSpecificationOutputTypeDef,
     AwsDynamoDbTableKeySchemaTypeDef,
     AwsDynamoDbTableProvisionedThroughputTypeDef,
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionOutputTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
-    AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
-    AwsEc2EipDetailsOutputTypeDef,
     AwsEc2EipDetailsTypeDef,
-    AwsEc2InstanceMetadataOptionsOutputTypeDef,
-    AwsEc2InstanceMonitoringDetailsOutputTypeDef,
-    AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
     AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
     AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
     AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
-    AwsEc2NetworkAclAssociationOutputTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
-    IcmpTypeCodeOutputTypeDef,
-    PortRangeFromToOutputTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
-    AwsEc2NetworkInterfaceAttachmentOutputTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
-    AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef,
-    AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef,
-    AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
-    PropagatingVgwSetDetailsOutputTypeDef,
-    RouteSetDetailsOutputTypeDef,
     PropagatingVgwSetDetailsTypeDef,
     RouteSetDetailsTypeDef,
-    AwsEc2SecurityGroupIpRangeOutputTypeDef,
-    AwsEc2SecurityGroupIpv6RangeOutputTypeDef,
-    AwsEc2SecurityGroupPrefixListIdOutputTypeDef,
-    AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
-    Ipv6CidrBlockAssociationOutputTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
     AwsEc2TransitGatewayDetailsOutputTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
-    AwsEc2VolumeAttachmentOutputTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
-    CidrBlockAssociationOutputTypeDef,
     CidrBlockAssociationTypeDef,
-    AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef,
-    AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
-    VpcInfoCidrBlockSetDetailsOutputTypeDef,
-    VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef,
-    VpcInfoPeeringOptionsDetailsOutputTypeDef,
     VpcInfoCidrBlockSetDetailsTypeDef,
     VpcInfoIpv6CidrBlockSetDetailsTypeDef,
     VpcInfoPeeringOptionsDetailsTypeDef,
-    AwsEc2VpnConnectionRoutesDetailsOutputTypeDef,
-    AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef,
     AwsEc2VpnConnectionRoutesDetailsTypeDef,
     AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef,
     AwsEcrContainerImageDetailsOutputTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
-    AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef,
-    AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef,
     AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
     AwsEcrRepositoryLifecyclePolicyDetailsTypeDef,
-    AwsEcsClusterClusterSettingsDetailsOutputTypeDef,
     AwsEcsClusterClusterSettingsDetailsTypeDef,
-    AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
-    AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef,
     AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef,
-    AwsMountPointOutputTypeDef,
     AwsMountPointTypeDef,
-    AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef,
     AwsEcsServiceCapacityProviderStrategyDetailsTypeDef,
-    AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef,
     AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
-    AwsEcsServiceDeploymentControllerDetailsOutputTypeDef,
     AwsEcsServiceDeploymentControllerDetailsTypeDef,
-    AwsEcsServiceLoadBalancersDetailsOutputTypeDef,
-    AwsEcsServicePlacementConstraintsDetailsOutputTypeDef,
-    AwsEcsServicePlacementStrategiesDetailsOutputTypeDef,
-    AwsEcsServiceServiceRegistriesDetailsOutputTypeDef,
     AwsEcsServiceLoadBalancersDetailsTypeDef,
     AwsEcsServicePlacementConstraintsDetailsTypeDef,
     AwsEcsServicePlacementStrategiesDetailsTypeDef,
     AwsEcsServiceServiceRegistriesDetailsTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef,
-    AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef,
     AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef,
-    AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
-    AwsEcsTaskVolumeHostDetailsOutputTypeDef,
     AwsEcsTaskVolumeHostDetailsTypeDef,
     AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
     AwsEfsAccessPointPosixUserDetailsTypeDef,
-    AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef,
     AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsTypeDef,
-    AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef,
-    AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef,
-    AwsElasticBeanstalkEnvironmentTierOutputTypeDef,
     AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef,
     AwsElasticBeanstalkEnvironmentOptionSettingTypeDef,
     AwsElasticBeanstalkEnvironmentTierTypeDef,
-    AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef,
-    AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef,
-    AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef,
-    AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef,
-    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
     AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
     AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
     AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
+    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainVPCOptionsTypeDef,
-    AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
-    AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
-    AwsElbAppCookieStickinessPolicyOutputTypeDef,
     AwsElbAppCookieStickinessPolicyTypeDef,
-    AwsElbLbCookieStickinessPolicyOutputTypeDef,
     AwsElbLbCookieStickinessPolicyTypeDef,
-    AwsElbLoadBalancerAccessLogOutputTypeDef,
     AwsElbLoadBalancerAccessLogTypeDef,
-    AwsElbLoadBalancerAdditionalAttributeOutputTypeDef,
     AwsElbLoadBalancerAdditionalAttributeTypeDef,
-    AwsElbLoadBalancerConnectionDrainingOutputTypeDef,
-    AwsElbLoadBalancerConnectionSettingsOutputTypeDef,
-    AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef,
     AwsElbLoadBalancerConnectionDrainingTypeDef,
     AwsElbLoadBalancerConnectionSettingsTypeDef,
     AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
-    AwsElbLoadBalancerHealthCheckOutputTypeDef,
-    AwsElbLoadBalancerInstanceOutputTypeDef,
-    AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
-    AwsElbLoadBalancerListenerOutputTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
-    AwsElbv2LoadBalancerAttributeOutputTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
-    LoadBalancerStateOutputTypeDef,
     LoadBalancerStateTypeDef,
-    AwsEventSchemasRegistryDetailsOutputTypeDef,
     AwsEventSchemasRegistryDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef,
-    AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef,
-    AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
-    AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef,
     AwsGuardDutyDetectorFeaturesDetailsTypeDef,
-    AwsIamAccessKeySessionContextAttributesOutputTypeDef,
     AwsIamAccessKeySessionContextAttributesTypeDef,
-    AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef,
     AwsIamAccessKeySessionContextSessionIssuerTypeDef,
-    AwsIamAttachedManagedPolicyOutputTypeDef,
     AwsIamAttachedManagedPolicyTypeDef,
-    AwsIamGroupPolicyOutputTypeDef,
     AwsIamGroupPolicyTypeDef,
-    AwsIamInstanceProfileRoleOutputTypeDef,
     AwsIamInstanceProfileRoleTypeDef,
-    AwsIamPermissionsBoundaryOutputTypeDef,
     AwsIamPermissionsBoundaryTypeDef,
-    AwsIamPolicyVersionOutputTypeDef,
     AwsIamPolicyVersionTypeDef,
-    AwsIamRolePolicyOutputTypeDef,
     AwsIamRolePolicyTypeDef,
-    AwsIamUserPolicyOutputTypeDef,
     AwsIamUserPolicyTypeDef,
-    AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef,
     AwsKinesisStreamStreamEncryptionDetailsTypeDef,
-    AwsKmsKeyDetailsOutputTypeDef,
     AwsKmsKeyDetailsTypeDef,
-    AwsLambdaFunctionCodeOutputTypeDef,
     AwsLambdaFunctionCodeTypeDef,
-    AwsLambdaFunctionDeadLetterConfigOutputTypeDef,
     AwsLambdaFunctionDeadLetterConfigTypeDef,
-    AwsLambdaFunctionLayerOutputTypeDef,
-    AwsLambdaFunctionTracingConfigOutputTypeDef,
-    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionLayerTypeDef,
     AwsLambdaFunctionTracingConfigTypeDef,
+    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionVpcConfigTypeDef,
-    AwsLambdaFunctionEnvironmentErrorOutputTypeDef,
     AwsLambdaFunctionEnvironmentErrorTypeDef,
     AwsLambdaLayerVersionDetailsOutputTypeDef,
     AwsLambdaLayerVersionDetailsTypeDef,
-    AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef,
-    AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
-    AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
-    AwsRdsDbClusterAssociatedRoleOutputTypeDef,
     AwsRdsDbClusterAssociatedRoleTypeDef,
-    AwsRdsDbClusterMemberOutputTypeDef,
-    AwsRdsDbClusterOptionGroupMembershipOutputTypeDef,
-    AwsRdsDbDomainMembershipOutputTypeDef,
-    AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef,
     AwsRdsDbClusterMemberTypeDef,
     AwsRdsDbClusterOptionGroupMembershipTypeDef,
     AwsRdsDbDomainMembershipTypeDef,
     AwsRdsDbInstanceVpcSecurityGroupTypeDef,
     AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef,
     AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef,
-    AwsRdsDbInstanceAssociatedRoleOutputTypeDef,
     AwsRdsDbInstanceAssociatedRoleTypeDef,
-    AwsRdsDbInstanceEndpointOutputTypeDef,
-    AwsRdsDbOptionGroupMembershipOutputTypeDef,
-    AwsRdsDbParameterGroupOutputTypeDef,
-    AwsRdsDbProcessorFeatureOutputTypeDef,
-    AwsRdsDbStatusInfoOutputTypeDef,
     AwsRdsDbInstanceEndpointTypeDef,
     AwsRdsDbOptionGroupMembershipTypeDef,
     AwsRdsDbParameterGroupTypeDef,
     AwsRdsDbProcessorFeatureTypeDef,
     AwsRdsDbStatusInfoTypeDef,
     AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
     AwsRdsPendingCloudWatchLogsExportsTypeDef,
-    AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef,
-    AwsRdsDbSecurityGroupIpRangeOutputTypeDef,
     AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef,
     AwsRdsDbSecurityGroupIpRangeTypeDef,
-    AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef,
     AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
     AwsRdsEventSubscriptionDetailsOutputTypeDef,
     AwsRdsEventSubscriptionDetailsTypeDef,
-    AwsRedshiftClusterClusterNodeOutputTypeDef,
     AwsRedshiftClusterClusterNodeTypeDef,
-    AwsRedshiftClusterClusterParameterStatusOutputTypeDef,
     AwsRedshiftClusterClusterParameterStatusTypeDef,
-    AwsRedshiftClusterClusterSecurityGroupOutputTypeDef,
     AwsRedshiftClusterClusterSecurityGroupTypeDef,
-    AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef,
     AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
-    AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef,
     AwsRedshiftClusterDeferredMaintenanceWindowTypeDef,
-    AwsRedshiftClusterElasticIpStatusOutputTypeDef,
-    AwsRedshiftClusterEndpointOutputTypeDef,
-    AwsRedshiftClusterHsmStatusOutputTypeDef,
-    AwsRedshiftClusterIamRoleOutputTypeDef,
-    AwsRedshiftClusterLoggingStatusOutputTypeDef,
-    AwsRedshiftClusterPendingModifiedValuesOutputTypeDef,
-    AwsRedshiftClusterResizeInfoOutputTypeDef,
-    AwsRedshiftClusterRestoreStatusOutputTypeDef,
-    AwsRedshiftClusterVpcSecurityGroupOutputTypeDef,
     AwsRedshiftClusterElasticIpStatusTypeDef,
     AwsRedshiftClusterEndpointTypeDef,
     AwsRedshiftClusterHsmStatusTypeDef,
     AwsRedshiftClusterIamRoleTypeDef,
     AwsRedshiftClusterLoggingStatusTypeDef,
     AwsRedshiftClusterPendingModifiedValuesTypeDef,
     AwsRedshiftClusterResizeInfoTypeDef,
     AwsRedshiftClusterRestoreStatusTypeDef,
     AwsRedshiftClusterVpcSecurityGroupTypeDef,
-    AwsS3AccountPublicAccessBlockDetailsOutputTypeDef,
     AwsS3AccountPublicAccessBlockDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
-    AwsS3BucketBucketVersioningConfigurationOutputTypeDef,
     AwsS3BucketBucketVersioningConfigurationTypeDef,
-    AwsS3BucketLoggingConfigurationOutputTypeDef,
     AwsS3BucketLoggingConfigurationTypeDef,
-    AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
-    AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
-    AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
-    AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
-    AwsS3ObjectDetailsOutputTypeDef,
     AwsS3ObjectDetailsTypeDef,
-    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
-    AwsSecretsManagerSecretRotationRulesOutputTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
-    BooleanFilterOutputTypeDef,
-    IpFilterOutputTypeDef,
-    KeywordFilterOutputTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
-    AwsSecurityFindingIdentifierOutputTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    MalwareOutputTypeDef,
-    NoteOutputTypeDef,
-    PatchSummaryOutputTypeDef,
-    ProcessDetailsOutputTypeDef,
-    SeverityOutputTypeDef,
-    ThreatIntelIndicatorOutputTypeDef,
-    WorkflowOutputTypeDef,
     MalwareTypeDef,
     NoteTypeDef,
     PatchSummaryTypeDef,
     ProcessDetailsTypeDef,
     SeverityTypeDef,
     ThreatIntelIndicatorTypeDef,
     WorkflowTypeDef,
-    AwsSnsTopicSubscriptionOutputTypeDef,
     AwsSnsTopicSubscriptionTypeDef,
-    AwsSqsQueueDetailsOutputTypeDef,
     AwsSqsQueueDetailsTypeDef,
-    AwsSsmComplianceSummaryOutputTypeDef,
     AwsSsmComplianceSummaryTypeDef,
-    AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
-    AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
-    AwsWafRateBasedRuleMatchPredicateOutputTypeDef,
     AwsWafRateBasedRuleMatchPredicateTypeDef,
-    AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef,
     AwsWafRegionalRateBasedRuleMatchPredicateTypeDef,
-    AwsWafRegionalRulePredicateListDetailsOutputTypeDef,
     AwsWafRegionalRulePredicateListDetailsTypeDef,
-    AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
-    AwsWafRulePredicateListDetailsOutputTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
-    AwsWafRuleGroupRulesActionDetailsOutputTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
-    WafActionOutputTypeDef,
-    WafExcludedRuleOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
-    AwsWafv2CustomHttpHeaderOutputTypeDef,
     AwsWafv2CustomHttpHeaderTypeDef,
-    AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     AwsWafv2VisibilityConfigDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef,
     AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
-    AwsXrayEncryptionConfigDetailsOutputTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDeleteAutomationRulesRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     StandardsSubscriptionRequestTypeDef,
     BatchGetAutomationRulesRequestRequestTypeDef,
     BatchGetSecurityControlsRequestRequestTypeDef,
     SecurityControlTypeDef,
     UnprocessedSecurityControlTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
     StandardsControlAssociationUpdateTypeDef,
-    CellOutputTypeDef,
     CellTypeDef,
-    ClassificationStatusOutputTypeDef,
     ClassificationStatusTypeDef,
-    StatusReasonOutputTypeDef,
     StatusReasonTypeDef,
-    VolumeMountOutputTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
     ResultTypeDef,
-    DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
@@ -1107,23 +781,19 @@
     DescribeStandardsRequestRequestTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
-    FilePathsOutputTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
     FindingHistoryUpdateSourceTypeDef,
     FindingHistoryUpdateTypeDef,
-    FindingProviderSeverityOutputTypeDef,
     FindingProviderSeverityTypeDef,
-    FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef,
-    FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
@@ -1139,91 +809,69 @@
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListSecurityControlDefinitionsRequestRequestTypeDef,
     SecurityControlDefinitionTypeDef,
     ListStandardsControlAssociationsRequestRequestTypeDef,
     StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PortRangeOutputTypeDef,
     PortRangeTypeDef,
-    RangeOutputTypeDef,
-    RecordOutputTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    RecommendationOutputTypeDef,
     RecommendationTypeDef,
     RuleGroupSourceListDetailsOutputTypeDef,
     RuleGroupSourceListDetailsTypeDef,
-    RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef,
-    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
+    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsOutputTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsOutputTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
-    SoftwarePackageOutputTypeDef,
     SoftwarePackageTypeDef,
     StandardsManagedByTypeDef,
-    StandardsControlAssociationIdOutputTypeDef,
-    StandardsControlAssociationUpdateOutputTypeDef,
     StandardsStatusReasonTypeDef,
-    StatelessCustomPublishMetricActionDimensionOutputTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
-    VulnerabilityVendorOutputTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
-    ActionRemoteIpDetailsOutputTypeDef,
     ActionRemoteIpDetailsTypeDef,
     CvssOutputTypeDef,
     CvssTypeDef,
-    AssociationSetDetailsOutputTypeDef,
     AssociationSetDetailsTypeDef,
     AutomationRulesFindingFieldsUpdateOutputTypeDef,
     AutomationRulesFindingFieldsUpdateTypeDef,
-    AwsAmazonMqBrokerLogsDetailsOutputTypeDef,
     AwsAmazonMqBrokerLogsDetailsTypeDef,
     AwsApiGatewayRestApiDetailsOutputTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
     AwsApiGatewayStageDetailsOutputTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
     AwsApiGatewayV2ApiDetailsOutputTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
     AwsApiGatewayV2StageDetailsOutputTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
-    AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
-    AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
     AwsBackupBackupVaultDetailsOutputTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
-    AwsBackupRecoveryPointDetailsOutputTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
     AwsCloudFormationStackDetailsOutputTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsTypeDef,
@@ -1231,35 +879,29 @@
     AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
     AwsCloudWatchAlarmDetailsOutputTypeDef,
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentOutputTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
-    AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
-    AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsOutputTypeDef,
     AwsEc2InstanceDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
-    AwsEc2NetworkAclEntryOutputTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsOutputTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionOutputTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsOutputTypeDef,
     AwsEc2SubnetDetailsTypeDef,
@@ -1269,136 +911,109 @@
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
     AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsDetailsTypeDef,
-    AwsEcrRepositoryDetailsOutputTypeDef,
     AwsEcrRepositoryDetailsTypeDef,
-    AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
     AwsEcsContainerDetailsOutputTypeDef,
     AwsEcsContainerDetailsTypeDef,
-    AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef,
     AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
-    AwsEcsTaskVolumeDetailsOutputTypeDef,
     AwsEcsTaskVolumeDetailsTypeDef,
-    AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef,
     AwsEfsAccessPointRootDirectoryDetailsTypeDef,
     AwsEksClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingDetailsTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
-    AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
-    AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
     AwsElbLoadBalancerPoliciesOutputTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
     AwsElbLoadBalancerAttributesOutputTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
     AwsElbLoadBalancerListenerDescriptionOutputTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
     AwsElbv2LoadBalancerDetailsOutputTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
-    AwsIamAccessKeySessionContextOutputTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
     AwsIamGroupDetailsOutputTypeDef,
     AwsIamGroupDetailsTypeDef,
     AwsIamInstanceProfileOutputTypeDef,
     AwsIamInstanceProfileTypeDef,
     AwsIamPolicyDetailsOutputTypeDef,
     AwsIamPolicyDetailsTypeDef,
     AwsIamUserDetailsOutputTypeDef,
     AwsIamUserDetailsTypeDef,
-    AwsKinesisStreamDetailsOutputTypeDef,
     AwsKinesisStreamDetailsTypeDef,
     AwsLambdaFunctionEnvironmentOutputTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
     AwsNetworkFirewallFirewallDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallDetailsTypeDef,
-    AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
-    AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
     AwsRdsDbClusterDetailsOutputTypeDef,
     AwsRdsDbClusterDetailsTypeDef,
     AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
     AwsRdsDbClusterSnapshotDetailsTypeDef,
     AwsRdsDbSnapshotDetailsOutputTypeDef,
     AwsRdsDbSnapshotDetailsTypeDef,
     AwsRdsDbPendingModifiedValuesOutputTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
     AwsRdsDbSecurityGroupDetailsOutputTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
-    AwsRdsDbSubnetGroupSubnetOutputTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupOutputTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
-    AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
-    AwsS3BucketServerSideEncryptionRuleOutputTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
     AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
-    AwsSecretsManagerSecretDetailsOutputTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
-    BatchUpdateFindingsUnprocessedFindingTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
+    BatchUpdateFindingsUnprocessedFindingTypeDef,
     GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
-    AwsSsmPatchOutputTypeDef,
     AwsSsmPatchTypeDef,
-    AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsOutputTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
-    AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsOutputTypeDef,
     AwsWafRuleDetailsTypeDef,
-    AwsWafRuleGroupRulesDetailsOutputTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleOutputTypeDef,
     AwsWafWebAclRuleTypeDef,
     AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
-    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomResponseDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef,
     AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
     CreateActionTargetResponseTypeDef,
     CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
@@ -1414,26 +1029,27 @@
     ListTagsForResourceResponseTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceOutputTypeDef,
     ComplianceTypeDef,
     ContainerDetailsOutputTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
-    DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
@@ -1457,51 +1073,43 @@
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
-    NetworkOutputTypeDef,
     NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
-    PageOutputTypeDef,
     PageTypeDef,
-    RemediationOutputTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesOutputTypeDef,
     RuleGroupVariablesTypeDef,
     StandardTypeDef,
-    UnprocessedStandardsControlAssociationTypeDef,
-    UnprocessedStandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionOutputTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionOutputTypeDef,
-    NetworkConnectionActionOutputTypeDef,
-    PortProbeDetailOutputTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityOutputTypeDef,
     VulnerabilityTypeDef,
     AwsEc2RouteTableDetailsOutputTypeDef,
     AwsEc2RouteTableDetailsTypeDef,
     AutomationRulesActionOutputTypeDef,
     AutomationRulesActionTypeDef,
     AwsAmazonMqBrokerDetailsOutputTypeDef,
     AwsAmazonMqBrokerDetailsTypeDef,
     AwsAppSyncGraphQlApiDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
@@ -1521,15 +1129,14 @@
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsOutputTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsOutputTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
-    AwsEcsClusterConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsOutputTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
@@ -1539,17 +1146,15 @@
     AwsEfsAccessPointDetailsTypeDef,
     AwsEksClusterDetailsOutputTypeDef,
     AwsEksClusterDetailsTypeDef,
     AwsElasticsearchDomainDetailsOutputTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
     AwsElbLoadBalancerDetailsOutputTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
-    AwsIamAccessKeyDetailsOutputTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
     AwsIamRoleDetailsOutputTypeDef,
     AwsIamRoleDetailsTypeDef,
     AwsLambdaFunctionDetailsOutputTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     AwsOpenSearchServiceDomainDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
@@ -1557,64 +1162,61 @@
     AwsRdsDbSubnetGroupTypeDef,
     AwsRedshiftClusterDetailsOutputTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
-    AwsS3BucketObjectLockConfigurationOutputTypeDef,
     AwsS3BucketObjectLockConfigurationTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
     AwsS3BucketWebsiteConfigurationOutputTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
-    AwsSsmPatchComplianceDetailsOutputTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsOutputTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsOutputTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsOutputTypeDef,
     AwsWafWebAclDetailsTypeDef,
     AwsWafv2ActionAllowDetailsOutputTypeDef,
     AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
     AwsWafv2RulesActionCountDetailsOutputTypeDef,
-    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionAllowDetailsTypeDef,
     AwsWafv2RulesActionCaptchaDetailsTypeDef,
     AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionBlockDetailsTypeDef,
+    BatchGetStandardsControlAssociationsResponseTypeDef,
+    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     AutomationRulesFindingFiltersOutputTypeDef,
-    AwsSecurityFindingFiltersOutputTypeDef,
     AutomationRulesFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderOutputTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesOutputTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
     DescribeStandardsResponseTypeDef,
-    BatchGetStandardsControlAssociationsResponseTypeDef,
-    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
-    AwsAthenaWorkGroupDetailsOutputTypeDef,
     AwsAthenaWorkGroupDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
@@ -1626,32 +1228,31 @@
     AwsDynamoDbTableDetailsTypeDef,
     AwsEc2LaunchTemplateDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsOutputTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsOutputTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
     AwsRdsDbInstanceDetailsOutputTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailOutputTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
     AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
     AwsWafv2RulesActionDetailsOutputTypeDef,
     AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    InsightTypeDef,
     CreateAutomationRuleRequestRequestTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
+    InsightTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
@@ -1676,16 +1277,16 @@
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationOutputTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
     AwsWafv2RulesDetailsOutputTypeDef,
     AwsWafv2RulesDetailsTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
-    GetInsightsResponseTypeDef,
     BatchUpdateAutomationRulesRequestRequestTypeDef,
+    GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultOutputTypeDef,
     SensitiveDataResultOutputTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsOutputTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef,
     FirewallPolicyDetailsTypeDef,
```

### Comparing `mypy-boto3-securityhub-1.28.12/README.md` & `mypy-boto3-securityhub-1.28.15/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-securityhub
+Version: 1.28.15
+Summary: Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 securityhub type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-securityhub"></a>
 
 # mypy-boto3-securityhub
 
 [![PyPI - mypy-boto3-securityhub](https://img.shields.io/pypi/v/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -386,682 +418,388 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    ActionLocalIpDetailsOutputTypeDef,
     ActionLocalIpDetailsTypeDef,
-    ActionLocalPortDetailsOutputTypeDef,
     ActionLocalPortDetailsTypeDef,
-    DnsRequestActionOutputTypeDef,
-    CityOutputTypeDef,
-    CountryOutputTypeDef,
-    GeoLocationOutputTypeDef,
-    IpOrganizationDetailsOutputTypeDef,
+    DnsRequestActionTypeDef,
     CityTypeDef,
     CountryTypeDef,
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
-    ActionRemotePortDetailsOutputTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
-    DnsRequestActionTypeDef,
-    AdjustmentOutputTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
-    AssociatedStandardOutputTypeDef,
     AssociatedStandardTypeDef,
-    AssociationStateDetailsOutputTypeDef,
     AssociationStateDetailsTypeDef,
-    NoteUpdateOutputTypeDef,
-    RelatedFindingOutputTypeDef,
-    SeverityUpdateOutputTypeDef,
-    WorkflowUpdateOutputTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
-    MapFilterOutputTypeDef,
-    NumberFilterOutputTypeDef,
-    StringFilterOutputTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
     AutomationRulesMetadataTypeDef,
-    AvailabilityZoneOutputTypeDef,
     AvailabilityZoneTypeDef,
-    AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
-    AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef,
-    AwsAmazonMqBrokerUsersDetailsOutputTypeDef,
     AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
     AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
     AwsAmazonMqBrokerUsersDetailsTypeDef,
-    AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
     AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
-    AwsApiCallActionDomainDetailsOutputTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
-    AwsApiGatewayAccessLogSettingsOutputTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsOutputTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationOutputTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
-    AwsApiGatewayMethodSettingsOutputTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationOutputTypeDef,
     AwsCorsConfigurationTypeDef,
-    AwsApiGatewayV2RouteSettingsOutputTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
-    AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
-    AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
-    AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
-    AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef,
-    AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef,
-    AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
     AwsBackupBackupPlanLifecycleDetailsTypeDef,
     AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
     AwsBackupBackupVaultNotificationsDetailsTypeDef,
-    AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef,
     AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef,
-    AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef,
     AwsBackupRecoveryPointCreatedByDetailsTypeDef,
-    AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef,
     AwsBackupRecoveryPointLifecycleDetailsTypeDef,
-    AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef,
-    AwsCertificateManagerCertificateKeyUsageOutputTypeDef,
-    AwsCertificateManagerCertificateOptionsOutputTypeDef,
     AwsCertificateManagerCertificateExtendedKeyUsageTypeDef,
     AwsCertificateManagerCertificateKeyUsageTypeDef,
     AwsCertificateManagerCertificateOptionsTypeDef,
-    AwsCertificateManagerCertificateResourceRecordOutputTypeDef,
     AwsCertificateManagerCertificateResourceRecordTypeDef,
-    AwsCloudFormationStackDriftInformationDetailsOutputTypeDef,
-    AwsCloudFormationStackOutputsDetailsOutputTypeDef,
     AwsCloudFormationStackDriftInformationDetailsTypeDef,
     AwsCloudFormationStackOutputsDetailsTypeDef,
-    AwsCloudFrontDistributionCacheBehaviorOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorTypeDef,
-    AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef,
     AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
-    AwsCloudFrontDistributionLoggingOutputTypeDef,
-    AwsCloudFrontDistributionViewerCertificateOutputTypeDef,
     AwsCloudFrontDistributionLoggingTypeDef,
     AwsCloudFrontDistributionViewerCertificateTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
-    AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef,
     AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
-    AwsCloudTrailTrailDetailsOutputTypeDef,
     AwsCloudTrailTrailDetailsTypeDef,
-    AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef,
     AwsCloudWatchAlarmDimensionsDetailsTypeDef,
-    AwsCodeBuildProjectArtifactsDetailsOutputTypeDef,
     AwsCodeBuildProjectArtifactsDetailsTypeDef,
-    AwsCodeBuildProjectSourceOutputTypeDef,
-    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectSourceTypeDef,
+    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectVpcConfigTypeDef,
-    AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef,
     AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef,
-    AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef,
     AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
-    AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
-    AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
-    AwsDynamoDbTableAttributeDefinitionOutputTypeDef,
     AwsDynamoDbTableAttributeDefinitionTypeDef,
-    AwsDynamoDbTableBillingModeSummaryOutputTypeDef,
     AwsDynamoDbTableBillingModeSummaryTypeDef,
-    AwsDynamoDbTableKeySchemaOutputTypeDef,
-    AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
-    AwsDynamoDbTableRestoreSummaryOutputTypeDef,
-    AwsDynamoDbTableSseDescriptionOutputTypeDef,
-    AwsDynamoDbTableStreamSpecificationOutputTypeDef,
     AwsDynamoDbTableKeySchemaTypeDef,
     AwsDynamoDbTableProvisionedThroughputTypeDef,
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionOutputTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
-    AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
-    AwsEc2EipDetailsOutputTypeDef,
     AwsEc2EipDetailsTypeDef,
-    AwsEc2InstanceMetadataOptionsOutputTypeDef,
-    AwsEc2InstanceMonitoringDetailsOutputTypeDef,
-    AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
     AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
     AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
     AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
-    AwsEc2NetworkAclAssociationOutputTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
-    IcmpTypeCodeOutputTypeDef,
-    PortRangeFromToOutputTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
-    AwsEc2NetworkInterfaceAttachmentOutputTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
-    AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef,
-    AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef,
-    AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
-    PropagatingVgwSetDetailsOutputTypeDef,
-    RouteSetDetailsOutputTypeDef,
     PropagatingVgwSetDetailsTypeDef,
     RouteSetDetailsTypeDef,
-    AwsEc2SecurityGroupIpRangeOutputTypeDef,
-    AwsEc2SecurityGroupIpv6RangeOutputTypeDef,
-    AwsEc2SecurityGroupPrefixListIdOutputTypeDef,
-    AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
-    Ipv6CidrBlockAssociationOutputTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
     AwsEc2TransitGatewayDetailsOutputTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
-    AwsEc2VolumeAttachmentOutputTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
-    CidrBlockAssociationOutputTypeDef,
     CidrBlockAssociationTypeDef,
-    AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef,
-    AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
-    VpcInfoCidrBlockSetDetailsOutputTypeDef,
-    VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef,
-    VpcInfoPeeringOptionsDetailsOutputTypeDef,
     VpcInfoCidrBlockSetDetailsTypeDef,
     VpcInfoIpv6CidrBlockSetDetailsTypeDef,
     VpcInfoPeeringOptionsDetailsTypeDef,
-    AwsEc2VpnConnectionRoutesDetailsOutputTypeDef,
-    AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef,
     AwsEc2VpnConnectionRoutesDetailsTypeDef,
     AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef,
     AwsEcrContainerImageDetailsOutputTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
-    AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef,
-    AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef,
     AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
     AwsEcrRepositoryLifecyclePolicyDetailsTypeDef,
-    AwsEcsClusterClusterSettingsDetailsOutputTypeDef,
     AwsEcsClusterClusterSettingsDetailsTypeDef,
-    AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
-    AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef,
     AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef,
-    AwsMountPointOutputTypeDef,
     AwsMountPointTypeDef,
-    AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef,
     AwsEcsServiceCapacityProviderStrategyDetailsTypeDef,
-    AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef,
     AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
-    AwsEcsServiceDeploymentControllerDetailsOutputTypeDef,
     AwsEcsServiceDeploymentControllerDetailsTypeDef,
-    AwsEcsServiceLoadBalancersDetailsOutputTypeDef,
-    AwsEcsServicePlacementConstraintsDetailsOutputTypeDef,
-    AwsEcsServicePlacementStrategiesDetailsOutputTypeDef,
-    AwsEcsServiceServiceRegistriesDetailsOutputTypeDef,
     AwsEcsServiceLoadBalancersDetailsTypeDef,
     AwsEcsServicePlacementConstraintsDetailsTypeDef,
     AwsEcsServicePlacementStrategiesDetailsTypeDef,
     AwsEcsServiceServiceRegistriesDetailsTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef,
-    AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef,
     AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef,
-    AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
-    AwsEcsTaskVolumeHostDetailsOutputTypeDef,
     AwsEcsTaskVolumeHostDetailsTypeDef,
     AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
     AwsEfsAccessPointPosixUserDetailsTypeDef,
-    AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef,
     AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsTypeDef,
-    AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef,
-    AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef,
-    AwsElasticBeanstalkEnvironmentTierOutputTypeDef,
     AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef,
     AwsElasticBeanstalkEnvironmentOptionSettingTypeDef,
     AwsElasticBeanstalkEnvironmentTierTypeDef,
-    AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef,
-    AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef,
-    AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef,
-    AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef,
-    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
     AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
     AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
     AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
+    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainVPCOptionsTypeDef,
-    AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
-    AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
-    AwsElbAppCookieStickinessPolicyOutputTypeDef,
     AwsElbAppCookieStickinessPolicyTypeDef,
-    AwsElbLbCookieStickinessPolicyOutputTypeDef,
     AwsElbLbCookieStickinessPolicyTypeDef,
-    AwsElbLoadBalancerAccessLogOutputTypeDef,
     AwsElbLoadBalancerAccessLogTypeDef,
-    AwsElbLoadBalancerAdditionalAttributeOutputTypeDef,
     AwsElbLoadBalancerAdditionalAttributeTypeDef,
-    AwsElbLoadBalancerConnectionDrainingOutputTypeDef,
-    AwsElbLoadBalancerConnectionSettingsOutputTypeDef,
-    AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef,
     AwsElbLoadBalancerConnectionDrainingTypeDef,
     AwsElbLoadBalancerConnectionSettingsTypeDef,
     AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
-    AwsElbLoadBalancerHealthCheckOutputTypeDef,
-    AwsElbLoadBalancerInstanceOutputTypeDef,
-    AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
-    AwsElbLoadBalancerListenerOutputTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
-    AwsElbv2LoadBalancerAttributeOutputTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
-    LoadBalancerStateOutputTypeDef,
     LoadBalancerStateTypeDef,
-    AwsEventSchemasRegistryDetailsOutputTypeDef,
     AwsEventSchemasRegistryDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef,
-    AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef,
-    AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
-    AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef,
     AwsGuardDutyDetectorFeaturesDetailsTypeDef,
-    AwsIamAccessKeySessionContextAttributesOutputTypeDef,
     AwsIamAccessKeySessionContextAttributesTypeDef,
-    AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef,
     AwsIamAccessKeySessionContextSessionIssuerTypeDef,
-    AwsIamAttachedManagedPolicyOutputTypeDef,
     AwsIamAttachedManagedPolicyTypeDef,
-    AwsIamGroupPolicyOutputTypeDef,
     AwsIamGroupPolicyTypeDef,
-    AwsIamInstanceProfileRoleOutputTypeDef,
     AwsIamInstanceProfileRoleTypeDef,
-    AwsIamPermissionsBoundaryOutputTypeDef,
     AwsIamPermissionsBoundaryTypeDef,
-    AwsIamPolicyVersionOutputTypeDef,
     AwsIamPolicyVersionTypeDef,
-    AwsIamRolePolicyOutputTypeDef,
     AwsIamRolePolicyTypeDef,
-    AwsIamUserPolicyOutputTypeDef,
     AwsIamUserPolicyTypeDef,
-    AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef,
     AwsKinesisStreamStreamEncryptionDetailsTypeDef,
-    AwsKmsKeyDetailsOutputTypeDef,
     AwsKmsKeyDetailsTypeDef,
-    AwsLambdaFunctionCodeOutputTypeDef,
     AwsLambdaFunctionCodeTypeDef,
-    AwsLambdaFunctionDeadLetterConfigOutputTypeDef,
     AwsLambdaFunctionDeadLetterConfigTypeDef,
-    AwsLambdaFunctionLayerOutputTypeDef,
-    AwsLambdaFunctionTracingConfigOutputTypeDef,
-    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionLayerTypeDef,
     AwsLambdaFunctionTracingConfigTypeDef,
+    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionVpcConfigTypeDef,
-    AwsLambdaFunctionEnvironmentErrorOutputTypeDef,
     AwsLambdaFunctionEnvironmentErrorTypeDef,
     AwsLambdaLayerVersionDetailsOutputTypeDef,
     AwsLambdaLayerVersionDetailsTypeDef,
-    AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef,
-    AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
-    AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
-    AwsRdsDbClusterAssociatedRoleOutputTypeDef,
     AwsRdsDbClusterAssociatedRoleTypeDef,
-    AwsRdsDbClusterMemberOutputTypeDef,
-    AwsRdsDbClusterOptionGroupMembershipOutputTypeDef,
-    AwsRdsDbDomainMembershipOutputTypeDef,
-    AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef,
     AwsRdsDbClusterMemberTypeDef,
     AwsRdsDbClusterOptionGroupMembershipTypeDef,
     AwsRdsDbDomainMembershipTypeDef,
     AwsRdsDbInstanceVpcSecurityGroupTypeDef,
     AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef,
     AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef,
-    AwsRdsDbInstanceAssociatedRoleOutputTypeDef,
     AwsRdsDbInstanceAssociatedRoleTypeDef,
-    AwsRdsDbInstanceEndpointOutputTypeDef,
-    AwsRdsDbOptionGroupMembershipOutputTypeDef,
-    AwsRdsDbParameterGroupOutputTypeDef,
-    AwsRdsDbProcessorFeatureOutputTypeDef,
-    AwsRdsDbStatusInfoOutputTypeDef,
     AwsRdsDbInstanceEndpointTypeDef,
     AwsRdsDbOptionGroupMembershipTypeDef,
     AwsRdsDbParameterGroupTypeDef,
     AwsRdsDbProcessorFeatureTypeDef,
     AwsRdsDbStatusInfoTypeDef,
     AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
     AwsRdsPendingCloudWatchLogsExportsTypeDef,
-    AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef,
-    AwsRdsDbSecurityGroupIpRangeOutputTypeDef,
     AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef,
     AwsRdsDbSecurityGroupIpRangeTypeDef,
-    AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef,
     AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
     AwsRdsEventSubscriptionDetailsOutputTypeDef,
     AwsRdsEventSubscriptionDetailsTypeDef,
-    AwsRedshiftClusterClusterNodeOutputTypeDef,
     AwsRedshiftClusterClusterNodeTypeDef,
-    AwsRedshiftClusterClusterParameterStatusOutputTypeDef,
     AwsRedshiftClusterClusterParameterStatusTypeDef,
-    AwsRedshiftClusterClusterSecurityGroupOutputTypeDef,
     AwsRedshiftClusterClusterSecurityGroupTypeDef,
-    AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef,
     AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
-    AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef,
     AwsRedshiftClusterDeferredMaintenanceWindowTypeDef,
-    AwsRedshiftClusterElasticIpStatusOutputTypeDef,
-    AwsRedshiftClusterEndpointOutputTypeDef,
-    AwsRedshiftClusterHsmStatusOutputTypeDef,
-    AwsRedshiftClusterIamRoleOutputTypeDef,
-    AwsRedshiftClusterLoggingStatusOutputTypeDef,
-    AwsRedshiftClusterPendingModifiedValuesOutputTypeDef,
-    AwsRedshiftClusterResizeInfoOutputTypeDef,
-    AwsRedshiftClusterRestoreStatusOutputTypeDef,
-    AwsRedshiftClusterVpcSecurityGroupOutputTypeDef,
     AwsRedshiftClusterElasticIpStatusTypeDef,
     AwsRedshiftClusterEndpointTypeDef,
     AwsRedshiftClusterHsmStatusTypeDef,
     AwsRedshiftClusterIamRoleTypeDef,
     AwsRedshiftClusterLoggingStatusTypeDef,
     AwsRedshiftClusterPendingModifiedValuesTypeDef,
     AwsRedshiftClusterResizeInfoTypeDef,
     AwsRedshiftClusterRestoreStatusTypeDef,
     AwsRedshiftClusterVpcSecurityGroupTypeDef,
-    AwsS3AccountPublicAccessBlockDetailsOutputTypeDef,
     AwsS3AccountPublicAccessBlockDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
-    AwsS3BucketBucketVersioningConfigurationOutputTypeDef,
     AwsS3BucketBucketVersioningConfigurationTypeDef,
-    AwsS3BucketLoggingConfigurationOutputTypeDef,
     AwsS3BucketLoggingConfigurationTypeDef,
-    AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
-    AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
-    AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
-    AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
-    AwsS3ObjectDetailsOutputTypeDef,
     AwsS3ObjectDetailsTypeDef,
-    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
-    AwsSecretsManagerSecretRotationRulesOutputTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
-    BooleanFilterOutputTypeDef,
-    IpFilterOutputTypeDef,
-    KeywordFilterOutputTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
-    AwsSecurityFindingIdentifierOutputTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    MalwareOutputTypeDef,
-    NoteOutputTypeDef,
-    PatchSummaryOutputTypeDef,
-    ProcessDetailsOutputTypeDef,
-    SeverityOutputTypeDef,
-    ThreatIntelIndicatorOutputTypeDef,
-    WorkflowOutputTypeDef,
     MalwareTypeDef,
     NoteTypeDef,
     PatchSummaryTypeDef,
     ProcessDetailsTypeDef,
     SeverityTypeDef,
     ThreatIntelIndicatorTypeDef,
     WorkflowTypeDef,
-    AwsSnsTopicSubscriptionOutputTypeDef,
     AwsSnsTopicSubscriptionTypeDef,
-    AwsSqsQueueDetailsOutputTypeDef,
     AwsSqsQueueDetailsTypeDef,
-    AwsSsmComplianceSummaryOutputTypeDef,
     AwsSsmComplianceSummaryTypeDef,
-    AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
-    AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
-    AwsWafRateBasedRuleMatchPredicateOutputTypeDef,
     AwsWafRateBasedRuleMatchPredicateTypeDef,
-    AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef,
     AwsWafRegionalRateBasedRuleMatchPredicateTypeDef,
-    AwsWafRegionalRulePredicateListDetailsOutputTypeDef,
     AwsWafRegionalRulePredicateListDetailsTypeDef,
-    AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
-    AwsWafRulePredicateListDetailsOutputTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
-    AwsWafRuleGroupRulesActionDetailsOutputTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
-    WafActionOutputTypeDef,
-    WafExcludedRuleOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
-    AwsWafv2CustomHttpHeaderOutputTypeDef,
     AwsWafv2CustomHttpHeaderTypeDef,
-    AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     AwsWafv2VisibilityConfigDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef,
     AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
-    AwsXrayEncryptionConfigDetailsOutputTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDeleteAutomationRulesRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     StandardsSubscriptionRequestTypeDef,
     BatchGetAutomationRulesRequestRequestTypeDef,
     BatchGetSecurityControlsRequestRequestTypeDef,
     SecurityControlTypeDef,
     UnprocessedSecurityControlTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
     StandardsControlAssociationUpdateTypeDef,
-    CellOutputTypeDef,
     CellTypeDef,
-    ClassificationStatusOutputTypeDef,
     ClassificationStatusTypeDef,
-    StatusReasonOutputTypeDef,
     StatusReasonTypeDef,
-    VolumeMountOutputTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
     ResultTypeDef,
-    DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
@@ -1075,23 +813,19 @@
     DescribeStandardsRequestRequestTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
-    FilePathsOutputTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
     FindingHistoryUpdateSourceTypeDef,
     FindingHistoryUpdateTypeDef,
-    FindingProviderSeverityOutputTypeDef,
     FindingProviderSeverityTypeDef,
-    FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef,
-    FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
@@ -1107,91 +841,69 @@
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListSecurityControlDefinitionsRequestRequestTypeDef,
     SecurityControlDefinitionTypeDef,
     ListStandardsControlAssociationsRequestRequestTypeDef,
     StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PortRangeOutputTypeDef,
     PortRangeTypeDef,
-    RangeOutputTypeDef,
-    RecordOutputTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    RecommendationOutputTypeDef,
     RecommendationTypeDef,
     RuleGroupSourceListDetailsOutputTypeDef,
     RuleGroupSourceListDetailsTypeDef,
-    RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef,
-    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
+    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsOutputTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsOutputTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
-    SoftwarePackageOutputTypeDef,
     SoftwarePackageTypeDef,
     StandardsManagedByTypeDef,
-    StandardsControlAssociationIdOutputTypeDef,
-    StandardsControlAssociationUpdateOutputTypeDef,
     StandardsStatusReasonTypeDef,
-    StatelessCustomPublishMetricActionDimensionOutputTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
-    VulnerabilityVendorOutputTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
-    ActionRemoteIpDetailsOutputTypeDef,
     ActionRemoteIpDetailsTypeDef,
     CvssOutputTypeDef,
     CvssTypeDef,
-    AssociationSetDetailsOutputTypeDef,
     AssociationSetDetailsTypeDef,
     AutomationRulesFindingFieldsUpdateOutputTypeDef,
     AutomationRulesFindingFieldsUpdateTypeDef,
-    AwsAmazonMqBrokerLogsDetailsOutputTypeDef,
     AwsAmazonMqBrokerLogsDetailsTypeDef,
     AwsApiGatewayRestApiDetailsOutputTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
     AwsApiGatewayStageDetailsOutputTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
     AwsApiGatewayV2ApiDetailsOutputTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
     AwsApiGatewayV2StageDetailsOutputTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
-    AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
-    AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
     AwsBackupBackupVaultDetailsOutputTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
-    AwsBackupRecoveryPointDetailsOutputTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
     AwsCloudFormationStackDetailsOutputTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsTypeDef,
@@ -1199,35 +911,29 @@
     AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
     AwsCloudWatchAlarmDetailsOutputTypeDef,
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentOutputTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
-    AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
-    AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsOutputTypeDef,
     AwsEc2InstanceDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
-    AwsEc2NetworkAclEntryOutputTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsOutputTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionOutputTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsOutputTypeDef,
     AwsEc2SubnetDetailsTypeDef,
@@ -1237,136 +943,109 @@
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
     AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsDetailsTypeDef,
-    AwsEcrRepositoryDetailsOutputTypeDef,
     AwsEcrRepositoryDetailsTypeDef,
-    AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
     AwsEcsContainerDetailsOutputTypeDef,
     AwsEcsContainerDetailsTypeDef,
-    AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef,
     AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
-    AwsEcsTaskVolumeDetailsOutputTypeDef,
     AwsEcsTaskVolumeDetailsTypeDef,
-    AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef,
     AwsEfsAccessPointRootDirectoryDetailsTypeDef,
     AwsEksClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingDetailsTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
-    AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
-    AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
     AwsElbLoadBalancerPoliciesOutputTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
     AwsElbLoadBalancerAttributesOutputTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
     AwsElbLoadBalancerListenerDescriptionOutputTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
     AwsElbv2LoadBalancerDetailsOutputTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
-    AwsIamAccessKeySessionContextOutputTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
     AwsIamGroupDetailsOutputTypeDef,
     AwsIamGroupDetailsTypeDef,
     AwsIamInstanceProfileOutputTypeDef,
     AwsIamInstanceProfileTypeDef,
     AwsIamPolicyDetailsOutputTypeDef,
     AwsIamPolicyDetailsTypeDef,
     AwsIamUserDetailsOutputTypeDef,
     AwsIamUserDetailsTypeDef,
-    AwsKinesisStreamDetailsOutputTypeDef,
     AwsKinesisStreamDetailsTypeDef,
     AwsLambdaFunctionEnvironmentOutputTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
     AwsNetworkFirewallFirewallDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallDetailsTypeDef,
-    AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
-    AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
     AwsRdsDbClusterDetailsOutputTypeDef,
     AwsRdsDbClusterDetailsTypeDef,
     AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
     AwsRdsDbClusterSnapshotDetailsTypeDef,
     AwsRdsDbSnapshotDetailsOutputTypeDef,
     AwsRdsDbSnapshotDetailsTypeDef,
     AwsRdsDbPendingModifiedValuesOutputTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
     AwsRdsDbSecurityGroupDetailsOutputTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
-    AwsRdsDbSubnetGroupSubnetOutputTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupOutputTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
-    AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
-    AwsS3BucketServerSideEncryptionRuleOutputTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
     AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
-    AwsSecretsManagerSecretDetailsOutputTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
-    BatchUpdateFindingsUnprocessedFindingTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
+    BatchUpdateFindingsUnprocessedFindingTypeDef,
     GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
-    AwsSsmPatchOutputTypeDef,
     AwsSsmPatchTypeDef,
-    AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsOutputTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
-    AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsOutputTypeDef,
     AwsWafRuleDetailsTypeDef,
-    AwsWafRuleGroupRulesDetailsOutputTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleOutputTypeDef,
     AwsWafWebAclRuleTypeDef,
     AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
-    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomResponseDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef,
     AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
     CreateActionTargetResponseTypeDef,
     CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
@@ -1382,26 +1061,27 @@
     ListTagsForResourceResponseTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceOutputTypeDef,
     ComplianceTypeDef,
     ContainerDetailsOutputTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
-    DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
@@ -1425,51 +1105,43 @@
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
-    NetworkOutputTypeDef,
     NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
-    PageOutputTypeDef,
     PageTypeDef,
-    RemediationOutputTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesOutputTypeDef,
     RuleGroupVariablesTypeDef,
     StandardTypeDef,
-    UnprocessedStandardsControlAssociationTypeDef,
-    UnprocessedStandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionOutputTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionOutputTypeDef,
-    NetworkConnectionActionOutputTypeDef,
-    PortProbeDetailOutputTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityOutputTypeDef,
     VulnerabilityTypeDef,
     AwsEc2RouteTableDetailsOutputTypeDef,
     AwsEc2RouteTableDetailsTypeDef,
     AutomationRulesActionOutputTypeDef,
     AutomationRulesActionTypeDef,
     AwsAmazonMqBrokerDetailsOutputTypeDef,
     AwsAmazonMqBrokerDetailsTypeDef,
     AwsAppSyncGraphQlApiDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
@@ -1489,15 +1161,14 @@
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsOutputTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsOutputTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
-    AwsEcsClusterConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsOutputTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
@@ -1507,17 +1178,15 @@
     AwsEfsAccessPointDetailsTypeDef,
     AwsEksClusterDetailsOutputTypeDef,
     AwsEksClusterDetailsTypeDef,
     AwsElasticsearchDomainDetailsOutputTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
     AwsElbLoadBalancerDetailsOutputTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
-    AwsIamAccessKeyDetailsOutputTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
     AwsIamRoleDetailsOutputTypeDef,
     AwsIamRoleDetailsTypeDef,
     AwsLambdaFunctionDetailsOutputTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     AwsOpenSearchServiceDomainDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
@@ -1525,64 +1194,61 @@
     AwsRdsDbSubnetGroupTypeDef,
     AwsRedshiftClusterDetailsOutputTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
-    AwsS3BucketObjectLockConfigurationOutputTypeDef,
     AwsS3BucketObjectLockConfigurationTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
     AwsS3BucketWebsiteConfigurationOutputTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
-    AwsSsmPatchComplianceDetailsOutputTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsOutputTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsOutputTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsOutputTypeDef,
     AwsWafWebAclDetailsTypeDef,
     AwsWafv2ActionAllowDetailsOutputTypeDef,
     AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
     AwsWafv2RulesActionCountDetailsOutputTypeDef,
-    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionAllowDetailsTypeDef,
     AwsWafv2RulesActionCaptchaDetailsTypeDef,
     AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionBlockDetailsTypeDef,
+    BatchGetStandardsControlAssociationsResponseTypeDef,
+    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     AutomationRulesFindingFiltersOutputTypeDef,
-    AwsSecurityFindingFiltersOutputTypeDef,
     AutomationRulesFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderOutputTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesOutputTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
     DescribeStandardsResponseTypeDef,
-    BatchGetStandardsControlAssociationsResponseTypeDef,
-    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
-    AwsAthenaWorkGroupDetailsOutputTypeDef,
     AwsAthenaWorkGroupDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
@@ -1594,32 +1260,31 @@
     AwsDynamoDbTableDetailsTypeDef,
     AwsEc2LaunchTemplateDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsOutputTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsOutputTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
     AwsRdsDbInstanceDetailsOutputTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailOutputTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
     AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
     AwsWafv2RulesActionDetailsOutputTypeDef,
     AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    InsightTypeDef,
     CreateAutomationRuleRequestRequestTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
+    InsightTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
@@ -1644,16 +1309,16 @@
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationOutputTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
     AwsWafv2RulesDetailsOutputTypeDef,
     AwsWafv2RulesDetailsTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
-    GetInsightsResponseTypeDef,
     BatchUpdateAutomationRulesRequestRequestTypeDef,
+    GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultOutputTypeDef,
     SensitiveDataResultOutputTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsOutputTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef,
     FirewallPolicyDetailsTypeDef,
```

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__init__.py` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__init__.pyi` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/__main__.py` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SecurityHub 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SecurityHub 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub\nOther"
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

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/client.py` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/client.pyi` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/literals.py` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/literals.pyi` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/paginator.py` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/paginator.pyi` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/type_defs.py` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/type_defs.py`

 * *Files 26% similar despite different names*

```diff
@@ -59,682 +59,388 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccountDetailsTypeDef",
-    "ActionLocalIpDetailsOutputTypeDef",
     "ActionLocalIpDetailsTypeDef",
-    "ActionLocalPortDetailsOutputTypeDef",
     "ActionLocalPortDetailsTypeDef",
-    "DnsRequestActionOutputTypeDef",
-    "CityOutputTypeDef",
-    "CountryOutputTypeDef",
-    "GeoLocationOutputTypeDef",
-    "IpOrganizationDetailsOutputTypeDef",
+    "DnsRequestActionTypeDef",
     "CityTypeDef",
     "CountryTypeDef",
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
-    "ActionRemotePortDetailsOutputTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
-    "DnsRequestActionTypeDef",
-    "AdjustmentOutputTypeDef",
     "AdjustmentTypeDef",
     "AdminAccountTypeDef",
-    "AssociatedStandardOutputTypeDef",
     "AssociatedStandardTypeDef",
-    "AssociationStateDetailsOutputTypeDef",
     "AssociationStateDetailsTypeDef",
-    "NoteUpdateOutputTypeDef",
-    "RelatedFindingOutputTypeDef",
-    "SeverityUpdateOutputTypeDef",
-    "WorkflowUpdateOutputTypeDef",
     "NoteUpdateTypeDef",
     "RelatedFindingTypeDef",
     "SeverityUpdateTypeDef",
     "WorkflowUpdateTypeDef",
-    "MapFilterOutputTypeDef",
-    "NumberFilterOutputTypeDef",
-    "StringFilterOutputTypeDef",
     "MapFilterTypeDef",
     "NumberFilterTypeDef",
     "StringFilterTypeDef",
     "AutomationRulesMetadataTypeDef",
-    "AvailabilityZoneOutputTypeDef",
     "AvailabilityZoneTypeDef",
-    "AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef",
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
-    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef",
-    "AwsAmazonMqBrokerUsersDetailsOutputTypeDef",
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
     "AwsAmazonMqBrokerUsersDetailsTypeDef",
-    "AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
-    "AwsApiCallActionDomainDetailsOutputTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
-    "AwsApiGatewayAccessLogSettingsOutputTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
     "AwsApiGatewayCanarySettingsOutputTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
     "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
-    "AwsApiGatewayMethodSettingsOutputTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
     "AwsCorsConfigurationOutputTypeDef",
     "AwsCorsConfigurationTypeDef",
-    "AwsApiGatewayV2RouteSettingsOutputTypeDef",
     "AwsApiGatewayV2RouteSettingsTypeDef",
-    "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef",
-    "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef",
-    "AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
-    "AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
-    "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef",
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef",
-    "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
-    "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef",
-    "AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef",
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
-    "AwsBackupBackupPlanLifecycleDetailsOutputTypeDef",
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
     "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
-    "AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef",
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
-    "AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef",
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
-    "AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef",
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
-    "AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef",
-    "AwsCertificateManagerCertificateKeyUsageOutputTypeDef",
-    "AwsCertificateManagerCertificateOptionsOutputTypeDef",
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     "AwsCertificateManagerCertificateKeyUsageTypeDef",
     "AwsCertificateManagerCertificateOptionsTypeDef",
-    "AwsCertificateManagerCertificateResourceRecordOutputTypeDef",
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
-    "AwsCloudFormationStackDriftInformationDetailsOutputTypeDef",
-    "AwsCloudFormationStackOutputsDetailsOutputTypeDef",
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     "AwsCloudFormationStackOutputsDetailsTypeDef",
-    "AwsCloudFrontDistributionCacheBehaviorOutputTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
-    "AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef",
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
-    "AwsCloudFrontDistributionLoggingOutputTypeDef",
-    "AwsCloudFrontDistributionViewerCertificateOutputTypeDef",
     "AwsCloudFrontDistributionLoggingTypeDef",
     "AwsCloudFrontDistributionViewerCertificateTypeDef",
     "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
-    "AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef",
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
-    "AwsCloudTrailTrailDetailsOutputTypeDef",
     "AwsCloudTrailTrailDetailsTypeDef",
-    "AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef",
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
-    "AwsCodeBuildProjectArtifactsDetailsOutputTypeDef",
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
-    "AwsCodeBuildProjectSourceOutputTypeDef",
-    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     "AwsCodeBuildProjectSourceTypeDef",
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     "AwsCodeBuildProjectVpcConfigTypeDef",
-    "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
-    "AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
-    "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef",
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
-    "AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef",
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
-    "AwsDynamoDbTableAttributeDefinitionOutputTypeDef",
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
-    "AwsDynamoDbTableBillingModeSummaryOutputTypeDef",
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
-    "AwsDynamoDbTableKeySchemaOutputTypeDef",
-    "AwsDynamoDbTableProvisionedThroughputOutputTypeDef",
-    "AwsDynamoDbTableRestoreSummaryOutputTypeDef",
-    "AwsDynamoDbTableSseDescriptionOutputTypeDef",
-    "AwsDynamoDbTableStreamSpecificationOutputTypeDef",
     "AwsDynamoDbTableKeySchemaTypeDef",
     "AwsDynamoDbTableProvisionedThroughputTypeDef",
     "AwsDynamoDbTableRestoreSummaryTypeDef",
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
     "AwsDynamoDbTableProjectionOutputTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
-    "AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
-    "AwsEc2EipDetailsOutputTypeDef",
     "AwsEc2EipDetailsTypeDef",
-    "AwsEc2InstanceMetadataOptionsOutputTypeDef",
-    "AwsEc2InstanceMonitoringDetailsOutputTypeDef",
-    "AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef",
     "AwsEc2InstanceMetadataOptionsTypeDef",
     "AwsEc2InstanceMonitoringDetailsTypeDef",
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
     "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
     "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
     "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
-    "AwsEc2NetworkAclAssociationOutputTypeDef",
     "AwsEc2NetworkAclAssociationTypeDef",
-    "IcmpTypeCodeOutputTypeDef",
-    "PortRangeFromToOutputTypeDef",
     "IcmpTypeCodeTypeDef",
     "PortRangeFromToTypeDef",
-    "AwsEc2NetworkInterfaceAttachmentOutputTypeDef",
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
-    "AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef",
-    "AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef",
-    "AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef",
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     "AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef",
     "AwsEc2NetworkInterfaceSecurityGroupTypeDef",
-    "PropagatingVgwSetDetailsOutputTypeDef",
-    "RouteSetDetailsOutputTypeDef",
     "PropagatingVgwSetDetailsTypeDef",
     "RouteSetDetailsTypeDef",
-    "AwsEc2SecurityGroupIpRangeOutputTypeDef",
-    "AwsEc2SecurityGroupIpv6RangeOutputTypeDef",
-    "AwsEc2SecurityGroupPrefixListIdOutputTypeDef",
-    "AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef",
     "AwsEc2SecurityGroupIpRangeTypeDef",
     "AwsEc2SecurityGroupIpv6RangeTypeDef",
     "AwsEc2SecurityGroupPrefixListIdTypeDef",
     "AwsEc2SecurityGroupUserIdGroupPairTypeDef",
-    "Ipv6CidrBlockAssociationOutputTypeDef",
     "Ipv6CidrBlockAssociationTypeDef",
     "AwsEc2TransitGatewayDetailsOutputTypeDef",
     "AwsEc2TransitGatewayDetailsTypeDef",
-    "AwsEc2VolumeAttachmentOutputTypeDef",
     "AwsEc2VolumeAttachmentTypeDef",
-    "CidrBlockAssociationOutputTypeDef",
     "CidrBlockAssociationTypeDef",
-    "AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef",
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
-    "AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
-    "VpcInfoCidrBlockSetDetailsOutputTypeDef",
-    "VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef",
-    "VpcInfoPeeringOptionsDetailsOutputTypeDef",
     "VpcInfoCidrBlockSetDetailsTypeDef",
     "VpcInfoIpv6CidrBlockSetDetailsTypeDef",
     "VpcInfoPeeringOptionsDetailsTypeDef",
-    "AwsEc2VpnConnectionRoutesDetailsOutputTypeDef",
-    "AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef",
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     "AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef",
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
     "AwsEcrContainerImageDetailsOutputTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
-    "AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef",
-    "AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef",
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     "AwsEcrRepositoryLifecyclePolicyDetailsTypeDef",
-    "AwsEcsClusterClusterSettingsDetailsOutputTypeDef",
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
-    "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
-    "AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef",
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
-    "AwsMountPointOutputTypeDef",
     "AwsMountPointTypeDef",
-    "AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef",
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
-    "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef",
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
-    "AwsEcsServiceDeploymentControllerDetailsOutputTypeDef",
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
-    "AwsEcsServiceLoadBalancersDetailsOutputTypeDef",
-    "AwsEcsServicePlacementConstraintsDetailsOutputTypeDef",
-    "AwsEcsServicePlacementStrategiesDetailsOutputTypeDef",
-    "AwsEcsServiceServiceRegistriesDetailsOutputTypeDef",
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     "AwsEcsServicePlacementConstraintsDetailsTypeDef",
     "AwsEcsServicePlacementStrategiesDetailsTypeDef",
     "AwsEcsServiceServiceRegistriesDetailsTypeDef",
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
-    "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     "AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef",
-    "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
-    "AwsEcsTaskVolumeHostDetailsOutputTypeDef",
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
-    "AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef",
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
     "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
-    "AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef",
-    "AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef",
-    "AwsElasticBeanstalkEnvironmentTierOutputTypeDef",
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     "AwsElasticBeanstalkEnvironmentOptionSettingTypeDef",
     "AwsElasticBeanstalkEnvironmentTierTypeDef",
-    "AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef",
-    "AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef",
-    "AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef",
-    "AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef",
-    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
     "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
     "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     "AwsElasticsearchDomainVPCOptionsTypeDef",
-    "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
-    "AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
-    "AwsElbAppCookieStickinessPolicyOutputTypeDef",
     "AwsElbAppCookieStickinessPolicyTypeDef",
-    "AwsElbLbCookieStickinessPolicyOutputTypeDef",
     "AwsElbLbCookieStickinessPolicyTypeDef",
-    "AwsElbLoadBalancerAccessLogOutputTypeDef",
     "AwsElbLoadBalancerAccessLogTypeDef",
-    "AwsElbLoadBalancerAdditionalAttributeOutputTypeDef",
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
-    "AwsElbLoadBalancerConnectionDrainingOutputTypeDef",
-    "AwsElbLoadBalancerConnectionSettingsOutputTypeDef",
-    "AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef",
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     "AwsElbLoadBalancerConnectionSettingsTypeDef",
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
     "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
-    "AwsElbLoadBalancerHealthCheckOutputTypeDef",
-    "AwsElbLoadBalancerInstanceOutputTypeDef",
-    "AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef",
     "AwsElbLoadBalancerHealthCheckTypeDef",
     "AwsElbLoadBalancerInstanceTypeDef",
     "AwsElbLoadBalancerSourceSecurityGroupTypeDef",
-    "AwsElbLoadBalancerListenerOutputTypeDef",
     "AwsElbLoadBalancerListenerTypeDef",
-    "AwsElbv2LoadBalancerAttributeOutputTypeDef",
     "AwsElbv2LoadBalancerAttributeTypeDef",
-    "LoadBalancerStateOutputTypeDef",
     "LoadBalancerStateTypeDef",
-    "AwsEventSchemasRegistryDetailsOutputTypeDef",
     "AwsEventSchemasRegistryDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef",
-    "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef",
-    "AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
-    "AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef",
     "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
-    "AwsIamAccessKeySessionContextAttributesOutputTypeDef",
     "AwsIamAccessKeySessionContextAttributesTypeDef",
-    "AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef",
     "AwsIamAccessKeySessionContextSessionIssuerTypeDef",
-    "AwsIamAttachedManagedPolicyOutputTypeDef",
     "AwsIamAttachedManagedPolicyTypeDef",
-    "AwsIamGroupPolicyOutputTypeDef",
     "AwsIamGroupPolicyTypeDef",
-    "AwsIamInstanceProfileRoleOutputTypeDef",
     "AwsIamInstanceProfileRoleTypeDef",
-    "AwsIamPermissionsBoundaryOutputTypeDef",
     "AwsIamPermissionsBoundaryTypeDef",
-    "AwsIamPolicyVersionOutputTypeDef",
     "AwsIamPolicyVersionTypeDef",
-    "AwsIamRolePolicyOutputTypeDef",
     "AwsIamRolePolicyTypeDef",
-    "AwsIamUserPolicyOutputTypeDef",
     "AwsIamUserPolicyTypeDef",
-    "AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef",
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
-    "AwsKmsKeyDetailsOutputTypeDef",
     "AwsKmsKeyDetailsTypeDef",
-    "AwsLambdaFunctionCodeOutputTypeDef",
     "AwsLambdaFunctionCodeTypeDef",
-    "AwsLambdaFunctionDeadLetterConfigOutputTypeDef",
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
-    "AwsLambdaFunctionLayerOutputTypeDef",
-    "AwsLambdaFunctionTracingConfigOutputTypeDef",
-    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     "AwsLambdaFunctionLayerTypeDef",
     "AwsLambdaFunctionTracingConfigTypeDef",
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     "AwsLambdaFunctionVpcConfigTypeDef",
-    "AwsLambdaFunctionEnvironmentErrorOutputTypeDef",
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
     "AwsLambdaLayerVersionDetailsOutputTypeDef",
     "AwsLambdaLayerVersionDetailsTypeDef",
-    "AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef",
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
-    "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef",
-    "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef",
-    "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef",
-    "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef",
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef",
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
-    "AwsRdsDbClusterAssociatedRoleOutputTypeDef",
     "AwsRdsDbClusterAssociatedRoleTypeDef",
-    "AwsRdsDbClusterMemberOutputTypeDef",
-    "AwsRdsDbClusterOptionGroupMembershipOutputTypeDef",
-    "AwsRdsDbDomainMembershipOutputTypeDef",
-    "AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef",
     "AwsRdsDbClusterMemberTypeDef",
     "AwsRdsDbClusterOptionGroupMembershipTypeDef",
     "AwsRdsDbDomainMembershipTypeDef",
     "AwsRdsDbInstanceVpcSecurityGroupTypeDef",
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef",
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef",
-    "AwsRdsDbInstanceAssociatedRoleOutputTypeDef",
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
-    "AwsRdsDbInstanceEndpointOutputTypeDef",
-    "AwsRdsDbOptionGroupMembershipOutputTypeDef",
-    "AwsRdsDbParameterGroupOutputTypeDef",
-    "AwsRdsDbProcessorFeatureOutputTypeDef",
-    "AwsRdsDbStatusInfoOutputTypeDef",
     "AwsRdsDbInstanceEndpointTypeDef",
     "AwsRdsDbOptionGroupMembershipTypeDef",
     "AwsRdsDbParameterGroupTypeDef",
     "AwsRdsDbProcessorFeatureTypeDef",
     "AwsRdsDbStatusInfoTypeDef",
     "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
-    "AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef",
-    "AwsRdsDbSecurityGroupIpRangeOutputTypeDef",
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     "AwsRdsDbSecurityGroupIpRangeTypeDef",
-    "AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef",
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     "AwsRdsEventSubscriptionDetailsOutputTypeDef",
     "AwsRdsEventSubscriptionDetailsTypeDef",
-    "AwsRedshiftClusterClusterNodeOutputTypeDef",
     "AwsRedshiftClusterClusterNodeTypeDef",
-    "AwsRedshiftClusterClusterParameterStatusOutputTypeDef",
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
-    "AwsRedshiftClusterClusterSecurityGroupOutputTypeDef",
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
-    "AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef",
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
-    "AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef",
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
-    "AwsRedshiftClusterElasticIpStatusOutputTypeDef",
-    "AwsRedshiftClusterEndpointOutputTypeDef",
-    "AwsRedshiftClusterHsmStatusOutputTypeDef",
-    "AwsRedshiftClusterIamRoleOutputTypeDef",
-    "AwsRedshiftClusterLoggingStatusOutputTypeDef",
-    "AwsRedshiftClusterPendingModifiedValuesOutputTypeDef",
-    "AwsRedshiftClusterResizeInfoOutputTypeDef",
-    "AwsRedshiftClusterRestoreStatusOutputTypeDef",
-    "AwsRedshiftClusterVpcSecurityGroupOutputTypeDef",
     "AwsRedshiftClusterElasticIpStatusTypeDef",
     "AwsRedshiftClusterEndpointTypeDef",
     "AwsRedshiftClusterHsmStatusTypeDef",
     "AwsRedshiftClusterIamRoleTypeDef",
     "AwsRedshiftClusterLoggingStatusTypeDef",
     "AwsRedshiftClusterPendingModifiedValuesTypeDef",
     "AwsRedshiftClusterResizeInfoTypeDef",
     "AwsRedshiftClusterRestoreStatusTypeDef",
     "AwsRedshiftClusterVpcSecurityGroupTypeDef",
-    "AwsS3AccountPublicAccessBlockDetailsOutputTypeDef",
     "AwsS3AccountPublicAccessBlockDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef",
-    "AwsS3BucketBucketVersioningConfigurationOutputTypeDef",
     "AwsS3BucketBucketVersioningConfigurationTypeDef",
-    "AwsS3BucketLoggingConfigurationOutputTypeDef",
     "AwsS3BucketLoggingConfigurationTypeDef",
-    "AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
-    "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef",
     "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
-    "AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef",
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
-    "AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
-    "AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
-    "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
-    "AwsS3ObjectDetailsOutputTypeDef",
     "AwsS3ObjectDetailsTypeDef",
-    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
-    "AwsSecretsManagerSecretRotationRulesOutputTypeDef",
     "AwsSecretsManagerSecretRotationRulesTypeDef",
-    "BooleanFilterOutputTypeDef",
-    "IpFilterOutputTypeDef",
-    "KeywordFilterOutputTypeDef",
     "BooleanFilterTypeDef",
     "IpFilterTypeDef",
     "KeywordFilterTypeDef",
-    "AwsSecurityFindingIdentifierOutputTypeDef",
     "AwsSecurityFindingIdentifierTypeDef",
-    "MalwareOutputTypeDef",
-    "NoteOutputTypeDef",
-    "PatchSummaryOutputTypeDef",
-    "ProcessDetailsOutputTypeDef",
-    "SeverityOutputTypeDef",
-    "ThreatIntelIndicatorOutputTypeDef",
-    "WorkflowOutputTypeDef",
     "MalwareTypeDef",
     "NoteTypeDef",
     "PatchSummaryTypeDef",
     "ProcessDetailsTypeDef",
     "SeverityTypeDef",
     "ThreatIntelIndicatorTypeDef",
     "WorkflowTypeDef",
-    "AwsSnsTopicSubscriptionOutputTypeDef",
     "AwsSnsTopicSubscriptionTypeDef",
-    "AwsSqsQueueDetailsOutputTypeDef",
     "AwsSqsQueueDetailsTypeDef",
-    "AwsSsmComplianceSummaryOutputTypeDef",
     "AwsSsmComplianceSummaryTypeDef",
-    "AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
-    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
-    "AwsWafRateBasedRuleMatchPredicateOutputTypeDef",
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
-    "AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef",
     "AwsWafRegionalRateBasedRuleMatchPredicateTypeDef",
-    "AwsWafRegionalRulePredicateListDetailsOutputTypeDef",
     "AwsWafRegionalRulePredicateListDetailsTypeDef",
-    "AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupRulesActionDetailsTypeDef",
-    "AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef",
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
-    "AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef",
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
-    "AwsWafRulePredicateListDetailsOutputTypeDef",
     "AwsWafRulePredicateListDetailsTypeDef",
-    "AwsWafRuleGroupRulesActionDetailsOutputTypeDef",
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
-    "WafActionOutputTypeDef",
-    "WafExcludedRuleOutputTypeDef",
-    "WafOverrideActionOutputTypeDef",
     "WafActionTypeDef",
     "WafExcludedRuleTypeDef",
     "WafOverrideActionTypeDef",
-    "AwsWafv2CustomHttpHeaderOutputTypeDef",
     "AwsWafv2CustomHttpHeaderTypeDef",
-    "AwsWafv2VisibilityConfigDetailsOutputTypeDef",
     "AwsWafv2VisibilityConfigDetailsTypeDef",
-    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef",
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
-    "AwsXrayEncryptionConfigDetailsOutputTypeDef",
     "AwsXrayEncryptionConfigDetailsTypeDef",
     "BatchDeleteAutomationRulesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedAutomationRuleTypeDef",
     "BatchDisableStandardsRequestRequestTypeDef",
     "StandardsSubscriptionRequestTypeDef",
     "BatchGetAutomationRulesRequestRequestTypeDef",
     "BatchGetSecurityControlsRequestRequestTypeDef",
     "SecurityControlTypeDef",
     "UnprocessedSecurityControlTypeDef",
     "StandardsControlAssociationIdTypeDef",
     "StandardsControlAssociationDetailTypeDef",
     "ImportFindingsErrorTypeDef",
     "StandardsControlAssociationUpdateTypeDef",
-    "CellOutputTypeDef",
     "CellTypeDef",
-    "ClassificationStatusOutputTypeDef",
     "ClassificationStatusTypeDef",
-    "StatusReasonOutputTypeDef",
     "StatusReasonTypeDef",
-    "VolumeMountOutputTypeDef",
     "VolumeMountTypeDef",
     "CreateActionTargetRequestRequestTypeDef",
     "CreateFindingAggregatorRequestRequestTypeDef",
     "ResultTypeDef",
-    "DateRangeOutputTypeDef",
     "DateRangeTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteActionTargetRequestRequestTypeDef",
     "DeleteFindingAggregatorRequestRequestTypeDef",
     "DeleteInsightRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
@@ -748,23 +454,19 @@
     "DescribeStandardsRequestRequestTypeDef",
     "DisableImportFindingsForProductRequestRequestTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "EnableImportFindingsForProductRequestRequestTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "EnableSecurityHubRequestRequestTypeDef",
-    "FilePathsOutputTypeDef",
     "FilePathsTypeDef",
     "FindingAggregatorTypeDef",
     "FindingHistoryUpdateSourceTypeDef",
     "FindingHistoryUpdateTypeDef",
-    "FindingProviderSeverityOutputTypeDef",
     "FindingProviderSeverityTypeDef",
-    "FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef",
-    "FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef",
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     "FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef",
     "InvitationTypeDef",
     "GetEnabledStandardsRequestRequestTypeDef",
     "GetFindingAggregatorRequestRequestTypeDef",
     "SortCriterionTypeDef",
     "GetInsightResultsRequestRequestTypeDef",
@@ -780,91 +482,69 @@
     "ListMembersRequestRequestTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListSecurityControlDefinitionsRequestRequestTypeDef",
     "SecurityControlDefinitionTypeDef",
     "ListStandardsControlAssociationsRequestRequestTypeDef",
     "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PortRangeOutputTypeDef",
     "PortRangeTypeDef",
-    "RangeOutputTypeDef",
-    "RecordOutputTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "RecommendationOutputTypeDef",
     "RecommendationTypeDef",
     "RuleGroupSourceListDetailsOutputTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
-    "RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef",
-    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
-    "SoftwarePackageOutputTypeDef",
     "SoftwarePackageTypeDef",
     "StandardsManagedByTypeDef",
-    "StandardsControlAssociationIdOutputTypeDef",
-    "StandardsControlAssociationUpdateOutputTypeDef",
     "StandardsStatusReasonTypeDef",
-    "StatelessCustomPublishMetricActionDimensionOutputTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     "UpdateStandardsControlRequestRequestTypeDef",
-    "VulnerabilityVendorOutputTypeDef",
     "VulnerabilityVendorTypeDef",
     "CreateMembersRequestRequestTypeDef",
-    "ActionRemoteIpDetailsOutputTypeDef",
     "ActionRemoteIpDetailsTypeDef",
     "CvssOutputTypeDef",
     "CvssTypeDef",
-    "AssociationSetDetailsOutputTypeDef",
     "AssociationSetDetailsTypeDef",
     "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     "AutomationRulesFindingFieldsUpdateTypeDef",
-    "AwsAmazonMqBrokerLogsDetailsOutputTypeDef",
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     "AwsApiGatewayRestApiDetailsOutputTypeDef",
     "AwsApiGatewayRestApiDetailsTypeDef",
     "AwsApiGatewayStageDetailsOutputTypeDef",
     "AwsApiGatewayStageDetailsTypeDef",
     "AwsApiGatewayV2ApiDetailsOutputTypeDef",
     "AwsApiGatewayV2ApiDetailsTypeDef",
     "AwsApiGatewayV2StageDetailsOutputTypeDef",
     "AwsApiGatewayV2StageDetailsTypeDef",
-    "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
-    "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef",
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
-    "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
-    "AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef",
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     "AwsBackupBackupVaultDetailsOutputTypeDef",
     "AwsBackupBackupVaultDetailsTypeDef",
-    "AwsBackupRecoveryPointDetailsOutputTypeDef",
     "AwsBackupRecoveryPointDetailsTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
     "AwsCloudFormationStackDetailsOutputTypeDef",
     "AwsCloudFormationStackDetailsTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
@@ -872,35 +552,29 @@
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
     "AwsCloudWatchAlarmDetailsOutputTypeDef",
     "AwsCloudWatchAlarmDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
-    "AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
-    "AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     "AwsEc2InstanceDetailsOutputTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
-    "AwsEc2NetworkAclEntryOutputTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
     "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     "AwsEc2SubnetDetailsOutputTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
@@ -910,136 +584,109 @@
     "AwsEc2VpcDetailsTypeDef",
     "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
     "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
-    "AwsEcrRepositoryDetailsOutputTypeDef",
     "AwsEcrRepositoryDetailsTypeDef",
-    "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     "AwsEcsContainerDetailsOutputTypeDef",
     "AwsEcsContainerDetailsTypeDef",
-    "AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
-    "AwsEcsTaskVolumeDetailsOutputTypeDef",
     "AwsEcsTaskVolumeDetailsTypeDef",
-    "AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef",
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
     "AwsEksClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingDetailsTypeDef",
     "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
-    "AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
-    "AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     "AwsElbLoadBalancerPoliciesOutputTypeDef",
     "AwsElbLoadBalancerPoliciesTypeDef",
     "AwsElbLoadBalancerAttributesOutputTypeDef",
     "AwsElbLoadBalancerAttributesTypeDef",
     "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     "AwsElbv2LoadBalancerDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
-    "AwsIamAccessKeySessionContextOutputTypeDef",
     "AwsIamAccessKeySessionContextTypeDef",
     "AwsIamGroupDetailsOutputTypeDef",
     "AwsIamGroupDetailsTypeDef",
     "AwsIamInstanceProfileOutputTypeDef",
     "AwsIamInstanceProfileTypeDef",
     "AwsIamPolicyDetailsOutputTypeDef",
     "AwsIamPolicyDetailsTypeDef",
     "AwsIamUserDetailsOutputTypeDef",
     "AwsIamUserDetailsTypeDef",
-    "AwsKinesisStreamDetailsOutputTypeDef",
     "AwsKinesisStreamDetailsTypeDef",
     "AwsLambdaFunctionEnvironmentOutputTypeDef",
     "AwsLambdaFunctionEnvironmentTypeDef",
     "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
     "AwsNetworkFirewallFirewallDetailsTypeDef",
-    "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
-    "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
     "AwsRdsDbClusterDetailsOutputTypeDef",
     "AwsRdsDbClusterDetailsTypeDef",
     "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     "AwsRdsDbSnapshotDetailsOutputTypeDef",
     "AwsRdsDbSnapshotDetailsTypeDef",
     "AwsRdsDbPendingModifiedValuesOutputTypeDef",
     "AwsRdsDbPendingModifiedValuesTypeDef",
     "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     "AwsRdsDbSecurityGroupDetailsTypeDef",
-    "AwsRdsDbSubnetGroupSubnetOutputTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
-    "AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef",
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
-    "AwsS3BucketServerSideEncryptionRuleOutputTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
-    "AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
-    "AwsSecretsManagerSecretDetailsOutputTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
-    "BatchUpdateFindingsUnprocessedFindingTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
+    "BatchUpdateFindingsUnprocessedFindingTypeDef",
     "GetFindingHistoryRequestRequestTypeDef",
     "AwsSnsTopicDetailsOutputTypeDef",
     "AwsSnsTopicDetailsTypeDef",
-    "AwsSsmPatchOutputTypeDef",
     "AwsSsmPatchTypeDef",
-    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     "AwsWafRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRuleDetailsOutputTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
-    "AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
-    "AwsWafRegionalWebAclRulesListDetailsOutputTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     "AwsWafRuleDetailsOutputTypeDef",
     "AwsWafRuleDetailsTypeDef",
-    "AwsWafRuleGroupRulesDetailsOutputTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
     "AwsWafWebAclRuleOutputTypeDef",
     "AwsWafWebAclRuleTypeDef",
     "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
-    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     "AwsWafv2CustomResponseDetailsTypeDef",
-    "AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef",
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     "CreateActionTargetResponseTypeDef",
     "CreateAutomationRuleResponseTypeDef",
     "CreateFindingAggregatorResponseTypeDef",
     "CreateInsightResponseTypeDef",
     "DeleteActionTargetResponseTypeDef",
     "DeleteInsightResponseTypeDef",
@@ -1055,26 +702,27 @@
     "ListTagsForResourceResponseTypeDef",
     "UpdateFindingAggregatorResponseTypeDef",
     "BatchDeleteAutomationRulesResponseTypeDef",
     "BatchUpdateAutomationRulesResponseTypeDef",
     "BatchEnableStandardsRequestRequestTypeDef",
     "BatchGetSecurityControlsResponseTypeDef",
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
+    "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
+    "UnprocessedStandardsControlAssociationUpdateTypeDef",
     "ComplianceOutputTypeDef",
     "ComplianceTypeDef",
     "ContainerDetailsOutputTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
-    "DateFilterOutputTypeDef",
     "DateFilterTypeDef",
     "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
     "DescribeProductsRequestDescribeProductsPaginateTypeDef",
     "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
     "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
     "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
@@ -1098,51 +746,43 @@
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
     "ListSecurityControlDefinitionsResponseTypeDef",
     "ListStandardsControlAssociationsResponseTypeDef",
-    "NetworkOutputTypeDef",
     "NetworkPathComponentDetailsOutputTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
-    "PageOutputTypeDef",
     "PageTypeDef",
-    "RemediationOutputTypeDef",
     "RemediationTypeDef",
     "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     "RuleGroupVariablesOutputTypeDef",
     "RuleGroupVariablesTypeDef",
     "StandardTypeDef",
-    "UnprocessedStandardsControlAssociationTypeDef",
-    "UnprocessedStandardsControlAssociationUpdateTypeDef",
     "StandardsSubscriptionTypeDef",
     "StatelessCustomPublishMetricActionOutputTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
     "AwsApiCallActionOutputTypeDef",
-    "NetworkConnectionActionOutputTypeDef",
-    "PortProbeDetailOutputTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "VulnerabilityOutputTypeDef",
     "VulnerabilityTypeDef",
     "AwsEc2RouteTableDetailsOutputTypeDef",
     "AwsEc2RouteTableDetailsTypeDef",
     "AutomationRulesActionOutputTypeDef",
     "AutomationRulesActionTypeDef",
     "AwsAmazonMqBrokerDetailsOutputTypeDef",
     "AwsAmazonMqBrokerDetailsTypeDef",
     "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiDetailsTypeDef",
-    "AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef",
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
@@ -1162,15 +802,14 @@
     "AwsEc2NetworkAclDetailsTypeDef",
     "AwsEc2SecurityGroupDetailsOutputTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     "AwsEc2VpnConnectionDetailsOutputTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
-    "AwsEcsClusterConfigurationDetailsOutputTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
     "AwsEcsServiceDetailsOutputTypeDef",
     "AwsEcsServiceDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
@@ -1180,17 +819,15 @@
     "AwsEfsAccessPointDetailsTypeDef",
     "AwsEksClusterDetailsOutputTypeDef",
     "AwsEksClusterDetailsTypeDef",
     "AwsElasticsearchDomainDetailsOutputTypeDef",
     "AwsElasticsearchDomainDetailsTypeDef",
     "AwsElbLoadBalancerDetailsOutputTypeDef",
     "AwsElbLoadBalancerDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
-    "AwsIamAccessKeyDetailsOutputTypeDef",
     "AwsIamAccessKeyDetailsTypeDef",
     "AwsIamRoleDetailsOutputTypeDef",
     "AwsIamRoleDetailsTypeDef",
     "AwsLambdaFunctionDetailsOutputTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainDetailsTypeDef",
@@ -1198,64 +835,61 @@
     "AwsRdsDbSubnetGroupTypeDef",
     "AwsRedshiftClusterDetailsOutputTypeDef",
     "AwsRedshiftClusterDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
-    "AwsS3BucketObjectLockConfigurationOutputTypeDef",
     "AwsS3BucketObjectLockConfigurationTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
-    "AwsSsmPatchComplianceDetailsOutputTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
     "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     "AwsWafRegionalWebAclDetailsOutputTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
     "AwsWafRuleGroupDetailsOutputTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
     "AwsWafWebAclDetailsOutputTypeDef",
     "AwsWafWebAclDetailsTypeDef",
     "AwsWafv2ActionAllowDetailsOutputTypeDef",
     "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
     "AwsWafv2RulesActionCountDetailsOutputTypeDef",
-    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     "AwsWafv2ActionAllowDetailsTypeDef",
     "AwsWafv2RulesActionCaptchaDetailsTypeDef",
     "AwsWafv2RulesActionCountDetailsTypeDef",
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     "AwsWafv2ActionBlockDetailsTypeDef",
+    "BatchGetStandardsControlAssociationsResponseTypeDef",
+    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     "AutomationRulesFindingFiltersOutputTypeDef",
-    "AwsSecurityFindingFiltersOutputTypeDef",
     "AutomationRulesFindingFiltersTypeDef",
+    "AwsSecurityFindingFiltersOutputTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
     "GetFindingHistoryResponseTypeDef",
     "GetInsightResultsResponseTypeDef",
     "NetworkHeaderOutputTypeDef",
     "NetworkHeaderTypeDef",
     "OccurrencesOutputTypeDef",
     "OccurrencesTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     "DescribeStandardsResponseTypeDef",
-    "BatchGetStandardsControlAssociationsResponseTypeDef",
-    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
     "StatelessCustomActionDefinitionOutputTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
     "PortProbeActionOutputTypeDef",
     "PortProbeActionTypeDef",
-    "AwsAthenaWorkGroupDetailsOutputTypeDef",
     "AwsAthenaWorkGroupDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     "AwsCertificateManagerCertificateDetailsOutputTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
@@ -1267,32 +901,31 @@
     "AwsDynamoDbTableDetailsTypeDef",
     "AwsEc2LaunchTemplateDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDetailsTypeDef",
     "AwsEcsClusterDetailsOutputTypeDef",
     "AwsEcsClusterDetailsTypeDef",
     "AwsEcsTaskDefinitionDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
     "AwsRdsDbInstanceDetailsOutputTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
     "AwsStepFunctionStateMachineDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineDetailsTypeDef",
     "AwsWafv2RulesActionDetailsOutputTypeDef",
     "AwsWafv2WebAclActionDetailsOutputTypeDef",
     "AwsWafv2RulesActionDetailsTypeDef",
     "AwsWafv2WebAclActionDetailsTypeDef",
     "AutomationRulesConfigTypeDef",
-    "InsightTypeDef",
     "CreateAutomationRuleRequestRequestTypeDef",
     "UpdateAutomationRulesRequestItemTypeDef",
+    "InsightTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
     "NetworkPathComponentOutputTypeDef",
     "NetworkPathComponentTypeDef",
@@ -1317,16 +950,16 @@
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationOutputTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
     "AwsWafv2RulesDetailsOutputTypeDef",
     "AwsWafv2RulesDetailsTypeDef",
     "BatchGetAutomationRulesResponseTypeDef",
-    "GetInsightsResponseTypeDef",
     "BatchUpdateAutomationRulesRequestRequestTypeDef",
+    "GetInsightsResponseTypeDef",
     "CustomDataIdentifiersResultOutputTypeDef",
     "SensitiveDataResultOutputTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
     "FirewallPolicyDetailsOutputTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyDetailsTypeDef",
@@ -1392,95 +1025,41 @@
 )
 
 
 class AccountDetailsTypeDef(_RequiredAccountDetailsTypeDef, _OptionalAccountDetailsTypeDef):
     pass
 
 
-ActionLocalIpDetailsOutputTypeDef = TypedDict(
-    "ActionLocalIpDetailsOutputTypeDef",
-    {
-        "IpAddressV4": str,
-    },
-    total=False,
-)
-
 ActionLocalIpDetailsTypeDef = TypedDict(
     "ActionLocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
 
-ActionLocalPortDetailsOutputTypeDef = TypedDict(
-    "ActionLocalPortDetailsOutputTypeDef",
-    {
-        "Port": int,
-        "PortName": str,
-    },
-    total=False,
-)
-
 ActionLocalPortDetailsTypeDef = TypedDict(
     "ActionLocalPortDetailsTypeDef",
     {
         "Port": int,
         "PortName": str,
     },
     total=False,
 )
 
-DnsRequestActionOutputTypeDef = TypedDict(
-    "DnsRequestActionOutputTypeDef",
+DnsRequestActionTypeDef = TypedDict(
+    "DnsRequestActionTypeDef",
     {
         "Domain": str,
         "Protocol": str,
         "Blocked": bool,
     },
     total=False,
 )
 
-CityOutputTypeDef = TypedDict(
-    "CityOutputTypeDef",
-    {
-        "CityName": str,
-    },
-    total=False,
-)
-
-CountryOutputTypeDef = TypedDict(
-    "CountryOutputTypeDef",
-    {
-        "CountryCode": str,
-        "CountryName": str,
-    },
-    total=False,
-)
-
-GeoLocationOutputTypeDef = TypedDict(
-    "GeoLocationOutputTypeDef",
-    {
-        "Lon": float,
-        "Lat": float,
-    },
-    total=False,
-)
-
-IpOrganizationDetailsOutputTypeDef = TypedDict(
-    "IpOrganizationDetailsOutputTypeDef",
-    {
-        "Asn": int,
-        "AsnOrg": str,
-        "Isp": str,
-        "Org": str,
-    },
-    total=False,
-)
-
 CityTypeDef = TypedDict(
     "CityTypeDef",
     {
         "CityName": str,
     },
     total=False,
 )
@@ -1510,23 +1089,14 @@
         "AsnOrg": str,
         "Isp": str,
         "Org": str,
     },
     total=False,
 )
 
-ActionRemotePortDetailsOutputTypeDef = TypedDict(
-    "ActionRemotePortDetailsOutputTypeDef",
-    {
-        "Port": int,
-        "PortName": str,
-    },
-    total=False,
-)
-
 ActionRemotePortDetailsTypeDef = TypedDict(
     "ActionRemotePortDetailsTypeDef",
     {
         "Port": int,
         "PortName": str,
     },
     total=False,
@@ -1537,33 +1107,14 @@
     {
         "ActionTargetArn": str,
         "Name": str,
         "Description": str,
     },
 )
 
-DnsRequestActionTypeDef = TypedDict(
-    "DnsRequestActionTypeDef",
-    {
-        "Domain": str,
-        "Protocol": str,
-        "Blocked": bool,
-    },
-    total=False,
-)
-
-AdjustmentOutputTypeDef = TypedDict(
-    "AdjustmentOutputTypeDef",
-    {
-        "Metric": str,
-        "Reason": str,
-    },
-    total=False,
-)
-
 AdjustmentTypeDef = TypedDict(
     "AdjustmentTypeDef",
     {
         "Metric": str,
         "Reason": str,
     },
     total=False,
@@ -1574,82 +1125,31 @@
     {
         "AccountId": str,
         "Status": AdminStatusType,
     },
     total=False,
 )
 
-AssociatedStandardOutputTypeDef = TypedDict(
-    "AssociatedStandardOutputTypeDef",
-    {
-        "StandardsId": str,
-    },
-    total=False,
-)
-
 AssociatedStandardTypeDef = TypedDict(
     "AssociatedStandardTypeDef",
     {
         "StandardsId": str,
     },
     total=False,
 )
 
-AssociationStateDetailsOutputTypeDef = TypedDict(
-    "AssociationStateDetailsOutputTypeDef",
-    {
-        "State": str,
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
 AssociationStateDetailsTypeDef = TypedDict(
     "AssociationStateDetailsTypeDef",
     {
         "State": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-NoteUpdateOutputTypeDef = TypedDict(
-    "NoteUpdateOutputTypeDef",
-    {
-        "Text": str,
-        "UpdatedBy": str,
-    },
-)
-
-RelatedFindingOutputTypeDef = TypedDict(
-    "RelatedFindingOutputTypeDef",
-    {
-        "ProductArn": str,
-        "Id": str,
-    },
-)
-
-SeverityUpdateOutputTypeDef = TypedDict(
-    "SeverityUpdateOutputTypeDef",
-    {
-        "Normalized": int,
-        "Product": float,
-        "Label": SeverityLabelType,
-    },
-    total=False,
-)
-
-WorkflowUpdateOutputTypeDef = TypedDict(
-    "WorkflowUpdateOutputTypeDef",
-    {
-        "Status": WorkflowStatusType,
-    },
-    total=False,
-)
-
 NoteUpdateTypeDef = TypedDict(
     "NoteUpdateTypeDef",
     {
         "Text": str,
         "UpdatedBy": str,
     },
 )
@@ -1676,43 +1176,14 @@
     "WorkflowUpdateTypeDef",
     {
         "Status": WorkflowStatusType,
     },
     total=False,
 )
 
-MapFilterOutputTypeDef = TypedDict(
-    "MapFilterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "Comparison": MapFilterComparisonType,
-    },
-    total=False,
-)
-
-NumberFilterOutputTypeDef = TypedDict(
-    "NumberFilterOutputTypeDef",
-    {
-        "Gte": float,
-        "Lte": float,
-        "Eq": float,
-    },
-    total=False,
-)
-
-StringFilterOutputTypeDef = TypedDict(
-    "StringFilterOutputTypeDef",
-    {
-        "Value": str,
-        "Comparison": StringFilterComparisonType,
-    },
-    total=False,
-)
-
 MapFilterTypeDef = TypedDict(
     "MapFilterTypeDef",
     {
         "Key": str,
         "Value": str,
         "Comparison": MapFilterComparisonType,
     },
@@ -1750,34 +1221,25 @@
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
-AvailabilityZoneOutputTypeDef = TypedDict(
-    "AvailabilityZoneOutputTypeDef",
-    {
-        "ZoneName": str,
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef",
+AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
     {
         "KmsKeyId": str,
         "UseAwsOwnedKey": bool,
     },
     total=False,
 )
 
@@ -1794,42 +1256,33 @@
         "UserRoleName": str,
         "UserSearchMatching": str,
         "UserSearchSubtree": bool,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef",
+AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
     {
         "DayOfWeek": str,
         "TimeOfDay": str,
         "TimeZone": str,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerUsersDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerUsersDetailsOutputTypeDef",
+AwsAmazonMqBrokerUsersDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerUsersDetailsTypeDef",
     {
         "PendingChange": str,
         "Username": str,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
-    "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
-    {
-        "KmsKeyId": str,
-        "UseAwsOwnedKey": bool,
-    },
-    total=False,
-)
-
 AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     {
         "Hosts": Sequence[str],
         "RoleBase": str,
         "RoleName": str,
         "RoleSearchMatching": str,
@@ -1839,76 +1292,31 @@
         "UserRoleName": str,
         "UserSearchMatching": str,
         "UserSearchSubtree": bool,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef = TypedDict(
-    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
-    {
-        "DayOfWeek": str,
-        "TimeOfDay": str,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-AwsAmazonMqBrokerUsersDetailsTypeDef = TypedDict(
-    "AwsAmazonMqBrokerUsersDetailsTypeDef",
-    {
-        "PendingChange": str,
-        "Username": str,
-    },
-    total=False,
-)
-
-AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef",
-    {
-        "Audit": bool,
-        "General": bool,
-    },
-    total=False,
-)
-
 AwsAmazonMqBrokerLogsPendingDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
 )
 
-AwsApiCallActionDomainDetailsOutputTypeDef = TypedDict(
-    "AwsApiCallActionDomainDetailsOutputTypeDef",
-    {
-        "Domain": str,
-    },
-    total=False,
-)
-
 AwsApiCallActionDomainDetailsTypeDef = TypedDict(
     "AwsApiCallActionDomainDetailsTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-AwsApiGatewayAccessLogSettingsOutputTypeDef = TypedDict(
-    "AwsApiGatewayAccessLogSettingsOutputTypeDef",
-    {
-        "Format": str,
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
 AwsApiGatewayAccessLogSettingsTypeDef = TypedDict(
     "AwsApiGatewayAccessLogSettingsTypeDef",
     {
         "Format": str,
         "DestinationArn": str,
     },
     total=False,
@@ -1948,33 +1356,14 @@
     "AwsApiGatewayEndpointConfigurationTypeDef",
     {
         "Types": Sequence[str],
     },
     total=False,
 )
 
-AwsApiGatewayMethodSettingsOutputTypeDef = TypedDict(
-    "AwsApiGatewayMethodSettingsOutputTypeDef",
-    {
-        "MetricsEnabled": bool,
-        "LoggingLevel": str,
-        "DataTraceEnabled": bool,
-        "ThrottlingBurstLimit": int,
-        "ThrottlingRateLimit": float,
-        "CachingEnabled": bool,
-        "CacheTtlInSeconds": int,
-        "CacheDataEncrypted": bool,
-        "RequireAuthorizationForCacheControl": bool,
-        "UnauthorizedCacheControlHeaderStrategy": str,
-        "HttpMethod": str,
-        "ResourcePath": str,
-    },
-    total=False,
-)
-
 AwsApiGatewayMethodSettingsTypeDef = TypedDict(
     "AwsApiGatewayMethodSettingsTypeDef",
     {
         "MetricsEnabled": bool,
         "LoggingLevel": str,
         "DataTraceEnabled": bool,
         "ThrottlingBurstLimit": int,
@@ -2012,70 +1401,26 @@
         "MaxAge": int,
         "AllowMethods": Sequence[str],
         "AllowHeaders": Sequence[str],
     },
     total=False,
 )
 
-AwsApiGatewayV2RouteSettingsOutputTypeDef = TypedDict(
-    "AwsApiGatewayV2RouteSettingsOutputTypeDef",
-    {
-        "DetailedMetricsEnabled": bool,
-        "LoggingLevel": str,
-        "DataTraceEnabled": bool,
-        "ThrottlingBurstLimit": int,
-        "ThrottlingRateLimit": float,
-    },
-    total=False,
-)
-
 AwsApiGatewayV2RouteSettingsTypeDef = TypedDict(
     "AwsApiGatewayV2RouteSettingsTypeDef",
     {
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": str,
         "DataTraceEnabled": bool,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
     total=False,
 )
 
-AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef",
-    {
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerUri": str,
-        "IdentityValidationExpression": str,
-    },
-    total=False,
-)
-
-AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef",
-    {
-        "AuthTtL": int,
-        "ClientId": str,
-        "IatTtL": int,
-        "Issuer": str,
-    },
-    total=False,
-)
-
-AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef",
-    {
-        "AppIdClientRegex": str,
-        "AwsRegion": str,
-        "DefaultAction": str,
-        "UserPoolId": str,
-    },
-    total=False,
-)
-
 AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     {
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerUri": str,
         "IdentityValidationExpression": str,
     },
@@ -2100,133 +1445,64 @@
         "AwsRegion": str,
         "DefaultAction": str,
         "UserPoolId": str,
     },
     total=False,
 )
 
-AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef",
-    {
-        "CloudWatchLogsRoleArn": str,
-        "ExcludeVerboseContent": bool,
-        "FieldLogLevel": str,
-    },
-    total=False,
-)
-
 AwsAppSyncGraphQlApiLogConfigDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     {
         "CloudWatchLogsRoleArn": str,
         "ExcludeVerboseContent": bool,
         "FieldLogLevel": str,
     },
     total=False,
 )
 
-AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef",
-    {
-        "EncryptionOption": str,
-        "KmsKey": str,
-    },
-    total=False,
-)
-
 AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef",
     {
         "EncryptionOption": str,
         "KmsKey": str,
     },
     total=False,
 )
 
-AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
-    {
-        "LaunchTemplateId": str,
-        "LaunchTemplateName": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
     total=False,
 )
 
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef",
-    {
-        "OnDemandAllocationStrategy": str,
-        "OnDemandBaseCapacity": int,
-        "OnDemandPercentageAboveBaseCapacity": int,
-        "SpotAllocationStrategy": str,
-        "SpotInstancePools": int,
-        "SpotMaxPrice": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     {
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
         "OnDemandPercentageAboveBaseCapacity": int,
         "SpotAllocationStrategy": str,
         "SpotInstancePools": int,
         "SpotMaxPrice": str,
     },
     total=False,
 )
 
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
-    {
-        "LaunchTemplateId": str,
-        "LaunchTemplateName": str,
-        "Version": str,
-    },
-    total=False,
-)
-
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef",
-    {
-        "InstanceType": str,
-        "WeightedCapacity": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
@@ -2238,58 +1514,27 @@
     {
         "InstanceType": str,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
-AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef",
-    {
-        "DeleteOnTermination": bool,
-        "Encrypted": bool,
-        "Iops": int,
-        "SnapshotId": str,
-        "VolumeSize": int,
-        "VolumeType": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
         "Iops": int,
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
     },
     total=False,
 )
 
-AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef",
-    {
-        "HttpEndpoint": str,
-        "HttpPutResponseHopLimit": int,
-        "HttpTokens": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -2318,23 +1563,14 @@
     {
         "BackupOptions": Mapping[str, str],
         "ResourceType": str,
     },
     total=False,
 )
 
-AwsBackupBackupPlanLifecycleDetailsOutputTypeDef = TypedDict(
-    "AwsBackupBackupPlanLifecycleDetailsOutputTypeDef",
-    {
-        "DeleteAfterDays": int,
-        "MoveToColdStorageAfterDays": int,
-    },
-    total=False,
-)
-
 AwsBackupBackupPlanLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
     total=False,
@@ -2354,97 +1590,43 @@
     {
         "BackupVaultEvents": Sequence[str],
         "SnsTopicArn": str,
     },
     total=False,
 )
 
-AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef = TypedDict(
-    "AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef",
-    {
-        "DeleteAt": str,
-        "MoveToColdStorageAt": str,
-    },
-    total=False,
-)
-
 AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
     {
         "DeleteAt": str,
         "MoveToColdStorageAt": str,
     },
     total=False,
 )
 
-AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef = TypedDict(
-    "AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef",
-    {
-        "BackupPlanArn": str,
-        "BackupPlanId": str,
-        "BackupPlanVersion": str,
-        "BackupRuleId": str,
-    },
-    total=False,
-)
-
 AwsBackupRecoveryPointCreatedByDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "BackupPlanVersion": str,
         "BackupRuleId": str,
     },
     total=False,
 )
 
-AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef = TypedDict(
-    "AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef",
-    {
-        "DeleteAfterDays": int,
-        "MoveToColdStorageAfterDays": int,
-    },
-    total=False,
-)
-
 AwsBackupRecoveryPointLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
     total=False,
 )
 
-AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef",
-    {
-        "Name": str,
-        "OId": str,
-    },
-    total=False,
-)
-
-AwsCertificateManagerCertificateKeyUsageOutputTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateKeyUsageOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-AwsCertificateManagerCertificateOptionsOutputTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateOptionsOutputTypeDef",
-    {
-        "CertificateTransparencyLoggingPreference": str,
-    },
-    total=False,
-)
-
 AwsCertificateManagerCertificateExtendedKeyUsageTypeDef = TypedDict(
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     {
         "Name": str,
         "OId": str,
     },
     total=False,
@@ -2462,52 +1644,24 @@
     "AwsCertificateManagerCertificateOptionsTypeDef",
     {
         "CertificateTransparencyLoggingPreference": str,
     },
     total=False,
 )
 
-AwsCertificateManagerCertificateResourceRecordOutputTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateResourceRecordOutputTypeDef",
-    {
-        "Name": str,
-        "Type": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsCertificateManagerCertificateResourceRecordTypeDef = TypedDict(
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
     {
         "Name": str,
         "Type": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsCloudFormationStackDriftInformationDetailsOutputTypeDef = TypedDict(
-    "AwsCloudFormationStackDriftInformationDetailsOutputTypeDef",
-    {
-        "StackDriftStatus": str,
-    },
-    total=False,
-)
-
-AwsCloudFormationStackOutputsDetailsOutputTypeDef = TypedDict(
-    "AwsCloudFormationStackOutputsDetailsOutputTypeDef",
-    {
-        "Description": str,
-        "OutputKey": str,
-        "OutputValue": str,
-    },
-    total=False,
-)
-
 AwsCloudFormationStackDriftInformationDetailsTypeDef = TypedDict(
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     {
         "StackDriftStatus": str,
     },
     total=False,
 )
@@ -2518,71 +1672,30 @@
         "Description": str,
         "OutputKey": str,
         "OutputValue": str,
     },
     total=False,
 )
 
-AwsCloudFrontDistributionCacheBehaviorOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionCacheBehaviorOutputTypeDef",
-    {
-        "ViewerProtocolPolicy": str,
-    },
-    total=False,
-)
-
 AwsCloudFrontDistributionCacheBehaviorTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
     total=False,
 )
 
-AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef",
-    {
-        "ViewerProtocolPolicy": str,
-    },
-    total=False,
-)
-
 AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef = TypedDict(
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
     total=False,
 )
 
-AwsCloudFrontDistributionLoggingOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionLoggingOutputTypeDef",
-    {
-        "Bucket": str,
-        "Enabled": bool,
-        "IncludeCookies": bool,
-        "Prefix": str,
-    },
-    total=False,
-)
-
-AwsCloudFrontDistributionViewerCertificateOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionViewerCertificateOutputTypeDef",
-    {
-        "AcmCertificateArn": str,
-        "Certificate": str,
-        "CertificateSource": str,
-        "CloudFrontDefaultCertificate": bool,
-        "IamCertificateId": str,
-        "MinimumProtocolVersion": str,
-        "SslSupportMethod": str,
-    },
-    total=False,
-)
-
 AwsCloudFrontDistributionLoggingTypeDef = TypedDict(
     "AwsCloudFrontDistributionLoggingTypeDef",
     {
         "Bucket": str,
         "Enabled": bool,
         "IncludeCookies": bool,
         "Prefix": str,
@@ -2636,52 +1749,22 @@
     {
         "Items": Sequence[int],
         "Quantity": int,
     },
     total=False,
 )
 
-AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef",
-    {
-        "OriginAccessIdentity": str,
-    },
-    total=False,
-)
-
 AwsCloudFrontDistributionOriginS3OriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
     },
     total=False,
 )
 
-AwsCloudTrailTrailDetailsOutputTypeDef = TypedDict(
-    "AwsCloudTrailTrailDetailsOutputTypeDef",
-    {
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "HasCustomEventSelectors": bool,
-        "HomeRegion": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "IsOrganizationTrail": bool,
-        "KmsKeyId": str,
-        "LogFileValidationEnabled": bool,
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicArn": str,
-        "SnsTopicName": str,
-        "TrailArn": str,
-    },
-    total=False,
-)
-
 AwsCloudTrailTrailDetailsTypeDef = TypedDict(
     "AwsCloudTrailTrailDetailsTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "CloudWatchLogsRoleArn": str,
         "HasCustomEventSelectors": bool,
         "HomeRegion": str,
@@ -2696,48 +1779,23 @@
         "SnsTopicArn": str,
         "SnsTopicName": str,
         "TrailArn": str,
     },
     total=False,
 )
 
-AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef = TypedDict(
-    "AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsCloudWatchAlarmDimensionsDetailsTypeDef = TypedDict(
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectArtifactsDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectArtifactsDetailsOutputTypeDef",
-    {
-        "ArtifactIdentifier": str,
-        "EncryptionDisabled": bool,
-        "Location": str,
-        "Name": str,
-        "NamespaceType": str,
-        "OverrideArtifactName": bool,
-        "Packaging": str,
-        "Path": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectArtifactsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
     {
         "ArtifactIdentifier": str,
         "EncryptionDisabled": bool,
         "Location": str,
         "Name": str,
@@ -2746,16 +1804,16 @@
         "Packaging": str,
         "Path": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectSourceOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectSourceOutputTypeDef",
+AwsCodeBuildProjectSourceTypeDef = TypedDict(
+    "AwsCodeBuildProjectSourceTypeDef",
     {
         "Type": str,
         "Location": str,
         "GitCloneDepth": int,
         "InsecureSsl": bool,
     },
     total=False,
@@ -2767,201 +1825,81 @@
         "VpcId": str,
         "Subnets": List[str],
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-AwsCodeBuildProjectSourceTypeDef = TypedDict(
-    "AwsCodeBuildProjectSourceTypeDef",
-    {
-        "Type": str,
-        "Location": str,
-        "GitCloneDepth": int,
-        "InsecureSsl": bool,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectVpcConfigTypeDef = TypedDict(
     "AwsCodeBuildProjectVpcConfigTypeDef",
     {
         "VpcId": str,
         "Subnets": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Type": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
     {
         "Name": str,
         "Type": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef",
-    {
-        "Credential": str,
-        "CredentialProvider": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
     {
         "Credential": str,
         "CredentialProvider": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef",
-    {
-        "GroupName": str,
-        "Status": str,
-        "StreamName": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
     {
         "GroupName": str,
         "Status": str,
         "StreamName": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef",
-    {
-        "EncryptionDisabled": bool,
-        "Location": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
     {
         "EncryptionDisabled": bool,
         "Location": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsDynamoDbTableAttributeDefinitionOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableAttributeDefinitionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": str,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableAttributeDefinitionTypeDef = TypedDict(
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": str,
     },
     total=False,
 )
 
-AwsDynamoDbTableBillingModeSummaryOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableBillingModeSummaryOutputTypeDef",
-    {
-        "BillingMode": str,
-        "LastUpdateToPayPerRequestDateTime": str,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableBillingModeSummaryTypeDef = TypedDict(
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
     {
         "BillingMode": str,
         "LastUpdateToPayPerRequestDateTime": str,
     },
     total=False,
 )
 
-AwsDynamoDbTableKeySchemaOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableKeySchemaOutputTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": str,
-    },
-    total=False,
-)
-
-AwsDynamoDbTableProvisionedThroughputOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableProvisionedThroughputOutputTypeDef",
-    {
-        "LastDecreaseDateTime": str,
-        "LastIncreaseDateTime": str,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-    total=False,
-)
-
-AwsDynamoDbTableRestoreSummaryOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableRestoreSummaryOutputTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-        "RestoreDateTime": str,
-        "RestoreInProgress": bool,
-    },
-    total=False,
-)
-
-AwsDynamoDbTableSseDescriptionOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableSseDescriptionOutputTypeDef",
-    {
-        "InaccessibleEncryptionDateTime": str,
-        "Status": str,
-        "SseType": str,
-        "KmsMasterKeyArn": str,
-    },
-    total=False,
-)
-
-AwsDynamoDbTableStreamSpecificationOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableStreamSpecificationOutputTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": str,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableKeySchemaTypeDef = TypedDict(
     "AwsDynamoDbTableKeySchemaTypeDef",
     {
         "AttributeName": str,
         "KeyType": str,
     },
     total=False,
@@ -3024,47 +1962,22 @@
     {
         "NonKeyAttributes": Sequence[str],
         "ProjectionType": str,
     },
     total=False,
 )
 
-AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableProvisionedThroughputOverrideTypeDef = TypedDict(
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": int,
     },
     total=False,
 )
 
-AwsEc2EipDetailsOutputTypeDef = TypedDict(
-    "AwsEc2EipDetailsOutputTypeDef",
-    {
-        "InstanceId": str,
-        "PublicIp": str,
-        "AllocationId": str,
-        "AssociationId": str,
-        "Domain": str,
-        "PublicIpv4Pool": str,
-        "NetworkBorderGroup": str,
-        "NetworkInterfaceId": str,
-        "NetworkInterfaceOwnerId": str,
-        "PrivateIpAddress": str,
-    },
-    total=False,
-)
-
 AwsEc2EipDetailsTypeDef = TypedDict(
     "AwsEc2EipDetailsTypeDef",
     {
         "InstanceId": str,
         "PublicIp": str,
         "AllocationId": str,
         "AssociationId": str,
@@ -3074,42 +1987,14 @@
         "NetworkInterfaceId": str,
         "NetworkInterfaceOwnerId": str,
         "PrivateIpAddress": str,
     },
     total=False,
 )
 
-AwsEc2InstanceMetadataOptionsOutputTypeDef = TypedDict(
-    "AwsEc2InstanceMetadataOptionsOutputTypeDef",
-    {
-        "HttpEndpoint": str,
-        "HttpProtocolIpv6": str,
-        "HttpPutResponseHopLimit": int,
-        "HttpTokens": str,
-        "InstanceMetadataTags": str,
-    },
-    total=False,
-)
-
-AwsEc2InstanceMonitoringDetailsOutputTypeDef = TypedDict(
-    "AwsEc2InstanceMonitoringDetailsOutputTypeDef",
-    {
-        "State": str,
-    },
-    total=False,
-)
-
-AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef",
-    {
-        "NetworkInterfaceId": str,
-    },
-    total=False,
-)
-
 AwsEc2InstanceMetadataOptionsTypeDef = TypedDict(
     "AwsEc2InstanceMetadataOptionsTypeDef",
     {
         "HttpEndpoint": str,
         "HttpProtocolIpv6": str,
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
@@ -3130,29 +2015,14 @@
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef",
-    {
-        "DeleteOnTermination": bool,
-        "Encrypted": bool,
-        "Iops": int,
-        "KmsKeyId": str,
-        "SnapshotId": str,
-        "Throughput": int,
-        "VolumeSize": int,
-        "VolumeType": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
         "Iops": int,
         "KmsKeyId": str,
@@ -3160,169 +2030,40 @@
         "Throughput": int,
         "VolumeSize": int,
         "VolumeType": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef",
-    {
-        "CapacityReservationId": str,
-        "CapacityReservationResourceGroupArn": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef",
-    {
-        "CoreCount": int,
-        "ThreadsPerCore": int,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef",
-    {
-        "CpuCredits": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
     {
         "CpuCredits": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef",
-    {
-        "Count": int,
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef",
-    {
-        "Configured": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef",
-    {
-        "AutoRecovery": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef",
-    {
-        "HttpEndpoint": str,
-        "HttpProtocolIpv6": str,
-        "HttpTokens": str,
-        "HttpPutResponseHopLimit": int,
-        "InstanceMetadataTags": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef",
-    {
-        "Affinity": str,
-        "AvailabilityZone": str,
-        "GroupName": str,
-        "HostId": str,
-        "HostResourceGroupArn": str,
-        "PartitionNumber": int,
-        "SpreadDomain": str,
-        "Tenancy": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef",
-    {
-        "EnableResourceNameDnsAAAARecord": bool,
-        "EnableResourceNameDnsARecord": bool,
-        "HostnameType": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
@@ -3418,141 +2159,53 @@
         "EnableResourceNameDnsAAAARecord": bool,
         "EnableResourceNameDnsARecord": bool,
         "HostnameType": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef",
-    {
-        "BlockDurationMinutes": int,
-        "InstanceInterruptionBehavior": str,
-        "MaxPrice": str,
-        "SpotInstanceType": str,
-        "ValidUntil": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
     {
         "BlockDurationMinutes": int,
         "InstanceInterruptionBehavior": str,
         "MaxPrice": str,
         "SpotInstanceType": str,
         "ValidUntil": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
     {
         "Max": int,
         "Min": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef",
-        {
-            "Max": int,
-            "Min": int,
-        },
-        total=False,
-    )
-)
-
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
     {
         "Max": int,
         "Min": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef",
-        {
-            "Max": int,
-            "Min": int,
-        },
-        total=False,
-    )
-)
-
 AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
     {
         "Max": int,
         "Min": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef",
-    {
-        "Max": float,
-        "Min": float,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef",
-    {
-        "Max": float,
-        "Min": float,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
     {
         "Max": float,
         "Min": float,
     },
     total=False,
@@ -3590,47 +2243,14 @@
     {
         "Max": int,
         "Min": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef",
-    {
-        "Ipv4Prefix": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef",
-    {
-        "Ipv6Address": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef",
-    {
-        "Ipv6Prefix": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef",
-    {
-        "Primary": bool,
-        "PrivateIpAddress": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
     {
         "Ipv4Prefix": str,
     },
     total=False,
 )
@@ -3656,52 +2276,24 @@
     {
         "Primary": bool,
         "PrivateIpAddress": str,
     },
     total=False,
 )
 
-AwsEc2NetworkAclAssociationOutputTypeDef = TypedDict(
-    "AwsEc2NetworkAclAssociationOutputTypeDef",
-    {
-        "NetworkAclAssociationId": str,
-        "NetworkAclId": str,
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclAssociationTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
     total=False,
 )
 
-IcmpTypeCodeOutputTypeDef = TypedDict(
-    "IcmpTypeCodeOutputTypeDef",
-    {
-        "Code": int,
-        "Type": int,
-    },
-    total=False,
-)
-
-PortRangeFromToOutputTypeDef = TypedDict(
-    "PortRangeFromToOutputTypeDef",
-    {
-        "From": int,
-        "To": int,
-    },
-    total=False,
-)
-
 IcmpTypeCodeTypeDef = TypedDict(
     "IcmpTypeCodeTypeDef",
     {
         "Code": int,
         "Type": int,
     },
     total=False,
@@ -3712,68 +2304,28 @@
     {
         "From": int,
         "To": int,
     },
     total=False,
 )
 
-AwsEc2NetworkInterfaceAttachmentOutputTypeDef = TypedDict(
-    "AwsEc2NetworkInterfaceAttachmentOutputTypeDef",
-    {
-        "AttachTime": str,
-        "AttachmentId": str,
-        "DeleteOnTermination": bool,
-        "DeviceIndex": int,
-        "InstanceId": str,
-        "InstanceOwnerId": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkInterfaceAttachmentTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
     {
         "AttachTime": str,
         "AttachmentId": str,
         "DeleteOnTermination": bool,
         "DeviceIndex": int,
         "InstanceId": str,
         "InstanceOwnerId": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef = TypedDict(
-    "AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef",
-    {
-        "IpV6Address": str,
-    },
-    total=False,
-)
-
-AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef = TypedDict(
-    "AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef",
-    {
-        "PrivateIpAddress": str,
-        "PrivateDnsName": str,
-    },
-    total=False,
-)
-
-AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef = TypedDict(
-    "AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef",
-    {
-        "GroupName": str,
-        "GroupId": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     {
         "IpV6Address": str,
     },
     total=False,
 )
@@ -3792,45 +2344,14 @@
     {
         "GroupName": str,
         "GroupId": str,
     },
     total=False,
 )
 
-PropagatingVgwSetDetailsOutputTypeDef = TypedDict(
-    "PropagatingVgwSetDetailsOutputTypeDef",
-    {
-        "GatewayId": str,
-    },
-    total=False,
-)
-
-RouteSetDetailsOutputTypeDef = TypedDict(
-    "RouteSetDetailsOutputTypeDef",
-    {
-        "CarrierGatewayId": str,
-        "CoreNetworkArn": str,
-        "DestinationCidrBlock": str,
-        "DestinationIpv6CidrBlock": str,
-        "DestinationPrefixListId": str,
-        "EgressOnlyInternetGatewayId": str,
-        "GatewayId": str,
-        "InstanceId": str,
-        "InstanceOwnerId": str,
-        "LocalGatewayId": str,
-        "NatGatewayId": str,
-        "NetworkInterfaceId": str,
-        "Origin": str,
-        "State": str,
-        "TransitGatewayId": str,
-        "VpcPeeringConnectionId": str,
-    },
-    total=False,
-)
-
 PropagatingVgwSetDetailsTypeDef = TypedDict(
     "PropagatingVgwSetDetailsTypeDef",
     {
         "GatewayId": str,
     },
     total=False,
 )
@@ -3854,51 +2375,14 @@
         "State": str,
         "TransitGatewayId": str,
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
-AwsEc2SecurityGroupIpRangeOutputTypeDef = TypedDict(
-    "AwsEc2SecurityGroupIpRangeOutputTypeDef",
-    {
-        "CidrIp": str,
-    },
-    total=False,
-)
-
-AwsEc2SecurityGroupIpv6RangeOutputTypeDef = TypedDict(
-    "AwsEc2SecurityGroupIpv6RangeOutputTypeDef",
-    {
-        "CidrIpv6": str,
-    },
-    total=False,
-)
-
-AwsEc2SecurityGroupPrefixListIdOutputTypeDef = TypedDict(
-    "AwsEc2SecurityGroupPrefixListIdOutputTypeDef",
-    {
-        "PrefixListId": str,
-    },
-    total=False,
-)
-
-AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef = TypedDict(
-    "AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef",
-    {
-        "GroupId": str,
-        "GroupName": str,
-        "PeeringStatus": str,
-        "UserId": str,
-        "VpcId": str,
-        "VpcPeeringConnectionId": str,
-    },
-    total=False,
-)
-
 AwsEc2SecurityGroupIpRangeTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpRangeTypeDef",
     {
         "CidrIp": str,
     },
     total=False,
 )
@@ -3928,24 +2412,14 @@
         "UserId": str,
         "VpcId": str,
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
-Ipv6CidrBlockAssociationOutputTypeDef = TypedDict(
-    "Ipv6CidrBlockAssociationOutputTypeDef",
-    {
-        "AssociationId": str,
-        "Ipv6CidrBlock": str,
-        "CidrBlockState": str,
-    },
-    total=False,
-)
-
 Ipv6CidrBlockAssociationTypeDef = TypedDict(
     "Ipv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "CidrBlockState": str,
     },
@@ -3986,116 +2460,52 @@
         "DnsSupport": str,
         "MulticastSupport": str,
         "AmazonSideAsn": int,
     },
     total=False,
 )
 
-AwsEc2VolumeAttachmentOutputTypeDef = TypedDict(
-    "AwsEc2VolumeAttachmentOutputTypeDef",
-    {
-        "AttachTime": str,
-        "DeleteOnTermination": bool,
-        "InstanceId": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsEc2VolumeAttachmentTypeDef = TypedDict(
     "AwsEc2VolumeAttachmentTypeDef",
     {
         "AttachTime": str,
         "DeleteOnTermination": bool,
         "InstanceId": str,
         "Status": str,
     },
     total=False,
 )
 
-CidrBlockAssociationOutputTypeDef = TypedDict(
-    "CidrBlockAssociationOutputTypeDef",
-    {
-        "AssociationId": str,
-        "CidrBlock": str,
-        "CidrBlockState": str,
-    },
-    total=False,
-)
-
 CidrBlockAssociationTypeDef = TypedDict(
     "CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "CidrBlock": str,
         "CidrBlockState": str,
     },
     total=False,
 )
 
-AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef = TypedDict(
-    "AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef",
-    {
-        "ServiceType": str,
-    },
-    total=False,
-)
-
 AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
     {
         "ServiceType": str,
     },
     total=False,
 )
 
-AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef = TypedDict(
-    "AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef",
-    {
-        "Code": str,
-        "Message": str,
-    },
-    total=False,
-)
-
 AwsEc2VpcPeeringConnectionStatusDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-VpcInfoCidrBlockSetDetailsOutputTypeDef = TypedDict(
-    "VpcInfoCidrBlockSetDetailsOutputTypeDef",
-    {
-        "CidrBlock": str,
-    },
-    total=False,
-)
-
-VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef = TypedDict(
-    "VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef",
-    {
-        "Ipv6CidrBlock": str,
-    },
-    total=False,
-)
-
-VpcInfoPeeringOptionsDetailsOutputTypeDef = TypedDict(
-    "VpcInfoPeeringOptionsDetailsOutputTypeDef",
-    {
-        "AllowDnsResolutionFromRemoteVpc": bool,
-        "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
-        "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
-    },
-    total=False,
-)
-
 VpcInfoCidrBlockSetDetailsTypeDef = TypedDict(
     "VpcInfoCidrBlockSetDetailsTypeDef",
     {
         "CidrBlock": str,
     },
     total=False,
 )
@@ -4114,36 +2524,14 @@
         "AllowDnsResolutionFromRemoteVpc": bool,
         "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
         "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
     },
     total=False,
 )
 
-AwsEc2VpnConnectionRoutesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2VpnConnectionRoutesDetailsOutputTypeDef",
-    {
-        "DestinationCidrBlock": str,
-        "State": str,
-    },
-    total=False,
-)
-
-AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef = TypedDict(
-    "AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef",
-    {
-        "AcceptedRouteCount": int,
-        "CertificateArn": str,
-        "LastStatusChange": str,
-        "OutsideIpAddress": str,
-        "Status": str,
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
 AwsEc2VpnConnectionRoutesDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     {
         "DestinationCidrBlock": str,
         "State": str,
     },
     total=False,
@@ -4230,31 +2618,14 @@
         "ImageDigest": str,
         "ImageTags": Sequence[str],
         "ImagePublishedAt": str,
     },
     total=False,
 )
 
-AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef",
-    {
-        "ScanOnPush": bool,
-    },
-    total=False,
-)
-
-AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef = TypedDict(
-    "AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef",
-    {
-        "LifecyclePolicyText": str,
-        "RegistryId": str,
-    },
-    total=False,
-)
-
 AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef = TypedDict(
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     {
         "ScanOnPush": bool,
     },
     total=False,
 )
@@ -4264,190 +2635,81 @@
     {
         "LifecyclePolicyText": str,
         "RegistryId": str,
     },
     total=False,
 )
 
-AwsEcsClusterClusterSettingsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsClusterClusterSettingsDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsEcsClusterClusterSettingsDetailsTypeDef = TypedDict(
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef",
-        {
-            "CloudWatchEncryptionEnabled": bool,
-            "CloudWatchLogGroupName": str,
-            "S3BucketName": str,
-            "S3EncryptionEnabled": bool,
-            "S3KeyPrefix": str,
-        },
-        total=False,
-    )
-)
-
 AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
     {
         "CloudWatchEncryptionEnabled": bool,
         "CloudWatchLogGroupName": str,
         "S3BucketName": str,
         "S3EncryptionEnabled": bool,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef = TypedDict(
-    "AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef",
-    {
-        "Base": int,
-        "CapacityProvider": str,
-        "Weight": int,
-    },
-    total=False,
-)
-
 AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef = TypedDict(
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
         "Weight": int,
     },
     total=False,
 )
 
-AwsMountPointOutputTypeDef = TypedDict(
-    "AwsMountPointOutputTypeDef",
-    {
-        "SourceVolume": str,
-        "ContainerPath": str,
-    },
-    total=False,
-)
-
 AwsMountPointTypeDef = TypedDict(
     "AwsMountPointTypeDef",
     {
         "SourceVolume": str,
         "ContainerPath": str,
     },
     total=False,
 )
 
-AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef",
-    {
-        "Base": int,
-        "CapacityProvider": str,
-        "Weight": int,
-    },
-    total=False,
-)
-
 AwsEcsServiceCapacityProviderStrategyDetailsTypeDef = TypedDict(
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
         "Weight": int,
     },
     total=False,
 )
 
-AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef",
-    {
-        "Enable": bool,
-        "Rollback": bool,
-    },
-    total=False,
-)
-
 AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
     {
         "Enable": bool,
         "Rollback": bool,
     },
     total=False,
 )
 
-AwsEcsServiceDeploymentControllerDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceDeploymentControllerDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsEcsServiceDeploymentControllerDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsEcsServiceLoadBalancersDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceLoadBalancersDetailsOutputTypeDef",
-    {
-        "ContainerName": str,
-        "ContainerPort": int,
-        "LoadBalancerName": str,
-        "TargetGroupArn": str,
-    },
-    total=False,
-)
-
-AwsEcsServicePlacementConstraintsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServicePlacementConstraintsDetailsOutputTypeDef",
-    {
-        "Expression": str,
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEcsServicePlacementStrategiesDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServicePlacementStrategiesDetailsOutputTypeDef",
-    {
-        "Field": str,
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEcsServiceServiceRegistriesDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceServiceRegistriesDetailsOutputTypeDef",
-    {
-        "ContainerName": str,
-        "ContainerPort": int,
-        "Port": int,
-        "RegistryArn": str,
-    },
-    total=False,
-)
-
 AwsEcsServiceLoadBalancersDetailsTypeDef = TypedDict(
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     {
         "ContainerName": str,
         "ContainerPort": int,
         "LoadBalancerName": str,
         "TargetGroupArn": str,
@@ -4500,52 +2762,43 @@
         "AssignPublicIp": str,
         "SecurityGroups": Sequence[str],
         "Subnets": Sequence[str],
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef",
-    {
-        "Condition": str,
-        "ContainerName": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
     {
         "Condition": str,
         "ContainerName": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
     {
         "Type": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
     {
         "Hostname": str,
         "IpAddress": str,
     },
     total=False,
 )
 
@@ -4566,115 +2819,88 @@
         "Retries": int,
         "StartPeriod": int,
         "Timeout": int,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
     {
         "ContainerPath": str,
         "ReadOnly": bool,
         "SourceVolume": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
     {
         "ContainerPort": int,
         "HostPort": int,
         "Protocol": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
     {
         "CredentialsParameter": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
     {
         "Type": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
     {
         "Name": str,
         "ValueFrom": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
     {
         "Namespace": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
     {
         "HardLimit": int,
         "Name": str,
         "SoftLimit": int,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
     {
         "ReadOnly": bool,
         "SourceContainer": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
-    {
-        "Type": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
-    {
-        "Hostname": str,
-        "IpAddress": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
     {
         "Options": Mapping[str, str],
         "Type": str,
     },
     total=False,
@@ -4688,88 +2914,14 @@
         "Retries": int,
         "StartPeriod": int,
         "Timeout": int,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
-    {
-        "ContainerPath": str,
-        "ReadOnly": bool,
-        "SourceVolume": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
-    {
-        "ContainerPort": int,
-        "HostPort": int,
-        "Protocol": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
-    {
-        "CredentialsParameter": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
-    {
-        "Type": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
-    {
-        "Name": str,
-        "ValueFrom": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
-    {
-        "Namespace": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
-    {
-        "HardLimit": int,
-        "Name": str,
-        "SoftLimit": int,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
-    {
-        "ReadOnly": bool,
-        "SourceContainer": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     {
         "Add": List[str],
         "Drop": List[str],
     },
     total=False,
@@ -4820,52 +2972,23 @@
         "ContainerPath": str,
         "MountOptions": Sequence[str],
         "Size": int,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef",
-        {
-            "Name": str,
-            "ValueFrom": str,
-        },
-        total=False,
-    )
-)
-
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
     {
         "Name": str,
         "ValueFrom": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef",
-    {
-        "DeviceName": str,
-        "DeviceType": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef",
-    {
-        "Expression": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     {
         "DeviceName": str,
         "DeviceType": str,
     },
     total=False,
@@ -4876,23 +2999,14 @@
     {
         "Expression": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -4906,16 +3020,16 @@
         "DriverOpts": Dict[str, str],
         "Labels": Dict[str, str],
         "Scope": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef",
+AwsEcsTaskDefinitionVolumesHostDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
@@ -4926,50 +3040,23 @@
         "DriverOpts": Mapping[str, str],
         "Labels": Mapping[str, str],
         "Scope": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionVolumesHostDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
-    {
-        "SourcePath": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef",
-        {
-            "AccessPointId": str,
-            "Iam": str,
-        },
-        total=False,
-    )
-)
-
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     {
         "AccessPointId": str,
         "Iam": str,
     },
     total=False,
 )
 
-AwsEcsTaskVolumeHostDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskVolumeHostDetailsOutputTypeDef",
-    {
-        "SourcePath": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskVolumeHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
     total=False,
 )
@@ -4990,24 +3077,14 @@
         "Gid": str,
         "SecondaryGids": Sequence[str],
         "Uid": str,
     },
     total=False,
 )
 
-AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef = TypedDict(
-    "AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef",
-    {
-        "OwnerGid": str,
-        "OwnerUid": str,
-        "Permissions": str,
-    },
-    total=False,
-)
-
 AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
     {
         "OwnerGid": str,
         "OwnerUid": str,
         "Permissions": str,
     },
@@ -5048,44 +3125,14 @@
     {
         "Enabled": bool,
         "Types": Sequence[str],
     },
     total=False,
 )
 
-AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef = TypedDict(
-    "AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef",
-    {
-        "EnvironmentName": str,
-        "LinkName": str,
-    },
-    total=False,
-)
-
-AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef = TypedDict(
-    "AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef",
-    {
-        "Namespace": str,
-        "OptionName": str,
-        "ResourceName": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsElasticBeanstalkEnvironmentTierOutputTypeDef = TypedDict(
-    "AwsElasticBeanstalkEnvironmentTierOutputTypeDef",
-    {
-        "Name": str,
-        "Type": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     {
         "EnvironmentName": str,
         "LinkName": str,
     },
     total=False,
@@ -5108,42 +3155,42 @@
         "Name": str,
         "Type": str,
         "Version": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef",
+AwsElasticsearchDomainDomainEndpointOptionsTypeDef = TypedDict(
+    "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef",
+AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef = TypedDict(
+    "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
     {
         "Enabled": bool,
         "KmsKeyId": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef",
+AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef = TypedDict(
+    "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef",
+AwsElasticsearchDomainServiceSoftwareOptionsTypeDef = TypedDict(
+    "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
     {
         "AutomatedUpdateDate": str,
         "Cancellable": bool,
         "CurrentVersion": str,
         "Description": str,
         "NewVersion": str,
         "UpdateAvailable": bool,
@@ -5159,200 +3206,80 @@
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "VPCId": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainDomainEndpointOptionsTypeDef = TypedDict(
-    "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
-    {
-        "EnforceHTTPS": bool,
-        "TLSSecurityPolicy": str,
-    },
-    total=False,
-)
-
-AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef = TypedDict(
-    "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
-    {
-        "Enabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef = TypedDict(
-    "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsElasticsearchDomainServiceSoftwareOptionsTypeDef = TypedDict(
-    "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
-    {
-        "AutomatedUpdateDate": str,
-        "Cancellable": bool,
-        "CurrentVersion": str,
-        "Description": str,
-        "NewVersion": str,
-        "UpdateAvailable": bool,
-        "UpdateStatus": str,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainVPCOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainVPCOptionsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VPCId": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
-    {
-        "AvailabilityZoneCount": int,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
     total=False,
 )
 
-AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef",
-    {
-        "CloudWatchLogsLogGroupArn": str,
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
     },
     total=False,
 )
 
-AwsElbAppCookieStickinessPolicyOutputTypeDef = TypedDict(
-    "AwsElbAppCookieStickinessPolicyOutputTypeDef",
-    {
-        "CookieName": str,
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsElbAppCookieStickinessPolicyTypeDef = TypedDict(
     "AwsElbAppCookieStickinessPolicyTypeDef",
     {
         "CookieName": str,
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsElbLbCookieStickinessPolicyOutputTypeDef = TypedDict(
-    "AwsElbLbCookieStickinessPolicyOutputTypeDef",
-    {
-        "CookieExpirationPeriod": int,
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsElbLbCookieStickinessPolicyTypeDef = TypedDict(
     "AwsElbLbCookieStickinessPolicyTypeDef",
     {
         "CookieExpirationPeriod": int,
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsElbLoadBalancerAccessLogOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerAccessLogOutputTypeDef",
-    {
-        "EmitInterval": int,
-        "Enabled": bool,
-        "S3BucketName": str,
-        "S3BucketPrefix": str,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerAccessLogTypeDef = TypedDict(
     "AwsElbLoadBalancerAccessLogTypeDef",
     {
         "EmitInterval": int,
         "Enabled": bool,
         "S3BucketName": str,
         "S3BucketPrefix": str,
     },
     total=False,
 )
 
-AwsElbLoadBalancerAdditionalAttributeOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerAdditionalAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerAdditionalAttributeTypeDef = TypedDict(
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsElbLoadBalancerConnectionDrainingOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerConnectionDrainingOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Timeout": int,
-    },
-    total=False,
-)
-
-AwsElbLoadBalancerConnectionSettingsOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerConnectionSettingsOutputTypeDef",
-    {
-        "IdleTimeout": int,
-    },
-    total=False,
-)
-
-AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerConnectionDrainingTypeDef = TypedDict(
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     {
         "Enabled": bool,
         "Timeout": int,
     },
     total=False,
@@ -5388,43 +3315,14 @@
     {
         "InstancePort": int,
         "PolicyNames": Sequence[str],
     },
     total=False,
 )
 
-AwsElbLoadBalancerHealthCheckOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerHealthCheckOutputTypeDef",
-    {
-        "HealthyThreshold": int,
-        "Interval": int,
-        "Target": str,
-        "Timeout": int,
-        "UnhealthyThreshold": int,
-    },
-    total=False,
-)
-
-AwsElbLoadBalancerInstanceOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerInstanceOutputTypeDef",
-    {
-        "InstanceId": str,
-    },
-    total=False,
-)
-
-AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef",
-    {
-        "GroupName": str,
-        "OwnerAlias": str,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerHealthCheckTypeDef = TypedDict(
     "AwsElbLoadBalancerHealthCheckTypeDef",
     {
         "HealthyThreshold": int,
         "Interval": int,
         "Target": str,
         "Timeout": int,
@@ -5446,134 +3344,62 @@
     {
         "GroupName": str,
         "OwnerAlias": str,
     },
     total=False,
 )
 
-AwsElbLoadBalancerListenerOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerListenerOutputTypeDef",
-    {
-        "InstancePort": int,
-        "InstanceProtocol": str,
-        "LoadBalancerPort": int,
-        "Protocol": str,
-        "SslCertificateId": str,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerListenerTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerTypeDef",
     {
         "InstancePort": int,
         "InstanceProtocol": str,
         "LoadBalancerPort": int,
         "Protocol": str,
         "SslCertificateId": str,
     },
     total=False,
 )
 
-AwsElbv2LoadBalancerAttributeOutputTypeDef = TypedDict(
-    "AwsElbv2LoadBalancerAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsElbv2LoadBalancerAttributeTypeDef = TypedDict(
     "AwsElbv2LoadBalancerAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-LoadBalancerStateOutputTypeDef = TypedDict(
-    "LoadBalancerStateOutputTypeDef",
-    {
-        "Code": str,
-        "Reason": str,
-    },
-    total=False,
-)
-
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
     total=False,
 )
 
-AwsEventSchemasRegistryDetailsOutputTypeDef = TypedDict(
-    "AwsEventSchemasRegistryDetailsOutputTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-    },
-    total=False,
-)
-
 AwsEventSchemasRegistryDetailsTypeDef = TypedDict(
     "AwsEventSchemasRegistryDetailsTypeDef",
     {
         "Description": str,
         "RegistryArn": str,
         "RegistryName": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
@@ -5590,271 +3416,135 @@
     "AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef",
-    {
-        "Reason": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
     {
         "Reason": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorFeaturesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
     {
         "Name": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsIamAccessKeySessionContextAttributesOutputTypeDef = TypedDict(
-    "AwsIamAccessKeySessionContextAttributesOutputTypeDef",
-    {
-        "MfaAuthenticated": bool,
-        "CreationDate": str,
-    },
-    total=False,
-)
-
 AwsIamAccessKeySessionContextAttributesTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextAttributesTypeDef",
     {
         "MfaAuthenticated": bool,
         "CreationDate": str,
     },
     total=False,
 )
 
-AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef = TypedDict(
-    "AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef",
-    {
-        "Type": str,
-        "PrincipalId": str,
-        "Arn": str,
-        "AccountId": str,
-        "UserName": str,
-    },
-    total=False,
-)
-
 AwsIamAccessKeySessionContextSessionIssuerTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextSessionIssuerTypeDef",
     {
         "Type": str,
         "PrincipalId": str,
         "Arn": str,
         "AccountId": str,
         "UserName": str,
     },
     total=False,
 )
 
-AwsIamAttachedManagedPolicyOutputTypeDef = TypedDict(
-    "AwsIamAttachedManagedPolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-        "PolicyArn": str,
-    },
-    total=False,
-)
-
 AwsIamAttachedManagedPolicyTypeDef = TypedDict(
     "AwsIamAttachedManagedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
     total=False,
 )
 
-AwsIamGroupPolicyOutputTypeDef = TypedDict(
-    "AwsIamGroupPolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsIamGroupPolicyTypeDef = TypedDict(
     "AwsIamGroupPolicyTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsIamInstanceProfileRoleOutputTypeDef = TypedDict(
-    "AwsIamInstanceProfileRoleOutputTypeDef",
-    {
-        "Arn": str,
-        "AssumeRolePolicyDocument": str,
-        "CreateDate": str,
-        "Path": str,
-        "RoleId": str,
-        "RoleName": str,
-    },
-    total=False,
-)
-
 AwsIamInstanceProfileRoleTypeDef = TypedDict(
     "AwsIamInstanceProfileRoleTypeDef",
     {
         "Arn": str,
         "AssumeRolePolicyDocument": str,
         "CreateDate": str,
         "Path": str,
         "RoleId": str,
         "RoleName": str,
     },
     total=False,
 )
 
-AwsIamPermissionsBoundaryOutputTypeDef = TypedDict(
-    "AwsIamPermissionsBoundaryOutputTypeDef",
-    {
-        "PermissionsBoundaryArn": str,
-        "PermissionsBoundaryType": str,
-    },
-    total=False,
-)
-
 AwsIamPermissionsBoundaryTypeDef = TypedDict(
     "AwsIamPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryArn": str,
         "PermissionsBoundaryType": str,
     },
     total=False,
 )
 
-AwsIamPolicyVersionOutputTypeDef = TypedDict(
-    "AwsIamPolicyVersionOutputTypeDef",
-    {
-        "VersionId": str,
-        "IsDefaultVersion": bool,
-        "CreateDate": str,
-    },
-    total=False,
-)
-
 AwsIamPolicyVersionTypeDef = TypedDict(
     "AwsIamPolicyVersionTypeDef",
     {
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": str,
     },
     total=False,
 )
 
-AwsIamRolePolicyOutputTypeDef = TypedDict(
-    "AwsIamRolePolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsIamRolePolicyTypeDef = TypedDict(
     "AwsIamRolePolicyTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsIamUserPolicyOutputTypeDef = TypedDict(
-    "AwsIamUserPolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsIamUserPolicyTypeDef = TypedDict(
     "AwsIamUserPolicyTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef = TypedDict(
-    "AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef",
-    {
-        "EncryptionType": str,
-        "KeyId": str,
-    },
-    total=False,
-)
-
 AwsKinesisStreamStreamEncryptionDetailsTypeDef = TypedDict(
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
     {
         "EncryptionType": str,
         "KeyId": str,
     },
     total=False,
 )
 
-AwsKmsKeyDetailsOutputTypeDef = TypedDict(
-    "AwsKmsKeyDetailsOutputTypeDef",
-    {
-        "AWSAccountId": str,
-        "CreationDate": float,
-        "KeyId": str,
-        "KeyManager": str,
-        "KeyState": str,
-        "Origin": str,
-        "Description": str,
-        "KeyRotationStatus": bool,
-    },
-    total=False,
-)
-
 AwsKmsKeyDetailsTypeDef = TypedDict(
     "AwsKmsKeyDetailsTypeDef",
     {
         "AWSAccountId": str,
         "CreationDate": float,
         "KeyId": str,
         "KeyManager": str,
@@ -5862,63 +3552,44 @@
         "Origin": str,
         "Description": str,
         "KeyRotationStatus": bool,
     },
     total=False,
 )
 
-AwsLambdaFunctionCodeOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionCodeOutputTypeDef",
-    {
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3ObjectVersion": str,
-        "ZipFile": str,
-    },
-    total=False,
-)
-
 AwsLambdaFunctionCodeTypeDef = TypedDict(
     "AwsLambdaFunctionCodeTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
         "S3ObjectVersion": str,
         "ZipFile": str,
     },
     total=False,
 )
 
-AwsLambdaFunctionDeadLetterConfigOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionDeadLetterConfigOutputTypeDef",
-    {
-        "TargetArn": str,
-    },
-    total=False,
-)
-
 AwsLambdaFunctionDeadLetterConfigTypeDef = TypedDict(
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
     {
         "TargetArn": str,
     },
     total=False,
 )
 
-AwsLambdaFunctionLayerOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionLayerOutputTypeDef",
+AwsLambdaFunctionLayerTypeDef = TypedDict(
+    "AwsLambdaFunctionLayerTypeDef",
     {
         "Arn": str,
         "CodeSize": int,
     },
     total=False,
 )
 
-AwsLambdaFunctionTracingConfigOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionTracingConfigOutputTypeDef",
+AwsLambdaFunctionTracingConfigTypeDef = TypedDict(
+    "AwsLambdaFunctionTracingConfigTypeDef",
     {
         "Mode": str,
     },
     total=False,
 )
 
 AwsLambdaFunctionVpcConfigOutputTypeDef = TypedDict(
@@ -5927,50 +3598,24 @@
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "VpcId": str,
     },
     total=False,
 )
 
-AwsLambdaFunctionLayerTypeDef = TypedDict(
-    "AwsLambdaFunctionLayerTypeDef",
-    {
-        "Arn": str,
-        "CodeSize": int,
-    },
-    total=False,
-)
-
-AwsLambdaFunctionTracingConfigTypeDef = TypedDict(
-    "AwsLambdaFunctionTracingConfigTypeDef",
-    {
-        "Mode": str,
-    },
-    total=False,
-)
-
 AwsLambdaFunctionVpcConfigTypeDef = TypedDict(
     "AwsLambdaFunctionVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VpcId": str,
     },
     total=False,
 )
 
-AwsLambdaFunctionEnvironmentErrorOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionEnvironmentErrorOutputTypeDef",
-    {
-        "ErrorCode": str,
-        "Message": str,
-    },
-    total=False,
-)
-
 AwsLambdaFunctionEnvironmentErrorTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -5992,119 +3637,40 @@
         "Version": int,
         "CompatibleRuntimes": Sequence[str],
         "CreatedDate": str,
     },
     total=False,
 )
 
-AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef = TypedDict(
-    "AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef",
-    {
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
     {
         "SubnetId": str,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef",
-    {
-        "MasterUserArn": str,
-        "MasterUserName": str,
-        "MasterUserPassword": str,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
     {
         "MasterUserArn": str,
         "MasterUserName": str,
         "MasterUserPassword": str,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
-    {
-        "AvailabilityZoneCount": int,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef",
-    {
-        "CustomEndpointCertificateArn": str,
-        "CustomEndpointEnabled": bool,
-        "EnforceHTTPS": bool,
-        "CustomEndpoint": str,
-        "TLSSecurityPolicy": str,
-    },
-    total=False,
-)
-
-AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef",
-    {
-        "AutomatedUpdateDate": str,
-        "Cancellable": bool,
-        "CurrentVersion": str,
-        "Description": str,
-        "NewVersion": str,
-        "UpdateAvailable": bool,
-        "UpdateStatus": str,
-        "OptionalDeployment": bool,
-    },
-    total=False,
-)
-
-AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     {
         "CustomEndpointCertificateArn": str,
         "CustomEndpointEnabled": bool,
         "EnforceHTTPS": bool,
         "CustomEndpoint": str,
@@ -6141,99 +3707,50 @@
         "UpdateAvailable": bool,
         "UpdateStatus": str,
         "OptionalDeployment": bool,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
+AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     {
-        "SecurityGroupIds": Sequence[str],
-        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef",
+AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
     {
-        "CloudWatchLogsLogGroupArn": str,
-        "Enabled": bool,
+        "SecurityGroupIds": Sequence[str],
+        "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
 AwsOpenSearchServiceDomainLogPublishingOptionTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
     },
     total=False,
 )
 
-AwsRdsDbClusterAssociatedRoleOutputTypeDef = TypedDict(
-    "AwsRdsDbClusterAssociatedRoleOutputTypeDef",
-    {
-        "RoleArn": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRdsDbClusterAssociatedRoleTypeDef = TypedDict(
     "AwsRdsDbClusterAssociatedRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsRdsDbClusterMemberOutputTypeDef = TypedDict(
-    "AwsRdsDbClusterMemberOutputTypeDef",
-    {
-        "IsClusterWriter": bool,
-        "PromotionTier": int,
-        "DbInstanceIdentifier": str,
-        "DbClusterParameterGroupStatus": str,
-    },
-    total=False,
-)
-
-AwsRdsDbClusterOptionGroupMembershipOutputTypeDef = TypedDict(
-    "AwsRdsDbClusterOptionGroupMembershipOutputTypeDef",
-    {
-        "DbClusterOptionGroupName": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRdsDbDomainMembershipOutputTypeDef = TypedDict(
-    "AwsRdsDbDomainMembershipOutputTypeDef",
-    {
-        "Domain": str,
-        "Status": str,
-        "Fqdn": str,
-        "IamRoleName": str,
-    },
-    total=False,
-)
-
-AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef = TypedDict(
-    "AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef",
-    {
-        "VpcSecurityGroupId": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRdsDbClusterMemberTypeDef = TypedDict(
     "AwsRdsDbClusterMemberTypeDef",
     {
         "IsClusterWriter": bool,
         "PromotionTier": int,
         "DbInstanceIdentifier": str,
         "DbClusterParameterGroupStatus": str,
@@ -6284,82 +3801,24 @@
     {
         "AttributeName": str,
         "AttributeValues": Sequence[str],
     },
     total=False,
 )
 
-AwsRdsDbInstanceAssociatedRoleOutputTypeDef = TypedDict(
-    "AwsRdsDbInstanceAssociatedRoleOutputTypeDef",
-    {
-        "RoleArn": str,
-        "FeatureName": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRdsDbInstanceAssociatedRoleTypeDef = TypedDict(
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsRdsDbInstanceEndpointOutputTypeDef = TypedDict(
-    "AwsRdsDbInstanceEndpointOutputTypeDef",
-    {
-        "Address": str,
-        "Port": int,
-        "HostedZoneId": str,
-    },
-    total=False,
-)
-
-AwsRdsDbOptionGroupMembershipOutputTypeDef = TypedDict(
-    "AwsRdsDbOptionGroupMembershipOutputTypeDef",
-    {
-        "OptionGroupName": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRdsDbParameterGroupOutputTypeDef = TypedDict(
-    "AwsRdsDbParameterGroupOutputTypeDef",
-    {
-        "DbParameterGroupName": str,
-        "ParameterApplyStatus": str,
-    },
-    total=False,
-)
-
-AwsRdsDbProcessorFeatureOutputTypeDef = TypedDict(
-    "AwsRdsDbProcessorFeatureOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsRdsDbStatusInfoOutputTypeDef = TypedDict(
-    "AwsRdsDbStatusInfoOutputTypeDef",
-    {
-        "StatusType": str,
-        "Normal": bool,
-        "Status": str,
-        "Message": str,
-    },
-    total=False,
-)
-
 AwsRdsDbInstanceEndpointTypeDef = TypedDict(
     "AwsRdsDbInstanceEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
@@ -6418,34 +3877,14 @@
     {
         "LogTypesToEnable": Sequence[str],
         "LogTypesToDisable": Sequence[str],
     },
     total=False,
 )
 
-AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef = TypedDict(
-    "AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef",
-    {
-        "Ec2SecurityGroupId": str,
-        "Ec2SecurityGroupName": str,
-        "Ec2SecurityGroupOwnerId": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRdsDbSecurityGroupIpRangeOutputTypeDef = TypedDict(
-    "AwsRdsDbSecurityGroupIpRangeOutputTypeDef",
-    {
-        "CidrIp": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     {
         "Ec2SecurityGroupId": str,
         "Ec2SecurityGroupName": str,
         "Ec2SecurityGroupOwnerId": str,
         "Status": str,
@@ -6458,22 +3897,14 @@
     {
         "CidrIp": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef = TypedDict(
-    "AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
 AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -6508,213 +3939,64 @@
         "SourceType": str,
         "Status": str,
         "SubscriptionCreationTime": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterClusterNodeOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterNodeOutputTypeDef",
-    {
-        "NodeRole": str,
-        "PrivateIpAddress": str,
-        "PublicIpAddress": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterClusterNodeTypeDef = TypedDict(
     "AwsRedshiftClusterClusterNodeTypeDef",
     {
         "NodeRole": str,
         "PrivateIpAddress": str,
         "PublicIpAddress": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterClusterParameterStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterParameterStatusOutputTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterApplyStatus": str,
-        "ParameterApplyErrorDescription": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterClusterParameterStatusTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterClusterSecurityGroupOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterSecurityGroupOutputTypeDef",
-    {
-        "ClusterSecurityGroupName": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterClusterSecurityGroupTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef",
-    {
-        "DestinationRegion": str,
-        "ManualSnapshotRetentionPeriod": int,
-        "RetentionPeriod": int,
-        "SnapshotCopyGrantName": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
     {
         "DestinationRegion": str,
         "ManualSnapshotRetentionPeriod": int,
         "RetentionPeriod": int,
         "SnapshotCopyGrantName": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef",
-    {
-        "DeferMaintenanceEndTime": str,
-        "DeferMaintenanceIdentifier": str,
-        "DeferMaintenanceStartTime": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterDeferredMaintenanceWindowTypeDef = TypedDict(
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
     {
         "DeferMaintenanceEndTime": str,
         "DeferMaintenanceIdentifier": str,
         "DeferMaintenanceStartTime": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterElasticIpStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterElasticIpStatusOutputTypeDef",
-    {
-        "ElasticIp": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterEndpointOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterEndpointOutputTypeDef",
-    {
-        "Address": str,
-        "Port": int,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterHsmStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterHsmStatusOutputTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "HsmConfigurationIdentifier": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterIamRoleOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterIamRoleOutputTypeDef",
-    {
-        "ApplyStatus": str,
-        "IamRoleArn": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterLoggingStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterLoggingStatusOutputTypeDef",
-    {
-        "BucketName": str,
-        "LastFailureMessage": str,
-        "LastFailureTime": str,
-        "LastSuccessfulDeliveryTime": str,
-        "LoggingEnabled": bool,
-        "S3KeyPrefix": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterPendingModifiedValuesOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterPendingModifiedValuesOutputTypeDef",
-    {
-        "AutomatedSnapshotRetentionPeriod": int,
-        "ClusterIdentifier": str,
-        "ClusterType": str,
-        "ClusterVersion": str,
-        "EncryptionType": str,
-        "EnhancedVpcRouting": bool,
-        "MaintenanceTrackName": str,
-        "MasterUserPassword": str,
-        "NodeType": str,
-        "NumberOfNodes": int,
-        "PubliclyAccessible": bool,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterResizeInfoOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterResizeInfoOutputTypeDef",
-    {
-        "AllowCancelResize": bool,
-        "ResizeType": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterRestoreStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterRestoreStatusOutputTypeDef",
-    {
-        "CurrentRestoreRateInMegaBytesPerSecond": float,
-        "ElapsedTimeInSeconds": int,
-        "EstimatedTimeToCompletionInSeconds": int,
-        "ProgressInMegaBytes": int,
-        "SnapshotSizeInMegaBytes": int,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterVpcSecurityGroupOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterVpcSecurityGroupOutputTypeDef",
-    {
-        "Status": str,
-        "VpcSecurityGroupId": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterElasticIpStatusTypeDef = TypedDict(
     "AwsRedshiftClusterElasticIpStatusTypeDef",
     {
         "ElasticIp": str,
         "Status": str,
     },
     total=False,
@@ -6806,73 +4088,35 @@
     {
         "Status": str,
         "VpcSecurityGroupId": str,
     },
     total=False,
 )
 
-AwsS3AccountPublicAccessBlockDetailsOutputTypeDef = TypedDict(
-    "AwsS3AccountPublicAccessBlockDetailsOutputTypeDef",
-    {
-        "BlockPublicAcls": bool,
-        "BlockPublicPolicy": bool,
-        "IgnorePublicAcls": bool,
-        "RestrictPublicBuckets": bool,
-    },
-    total=False,
-)
-
 AwsS3AccountPublicAccessBlockDetailsTypeDef = TypedDict(
     "AwsS3AccountPublicAccessBlockDetailsTypeDef",
     {
         "BlockPublicAcls": bool,
         "BlockPublicPolicy": bool,
         "IgnorePublicAcls": bool,
         "RestrictPublicBuckets": bool,
     },
     total=False,
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef",
-    {
-        "DaysAfterInitiation": int,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef = (
     TypedDict(
         "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef",
         {
             "DaysAfterInitiation": int,
         },
         total=False,
     )
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef",
-    {
-        "Days": int,
-        "StorageClass": str,
-    },
-    total=False,
-)
-
-AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef",
-    {
-        "Date": str,
-        "Days": int,
-        "StorageClass": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef",
     {
         "Days": int,
         "StorageClass": str,
     },
     total=False,
@@ -6884,284 +4128,137 @@
         "Date": str,
         "Days": int,
         "StorageClass": str,
     },
     total=False,
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsS3BucketBucketVersioningConfigurationOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketVersioningConfigurationOutputTypeDef",
-    {
-        "IsMfaDeleteEnabled": bool,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketVersioningConfigurationTypeDef = TypedDict(
     "AwsS3BucketBucketVersioningConfigurationTypeDef",
     {
         "IsMfaDeleteEnabled": bool,
         "Status": str,
     },
     total=False,
 )
 
-AwsS3BucketLoggingConfigurationOutputTypeDef = TypedDict(
-    "AwsS3BucketLoggingConfigurationOutputTypeDef",
-    {
-        "DestinationBucketName": str,
-        "LogFilePrefix": str,
-    },
-    total=False,
-)
-
 AwsS3BucketLoggingConfigurationTypeDef = TypedDict(
     "AwsS3BucketLoggingConfigurationTypeDef",
     {
         "DestinationBucketName": str,
         "LogFilePrefix": str,
     },
     total=False,
 )
 
-AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef",
-    {
-        "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
     {
         "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
         "Value": str,
     },
     total=False,
 )
 
-AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef",
-    {
-        "Days": int,
-        "Mode": str,
-        "Years": int,
-    },
-    total=False,
-)
-
 AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
     {
         "Days": int,
         "Mode": str,
         "Years": int,
     },
     total=False,
 )
 
-AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef = TypedDict(
-    "AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef",
-    {
-        "SSEAlgorithm": str,
-        "KMSMasterKeyID": str,
-    },
-    total=False,
-)
-
 AwsS3BucketServerSideEncryptionByDefaultTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": str,
         "KMSMasterKeyID": str,
     },
     total=False,
 )
 
-AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef",
-    {
-        "Hostname": str,
-        "Protocol": str,
-    },
-    total=False,
-)
-
 AwsS3BucketWebsiteConfigurationRedirectToTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     {
         "Hostname": str,
         "Protocol": str,
     },
     total=False,
 )
 
-AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef",
-    {
-        "HttpErrorCodeReturnedEquals": str,
-        "KeyPrefixEquals": str,
-    },
-    total=False,
-)
-
 AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
     total=False,
 )
 
-AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef",
-    {
-        "Hostname": str,
-        "HttpRedirectCode": str,
-        "Protocol": str,
-        "ReplaceKeyPrefixWith": str,
-        "ReplaceKeyWith": str,
-    },
-    total=False,
-)
-
 AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     {
         "Hostname": str,
         "HttpRedirectCode": str,
         "Protocol": str,
         "ReplaceKeyPrefixWith": str,
         "ReplaceKeyWith": str,
     },
     total=False,
 )
 
-AwsS3ObjectDetailsOutputTypeDef = TypedDict(
-    "AwsS3ObjectDetailsOutputTypeDef",
-    {
-        "LastModified": str,
-        "ETag": str,
-        "VersionId": str,
-        "ContentType": str,
-        "ServerSideEncryption": str,
-        "SSEKMSKeyId": str,
-    },
-    total=False,
-)
-
 AwsS3ObjectDetailsTypeDef = TypedDict(
     "AwsS3ObjectDetailsTypeDef",
     {
         "LastModified": str,
         "ETag": str,
         "VersionId": str,
         "ContentType": str,
         "ServerSideEncryption": str,
         "SSEKMSKeyId": str,
     },
     total=False,
 )
 
-AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef",
-    {
-        "MinimumInstanceMetadataServiceVersion": str,
-    },
-    total=False,
-)
-
 AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     {
         "MinimumInstanceMetadataServiceVersion": str,
     },
     total=False,
 )
 
-AwsSecretsManagerSecretRotationRulesOutputTypeDef = TypedDict(
-    "AwsSecretsManagerSecretRotationRulesOutputTypeDef",
-    {
-        "AutomaticallyAfterDays": int,
-    },
-    total=False,
-)
-
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
     total=False,
 )
 
-BooleanFilterOutputTypeDef = TypedDict(
-    "BooleanFilterOutputTypeDef",
-    {
-        "Value": bool,
-    },
-    total=False,
-)
-
-IpFilterOutputTypeDef = TypedDict(
-    "IpFilterOutputTypeDef",
-    {
-        "Cidr": str,
-    },
-    total=False,
-)
-
-KeywordFilterOutputTypeDef = TypedDict(
-    "KeywordFilterOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
 BooleanFilterTypeDef = TypedDict(
     "BooleanFilterTypeDef",
     {
         "Value": bool,
     },
     total=False,
 )
@@ -7178,135 +4275,22 @@
     "KeywordFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-AwsSecurityFindingIdentifierOutputTypeDef = TypedDict(
-    "AwsSecurityFindingIdentifierOutputTypeDef",
-    {
-        "Id": str,
-        "ProductArn": str,
-    },
-)
-
 AwsSecurityFindingIdentifierTypeDef = TypedDict(
     "AwsSecurityFindingIdentifierTypeDef",
     {
         "Id": str,
         "ProductArn": str,
     },
 )
 
-_RequiredMalwareOutputTypeDef = TypedDict(
-    "_RequiredMalwareOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalMalwareOutputTypeDef = TypedDict(
-    "_OptionalMalwareOutputTypeDef",
-    {
-        "Type": MalwareTypeType,
-        "Path": str,
-        "State": MalwareStateType,
-    },
-    total=False,
-)
-
-
-class MalwareOutputTypeDef(_RequiredMalwareOutputTypeDef, _OptionalMalwareOutputTypeDef):
-    pass
-
-
-NoteOutputTypeDef = TypedDict(
-    "NoteOutputTypeDef",
-    {
-        "Text": str,
-        "UpdatedBy": str,
-        "UpdatedAt": str,
-    },
-)
-
-_RequiredPatchSummaryOutputTypeDef = TypedDict(
-    "_RequiredPatchSummaryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalPatchSummaryOutputTypeDef = TypedDict(
-    "_OptionalPatchSummaryOutputTypeDef",
-    {
-        "InstalledCount": int,
-        "MissingCount": int,
-        "FailedCount": int,
-        "InstalledOtherCount": int,
-        "InstalledRejectedCount": int,
-        "InstalledPendingReboot": int,
-        "OperationStartTime": str,
-        "OperationEndTime": str,
-        "RebootOption": str,
-        "Operation": str,
-    },
-    total=False,
-)
-
-
-class PatchSummaryOutputTypeDef(
-    _RequiredPatchSummaryOutputTypeDef, _OptionalPatchSummaryOutputTypeDef
-):
-    pass
-
-
-ProcessDetailsOutputTypeDef = TypedDict(
-    "ProcessDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Path": str,
-        "Pid": int,
-        "ParentPid": int,
-        "LaunchedAt": str,
-        "TerminatedAt": str,
-    },
-    total=False,
-)
-
-SeverityOutputTypeDef = TypedDict(
-    "SeverityOutputTypeDef",
-    {
-        "Product": float,
-        "Label": SeverityLabelType,
-        "Normalized": int,
-        "Original": str,
-    },
-    total=False,
-)
-
-ThreatIntelIndicatorOutputTypeDef = TypedDict(
-    "ThreatIntelIndicatorOutputTypeDef",
-    {
-        "Type": ThreatIntelIndicatorTypeType,
-        "Value": str,
-        "Category": ThreatIntelIndicatorCategoryType,
-        "LastObservedAt": str,
-        "Source": str,
-        "SourceUrl": str,
-    },
-    total=False,
-)
-
-WorkflowOutputTypeDef = TypedDict(
-    "WorkflowOutputTypeDef",
-    {
-        "Status": WorkflowStatusType,
-    },
-    total=False,
-)
-
 _RequiredMalwareTypeDef = TypedDict(
     "_RequiredMalwareTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalMalwareTypeDef = TypedDict(
@@ -7402,79 +4386,34 @@
     "WorkflowTypeDef",
     {
         "Status": WorkflowStatusType,
     },
     total=False,
 )
 
-AwsSnsTopicSubscriptionOutputTypeDef = TypedDict(
-    "AwsSnsTopicSubscriptionOutputTypeDef",
-    {
-        "Endpoint": str,
-        "Protocol": str,
-    },
-    total=False,
-)
-
 AwsSnsTopicSubscriptionTypeDef = TypedDict(
     "AwsSnsTopicSubscriptionTypeDef",
     {
         "Endpoint": str,
         "Protocol": str,
     },
     total=False,
 )
 
-AwsSqsQueueDetailsOutputTypeDef = TypedDict(
-    "AwsSqsQueueDetailsOutputTypeDef",
-    {
-        "KmsDataKeyReusePeriodSeconds": int,
-        "KmsMasterKeyId": str,
-        "QueueName": str,
-        "DeadLetterTargetArn": str,
-    },
-    total=False,
-)
-
 AwsSqsQueueDetailsTypeDef = TypedDict(
     "AwsSqsQueueDetailsTypeDef",
     {
         "KmsDataKeyReusePeriodSeconds": int,
         "KmsMasterKeyId": str,
         "QueueName": str,
         "DeadLetterTargetArn": str,
     },
     total=False,
 )
 
-AwsSsmComplianceSummaryOutputTypeDef = TypedDict(
-    "AwsSsmComplianceSummaryOutputTypeDef",
-    {
-        "Status": str,
-        "CompliantCriticalCount": int,
-        "CompliantHighCount": int,
-        "CompliantMediumCount": int,
-        "ExecutionType": str,
-        "NonCompliantCriticalCount": int,
-        "CompliantInformationalCount": int,
-        "NonCompliantInformationalCount": int,
-        "CompliantUnspecifiedCount": int,
-        "NonCompliantLowCount": int,
-        "NonCompliantHighCount": int,
-        "CompliantLowCount": int,
-        "ComplianceType": str,
-        "PatchBaselineId": str,
-        "OverallSeverity": str,
-        "NonCompliantMediumCount": int,
-        "NonCompliantUnspecifiedCount": int,
-        "PatchGroup": str,
-    },
-    total=False,
-)
-
 AwsSsmComplianceSummaryTypeDef = TypedDict(
     "AwsSsmComplianceSummaryTypeDef",
     {
         "Status": str,
         "CompliantCriticalCount": int,
         "CompliantHighCount": int,
         "CompliantMediumCount": int,
@@ -7492,214 +4431,102 @@
         "NonCompliantMediumCount": int,
         "NonCompliantUnspecifiedCount": int,
         "PatchGroup": str,
     },
     total=False,
 )
 
-AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef",
-    {
-        "LogGroupArn": str,
-    },
-    total=False,
-)
-
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
     {
         "LogGroupArn": str,
     },
     total=False,
 )
 
-AwsWafRateBasedRuleMatchPredicateOutputTypeDef = TypedDict(
-    "AwsWafRateBasedRuleMatchPredicateOutputTypeDef",
-    {
-        "DataId": str,
-        "Negated": bool,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef = TypedDict(
-    "AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef",
-    {
-        "DataId": str,
-        "Negated": bool,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalRulePredicateListDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalRulePredicateListDetailsOutputTypeDef",
-    {
-        "DataId": str,
-        "Negated": bool,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalRulePredicateListDetailsTypeDef = TypedDict(
     "AwsWafRegionalRulePredicateListDetailsTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalRuleGroupRulesActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesActionDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalWebAclRulesListActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRulePredicateListDetailsOutputTypeDef = TypedDict(
-    "AwsWafRulePredicateListDetailsOutputTypeDef",
-    {
-        "DataId": str,
-        "Negated": bool,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRulePredicateListDetailsTypeDef = TypedDict(
     "AwsWafRulePredicateListDetailsTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRuleGroupRulesActionDetailsOutputTypeDef = TypedDict(
-    "AwsWafRuleGroupRulesActionDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRuleGroupRulesActionDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-WafActionOutputTypeDef = TypedDict(
-    "WafActionOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
-WafExcludedRuleOutputTypeDef = TypedDict(
-    "WafExcludedRuleOutputTypeDef",
-    {
-        "RuleId": str,
-    },
-    total=False,
-)
-
-WafOverrideActionOutputTypeDef = TypedDict(
-    "WafOverrideActionOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 WafActionTypeDef = TypedDict(
     "WafActionTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
@@ -7716,78 +4543,41 @@
     "WafOverrideActionTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafv2CustomHttpHeaderOutputTypeDef = TypedDict(
-    "AwsWafv2CustomHttpHeaderOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsWafv2CustomHttpHeaderTypeDef = TypedDict(
     "AwsWafv2CustomHttpHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsWafv2VisibilityConfigDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2VisibilityConfigDetailsOutputTypeDef",
-    {
-        "CloudWatchMetricsEnabled": bool,
-        "MetricName": str,
-        "SampledRequestsEnabled": bool,
-    },
-    total=False,
-)
-
 AwsWafv2VisibilityConfigDetailsTypeDef = TypedDict(
     "AwsWafv2VisibilityConfigDetailsTypeDef",
     {
         "CloudWatchMetricsEnabled": bool,
         "MetricName": str,
         "SampledRequestsEnabled": bool,
     },
     total=False,
 )
 
-AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef",
-    {
-        "ImmunityTime": int,
-    },
-    total=False,
-)
-
 AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     {
         "ImmunityTime": int,
     },
     total=False,
 )
 
-AwsXrayEncryptionConfigDetailsOutputTypeDef = TypedDict(
-    "AwsXrayEncryptionConfigDetailsOutputTypeDef",
-    {
-        "KeyId": str,
-        "Status": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsXrayEncryptionConfigDetailsTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsTypeDef",
     {
         "KeyId": str,
         "Status": str,
         "Type": str,
     },
@@ -7966,75 +4756,34 @@
 class StandardsControlAssociationUpdateTypeDef(
     _RequiredStandardsControlAssociationUpdateTypeDef,
     _OptionalStandardsControlAssociationUpdateTypeDef,
 ):
     pass
 
 
-CellOutputTypeDef = TypedDict(
-    "CellOutputTypeDef",
-    {
-        "Column": int,
-        "Row": int,
-        "ColumnName": str,
-        "CellReference": str,
-    },
-    total=False,
-)
-
 CellTypeDef = TypedDict(
     "CellTypeDef",
     {
         "Column": int,
         "Row": int,
         "ColumnName": str,
         "CellReference": str,
     },
     total=False,
 )
 
-ClassificationStatusOutputTypeDef = TypedDict(
-    "ClassificationStatusOutputTypeDef",
-    {
-        "Code": str,
-        "Reason": str,
-    },
-    total=False,
-)
-
 ClassificationStatusTypeDef = TypedDict(
     "ClassificationStatusTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
     total=False,
 )
 
-_RequiredStatusReasonOutputTypeDef = TypedDict(
-    "_RequiredStatusReasonOutputTypeDef",
-    {
-        "ReasonCode": str,
-    },
-)
-_OptionalStatusReasonOutputTypeDef = TypedDict(
-    "_OptionalStatusReasonOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-
-class StatusReasonOutputTypeDef(
-    _RequiredStatusReasonOutputTypeDef, _OptionalStatusReasonOutputTypeDef
-):
-    pass
-
-
 _RequiredStatusReasonTypeDef = TypedDict(
     "_RequiredStatusReasonTypeDef",
     {
         "ReasonCode": str,
     },
 )
 _OptionalStatusReasonTypeDef = TypedDict(
@@ -8046,23 +4795,14 @@
 )
 
 
 class StatusReasonTypeDef(_RequiredStatusReasonTypeDef, _OptionalStatusReasonTypeDef):
     pass
 
 
-VolumeMountOutputTypeDef = TypedDict(
-    "VolumeMountOutputTypeDef",
-    {
-        "Name": str,
-        "MountPath": str,
-    },
-    total=False,
-)
-
 VolumeMountTypeDef = TypedDict(
     "VolumeMountTypeDef",
     {
         "Name": str,
         "MountPath": str,
     },
     total=False,
@@ -8104,23 +4844,14 @@
     {
         "AccountId": str,
         "ProcessingResult": str,
     },
     total=False,
 )
 
-DateRangeOutputTypeDef = TypedDict(
-    "DateRangeOutputTypeDef",
-    {
-        "Value": int,
-        "Unit": Literal["DAYS"],
-    },
-    total=False,
-)
-
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
     },
     total=False,
@@ -8322,25 +5053,14 @@
         "Tags": Mapping[str, str],
         "EnableDefaultStandards": bool,
         "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
-FilePathsOutputTypeDef = TypedDict(
-    "FilePathsOutputTypeDef",
-    {
-        "FilePath": str,
-        "FileName": str,
-        "ResourceId": str,
-        "Hash": str,
-    },
-    total=False,
-)
-
 FilePathsTypeDef = TypedDict(
     "FilePathsTypeDef",
     {
         "FilePath": str,
         "FileName": str,
         "ResourceId": str,
         "Hash": str,
@@ -8371,49 +5091,23 @@
         "UpdatedField": str,
         "OldValue": str,
         "NewValue": str,
     },
     total=False,
 )
 
-FindingProviderSeverityOutputTypeDef = TypedDict(
-    "FindingProviderSeverityOutputTypeDef",
-    {
-        "Label": SeverityLabelType,
-        "Original": str,
-    },
-    total=False,
-)
-
 FindingProviderSeverityTypeDef = TypedDict(
     "FindingProviderSeverityTypeDef",
     {
         "Label": SeverityLabelType,
         "Original": str,
     },
     total=False,
 )
 
-FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef = TypedDict(
-    "FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef",
-    {
-        "ResourceArn": str,
-    },
-    total=False,
-)
-
-FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef = TypedDict(
-    "FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef",
-    {
-        "Priority": int,
-        "ResourceArn": str,
-    },
-    total=False,
-)
-
 FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef = TypedDict(
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
@@ -8649,51 +5343,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PortRangeOutputTypeDef = TypedDict(
-    "PortRangeOutputTypeDef",
-    {
-        "Begin": int,
-        "End": int,
-    },
-    total=False,
-)
-
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "Begin": int,
         "End": int,
     },
     total=False,
 )
 
-RangeOutputTypeDef = TypedDict(
-    "RangeOutputTypeDef",
-    {
-        "Start": int,
-        "End": int,
-        "StartColumn": int,
-    },
-    total=False,
-)
-
-RecordOutputTypeDef = TypedDict(
-    "RecordOutputTypeDef",
-    {
-        "JsonPath": str,
-        "RecordIndex": int,
-    },
-    total=False,
-)
-
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Start": int,
         "End": int,
         "StartColumn": int,
     },
@@ -8705,23 +5371,14 @@
     {
         "JsonPath": str,
         "RecordIndex": int,
     },
     total=False,
 )
 
-RecommendationOutputTypeDef = TypedDict(
-    "RecommendationOutputTypeDef",
-    {
-        "Text": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": str,
         "Url": str,
     },
     total=False,
@@ -8743,16 +5400,16 @@
         "GeneratedRulesType": str,
         "TargetTypes": Sequence[str],
         "Targets": Sequence[str],
     },
     total=False,
 )
 
-RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef",
+RuleGroupSourceStatefulRulesHeaderDetailsTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
     {
         "Destination": str,
         "DestinationPort": str,
         "Direction": str,
         "Protocol": str,
         "Source": str,
         "SourcePort": str,
@@ -8765,81 +5422,51 @@
     {
         "Keyword": str,
         "Settings": List[str],
     },
     total=False,
 )
 
-RuleGroupSourceStatefulRulesHeaderDetailsTypeDef = TypedDict(
-    "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
-    {
-        "Destination": str,
-        "DestinationPort": str,
-        "Direction": str,
-        "Protocol": str,
-        "Source": str,
-        "SourcePort": str,
-    },
-    total=False,
-)
-
 RuleGroupSourceStatefulRulesOptionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     {
         "Keyword": str,
         "Settings": Sequence[str],
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef",
-    {
-        "FromPort": int,
-        "ToPort": int,
-    },
-    total=False,
-)
-
 RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef",
-    {
-        "AddressDefinition": str,
-    },
-    total=False,
-)
-
 RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     {
         "AddressDefinition": str,
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef",
+RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef",
+RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     {
         "AddressDefinition": str,
     },
     total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef = TypedDict(
@@ -8847,31 +5474,14 @@
     {
         "Flags": List[str],
         "Masks": List[str],
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
-    {
-        "FromPort": int,
-        "ToPort": int,
-    },
-    total=False,
-)
-
-RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
-    {
-        "AddressDefinition": str,
-    },
-    total=False,
-)
-
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     {
         "Flags": Sequence[str],
         "Masks": Sequence[str],
     },
     total=False,
@@ -8905,32 +5515,14 @@
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
 
-SoftwarePackageOutputTypeDef = TypedDict(
-    "SoftwarePackageOutputTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-        "Epoch": str,
-        "Release": str,
-        "Architecture": str,
-        "PackageManager": str,
-        "FilePath": str,
-        "FixedInVersion": str,
-        "Remediation": str,
-        "SourceLayerHash": str,
-        "SourceLayerArn": str,
-    },
-    total=False,
-)
-
 SoftwarePackageTypeDef = TypedDict(
     "SoftwarePackageTypeDef",
     {
         "Name": str,
         "Version": str,
         "Epoch": str,
         "Release": str,
@@ -8950,61 +5542,21 @@
     {
         "Company": str,
         "Product": str,
     },
     total=False,
 )
 
-StandardsControlAssociationIdOutputTypeDef = TypedDict(
-    "StandardsControlAssociationIdOutputTypeDef",
-    {
-        "SecurityControlId": str,
-        "StandardsArn": str,
-    },
-)
-
-_RequiredStandardsControlAssociationUpdateOutputTypeDef = TypedDict(
-    "_RequiredStandardsControlAssociationUpdateOutputTypeDef",
-    {
-        "StandardsArn": str,
-        "SecurityControlId": str,
-        "AssociationStatus": AssociationStatusType,
-    },
-)
-_OptionalStandardsControlAssociationUpdateOutputTypeDef = TypedDict(
-    "_OptionalStandardsControlAssociationUpdateOutputTypeDef",
-    {
-        "UpdatedReason": str,
-    },
-    total=False,
-)
-
-
-class StandardsControlAssociationUpdateOutputTypeDef(
-    _RequiredStandardsControlAssociationUpdateOutputTypeDef,
-    _OptionalStandardsControlAssociationUpdateOutputTypeDef,
-):
-    pass
-
-
 StandardsStatusReasonTypeDef = TypedDict(
     "StandardsStatusReasonTypeDef",
     {
         "StatusReasonCode": StatusReasonCodeType,
     },
 )
 
-StatelessCustomPublishMetricActionDimensionOutputTypeDef = TypedDict(
-    "StatelessCustomPublishMetricActionDimensionOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
 StatelessCustomPublishMetricActionDimensionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
@@ -9121,38 +5673,14 @@
 class UpdateStandardsControlRequestRequestTypeDef(
     _RequiredUpdateStandardsControlRequestRequestTypeDef,
     _OptionalUpdateStandardsControlRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredVulnerabilityVendorOutputTypeDef = TypedDict(
-    "_RequiredVulnerabilityVendorOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalVulnerabilityVendorOutputTypeDef = TypedDict(
-    "_OptionalVulnerabilityVendorOutputTypeDef",
-    {
-        "Url": str,
-        "VendorSeverity": str,
-        "VendorCreatedAt": str,
-        "VendorUpdatedAt": str,
-    },
-    total=False,
-)
-
-
-class VulnerabilityVendorOutputTypeDef(
-    _RequiredVulnerabilityVendorOutputTypeDef, _OptionalVulnerabilityVendorOutputTypeDef
-):
-    pass
-
-
 _RequiredVulnerabilityVendorTypeDef = TypedDict(
     "_RequiredVulnerabilityVendorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVulnerabilityVendorTypeDef = TypedDict(
@@ -9176,26 +5704,14 @@
 CreateMembersRequestRequestTypeDef = TypedDict(
     "CreateMembersRequestRequestTypeDef",
     {
         "AccountDetails": Sequence[AccountDetailsTypeDef],
     },
 )
 
-ActionRemoteIpDetailsOutputTypeDef = TypedDict(
-    "ActionRemoteIpDetailsOutputTypeDef",
-    {
-        "IpAddressV4": str,
-        "Organization": IpOrganizationDetailsOutputTypeDef,
-        "Country": CountryOutputTypeDef,
-        "City": CityOutputTypeDef,
-        "GeoLocation": GeoLocationOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionRemoteIpDetailsTypeDef = TypedDict(
     "ActionRemoteIpDetailsTypeDef",
     {
         "IpAddressV4": str,
         "Organization": IpOrganizationDetailsTypeDef,
         "Country": CountryTypeDef,
         "City": CityTypeDef,
@@ -9207,15 +5723,15 @@
 CvssOutputTypeDef = TypedDict(
     "CvssOutputTypeDef",
     {
         "Version": str,
         "BaseScore": float,
         "BaseVector": str,
         "Source": str,
-        "Adjustments": List[AdjustmentOutputTypeDef],
+        "Adjustments": List[AdjustmentTypeDef],
     },
     total=False,
 )
 
 CvssTypeDef = TypedDict(
     "CvssTypeDef",
     {
@@ -9224,27 +5740,14 @@
         "BaseVector": str,
         "Source": str,
         "Adjustments": Sequence[AdjustmentTypeDef],
     },
     total=False,
 )
 
-AssociationSetDetailsOutputTypeDef = TypedDict(
-    "AssociationSetDetailsOutputTypeDef",
-    {
-        "AssociationState": AssociationStateDetailsOutputTypeDef,
-        "GatewayId": str,
-        "Main": bool,
-        "RouteTableAssociationId": str,
-        "RouteTableId": str,
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AssociationSetDetailsTypeDef = TypedDict(
     "AssociationSetDetailsTypeDef",
     {
         "AssociationState": AssociationStateDetailsTypeDef,
         "GatewayId": str,
         "Main": bool,
         "RouteTableAssociationId": str,
@@ -9253,23 +5756,23 @@
     },
     total=False,
 )
 
 AutomationRulesFindingFieldsUpdateOutputTypeDef = TypedDict(
     "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     {
-        "Note": NoteUpdateOutputTypeDef,
-        "Severity": SeverityUpdateOutputTypeDef,
+        "Note": NoteUpdateTypeDef,
+        "Severity": SeverityUpdateTypeDef,
         "VerificationState": VerificationStateType,
         "Confidence": int,
         "Criticality": int,
         "Types": List[str],
         "UserDefinedFields": Dict[str, str],
-        "Workflow": WorkflowUpdateOutputTypeDef,
-        "RelatedFindings": List[RelatedFindingOutputTypeDef],
+        "Workflow": WorkflowUpdateTypeDef,
+        "RelatedFindings": List[RelatedFindingTypeDef],
     },
     total=False,
 )
 
 AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
     "AutomationRulesFindingFieldsUpdateTypeDef",
     {
@@ -9282,26 +5785,14 @@
         "UserDefinedFields": Mapping[str, str],
         "Workflow": WorkflowUpdateTypeDef,
         "RelatedFindings": Sequence[RelatedFindingTypeDef],
     },
     total=False,
 )
 
-AwsAmazonMqBrokerLogsDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerLogsDetailsOutputTypeDef",
-    {
-        "Audit": bool,
-        "General": bool,
-        "AuditLogGroup": str,
-        "GeneralLogGroup": str,
-        "Pending": AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
         "AuditLogGroup": str,
         "GeneralLogGroup": str,
@@ -9348,18 +5839,18 @@
         "DeploymentId": str,
         "ClientCertificateId": str,
         "StageName": str,
         "Description": str,
         "CacheClusterEnabled": bool,
         "CacheClusterSize": str,
         "CacheClusterStatus": str,
-        "MethodSettings": List[AwsApiGatewayMethodSettingsOutputTypeDef],
+        "MethodSettings": List[AwsApiGatewayMethodSettingsTypeDef],
         "Variables": Dict[str, str],
         "DocumentationVersion": str,
-        "AccessLogSettings": AwsApiGatewayAccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AwsApiGatewayAccessLogSettingsTypeDef,
         "CanarySettings": AwsApiGatewayCanarySettingsOutputTypeDef,
         "TracingEnabled": bool,
         "CreatedDate": str,
         "LastUpdatedDate": str,
         "WebAclArn": str,
     },
     total=False,
@@ -9424,21 +5915,21 @@
 
 AwsApiGatewayV2StageDetailsOutputTypeDef = TypedDict(
     "AwsApiGatewayV2StageDetailsOutputTypeDef",
     {
         "ClientCertificateId": str,
         "CreatedDate": str,
         "Description": str,
-        "DefaultRouteSettings": AwsApiGatewayV2RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
         "DeploymentId": str,
         "LastUpdatedDate": str,
-        "RouteSettings": AwsApiGatewayV2RouteSettingsOutputTypeDef,
+        "RouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
         "StageName": str,
         "StageVariables": Dict[str, str],
-        "AccessLogSettings": AwsApiGatewayAccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AwsApiGatewayAccessLogSettingsTypeDef,
         "AutoDeploy": bool,
         "LastDeploymentStatusMessage": str,
         "ApiGatewayManaged": bool,
     },
     total=False,
 )
 
@@ -9458,60 +5949,41 @@
         "AutoDeploy": bool,
         "LastDeploymentStatusMessage": str,
         "ApiGatewayManaged": bool,
     },
     total=False,
 )
 
-AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef",
-    {
-        "AuthenticationType": str,
-        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
-        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
-        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
     {
         "AuthenticationType": str,
         "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
         "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
         "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
     },
     total=False,
 )
 
-AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef",
-    {
-        "EncryptionConfiguration": AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
     {
         "EncryptionConfiguration": (
             AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef
         ),
     },
     total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     {
-        "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "Overrides": List[
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
         ],
     },
     total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
@@ -9520,45 +5992,25 @@
         "Overrides": Sequence[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
         ],
     },
     total=False,
 )
 
-AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef",
-    {
-        "DeviceName": str,
-        "Ebs": AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef,
-        "NoDevice": bool,
-        "VirtualName": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
         "NoDevice": bool,
         "VirtualName": str,
     },
     total=False,
 )
 
-AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef = TypedDict(
-    "AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef",
-    {
-        "DestinationBackupVaultArn": str,
-        "Lifecycle": AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     {
         "DestinationBackupVaultArn": str,
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
     },
     total=False,
@@ -9584,40 +6036,14 @@
         "EncryptionKeyArn": str,
         "Notifications": AwsBackupBackupVaultNotificationsDetailsTypeDef,
         "AccessPolicy": str,
     },
     total=False,
 )
 
-AwsBackupRecoveryPointDetailsOutputTypeDef = TypedDict(
-    "AwsBackupRecoveryPointDetailsOutputTypeDef",
-    {
-        "BackupSizeInBytes": int,
-        "BackupVaultArn": str,
-        "BackupVaultName": str,
-        "CalculatedLifecycle": AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef,
-        "CompletionDate": str,
-        "CreatedBy": AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef,
-        "CreationDate": str,
-        "EncryptionKeyArn": str,
-        "IamRoleArn": str,
-        "IsEncrypted": bool,
-        "LastRestoreTime": str,
-        "Lifecycle": AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef,
-        "RecoveryPointArn": str,
-        "ResourceArn": str,
-        "ResourceType": str,
-        "SourceBackupVaultArn": str,
-        "Status": str,
-        "StatusMessage": str,
-        "StorageClass": str,
-    },
-    total=False,
-)
-
 AwsBackupRecoveryPointDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointDetailsTypeDef",
     {
         "BackupSizeInBytes": int,
         "BackupVaultArn": str,
         "BackupVaultName": str,
         "CalculatedLifecycle": AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef,
@@ -9640,15 +6066,15 @@
     total=False,
 )
 
 AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     {
         "DomainName": str,
-        "ResourceRecord": AwsCertificateManagerCertificateResourceRecordOutputTypeDef,
+        "ResourceRecord": AwsCertificateManagerCertificateResourceRecordTypeDef,
         "ValidationDomain": str,
         "ValidationEmails": List[str],
         "ValidationMethod": str,
         "ValidationStatus": str,
     },
     total=False,
 )
@@ -9669,19 +6095,19 @@
 AwsCloudFormationStackDetailsOutputTypeDef = TypedDict(
     "AwsCloudFormationStackDetailsOutputTypeDef",
     {
         "Capabilities": List[str],
         "CreationTime": str,
         "Description": str,
         "DisableRollback": bool,
-        "DriftInformation": AwsCloudFormationStackDriftInformationDetailsOutputTypeDef,
+        "DriftInformation": AwsCloudFormationStackDriftInformationDetailsTypeDef,
         "EnableTerminationProtection": bool,
         "LastUpdatedTime": str,
         "NotificationArns": List[str],
-        "Outputs": List[AwsCloudFormationStackOutputsDetailsOutputTypeDef],
+        "Outputs": List[AwsCloudFormationStackOutputsDetailsTypeDef],
         "RoleArn": str,
         "StackId": str,
         "StackName": str,
         "StackStatus": str,
         "StackStatusReason": str,
         "TimeoutInMinutes": int,
     },
@@ -9709,15 +6135,15 @@
     },
     total=False,
 )
 
 AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     {
-        "Items": List[AwsCloudFrontDistributionCacheBehaviorOutputTypeDef],
+        "Items": List[AwsCloudFrontDistributionCacheBehaviorTypeDef],
     },
     total=False,
 )
 
 AwsCloudFrontDistributionCacheBehaviorsTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
     {
@@ -9775,15 +6201,15 @@
         "AlarmActions": List[str],
         "AlarmArn": str,
         "AlarmConfigurationUpdatedTimestamp": str,
         "AlarmDescription": str,
         "AlarmName": str,
         "ComparisonOperator": str,
         "DatapointsToAlarm": int,
-        "Dimensions": List[AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef],
+        "Dimensions": List[AwsCloudWatchAlarmDimensionsDetailsTypeDef],
         "EvaluateLowSampleCountPercentile": str,
         "EvaluationPeriods": int,
         "ExtendedStatistic": str,
         "InsufficientDataActions": List[str],
         "MetricName": str,
         "Namespace": str,
         "OkActions": List[str],
@@ -9827,19 +6253,19 @@
 )
 
 AwsCodeBuildProjectEnvironmentOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     {
         "Certificate": str,
         "EnvironmentVariables": List[
-            AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef
+            AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef
         ],
         "PrivilegedMode": bool,
         "ImagePullCredentialsType": str,
-        "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef,
+        "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 AwsCodeBuildProjectEnvironmentTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentTypeDef",
@@ -9852,23 +6278,14 @@
         "ImagePullCredentialsType": str,
         "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
         "Type": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef",
-    {
-        "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef,
-        "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectLogsConfigDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     {
         "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
         "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
     },
     total=False,
@@ -9879,27 +6296,27 @@
     {
         "Backfilling": bool,
         "IndexArn": str,
         "IndexName": str,
         "IndexSizeBytes": int,
         "IndexStatus": str,
         "ItemCount": int,
-        "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
         "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
-        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
+        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
 AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef = TypedDict(
     "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     {
         "IndexArn": str,
         "IndexName": str,
-        "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
         "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
     },
     total=False,
 )
 
 AwsDynamoDbTableGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
@@ -9924,23 +6341,14 @@
         "IndexName": str,
         "KeySchema": Sequence[AwsDynamoDbTableKeySchemaTypeDef],
         "Projection": AwsDynamoDbTableProjectionTypeDef,
     },
     total=False,
 )
 
-AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     },
     total=False,
@@ -9954,18 +6362,18 @@
         "IpV4Addresses": List[str],
         "IpV6Addresses": List[str],
         "KeyName": str,
         "IamInstanceProfileArn": str,
         "VpcId": str,
         "SubnetId": str,
         "LaunchedAt": str,
-        "NetworkInterfaces": List[AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef],
+        "NetworkInterfaces": List[AwsEc2InstanceNetworkInterfacesDetailsTypeDef],
         "VirtualizationType": str,
-        "MetadataOptions": AwsEc2InstanceMetadataOptionsOutputTypeDef,
-        "Monitoring": AwsEc2InstanceMonitoringDetailsOutputTypeDef,
+        "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
+        "Monitoring": AwsEc2InstanceMonitoringDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEc2InstanceDetailsTypeDef = TypedDict(
     "AwsEc2InstanceDetailsTypeDef",
     {
@@ -9982,106 +6390,79 @@
         "VirtualizationType": str,
         "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
         "Monitoring": AwsEc2InstanceMonitoringDetailsTypeDef,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef",
-    {
-        "DeviceName": str,
-        "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef,
-        "NoDevice": str,
-        "VirtualName": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
         "NoDevice": str,
         "VirtualName": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef",
-    {
-        "CapacityReservationPreference": str,
-        "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
     {
         "CapacityReservationPreference": str,
         "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef",
-    {
-        "MarketType": str,
-        "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
     {
         "MarketType": str,
         "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     {
         "AcceleratorCount": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
         ),
         "AcceleratorManufacturers": List[str],
         "AcceleratorNames": List[str],
-        "AcceleratorTotalMemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef,
+        "AcceleratorTotalMemoryMiB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
+        ),
         "AcceleratorTypes": List[str],
         "BareMetal": str,
         "BaselineEbsBandwidthMbps": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
         ),
         "BurstablePerformance": str,
         "CpuManufacturers": List[str],
         "ExcludedInstanceTypes": List[str],
         "InstanceGenerations": List[str],
         "LocalStorage": str,
         "LocalStorageTypes": List[str],
         "MemoryGiBPerVCpu": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
         ),
-        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef,
+        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
         "NetworkInterfaceCount": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
         ),
         "OnDemandMaxPricePercentageOverLowestPrice": int,
         "RequireHibernateSupport": bool,
         "SpotMaxPricePercentageOverLowestPrice": int,
         "TotalLocalStorageGB": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
         ),
-        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef,
+        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
     {
@@ -10129,30 +6510,26 @@
         "AssociatePublicIpAddress": bool,
         "DeleteOnTermination": bool,
         "Description": str,
         "DeviceIndex": int,
         "Groups": List[str],
         "InterfaceType": str,
         "Ipv4PrefixCount": int,
-        "Ipv4Prefixes": List[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef
-        ],
+        "Ipv4Prefixes": List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef],
         "Ipv6AddressCount": int,
         "Ipv6Addresses": List[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef
         ],
         "Ipv6PrefixCount": int,
-        "Ipv6Prefixes": List[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef
-        ],
+        "Ipv6Prefixes": List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef],
         "NetworkCardIndex": int,
         "NetworkInterfaceId": str,
         "PrivateIpAddress": str,
         "PrivateIpAddresses": List[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef
         ],
         "SecondaryPrivateIpAddressCount": int,
         "SubnetId": str,
     },
     total=False,
 )
 
@@ -10186,29 +6563,14 @@
         ],
         "SecondaryPrivateIpAddressCount": int,
         "SubnetId": str,
     },
     total=False,
 )
 
-AwsEc2NetworkAclEntryOutputTypeDef = TypedDict(
-    "AwsEc2NetworkAclEntryOutputTypeDef",
-    {
-        "CidrBlock": str,
-        "Egress": bool,
-        "IcmpTypeCode": IcmpTypeCodeOutputTypeDef,
-        "Ipv6CidrBlock": str,
-        "PortRange": PortRangeFromToOutputTypeDef,
-        "Protocol": str,
-        "RuleAction": str,
-        "RuleNumber": int,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclEntryTypeDef = TypedDict(
     "AwsEc2NetworkAclEntryTypeDef",
     {
         "CidrBlock": str,
         "Egress": bool,
         "IcmpTypeCode": IcmpTypeCodeTypeDef,
         "Ipv6CidrBlock": str,
@@ -10219,20 +6581,20 @@
     },
     total=False,
 )
 
 AwsEc2NetworkInterfaceDetailsOutputTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     {
-        "Attachment": AwsEc2NetworkInterfaceAttachmentOutputTypeDef,
+        "Attachment": AwsEc2NetworkInterfaceAttachmentTypeDef,
         "NetworkInterfaceId": str,
-        "SecurityGroups": List[AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef],
+        "SecurityGroups": List[AwsEc2NetworkInterfaceSecurityGroupTypeDef],
         "SourceDestCheck": bool,
-        "IpV6Addresses": List[AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef],
-        "PrivateIpAddresses": List[AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef],
+        "IpV6Addresses": List[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef],
+        "PrivateIpAddresses": List[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef],
         "PublicDnsName": str,
         "PublicIp": str,
     },
     total=False,
 )
 
 AwsEc2NetworkInterfaceDetailsTypeDef = TypedDict(
@@ -10252,18 +6614,18 @@
 
 AwsEc2SecurityGroupIpPermissionOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     {
         "IpProtocol": str,
         "FromPort": int,
         "ToPort": int,
-        "UserIdGroupPairs": List[AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef],
-        "IpRanges": List[AwsEc2SecurityGroupIpRangeOutputTypeDef],
-        "Ipv6Ranges": List[AwsEc2SecurityGroupIpv6RangeOutputTypeDef],
-        "PrefixListIds": List[AwsEc2SecurityGroupPrefixListIdOutputTypeDef],
+        "UserIdGroupPairs": List[AwsEc2SecurityGroupUserIdGroupPairTypeDef],
+        "IpRanges": List[AwsEc2SecurityGroupIpRangeTypeDef],
+        "Ipv6Ranges": List[AwsEc2SecurityGroupIpv6RangeTypeDef],
+        "PrefixListIds": List[AwsEc2SecurityGroupPrefixListIdTypeDef],
     },
     total=False,
 )
 
 AwsEc2SecurityGroupIpPermissionTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     {
@@ -10289,15 +6651,15 @@
         "DefaultForAz": bool,
         "MapPublicIpOnLaunch": bool,
         "OwnerId": str,
         "State": str,
         "SubnetArn": str,
         "SubnetId": str,
         "VpcId": str,
-        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationOutputTypeDef],
+        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationTypeDef],
     },
     total=False,
 )
 
 AwsEc2SubnetDetailsTypeDef = TypedDict(
     "AwsEc2SubnetDetailsTypeDef",
     {
@@ -10324,15 +6686,15 @@
         "CreateTime": str,
         "DeviceName": str,
         "Encrypted": bool,
         "Size": int,
         "SnapshotId": str,
         "Status": str,
         "KmsKeyId": str,
-        "Attachments": List[AwsEc2VolumeAttachmentOutputTypeDef],
+        "Attachments": List[AwsEc2VolumeAttachmentTypeDef],
         "VolumeId": str,
         "VolumeType": str,
         "VolumeScanStatus": str,
     },
     total=False,
 )
 
@@ -10353,16 +6715,16 @@
     },
     total=False,
 )
 
 AwsEc2VpcDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcDetailsOutputTypeDef",
     {
-        "CidrBlockAssociationSet": List[CidrBlockAssociationOutputTypeDef],
-        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationOutputTypeDef],
+        "CidrBlockAssociationSet": List[CidrBlockAssociationTypeDef],
+        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationTypeDef],
         "DhcpOptionsId": str,
         "State": str,
     },
     total=False,
 )
 
 AwsEc2VpcDetailsTypeDef = TypedDict(
@@ -10385,15 +6747,15 @@
         "ManagesVpcEndpoints": bool,
         "GatewayLoadBalancerArns": List[str],
         "NetworkLoadBalancerArns": List[str],
         "PrivateDnsName": str,
         "ServiceId": str,
         "ServiceName": str,
         "ServiceState": str,
-        "ServiceType": List[AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef],
+        "ServiceType": List[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef],
     },
     total=False,
 )
 
 AwsEc2VpcEndpointServiceDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
     {
@@ -10412,18 +6774,18 @@
     total=False,
 )
 
 AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     {
         "CidrBlock": str,
-        "CidrBlockSet": List[VpcInfoCidrBlockSetDetailsOutputTypeDef],
-        "Ipv6CidrBlockSet": List[VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef],
+        "CidrBlockSet": List[VpcInfoCidrBlockSetDetailsTypeDef],
+        "Ipv6CidrBlockSet": List[VpcInfoIpv6CidrBlockSetDetailsTypeDef],
         "OwnerId": str,
-        "PeeringOptions": VpcInfoPeeringOptionsDetailsOutputTypeDef,
+        "PeeringOptions": VpcInfoPeeringOptionsDetailsTypeDef,
         "Region": str,
         "VpcId": str,
     },
     total=False,
 )
 
 AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef = TypedDict(
@@ -10454,52 +6816,27 @@
     {
         "StaticRoutesOnly": bool,
         "TunnelOptions": Sequence[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef],
     },
     total=False,
 )
 
-AwsEcrRepositoryDetailsOutputTypeDef = TypedDict(
-    "AwsEcrRepositoryDetailsOutputTypeDef",
-    {
-        "Arn": str,
-        "ImageScanningConfiguration": (
-            AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef
-        ),
-        "ImageTagMutability": str,
-        "LifecyclePolicy": AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef,
-        "RepositoryName": str,
-        "RepositoryPolicyText": str,
-    },
-    total=False,
-)
-
 AwsEcrRepositoryDetailsTypeDef = TypedDict(
     "AwsEcrRepositoryDetailsTypeDef",
     {
         "Arn": str,
         "ImageScanningConfiguration": AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
         "ImageTagMutability": str,
         "LifecyclePolicy": AwsEcrRepositoryLifecyclePolicyDetailsTypeDef,
         "RepositoryName": str,
         "RepositoryPolicyText": str,
     },
     total=False,
 )
 
-AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef",
-    {
-        "KmsKeyId": str,
-        "LogConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef,
-        "Logging": str,
-    },
-    total=False,
-)
-
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     {
         "KmsKeyId": str,
         "LogConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
         ),
@@ -10509,15 +6846,15 @@
 )
 
 AwsEcsContainerDetailsOutputTypeDef = TypedDict(
     "AwsEcsContainerDetailsOutputTypeDef",
     {
         "Name": str,
         "Image": str,
-        "MountPoints": List[AwsMountPointOutputTypeDef],
+        "MountPoints": List[AwsMountPointTypeDef],
         "Privileged": bool,
     },
     total=False,
 )
 
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
@@ -10526,26 +6863,14 @@
         "Image": str,
         "MountPoints": Sequence[AwsMountPointTypeDef],
         "Privileged": bool,
     },
     total=False,
 )
 
-AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef",
-    {
-        "DeploymentCircuitBreaker": (
-            AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef
-        ),
-        "MaximumPercent": int,
-        "MinimumHealthyPercent": int,
-    },
-    total=False,
-)
-
 AwsEcsServiceDeploymentConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     {
         "DeploymentCircuitBreaker": (
             AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
         ),
         "MaximumPercent": int,
@@ -10614,15 +6939,15 @@
 
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     {
         "LogDriver": str,
         "Options": Dict[str, str],
         "SecretOptions": List[
-            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
         ],
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
@@ -10637,15 +6962,15 @@
 )
 
 AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     {
         "ContainerName": str,
         "ProxyConfigurationProperties": List[
-            AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef
+            AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef
         ],
         "Type": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef = TypedDict(
@@ -10656,69 +6981,37 @@
             AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef
         ],
         "Type": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef",
-    {
-        "AuthorizationConfig": (
-            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef
-        ),
-        "FilesystemId": str,
-        "RootDirectory": str,
-        "TransitEncryption": str,
-        "TransitEncryptionPort": int,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     {
         "AuthorizationConfig": (
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef
         ),
         "FilesystemId": str,
         "RootDirectory": str,
         "TransitEncryption": str,
         "TransitEncryptionPort": int,
     },
     total=False,
 )
 
-AwsEcsTaskVolumeDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskVolumeDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Host": AwsEcsTaskVolumeHostDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsEcsTaskVolumeDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeDetailsTypeDef",
     {
         "Name": str,
         "Host": AwsEcsTaskVolumeHostDetailsTypeDef,
     },
     total=False,
 )
 
-AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef = TypedDict(
-    "AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef",
-    {
-        "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef,
-        "Path": str,
-    },
-    total=False,
-)
-
 AwsEfsAccessPointRootDirectoryDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
     {
         "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
         "Path": str,
     },
     total=False,
@@ -10747,21 +7040,21 @@
         "Cname": str,
         "DateCreated": str,
         "DateUpdated": str,
         "Description": str,
         "EndpointUrl": str,
         "EnvironmentArn": str,
         "EnvironmentId": str,
-        "EnvironmentLinks": List[AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef],
+        "EnvironmentLinks": List[AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef],
         "EnvironmentName": str,
-        "OptionSettings": List[AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef],
+        "OptionSettings": List[AwsElasticBeanstalkEnvironmentOptionSettingTypeDef],
         "PlatformArn": str,
         "SolutionStackName": str,
         "Status": str,
-        "Tier": AwsElasticBeanstalkEnvironmentTierOutputTypeDef,
+        "Tier": AwsElasticBeanstalkEnvironmentTierTypeDef,
         "VersionLabel": str,
     },
     total=False,
 )
 
 AwsElasticBeanstalkEnvironmentDetailsTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
@@ -10782,30 +7075,14 @@
         "Status": str,
         "Tier": AwsElasticBeanstalkEnvironmentTierTypeDef,
         "VersionLabel": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef",
-    {
-        "DedicatedMasterCount": int,
-        "DedicatedMasterEnabled": bool,
-        "DedicatedMasterType": str,
-        "InstanceCount": int,
-        "InstanceType": str,
-        "ZoneAwarenessConfig": (
-            AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef
-        ),
-        "ZoneAwarenessEnabled": bool,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     {
         "DedicatedMasterCount": int,
         "DedicatedMasterEnabled": bool,
         "DedicatedMasterType": str,
         "InstanceCount": int,
@@ -10814,39 +7091,29 @@
             AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef
         ),
         "ZoneAwarenessEnabled": bool,
     },
     total=False,
 )
 
-AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef",
-    {
-        "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
-        "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
-        "AuditLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainLogPublishingOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     {
         "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "AuditLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
     },
     total=False,
 )
 
 AwsElbLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesOutputTypeDef",
     {
-        "AppCookieStickinessPolicies": List[AwsElbAppCookieStickinessPolicyOutputTypeDef],
-        "LbCookieStickinessPolicies": List[AwsElbLbCookieStickinessPolicyOutputTypeDef],
+        "AppCookieStickinessPolicies": List[AwsElbAppCookieStickinessPolicyTypeDef],
+        "LbCookieStickinessPolicies": List[AwsElbLbCookieStickinessPolicyTypeDef],
         "OtherPolicies": List[str],
     },
     total=False,
 )
 
 AwsElbLoadBalancerPoliciesTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesTypeDef",
@@ -10857,19 +7124,19 @@
     },
     total=False,
 )
 
 AwsElbLoadBalancerAttributesOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerAttributesOutputTypeDef",
     {
-        "AccessLog": AwsElbLoadBalancerAccessLogOutputTypeDef,
-        "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingOutputTypeDef,
-        "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsOutputTypeDef,
-        "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef,
-        "AdditionalAttributes": List[AwsElbLoadBalancerAdditionalAttributeOutputTypeDef],
+        "AccessLog": AwsElbLoadBalancerAccessLogTypeDef,
+        "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingTypeDef,
+        "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsTypeDef,
+        "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
+        "AdditionalAttributes": List[AwsElbLoadBalancerAdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 AwsElbLoadBalancerAttributesTypeDef = TypedDict(
     "AwsElbLoadBalancerAttributesTypeDef",
     {
@@ -10881,15 +7148,15 @@
     },
     total=False,
 )
 
 AwsElbLoadBalancerListenerDescriptionOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     {
-        "Listener": AwsElbLoadBalancerListenerOutputTypeDef,
+        "Listener": AwsElbLoadBalancerListenerTypeDef,
         "PolicyNames": List[str],
     },
     total=False,
 )
 
 AwsElbLoadBalancerListenerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
@@ -10899,25 +7166,25 @@
     },
     total=False,
 )
 
 AwsElbv2LoadBalancerDetailsOutputTypeDef = TypedDict(
     "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     {
-        "AvailabilityZones": List[AvailabilityZoneOutputTypeDef],
+        "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "CanonicalHostedZoneId": str,
         "CreatedTime": str,
         "DNSName": str,
         "IpAddressType": str,
         "Scheme": str,
         "SecurityGroups": List[str],
-        "State": LoadBalancerStateOutputTypeDef,
+        "State": LoadBalancerStateTypeDef,
         "Type": str,
         "VpcId": str,
-        "LoadBalancerAttributes": List[AwsElbv2LoadBalancerAttributeOutputTypeDef],
+        "LoadBalancerAttributes": List[AwsElbv2LoadBalancerAttributeTypeDef],
     },
     total=False,
 )
 
 AwsElbv2LoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbv2LoadBalancerDetailsTypeDef",
     {
@@ -10932,72 +7199,47 @@
         "Type": str,
         "VpcId": str,
         "LoadBalancerAttributes": Sequence[AwsElbv2LoadBalancerAttributeTypeDef],
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef",
-    {
-        "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
     {
         "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef",
-    {
-        "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     {
         "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
     },
     total=False,
 )
 
-AwsIamAccessKeySessionContextOutputTypeDef = TypedDict(
-    "AwsIamAccessKeySessionContextOutputTypeDef",
-    {
-        "Attributes": AwsIamAccessKeySessionContextAttributesOutputTypeDef,
-        "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsIamAccessKeySessionContextTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextTypeDef",
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     },
     total=False,
 )
 
 AwsIamGroupDetailsOutputTypeDef = TypedDict(
     "AwsIamGroupDetailsOutputTypeDef",
     {
-        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyOutputTypeDef],
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "GroupId": str,
         "GroupName": str,
-        "GroupPolicyList": List[AwsIamGroupPolicyOutputTypeDef],
+        "GroupPolicyList": List[AwsIamGroupPolicyTypeDef],
         "Path": str,
     },
     total=False,
 )
 
 AwsIamGroupDetailsTypeDef = TypedDict(
     "AwsIamGroupDetailsTypeDef",
@@ -11016,15 +7258,15 @@
     "AwsIamInstanceProfileOutputTypeDef",
     {
         "Arn": str,
         "CreateDate": str,
         "InstanceProfileId": str,
         "InstanceProfileName": str,
         "Path": str,
-        "Roles": List[AwsIamInstanceProfileRoleOutputTypeDef],
+        "Roles": List[AwsIamInstanceProfileRoleTypeDef],
     },
     total=False,
 )
 
 AwsIamInstanceProfileTypeDef = TypedDict(
     "AwsIamInstanceProfileTypeDef",
     {
@@ -11046,15 +7288,15 @@
         "DefaultVersionId": str,
         "Description": str,
         "IsAttachable": bool,
         "Path": str,
         "PermissionsBoundaryUsageCount": int,
         "PolicyId": str,
         "PolicyName": str,
-        "PolicyVersionList": List[AwsIamPolicyVersionOutputTypeDef],
+        "PolicyVersionList": List[AwsIamPolicyVersionTypeDef],
         "UpdateDate": str,
     },
     total=False,
 )
 
 AwsIamPolicyDetailsTypeDef = TypedDict(
     "AwsIamPolicyDetailsTypeDef",
@@ -11073,22 +7315,22 @@
     },
     total=False,
 )
 
 AwsIamUserDetailsOutputTypeDef = TypedDict(
     "AwsIamUserDetailsOutputTypeDef",
     {
-        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyOutputTypeDef],
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "GroupList": List[str],
         "Path": str,
-        "PermissionsBoundary": AwsIamPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AwsIamPermissionsBoundaryTypeDef,
         "UserId": str,
         "UserName": str,
-        "UserPolicyList": List[AwsIamUserPolicyOutputTypeDef],
+        "UserPolicyList": List[AwsIamUserPolicyTypeDef],
     },
     total=False,
 )
 
 AwsIamUserDetailsTypeDef = TypedDict(
     "AwsIamUserDetailsTypeDef",
     {
@@ -11100,26 +7342,14 @@
         "UserId": str,
         "UserName": str,
         "UserPolicyList": Sequence[AwsIamUserPolicyTypeDef],
     },
     total=False,
 )
 
-AwsKinesisStreamDetailsOutputTypeDef = TypedDict(
-    "AwsKinesisStreamDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "StreamEncryption": AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef,
-        "ShardCount": int,
-        "RetentionPeriodHours": int,
-    },
-    total=False,
-)
-
 AwsKinesisStreamDetailsTypeDef = TypedDict(
     "AwsKinesisStreamDetailsTypeDef",
     {
         "Name": str,
         "Arn": str,
         "StreamEncryption": AwsKinesisStreamStreamEncryptionDetailsTypeDef,
         "ShardCount": int,
@@ -11128,15 +7358,15 @@
     total=False,
 )
 
 AwsLambdaFunctionEnvironmentOutputTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentOutputTypeDef",
     {
         "Variables": Dict[str, str],
-        "Error": AwsLambdaFunctionEnvironmentErrorOutputTypeDef,
+        "Error": AwsLambdaFunctionEnvironmentErrorTypeDef,
     },
     total=False,
 )
 
 AwsLambdaFunctionEnvironmentTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentTypeDef",
     {
@@ -11153,15 +7383,15 @@
         "Description": str,
         "FirewallArn": str,
         "FirewallId": str,
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyChangeProtection": bool,
         "SubnetChangeProtection": bool,
-        "SubnetMappings": List[AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef],
+        "SubnetMappings": List[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
 AwsNetworkFirewallFirewallDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallDetailsTypeDef",
@@ -11176,53 +7406,24 @@
         "SubnetChangeProtection": bool,
         "SubnetMappings": Sequence[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "InternalUserDatabaseEnabled": bool,
-        "MasterUserOptions": AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
         "MasterUserOptions": AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef",
-    {
-        "InstanceCount": int,
-        "WarmEnabled": bool,
-        "WarmCount": int,
-        "DedicatedMasterEnabled": bool,
-        "ZoneAwarenessConfig": (
-            AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef
-        ),
-        "DedicatedMasterCount": int,
-        "InstanceType": str,
-        "WarmType": str,
-        "ZoneAwarenessEnabled": bool,
-        "DedicatedMasterType": str,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     {
         "InstanceCount": int,
         "WarmEnabled": bool,
         "WarmCount": int,
         "DedicatedMasterEnabled": bool,
@@ -11234,24 +7435,14 @@
         "WarmType": str,
         "ZoneAwarenessEnabled": bool,
         "DedicatedMasterType": str,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef",
-    {
-        "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
-        "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
-        "AuditLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
     {
         "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "AuditLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
     },
@@ -11273,34 +7464,34 @@
         "Engine": str,
         "EngineVersion": str,
         "Port": int,
         "MasterUsername": str,
         "PreferredBackupWindow": str,
         "PreferredMaintenanceWindow": str,
         "ReadReplicaIdentifiers": List[str],
-        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef],
+        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupTypeDef],
         "HostedZoneId": str,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "DbClusterResourceId": str,
-        "AssociatedRoles": List[AwsRdsDbClusterAssociatedRoleOutputTypeDef],
+        "AssociatedRoles": List[AwsRdsDbClusterAssociatedRoleTypeDef],
         "ClusterCreateTime": str,
         "EnabledCloudWatchLogsExports": List[str],
         "EngineMode": str,
         "DeletionProtection": bool,
         "HttpEndpointEnabled": bool,
         "ActivityStreamStatus": str,
         "CopyTagsToSnapshot": bool,
         "CrossAccountClone": bool,
-        "DomainMemberships": List[AwsRdsDbDomainMembershipOutputTypeDef],
+        "DomainMemberships": List[AwsRdsDbDomainMembershipTypeDef],
         "DbClusterParameterGroup": str,
         "DbSubnetGroup": str,
-        "DbClusterOptionGroupMemberships": List[AwsRdsDbClusterOptionGroupMembershipOutputTypeDef],
+        "DbClusterOptionGroupMemberships": List[AwsRdsDbClusterOptionGroupMembershipTypeDef],
         "DbClusterIdentifier": str,
-        "DbClusterMembers": List[AwsRdsDbClusterMemberOutputTypeDef],
+        "DbClusterMembers": List[AwsRdsDbClusterMemberTypeDef],
         "IamDatabaseAuthenticationEnabled": bool,
     },
     total=False,
 )
 
 AwsRdsDbClusterDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterDetailsTypeDef",
@@ -11426,15 +7617,15 @@
         "SourceDbSnapshotIdentifier": str,
         "StorageType": str,
         "TdeCredentialArn": str,
         "Encrypted": bool,
         "KmsKeyId": str,
         "Timezone": str,
         "IamDatabaseAuthenticationEnabled": bool,
-        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
         "DbiResourceId": str,
     },
     total=False,
 )
 
 AwsRdsDbSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbSnapshotDetailsTypeDef",
@@ -11483,15 +7674,15 @@
         "LicenseModel": str,
         "Iops": int,
         "DbInstanceIdentifier": str,
         "StorageType": str,
         "CaCertificateIdentifier": str,
         "DbSubnetGroupName": str,
         "PendingCloudWatchLogsExports": AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
-        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
     },
     total=False,
 )
 
 AwsRdsDbPendingModifiedValuesTypeDef = TypedDict(
     "AwsRdsDbPendingModifiedValuesTypeDef",
     {
@@ -11516,16 +7707,16 @@
 
 AwsRdsDbSecurityGroupDetailsOutputTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     {
         "DbSecurityGroupArn": str,
         "DbSecurityGroupDescription": str,
         "DbSecurityGroupName": str,
-        "Ec2SecurityGroups": List[AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef],
-        "IpRanges": List[AwsRdsDbSecurityGroupIpRangeOutputTypeDef],
+        "Ec2SecurityGroups": List[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef],
+        "IpRanges": List[AwsRdsDbSecurityGroupIpRangeTypeDef],
         "OwnerId": str,
         "VpcId": str,
     },
     total=False,
 )
 
 AwsRdsDbSecurityGroupDetailsTypeDef = TypedDict(
@@ -11538,38 +7729,28 @@
         "IpRanges": Sequence[AwsRdsDbSecurityGroupIpRangeTypeDef],
         "OwnerId": str,
         "VpcId": str,
     },
     total=False,
 )
 
-AwsRdsDbSubnetGroupSubnetOutputTypeDef = TypedDict(
-    "AwsRdsDbSubnetGroupSubnetOutputTypeDef",
-    {
-        "SubnetIdentifier": str,
-        "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef,
-        "SubnetStatus": str,
-    },
-    total=False,
-)
-
 AwsRdsDbSubnetGroupSubnetTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
     total=False,
 )
 
 AwsRedshiftClusterClusterParameterGroupOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     {
-        "ClusterParameterStatusList": List[AwsRedshiftClusterClusterParameterStatusOutputTypeDef],
+        "ClusterParameterStatusList": List[AwsRedshiftClusterClusterParameterStatusTypeDef],
         "ParameterApplyStatus": str,
         "ParameterGroupName": str,
     },
     total=False,
 )
 
 AwsRedshiftClusterClusterParameterGroupTypeDef = TypedDict(
@@ -11578,93 +7759,56 @@
         "ClusterParameterStatusList": Sequence[AwsRedshiftClusterClusterParameterStatusTypeDef],
         "ParameterApplyStatus": str,
         "ParameterGroupName": str,
     },
     total=False,
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     {
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     {
-        "FilterRules": List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef],
+        "FilterRules": List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
     total=False,
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
     total=False,
 )
 
-AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef",
-    {
-        "DefaultRetention": (
-            AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
 AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     {
         "DefaultRetention": AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
     },
     total=False,
 )
 
-AwsS3BucketServerSideEncryptionRuleOutputTypeDef = TypedDict(
-    "AwsS3BucketServerSideEncryptionRuleOutputTypeDef",
-    {
-        "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsS3BucketServerSideEncryptionRuleTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     },
     total=False,
 )
 
-AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef",
-    {
-        "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef,
-        "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     },
     total=False,
@@ -11675,15 +7819,15 @@
     {
         "AcceleratorTypes": List[str],
         "AdditionalCodeRepositories": List[str],
         "DefaultCodeRepository": str,
         "DirectInternetAccess": str,
         "FailureReason": str,
         "InstanceMetadataServiceConfiguration": (
-            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef
+            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
         ),
         "InstanceType": str,
         "KmsKeyId": str,
         "NetworkInterfaceId": str,
         "NotebookInstanceArn": str,
         "NotebookInstanceLifecycleConfigName": str,
         "NotebookInstanceName": str,
@@ -11724,29 +7868,14 @@
         "SubnetId": str,
         "Url": str,
         "VolumeSizeInGB": int,
     },
     total=False,
 )
 
-AwsSecretsManagerSecretDetailsOutputTypeDef = TypedDict(
-    "AwsSecretsManagerSecretDetailsOutputTypeDef",
-    {
-        "RotationRules": AwsSecretsManagerSecretRotationRulesOutputTypeDef,
-        "RotationOccurredWithinFrequency": bool,
-        "KmsKeyId": str,
-        "RotationEnabled": bool,
-        "RotationLambdaArn": str,
-        "Deleted": bool,
-        "Name": str,
-        "Description": str,
-    },
-    total=False,
-)
-
 AwsSecretsManagerSecretDetailsTypeDef = TypedDict(
     "AwsSecretsManagerSecretDetailsTypeDef",
     {
         "RotationRules": AwsSecretsManagerSecretRotationRulesTypeDef,
         "RotationOccurredWithinFrequency": bool,
         "KmsKeyId": str,
         "RotationEnabled": bool,
@@ -11754,23 +7883,14 @@
         "Deleted": bool,
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-BatchUpdateFindingsUnprocessedFindingTypeDef = TypedDict(
-    "BatchUpdateFindingsUnprocessedFindingTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierOutputTypeDef,
-        "ErrorCode": str,
-        "ErrorMessage": str,
-    },
-)
-
 _RequiredBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateFindingsRequestRequestTypeDef",
     {
         "FindingIdentifiers": Sequence[AwsSecurityFindingIdentifierTypeDef],
     },
 )
 _OptionalBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
@@ -11793,14 +7913,23 @@
 class BatchUpdateFindingsRequestRequestTypeDef(
     _RequiredBatchUpdateFindingsRequestRequestTypeDef,
     _OptionalBatchUpdateFindingsRequestRequestTypeDef,
 ):
     pass
 
 
+BatchUpdateFindingsUnprocessedFindingTypeDef = TypedDict(
+    "BatchUpdateFindingsUnprocessedFindingTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+)
+
 _RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingHistoryRequestRequestTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
     },
 )
 _OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
@@ -11821,15 +7950,15 @@
     pass
 
 
 AwsSnsTopicDetailsOutputTypeDef = TypedDict(
     "AwsSnsTopicDetailsOutputTypeDef",
     {
         "KmsMasterKeyId": str,
-        "Subscription": List[AwsSnsTopicSubscriptionOutputTypeDef],
+        "Subscription": List[AwsSnsTopicSubscriptionTypeDef],
         "TopicName": str,
         "Owner": str,
         "SqsSuccessFeedbackRoleArn": str,
         "SqsFailureFeedbackRoleArn": str,
         "ApplicationSuccessFeedbackRoleArn": str,
         "FirehoseSuccessFeedbackRoleArn": str,
         "FirehoseFailureFeedbackRoleArn": str,
@@ -11853,38 +7982,22 @@
         "FirehoseFailureFeedbackRoleArn": str,
         "HttpSuccessFeedbackRoleArn": str,
         "HttpFailureFeedbackRoleArn": str,
     },
     total=False,
 )
 
-AwsSsmPatchOutputTypeDef = TypedDict(
-    "AwsSsmPatchOutputTypeDef",
-    {
-        "ComplianceSummary": AwsSsmComplianceSummaryOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsSsmPatchTypeDef = TypedDict(
     "AwsSsmPatchTypeDef",
     {
         "ComplianceSummary": AwsSsmComplianceSummaryTypeDef,
     },
     total=False,
 )
 
-AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef",
-    {
-        "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     {
         "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     },
     total=False,
 )
@@ -11893,15 +8006,15 @@
     "AwsWafRateBasedRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
-        "MatchPredicates": List[AwsWafRateBasedRuleMatchPredicateOutputTypeDef],
+        "MatchPredicates": List[AwsWafRateBasedRuleMatchPredicateTypeDef],
     },
     total=False,
 )
 
 AwsWafRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRateBasedRuleDetailsTypeDef",
     {
@@ -11919,15 +8032,15 @@
     "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
-        "MatchPredicates": List[AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef],
+        "MatchPredicates": List[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef],
     },
     total=False,
 )
 
 AwsWafRegionalRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     {
@@ -11942,15 +8055,15 @@
 )
 
 AwsWafRegionalRuleDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
-        "PredicateList": List[AwsWafRegionalRulePredicateListDetailsOutputTypeDef],
+        "PredicateList": List[AwsWafRegionalRulePredicateListDetailsTypeDef],
         "RuleId": str,
     },
     total=False,
 )
 
 AwsWafRegionalRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleDetailsTypeDef",
@@ -11959,48 +8072,25 @@
         "Name": str,
         "PredicateList": Sequence[AwsWafRegionalRulePredicateListDetailsTypeDef],
         "RuleId": str,
     },
     total=False,
 )
 
-AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef",
-    {
-        "Action": AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef,
-        "Priority": int,
-        "RuleId": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalRuleGroupRulesDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     {
         "Action": AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalWebAclRulesListDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalWebAclRulesListDetailsOutputTypeDef",
-    {
-        "Action": AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef,
-        "OverrideAction": AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef,
-        "Priority": int,
-        "RuleId": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalWebAclRulesListDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     {
         "Action": AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
         "OverrideAction": AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
         "Priority": int,
         "RuleId": str,
@@ -12010,15 +8100,15 @@
 )
 
 AwsWafRuleDetailsOutputTypeDef = TypedDict(
     "AwsWafRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
-        "PredicateList": List[AwsWafRulePredicateListDetailsOutputTypeDef],
+        "PredicateList": List[AwsWafRulePredicateListDetailsTypeDef],
         "RuleId": str,
     },
     total=False,
 )
 
 AwsWafRuleDetailsTypeDef = TypedDict(
     "AwsWafRuleDetailsTypeDef",
@@ -12027,42 +8117,31 @@
         "Name": str,
         "PredicateList": Sequence[AwsWafRulePredicateListDetailsTypeDef],
         "RuleId": str,
     },
     total=False,
 )
 
-AwsWafRuleGroupRulesDetailsOutputTypeDef = TypedDict(
-    "AwsWafRuleGroupRulesDetailsOutputTypeDef",
-    {
-        "Action": AwsWafRuleGroupRulesActionDetailsOutputTypeDef,
-        "Priority": int,
-        "RuleId": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRuleGroupRulesDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupRulesDetailsTypeDef",
     {
         "Action": AwsWafRuleGroupRulesActionDetailsTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
 AwsWafWebAclRuleOutputTypeDef = TypedDict(
     "AwsWafWebAclRuleOutputTypeDef",
     {
-        "Action": WafActionOutputTypeDef,
-        "ExcludedRules": List[WafExcludedRuleOutputTypeDef],
-        "OverrideAction": WafOverrideActionOutputTypeDef,
+        "Action": WafActionTypeDef,
+        "ExcludedRules": List[WafExcludedRuleTypeDef],
+        "OverrideAction": WafOverrideActionTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
@@ -12078,51 +8157,43 @@
     },
     total=False,
 )
 
 AwsWafv2CustomRequestHandlingDetailsOutputTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     {
-        "InsertHeaders": List[AwsWafv2CustomHttpHeaderOutputTypeDef],
-    },
-    total=False,
-)
-
-AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2CustomResponseDetailsOutputTypeDef",
-    {
-        "CustomResponseBodyKey": str,
-        "ResponseCode": int,
-        "ResponseHeaders": List[AwsWafv2CustomHttpHeaderOutputTypeDef],
+        "InsertHeaders": List[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
 AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
         "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
-AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
-    "AwsWafv2CustomResponseDetailsTypeDef",
+AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     {
         "CustomResponseBodyKey": str,
         "ResponseCode": int,
-        "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
+        "ResponseHeaders": List[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
-AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef",
+AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsTypeDef",
     {
-        "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef,
+        "CustomResponseBodyKey": str,
+        "ResponseCode": int,
+        "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
 AwsWafv2WebAclCaptchaConfigDetailsTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     {
@@ -12322,14 +8393,37 @@
 BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
     },
 )
 
+_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
+    {
+        "StandardsControlAssociationId": StandardsControlAssociationIdTypeDef,
+        "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
+    {
+        "ErrorReason": str,
+    },
+    total=False,
+)
+
+
+class UnprocessedStandardsControlAssociationTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationTypeDef,
+):
+    pass
+
+
 BatchImportFindingsResponseTypeDef = TypedDict(
     "BatchImportFindingsResponseTypeDef",
     {
         "FailedCount": int,
         "SuccessCount": int,
         "FailedFindings": List[ImportFindingsErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -12339,22 +8433,45 @@
 BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationUpdates": Sequence[StandardsControlAssociationUpdateTypeDef],
     },
 )
 
+_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
+    {
+        "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateTypeDef,
+        "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
+    {
+        "ErrorReason": str,
+    },
+    total=False,
+)
+
+
+class UnprocessedStandardsControlAssociationUpdateTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
+):
+    pass
+
+
 ComplianceOutputTypeDef = TypedDict(
     "ComplianceOutputTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": List[str],
-        "StatusReasons": List[StatusReasonOutputTypeDef],
+        "StatusReasons": List[StatusReasonTypeDef],
         "SecurityControlId": str,
-        "AssociatedStandards": List[AssociatedStandardOutputTypeDef],
+        "AssociatedStandards": List[AssociatedStandardTypeDef],
     },
     total=False,
 )
 
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
@@ -12371,15 +8488,15 @@
     "ContainerDetailsOutputTypeDef",
     {
         "ContainerRuntime": str,
         "Name": str,
         "ImageId": str,
         "ImageName": str,
         "LaunchedAt": str,
-        "VolumeMounts": List[VolumeMountOutputTypeDef],
+        "VolumeMounts": List[VolumeMountTypeDef],
         "Privileged": bool,
     },
     total=False,
 )
 
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
@@ -12431,24 +8548,14 @@
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DateFilterOutputTypeDef = TypedDict(
-    "DateFilterOutputTypeDef",
-    {
-        "Start": str,
-        "End": str,
-        "DateRange": DateRangeOutputTypeDef,
-    },
-    total=False,
-)
-
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "Start": str,
         "End": str,
         "DateRange": DateRangeTypeDef,
     },
@@ -12637,15 +8744,15 @@
 
 ThreatOutputTypeDef = TypedDict(
     "ThreatOutputTypeDef",
     {
         "Name": str,
         "Severity": str,
         "ItemCount": int,
-        "FilePaths": List[FilePathsOutputTypeDef],
+        "FilePaths": List[FilePathsTypeDef],
     },
     total=False,
 )
 
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
@@ -12665,31 +8772,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingHistoryRecordTypeDef = TypedDict(
     "FindingHistoryRecordTypeDef",
     {
-        "FindingIdentifier": AwsSecurityFindingIdentifierOutputTypeDef,
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "UpdateTime": datetime,
         "FindingCreated": bool,
         "UpdateSource": FindingHistoryUpdateSourceTypeDef,
         "Updates": List[FindingHistoryUpdateTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
 FindingProviderFieldsOutputTypeDef = TypedDict(
     "FindingProviderFieldsOutputTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
-        "RelatedFindings": List[RelatedFindingOutputTypeDef],
-        "Severity": FindingProviderSeverityOutputTypeDef,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+        "Severity": FindingProviderSeverityTypeDef,
         "Types": List[str],
     },
     total=False,
 )
 
 FindingProviderFieldsTypeDef = TypedDict(
     "FindingProviderFieldsTypeDef",
@@ -12769,38 +8876,19 @@
     {
         "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkOutputTypeDef = TypedDict(
-    "NetworkOutputTypeDef",
-    {
-        "Direction": NetworkDirectionType,
-        "Protocol": str,
-        "OpenPortRange": PortRangeOutputTypeDef,
-        "SourceIpV4": str,
-        "SourceIpV6": str,
-        "SourcePort": int,
-        "SourceDomain": str,
-        "SourceMac": str,
-        "DestinationIpV4": str,
-        "DestinationIpV6": str,
-        "DestinationPort": int,
-        "DestinationDomain": str,
-    },
-    total=False,
-)
-
 NetworkPathComponentDetailsOutputTypeDef = TypedDict(
     "NetworkPathComponentDetailsOutputTypeDef",
     {
         "Address": List[str],
-        "PortRanges": List[PortRangeOutputTypeDef],
+        "PortRanges": List[PortRangeTypeDef],
     },
     total=False,
 )
 
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
@@ -12825,55 +8913,37 @@
         "DestinationIpV6": str,
         "DestinationPort": int,
         "DestinationDomain": str,
     },
     total=False,
 )
 
-PageOutputTypeDef = TypedDict(
-    "PageOutputTypeDef",
-    {
-        "PageNumber": int,
-        "LineRange": RangeOutputTypeDef,
-        "OffsetRange": RangeOutputTypeDef,
-    },
-    total=False,
-)
-
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
         "PageNumber": int,
         "LineRange": RangeTypeDef,
         "OffsetRange": RangeTypeDef,
     },
     total=False,
 )
 
-RemediationOutputTypeDef = TypedDict(
-    "RemediationOutputTypeDef",
-    {
-        "Recommendation": RecommendationOutputTypeDef,
-    },
-    total=False,
-)
-
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "Recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
 RuleGroupSourceStatefulRulesDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     {
         "Action": str,
-        "Header": RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef,
+        "Header": RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
         "RuleOptions": List[RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef],
     },
     total=False,
 )
 
 RuleGroupSourceStatefulRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
@@ -12885,20 +8955,20 @@
     total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
     {
         "DestinationPorts": List[
-            RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef
+            RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef
         ],
-        "Destinations": List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef],
+        "Destinations": List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef],
         "Protocols": List[int],
-        "SourcePorts": List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef],
-        "Sources": List[RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef],
+        "SourcePorts": List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef],
+        "Sources": List[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef],
         "TcpFlags": List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef],
     },
     total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
@@ -12941,60 +9011,14 @@
         "Description": str,
         "EnabledByDefault": bool,
         "StandardsManagedBy": StandardsManagedByTypeDef,
     },
     total=False,
 )
 
-_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
-    {
-        "StandardsControlAssociationId": StandardsControlAssociationIdOutputTypeDef,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-
-class UnprocessedStandardsControlAssociationTypeDef(
-    _RequiredUnprocessedStandardsControlAssociationTypeDef,
-    _OptionalUnprocessedStandardsControlAssociationTypeDef,
-):
-    pass
-
-
-_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
-    {
-        "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateOutputTypeDef,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-
-class UnprocessedStandardsControlAssociationUpdateTypeDef(
-    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
-    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
-):
-    pass
-
-
 _RequiredStandardsSubscriptionTypeDef = TypedDict(
     "_RequiredStandardsSubscriptionTypeDef",
     {
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
@@ -13014,15 +9038,15 @@
 ):
     pass
 
 
 StatelessCustomPublishMetricActionOutputTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionOutputTypeDef",
     {
-        "Dimensions": List[StatelessCustomPublishMetricActionDimensionOutputTypeDef],
+        "Dimensions": List[StatelessCustomPublishMetricActionDimensionTypeDef],
     },
     total=False,
 )
 
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
@@ -13033,46 +9057,23 @@
 
 AwsApiCallActionOutputTypeDef = TypedDict(
     "AwsApiCallActionOutputTypeDef",
     {
         "Api": str,
         "ServiceName": str,
         "CallerType": str,
-        "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
-        "DomainDetails": AwsApiCallActionDomainDetailsOutputTypeDef,
+        "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
+        "DomainDetails": AwsApiCallActionDomainDetailsTypeDef,
         "AffectedResources": Dict[str, str],
         "FirstSeen": str,
         "LastSeen": str,
     },
     total=False,
 )
 
-NetworkConnectionActionOutputTypeDef = TypedDict(
-    "NetworkConnectionActionOutputTypeDef",
-    {
-        "ConnectionDirection": str,
-        "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
-        "RemotePortDetails": ActionRemotePortDetailsOutputTypeDef,
-        "LocalPortDetails": ActionLocalPortDetailsOutputTypeDef,
-        "Protocol": str,
-        "Blocked": bool,
-    },
-    total=False,
-)
-
-PortProbeDetailOutputTypeDef = TypedDict(
-    "PortProbeDetailOutputTypeDef",
-    {
-        "LocalPortDetails": ActionLocalPortDetailsOutputTypeDef,
-        "LocalIpDetails": ActionLocalIpDetailsOutputTypeDef,
-        "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsApiCallActionTypeDef = TypedDict(
     "AwsApiCallActionTypeDef",
     {
         "Api": str,
         "ServiceName": str,
         "CallerType": str,
         "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
@@ -13112,18 +9113,18 @@
     {
         "Id": str,
     },
 )
 _OptionalVulnerabilityOutputTypeDef = TypedDict(
     "_OptionalVulnerabilityOutputTypeDef",
     {
-        "VulnerablePackages": List[SoftwarePackageOutputTypeDef],
+        "VulnerablePackages": List[SoftwarePackageTypeDef],
         "Cvss": List[CvssOutputTypeDef],
         "RelatedVulnerabilities": List[str],
-        "Vendor": VulnerabilityVendorOutputTypeDef,
+        "Vendor": VulnerabilityVendorTypeDef,
         "ReferenceUrls": List[str],
         "FixAvailable": VulnerabilityFixAvailableType,
     },
     total=False,
 )
 
 
@@ -13156,19 +9157,19 @@
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
 
 AwsEc2RouteTableDetailsOutputTypeDef = TypedDict(
     "AwsEc2RouteTableDetailsOutputTypeDef",
     {
-        "AssociationSet": List[AssociationSetDetailsOutputTypeDef],
+        "AssociationSet": List[AssociationSetDetailsTypeDef],
         "OwnerId": str,
-        "PropagatingVgwSet": List[PropagatingVgwSetDetailsOutputTypeDef],
+        "PropagatingVgwSet": List[PropagatingVgwSetDetailsTypeDef],
         "RouteTableId": str,
-        "RouteSet": List[RouteSetDetailsOutputTypeDef],
+        "RouteSet": List[RouteSetDetailsTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
 AwsEc2RouteTableDetailsTypeDef = TypedDict(
     "AwsEc2RouteTableDetailsTypeDef",
@@ -13205,29 +9206,27 @@
     "AwsAmazonMqBrokerDetailsOutputTypeDef",
     {
         "AuthenticationStrategy": str,
         "AutoMinorVersionUpgrade": bool,
         "BrokerArn": str,
         "BrokerName": str,
         "DeploymentMode": str,
-        "EncryptionOptions": AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef,
+        "EncryptionOptions": AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
         "EngineType": str,
         "EngineVersion": str,
         "HostInstanceType": str,
         "BrokerId": str,
         "LdapServerMetadata": AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
-        "Logs": AwsAmazonMqBrokerLogsDetailsOutputTypeDef,
-        "MaintenanceWindowStartTime": (
-            AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef
-        ),
+        "Logs": AwsAmazonMqBrokerLogsDetailsTypeDef,
+        "MaintenanceWindowStartTime": AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
         "StorageType": str,
         "SubnetIds": List[str],
-        "Users": List[AwsAmazonMqBrokerUsersDetailsOutputTypeDef],
+        "Users": List[AwsAmazonMqBrokerUsersDetailsTypeDef],
     },
     total=False,
 )
 
 AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerDetailsTypeDef",
     {
@@ -13254,24 +9253,24 @@
 )
 
 AwsAppSyncGraphQlApiDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     {
         "ApiId": str,
         "Id": str,
-        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
+        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
         "Name": str,
-        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
+        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
         "XrayEnabled": bool,
         "Arn": str,
-        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
+        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
         "AuthenticationType": str,
-        "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef,
+        "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
         "AdditionalAuthenticationProviders": List[
-            AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef
+            AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
         ],
         "WafWebAclArn": str,
     },
     total=False,
 )
 
 AwsAppSyncGraphQlApiDetailsTypeDef = TypedDict(
@@ -13291,36 +9290,28 @@
             AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
         ],
         "WafWebAclArn": str,
     },
     total=False,
 )
 
-AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef",
-    {
-        "ResultConfiguration": (
-            AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
 AwsAthenaWorkGroupConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
     {
         "ResultConfiguration": AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef,
     },
     total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     {
-        "InstancesDistribution": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef,
+        "InstancesDistribution": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
+        ),
         "LaunchTemplate": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef
         ),
     },
     total=False,
 )
 
@@ -13338,35 +9329,33 @@
 )
 
 AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BlockDeviceMappings": List[
-            AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef
+            AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef
         ],
         "ClassicLinkVpcId": str,
         "ClassicLinkVpcSecurityGroups": List[str],
         "CreatedTime": str,
         "EbsOptimized": bool,
         "IamInstanceProfile": str,
         "ImageId": str,
-        "InstanceMonitoring": (
-            AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef
-        ),
+        "InstanceMonitoring": AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
         "InstanceType": str,
         "KernelId": str,
         "KeyName": str,
         "LaunchConfigurationName": str,
         "PlacementTenancy": str,
         "RamdiskId": str,
         "SecurityGroups": List[str],
         "SpotPrice": str,
         "UserData": str,
-        "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef,
+        "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
     },
     total=False,
 )
 
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
@@ -13401,16 +9390,16 @@
         "TargetBackupVault": str,
         "StartWindowMinutes": int,
         "ScheduleExpression": str,
         "RuleName": str,
         "RuleId": str,
         "EnableContinuousBackup": bool,
         "CompletionWindowMinutes": int,
-        "CopyActions": List[AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef],
-        "Lifecycle": AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
+        "CopyActions": List[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef],
+        "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
     },
     total=False,
 )
 
 AwsBackupBackupPlanRuleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     {
@@ -13455,15 +9444,15 @@
 
 AwsCloudFrontDistributionOriginItemOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemOutputTypeDef",
     {
         "DomainName": str,
         "Id": str,
         "OriginPath": str,
-        "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef,
+        "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
         "CustomOriginConfig": AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
     },
     total=False,
 )
 
 AwsCloudFrontDistributionOriginItemTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemTypeDef",
@@ -13493,22 +9482,22 @@
     total=False,
 )
 
 AwsCodeBuildProjectDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsOutputTypeDef",
     {
         "EncryptionKey": str,
-        "Artifacts": List[AwsCodeBuildProjectArtifactsDetailsOutputTypeDef],
+        "Artifacts": List[AwsCodeBuildProjectArtifactsDetailsTypeDef],
         "Environment": AwsCodeBuildProjectEnvironmentOutputTypeDef,
         "Name": str,
-        "Source": AwsCodeBuildProjectSourceOutputTypeDef,
+        "Source": AwsCodeBuildProjectSourceTypeDef,
         "ServiceRole": str,
-        "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef,
+        "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsTypeDef,
         "VpcConfig": AwsCodeBuildProjectVpcConfigOutputTypeDef,
-        "SecondaryArtifacts": List[AwsCodeBuildProjectArtifactsDetailsOutputTypeDef],
+        "SecondaryArtifacts": List[AwsCodeBuildProjectArtifactsDetailsTypeDef],
     },
     total=False,
 )
 
 AwsCodeBuildProjectDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsTypeDef",
     {
@@ -13524,17 +9513,17 @@
     },
     total=False,
 )
 
 AwsDynamoDbTableReplicaOutputTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaOutputTypeDef",
     {
-        "GlobalSecondaryIndexes": List[AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef],
+        "GlobalSecondaryIndexes": List[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef],
         "KmsMasterKeyId": str,
-        "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
+        "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
     total=False,
 )
 
@@ -13550,50 +9539,48 @@
     },
     total=False,
 )
 
 AwsEc2LaunchTemplateDataDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
     {
-        "BlockDeviceMappingSet": List[
-            AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef
-        ],
+        "BlockDeviceMappingSet": List[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef],
         "CapacityReservationSpecification": (
-            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
         ),
-        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef,
-        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef,
+        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
         "DisableApiStop": bool,
         "DisableApiTermination": bool,
         "EbsOptimized": bool,
         "ElasticGpuSpecificationSet": List[
-            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef
         ],
         "ElasticInferenceAcceleratorSet": List[
-            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef
         ],
-        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef,
-        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef,
-        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef,
+        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
         "ImageId": str,
         "InstanceInitiatedShutdownBehavior": str,
-        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef,
+        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
         "InstanceRequirements": AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
         "InstanceType": str,
         "KernelId": str,
         "KeyName": str,
-        "LicenseSet": List[AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef],
-        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef,
-        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef,
-        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef,
+        "LicenseSet": List[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef],
+        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
         "NetworkInterfaceSet": List[
             AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef
         ],
-        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef,
-        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef,
+        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
         "RamDiskId": str,
         "SecurityGroupIdSet": List[str],
         "SecurityGroupSet": List[str],
         "UserData": str,
     },
     total=False,
 )
@@ -13646,16 +9633,16 @@
 AwsEc2NetworkAclDetailsOutputTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsOutputTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
-        "Associations": List[AwsEc2NetworkAclAssociationOutputTypeDef],
-        "Entries": List[AwsEc2NetworkAclEntryOutputTypeDef],
+        "Associations": List[AwsEc2NetworkAclAssociationTypeDef],
+        "Entries": List[AwsEc2NetworkAclEntryTypeDef],
     },
     total=False,
 )
 
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
@@ -13697,15 +9684,15 @@
 
 AwsEc2VpcPeeringConnectionDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     {
         "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
         "ExpirationTime": str,
         "RequesterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
-        "Status": AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef,
+        "Status": AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
 AwsEc2VpcPeeringConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
@@ -13725,17 +9712,17 @@
         "VpnConnectionId": str,
         "State": str,
         "CustomerGatewayId": str,
         "CustomerGatewayConfiguration": str,
         "Type": str,
         "VpnGatewayId": str,
         "Category": str,
-        "VgwTelemetry": List[AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef],
+        "VgwTelemetry": List[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef],
         "Options": AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
-        "Routes": List[AwsEc2VpnConnectionRoutesDetailsOutputTypeDef],
+        "Routes": List[AwsEc2VpnConnectionRoutesDetailsTypeDef],
         "TransitGatewayId": str,
     },
     total=False,
 )
 
 AwsEc2VpnConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionDetailsTypeDef",
@@ -13751,58 +9738,48 @@
         "Options": AwsEc2VpnConnectionOptionsDetailsTypeDef,
         "Routes": Sequence[AwsEc2VpnConnectionRoutesDetailsTypeDef],
         "TransitGatewayId": str,
     },
     total=False,
 )
 
-AwsEcsClusterConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcsClusterConfigurationDetailsOutputTypeDef",
-    {
-        "ExecuteCommandConfiguration": (
-            AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
 AwsEcsClusterConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
         "ExecuteCommandConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
         ),
     },
     total=False,
 )
 
 AwsEcsServiceDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceDetailsOutputTypeDef",
     {
-        "CapacityProviderStrategy": List[AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef],
+        "CapacityProviderStrategy": List[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef],
         "Cluster": str,
-        "DeploymentConfiguration": AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef,
-        "DeploymentController": AwsEcsServiceDeploymentControllerDetailsOutputTypeDef,
+        "DeploymentConfiguration": AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
+        "DeploymentController": AwsEcsServiceDeploymentControllerDetailsTypeDef,
         "DesiredCount": int,
         "EnableEcsManagedTags": bool,
         "EnableExecuteCommand": bool,
         "HealthCheckGracePeriodSeconds": int,
         "LaunchType": str,
-        "LoadBalancers": List[AwsEcsServiceLoadBalancersDetailsOutputTypeDef],
+        "LoadBalancers": List[AwsEcsServiceLoadBalancersDetailsTypeDef],
         "Name": str,
         "NetworkConfiguration": AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
-        "PlacementConstraints": List[AwsEcsServicePlacementConstraintsDetailsOutputTypeDef],
-        "PlacementStrategies": List[AwsEcsServicePlacementStrategiesDetailsOutputTypeDef],
+        "PlacementConstraints": List[AwsEcsServicePlacementConstraintsDetailsTypeDef],
+        "PlacementStrategies": List[AwsEcsServicePlacementStrategiesDetailsTypeDef],
         "PlatformVersion": str,
         "PropagateTags": str,
         "Role": str,
         "SchedulingStrategy": str,
         "ServiceArn": str,
         "ServiceName": str,
-        "ServiceRegistries": List[AwsEcsServiceServiceRegistriesDetailsOutputTypeDef],
+        "ServiceRegistries": List[AwsEcsServiceServiceRegistriesDetailsTypeDef],
         "TaskDefinition": str,
     },
     total=False,
 )
 
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
@@ -13834,29 +9811,27 @@
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     {
         "Command": List[str],
         "Cpu": int,
-        "DependsOn": List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef],
+        "DependsOn": List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef],
         "DisableNetworking": bool,
         "DnsSearchDomains": List[str],
         "DnsServers": List[str],
         "DockerLabels": Dict[str, str],
         "DockerSecurityOptions": List[str],
         "EntryPoint": List[str],
-        "Environment": List[
-            AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef
-        ],
+        "Environment": List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef],
         "EnvironmentFiles": List[
-            AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef
         ],
         "Essential": bool,
-        "ExtraHosts": List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef],
+        "ExtraHosts": List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef],
         "FirelensConfiguration": (
             AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef
         ),
         "HealthCheck": AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
         "Hostname": str,
         "Image": str,
         "Interactive": bool,
@@ -13865,41 +9840,35 @@
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef
         ),
         "LogConfiguration": (
             AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef
         ),
         "Memory": int,
         "MemoryReservation": int,
-        "MountPoints": List[
-            AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef
-        ],
+        "MountPoints": List[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef],
         "Name": str,
-        "PortMappings": List[
-            AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef
-        ],
+        "PortMappings": List[AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef],
         "Privileged": bool,
         "PseudoTerminal": bool,
         "ReadonlyRootFilesystem": bool,
         "RepositoryCredentials": (
-            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
         ),
         "ResourceRequirements": List[
-            AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef
         ],
-        "Secrets": List[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef],
+        "Secrets": List[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef],
         "StartTimeout": int,
         "StopTimeout": int,
         "SystemControls": List[
-            AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef
         ],
-        "Ulimits": List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef],
+        "Ulimits": List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef],
         "User": str,
-        "VolumesFrom": List[
-            AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef
-        ],
+        "VolumesFrom": List[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef],
         "WorkingDirectory": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
@@ -13961,18 +9930,16 @@
 
 AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     {
         "DockerVolumeConfiguration": (
             AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef
         ),
-        "EfsVolumeConfiguration": (
-            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef
-        ),
-        "Host": AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef,
+        "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
+        "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
@@ -13993,15 +9960,15 @@
         "ClusterArn": str,
         "TaskDefinitionArn": str,
         "Version": str,
         "CreatedAt": str,
         "StartedAt": str,
         "StartedBy": str,
         "Group": str,
-        "Volumes": List[AwsEcsTaskVolumeDetailsOutputTypeDef],
+        "Volumes": List[AwsEcsTaskVolumeDetailsTypeDef],
         "Containers": List[AwsEcsContainerDetailsOutputTypeDef],
     },
     total=False,
 )
 
 AwsEcsTaskDetailsTypeDef = TypedDict(
     "AwsEcsTaskDetailsTypeDef",
@@ -14023,15 +9990,15 @@
     "AwsEfsAccessPointDetailsOutputTypeDef",
     {
         "AccessPointId": str,
         "Arn": str,
         "ClientToken": str,
         "FileSystemId": str,
         "PosixUser": AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
-        "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef,
+        "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEfsAccessPointDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointDetailsTypeDef",
     {
@@ -14077,29 +10044,27 @@
     total=False,
 )
 
 AwsElasticsearchDomainDetailsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsOutputTypeDef",
     {
         "AccessPolicies": str,
-        "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef,
+        "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
         "DomainId": str,
         "DomainName": str,
         "Endpoint": str,
         "Endpoints": Dict[str, str],
         "ElasticsearchVersion": str,
         "ElasticsearchClusterConfig": (
-            AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef
-        ),
-        "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef,
-        "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef,
-        "NodeToNodeEncryptionOptions": (
-            AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef
+            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
         ),
-        "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef,
+        "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
+        "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsTypeDef,
+        "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
+        "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     },
     total=False,
 )
 
 AwsElasticsearchDomainDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsTypeDef",
@@ -14128,23 +10093,23 @@
     {
         "AvailabilityZones": List[str],
         "BackendServerDescriptions": List[AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef],
         "CanonicalHostedZoneName": str,
         "CanonicalHostedZoneNameID": str,
         "CreatedTime": str,
         "DnsName": str,
-        "HealthCheck": AwsElbLoadBalancerHealthCheckOutputTypeDef,
-        "Instances": List[AwsElbLoadBalancerInstanceOutputTypeDef],
+        "HealthCheck": AwsElbLoadBalancerHealthCheckTypeDef,
+        "Instances": List[AwsElbLoadBalancerInstanceTypeDef],
         "ListenerDescriptions": List[AwsElbLoadBalancerListenerDescriptionOutputTypeDef],
         "LoadBalancerAttributes": AwsElbLoadBalancerAttributesOutputTypeDef,
         "LoadBalancerName": str,
         "Policies": AwsElbLoadBalancerPoliciesOutputTypeDef,
         "Scheme": str,
         "SecurityGroups": List[str],
-        "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef,
+        "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupTypeDef,
         "Subnets": List[str],
         "VpcId": str,
     },
     total=False,
 )
 
 AwsElbLoadBalancerDetailsTypeDef = TypedDict(
@@ -14167,48 +10132,23 @@
         "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupTypeDef,
         "Subnets": Sequence[str],
         "VpcId": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef",
-    {
-        "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef,
-        "ServiceRole": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     {
         "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
         "ServiceRole": str,
     },
     total=False,
 )
 
-AwsIamAccessKeyDetailsOutputTypeDef = TypedDict(
-    "AwsIamAccessKeyDetailsOutputTypeDef",
-    {
-        "UserName": str,
-        "Status": AwsIamAccessKeyStatusType,
-        "CreatedAt": str,
-        "PrincipalId": str,
-        "PrincipalType": str,
-        "PrincipalName": str,
-        "AccountId": str,
-        "AccessKeyId": str,
-        "SessionContext": AwsIamAccessKeySessionContextOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsIamAccessKeyDetailsTypeDef = TypedDict(
     "AwsIamAccessKeyDetailsTypeDef",
     {
         "UserName": str,
         "Status": AwsIamAccessKeyStatusType,
         "CreatedAt": str,
         "PrincipalId": str,
@@ -14221,21 +10161,21 @@
     total=False,
 )
 
 AwsIamRoleDetailsOutputTypeDef = TypedDict(
     "AwsIamRoleDetailsOutputTypeDef",
     {
         "AssumeRolePolicyDocument": str,
-        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyOutputTypeDef],
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "InstanceProfileList": List[AwsIamInstanceProfileOutputTypeDef],
-        "PermissionsBoundary": AwsIamPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AwsIamPermissionsBoundaryTypeDef,
         "RoleId": str,
         "RoleName": str,
-        "RolePolicyList": List[AwsIamRolePolicyOutputTypeDef],
+        "RolePolicyList": List[AwsIamRolePolicyTypeDef],
         "MaxSessionDuration": int,
         "Path": str,
     },
     total=False,
 )
 
 AwsIamRoleDetailsTypeDef = TypedDict(
@@ -14254,30 +10194,30 @@
     },
     total=False,
 )
 
 AwsLambdaFunctionDetailsOutputTypeDef = TypedDict(
     "AwsLambdaFunctionDetailsOutputTypeDef",
     {
-        "Code": AwsLambdaFunctionCodeOutputTypeDef,
+        "Code": AwsLambdaFunctionCodeTypeDef,
         "CodeSha256": str,
-        "DeadLetterConfig": AwsLambdaFunctionDeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": AwsLambdaFunctionDeadLetterConfigTypeDef,
         "Environment": AwsLambdaFunctionEnvironmentOutputTypeDef,
         "FunctionName": str,
         "Handler": str,
         "KmsKeyArn": str,
         "LastModified": str,
-        "Layers": List[AwsLambdaFunctionLayerOutputTypeDef],
+        "Layers": List[AwsLambdaFunctionLayerTypeDef],
         "MasterArn": str,
         "MemorySize": int,
         "RevisionId": str,
         "Role": str,
         "Runtime": str,
         "Timeout": int,
-        "TracingConfig": AwsLambdaFunctionTracingConfigOutputTypeDef,
+        "TracingConfig": AwsLambdaFunctionTracingConfigTypeDef,
         "VpcConfig": AwsLambdaFunctionVpcConfigOutputTypeDef,
         "Version": str,
         "Architectures": List[str],
         "PackageType": str,
     },
     total=False,
 )
@@ -14314,33 +10254,25 @@
     {
         "Arn": str,
         "AccessPolicies": str,
         "DomainName": str,
         "Id": str,
         "DomainEndpoint": str,
         "EngineVersion": str,
-        "EncryptionAtRestOptions": (
-            AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef
-        ),
+        "EncryptionAtRestOptions": AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
         "NodeToNodeEncryptionOptions": (
-            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef
-        ),
-        "ServiceSoftwareOptions": (
-            AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef
-        ),
-        "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef,
-        "DomainEndpointOptions": (
-            AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef
+            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
         ),
+        "ServiceSoftwareOptions": AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+        "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
+        "DomainEndpointOptions": AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
         "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
-        "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef,
+        "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
         "DomainEndpoints": Dict[str, str],
-        "AdvancedSecurityOptions": (
-            AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef
-        ),
+        "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
     },
     total=False,
 )
 
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
@@ -14368,15 +10300,15 @@
 AwsRdsDbSubnetGroupOutputTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupOutputTypeDef",
     {
         "DbSubnetGroupName": str,
         "DbSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
-        "Subnets": List[AwsRdsDbSubnetGroupSubnetOutputTypeDef],
+        "Subnets": List[AwsRdsDbSubnetGroupSubnetTypeDef],
         "DbSubnetGroupArn": str,
     },
     total=False,
 )
 
 AwsRdsDbSubnetGroupTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupTypeDef",
@@ -14396,54 +10328,52 @@
     {
         "AllowVersionUpgrade": bool,
         "AutomatedSnapshotRetentionPeriod": int,
         "AvailabilityZone": str,
         "ClusterAvailabilityStatus": str,
         "ClusterCreateTime": str,
         "ClusterIdentifier": str,
-        "ClusterNodes": List[AwsRedshiftClusterClusterNodeOutputTypeDef],
+        "ClusterNodes": List[AwsRedshiftClusterClusterNodeTypeDef],
         "ClusterParameterGroups": List[AwsRedshiftClusterClusterParameterGroupOutputTypeDef],
         "ClusterPublicKey": str,
         "ClusterRevisionNumber": str,
-        "ClusterSecurityGroups": List[AwsRedshiftClusterClusterSecurityGroupOutputTypeDef],
-        "ClusterSnapshotCopyStatus": AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef,
+        "ClusterSecurityGroups": List[AwsRedshiftClusterClusterSecurityGroupTypeDef],
+        "ClusterSnapshotCopyStatus": AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
         "ClusterStatus": str,
         "ClusterSubnetGroupName": str,
         "ClusterVersion": str,
         "DBName": str,
-        "DeferredMaintenanceWindows": List[
-            AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef
-        ],
-        "ElasticIpStatus": AwsRedshiftClusterElasticIpStatusOutputTypeDef,
+        "DeferredMaintenanceWindows": List[AwsRedshiftClusterDeferredMaintenanceWindowTypeDef],
+        "ElasticIpStatus": AwsRedshiftClusterElasticIpStatusTypeDef,
         "ElasticResizeNumberOfNodeOptions": str,
         "Encrypted": bool,
-        "Endpoint": AwsRedshiftClusterEndpointOutputTypeDef,
+        "Endpoint": AwsRedshiftClusterEndpointTypeDef,
         "EnhancedVpcRouting": bool,
         "ExpectedNextSnapshotScheduleTime": str,
         "ExpectedNextSnapshotScheduleTimeStatus": str,
-        "HsmStatus": AwsRedshiftClusterHsmStatusOutputTypeDef,
-        "IamRoles": List[AwsRedshiftClusterIamRoleOutputTypeDef],
+        "HsmStatus": AwsRedshiftClusterHsmStatusTypeDef,
+        "IamRoles": List[AwsRedshiftClusterIamRoleTypeDef],
         "KmsKeyId": str,
         "MaintenanceTrackName": str,
         "ManualSnapshotRetentionPeriod": int,
         "MasterUsername": str,
         "NextMaintenanceWindowStartTime": str,
         "NodeType": str,
         "NumberOfNodes": int,
         "PendingActions": List[str],
-        "PendingModifiedValues": AwsRedshiftClusterPendingModifiedValuesOutputTypeDef,
+        "PendingModifiedValues": AwsRedshiftClusterPendingModifiedValuesTypeDef,
         "PreferredMaintenanceWindow": str,
         "PubliclyAccessible": bool,
-        "ResizeInfo": AwsRedshiftClusterResizeInfoOutputTypeDef,
-        "RestoreStatus": AwsRedshiftClusterRestoreStatusOutputTypeDef,
+        "ResizeInfo": AwsRedshiftClusterResizeInfoTypeDef,
+        "RestoreStatus": AwsRedshiftClusterRestoreStatusTypeDef,
         "SnapshotScheduleIdentifier": str,
         "SnapshotScheduleState": str,
         "VpcId": str,
-        "VpcSecurityGroups": List[AwsRedshiftClusterVpcSecurityGroupOutputTypeDef],
-        "LoggingStatus": AwsRedshiftClusterLoggingStatusOutputTypeDef,
+        "VpcSecurityGroups": List[AwsRedshiftClusterVpcSecurityGroupTypeDef],
+        "LoggingStatus": AwsRedshiftClusterLoggingStatusTypeDef,
     },
     total=False,
 )
 
 AwsRedshiftClusterDetailsTypeDef = TypedDict(
     "AwsRedshiftClusterDetailsTypeDef",
     {
@@ -14495,18 +10425,18 @@
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     {
         "Operands": List[
-            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef
         ],
         "Prefix": str,
-        "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef,
+        "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
@@ -14533,36 +10463,27 @@
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     },
     total=False,
 )
 
-AwsS3BucketObjectLockConfigurationOutputTypeDef = TypedDict(
-    "AwsS3BucketObjectLockConfigurationOutputTypeDef",
-    {
-        "ObjectLockEnabled": str,
-        "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsS3BucketObjectLockConfigurationTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": str,
         "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     },
     total=False,
 )
 
 AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     {
-        "Rules": List[AwsS3BucketServerSideEncryptionRuleOutputTypeDef],
+        "Rules": List[AwsS3BucketServerSideEncryptionRuleTypeDef],
     },
     total=False,
 )
 
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
@@ -14572,16 +10493,16 @@
 )
 
 AwsS3BucketWebsiteConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     {
         "ErrorDocument": str,
         "IndexDocumentSuffix": str,
-        "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef,
-        "RoutingRules": List[AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef],
+        "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
+        "RoutingRules": List[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef],
     },
     total=False,
 )
 
 AwsS3BucketWebsiteConfigurationTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationTypeDef",
     {
@@ -14592,41 +10513,33 @@
     },
     total=False,
 )
 
 BatchUpdateFindingsResponseTypeDef = TypedDict(
     "BatchUpdateFindingsResponseTypeDef",
     {
-        "ProcessedFindings": List[AwsSecurityFindingIdentifierOutputTypeDef],
+        "ProcessedFindings": List[AwsSecurityFindingIdentifierTypeDef],
         "UnprocessedFindings": List[BatchUpdateFindingsUnprocessedFindingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AwsSsmPatchComplianceDetailsOutputTypeDef = TypedDict(
-    "AwsSsmPatchComplianceDetailsOutputTypeDef",
-    {
-        "Patch": AwsSsmPatchOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": AwsSsmPatchTypeDef,
     },
     total=False,
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     {
         "Destinations": List[
-            AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef
+            AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
         ],
         "IncludeExecutionData": bool,
         "Level": str,
     },
     total=False,
 )
 
@@ -14644,15 +10557,15 @@
 
 AwsWafRegionalRuleGroupDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
-        "Rules": List[AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef],
+        "Rules": List[AwsWafRegionalRuleGroupRulesDetailsTypeDef],
     },
     total=False,
 )
 
 AwsWafRegionalRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     {
@@ -14666,15 +10579,15 @@
 
 AwsWafRegionalWebAclDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalWebAclDetailsOutputTypeDef",
     {
         "DefaultAction": str,
         "MetricName": str,
         "Name": str,
-        "RulesList": List[AwsWafRegionalWebAclRulesListDetailsOutputTypeDef],
+        "RulesList": List[AwsWafRegionalWebAclRulesListDetailsTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
 AwsWafRegionalWebAclDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclDetailsTypeDef",
@@ -14690,15 +10603,15 @@
 
 AwsWafRuleGroupDetailsOutputTypeDef = TypedDict(
     "AwsWafRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
-        "Rules": List[AwsWafRuleGroupRulesDetailsOutputTypeDef],
+        "Rules": List[AwsWafRuleGroupRulesDetailsTypeDef],
     },
     total=False,
 )
 
 AwsWafRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupDetailsTypeDef",
     {
@@ -14752,22 +10665,14 @@
     "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     },
     total=False,
 )
 
-AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2ActionBlockDetailsOutputTypeDef",
-    {
-        "CustomResponse": AwsWafv2CustomResponseDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
     total=False,
 )
@@ -14784,164 +10689,85 @@
     "AwsWafv2RulesActionCountDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
     total=False,
 )
 
+AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
+    {
+        "CustomResponse": AwsWafv2CustomResponseDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
     "AwsWafv2ActionBlockDetailsTypeDef",
     {
         "CustomResponse": AwsWafv2CustomResponseDetailsTypeDef,
     },
     total=False,
 )
 
-AutomationRulesFindingFiltersOutputTypeDef = TypedDict(
-    "AutomationRulesFindingFiltersOutputTypeDef",
+BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "BatchGetStandardsControlAssociationsResponseTypeDef",
     {
-        "ProductArn": List[StringFilterOutputTypeDef],
-        "AwsAccountId": List[StringFilterOutputTypeDef],
-        "Id": List[StringFilterOutputTypeDef],
-        "GeneratorId": List[StringFilterOutputTypeDef],
-        "Type": List[StringFilterOutputTypeDef],
-        "FirstObservedAt": List[DateFilterOutputTypeDef],
-        "LastObservedAt": List[DateFilterOutputTypeDef],
-        "CreatedAt": List[DateFilterOutputTypeDef],
-        "UpdatedAt": List[DateFilterOutputTypeDef],
-        "Confidence": List[NumberFilterOutputTypeDef],
-        "Criticality": List[NumberFilterOutputTypeDef],
-        "Title": List[StringFilterOutputTypeDef],
-        "Description": List[StringFilterOutputTypeDef],
-        "SourceUrl": List[StringFilterOutputTypeDef],
-        "ProductName": List[StringFilterOutputTypeDef],
-        "CompanyName": List[StringFilterOutputTypeDef],
-        "SeverityLabel": List[StringFilterOutputTypeDef],
-        "ResourceType": List[StringFilterOutputTypeDef],
-        "ResourceId": List[StringFilterOutputTypeDef],
-        "ResourcePartition": List[StringFilterOutputTypeDef],
-        "ResourceRegion": List[StringFilterOutputTypeDef],
-        "ResourceTags": List[MapFilterOutputTypeDef],
-        "ResourceDetailsOther": List[MapFilterOutputTypeDef],
-        "ComplianceStatus": List[StringFilterOutputTypeDef],
-        "ComplianceSecurityControlId": List[StringFilterOutputTypeDef],
-        "ComplianceAssociatedStandardsId": List[StringFilterOutputTypeDef],
-        "VerificationState": List[StringFilterOutputTypeDef],
-        "WorkflowStatus": List[StringFilterOutputTypeDef],
-        "RecordState": List[StringFilterOutputTypeDef],
-        "RelatedFindingsProductArn": List[StringFilterOutputTypeDef],
-        "RelatedFindingsId": List[StringFilterOutputTypeDef],
-        "NoteText": List[StringFilterOutputTypeDef],
-        "NoteUpdatedAt": List[DateFilterOutputTypeDef],
-        "NoteUpdatedBy": List[StringFilterOutputTypeDef],
-        "UserDefinedFields": List[MapFilterOutputTypeDef],
+        "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
+        "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
-    "AwsSecurityFindingFiltersOutputTypeDef",
+BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     {
-        "ProductArn": List[StringFilterOutputTypeDef],
-        "AwsAccountId": List[StringFilterOutputTypeDef],
-        "Id": List[StringFilterOutputTypeDef],
-        "GeneratorId": List[StringFilterOutputTypeDef],
-        "Region": List[StringFilterOutputTypeDef],
-        "Type": List[StringFilterOutputTypeDef],
-        "FirstObservedAt": List[DateFilterOutputTypeDef],
-        "LastObservedAt": List[DateFilterOutputTypeDef],
-        "CreatedAt": List[DateFilterOutputTypeDef],
-        "UpdatedAt": List[DateFilterOutputTypeDef],
-        "SeverityProduct": List[NumberFilterOutputTypeDef],
-        "SeverityNormalized": List[NumberFilterOutputTypeDef],
-        "SeverityLabel": List[StringFilterOutputTypeDef],
-        "Confidence": List[NumberFilterOutputTypeDef],
-        "Criticality": List[NumberFilterOutputTypeDef],
-        "Title": List[StringFilterOutputTypeDef],
-        "Description": List[StringFilterOutputTypeDef],
-        "RecommendationText": List[StringFilterOutputTypeDef],
-        "SourceUrl": List[StringFilterOutputTypeDef],
-        "ProductFields": List[MapFilterOutputTypeDef],
-        "ProductName": List[StringFilterOutputTypeDef],
-        "CompanyName": List[StringFilterOutputTypeDef],
-        "UserDefinedFields": List[MapFilterOutputTypeDef],
-        "MalwareName": List[StringFilterOutputTypeDef],
-        "MalwareType": List[StringFilterOutputTypeDef],
-        "MalwarePath": List[StringFilterOutputTypeDef],
-        "MalwareState": List[StringFilterOutputTypeDef],
-        "NetworkDirection": List[StringFilterOutputTypeDef],
-        "NetworkProtocol": List[StringFilterOutputTypeDef],
-        "NetworkSourceIpV4": List[IpFilterOutputTypeDef],
-        "NetworkSourceIpV6": List[IpFilterOutputTypeDef],
-        "NetworkSourcePort": List[NumberFilterOutputTypeDef],
-        "NetworkSourceDomain": List[StringFilterOutputTypeDef],
-        "NetworkSourceMac": List[StringFilterOutputTypeDef],
-        "NetworkDestinationIpV4": List[IpFilterOutputTypeDef],
-        "NetworkDestinationIpV6": List[IpFilterOutputTypeDef],
-        "NetworkDestinationPort": List[NumberFilterOutputTypeDef],
-        "NetworkDestinationDomain": List[StringFilterOutputTypeDef],
-        "ProcessName": List[StringFilterOutputTypeDef],
-        "ProcessPath": List[StringFilterOutputTypeDef],
-        "ProcessPid": List[NumberFilterOutputTypeDef],
-        "ProcessParentPid": List[NumberFilterOutputTypeDef],
-        "ProcessLaunchedAt": List[DateFilterOutputTypeDef],
-        "ProcessTerminatedAt": List[DateFilterOutputTypeDef],
-        "ThreatIntelIndicatorType": List[StringFilterOutputTypeDef],
-        "ThreatIntelIndicatorValue": List[StringFilterOutputTypeDef],
-        "ThreatIntelIndicatorCategory": List[StringFilterOutputTypeDef],
-        "ThreatIntelIndicatorLastObservedAt": List[DateFilterOutputTypeDef],
-        "ThreatIntelIndicatorSource": List[StringFilterOutputTypeDef],
-        "ThreatIntelIndicatorSourceUrl": List[StringFilterOutputTypeDef],
-        "ResourceType": List[StringFilterOutputTypeDef],
-        "ResourceId": List[StringFilterOutputTypeDef],
-        "ResourcePartition": List[StringFilterOutputTypeDef],
-        "ResourceRegion": List[StringFilterOutputTypeDef],
-        "ResourceTags": List[MapFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceType": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceImageId": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceIpV4Addresses": List[IpFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceIpV6Addresses": List[IpFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceKeyName": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceIamInstanceProfileArn": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceVpcId": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceSubnetId": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceLaunchedAt": List[DateFilterOutputTypeDef],
-        "ResourceAwsS3BucketOwnerId": List[StringFilterOutputTypeDef],
-        "ResourceAwsS3BucketOwnerName": List[StringFilterOutputTypeDef],
-        "ResourceAwsIamAccessKeyUserName": List[StringFilterOutputTypeDef],
-        "ResourceAwsIamAccessKeyPrincipalName": List[StringFilterOutputTypeDef],
-        "ResourceAwsIamAccessKeyStatus": List[StringFilterOutputTypeDef],
-        "ResourceAwsIamAccessKeyCreatedAt": List[DateFilterOutputTypeDef],
-        "ResourceAwsIamUserUserName": List[StringFilterOutputTypeDef],
-        "ResourceContainerName": List[StringFilterOutputTypeDef],
-        "ResourceContainerImageId": List[StringFilterOutputTypeDef],
-        "ResourceContainerImageName": List[StringFilterOutputTypeDef],
-        "ResourceContainerLaunchedAt": List[DateFilterOutputTypeDef],
-        "ResourceDetailsOther": List[MapFilterOutputTypeDef],
-        "ComplianceStatus": List[StringFilterOutputTypeDef],
-        "VerificationState": List[StringFilterOutputTypeDef],
-        "WorkflowState": List[StringFilterOutputTypeDef],
-        "WorkflowStatus": List[StringFilterOutputTypeDef],
-        "RecordState": List[StringFilterOutputTypeDef],
-        "RelatedFindingsProductArn": List[StringFilterOutputTypeDef],
-        "RelatedFindingsId": List[StringFilterOutputTypeDef],
-        "NoteText": List[StringFilterOutputTypeDef],
-        "NoteUpdatedAt": List[DateFilterOutputTypeDef],
-        "NoteUpdatedBy": List[StringFilterOutputTypeDef],
-        "Keyword": List[KeywordFilterOutputTypeDef],
-        "FindingProviderFieldsConfidence": List[NumberFilterOutputTypeDef],
-        "FindingProviderFieldsCriticality": List[NumberFilterOutputTypeDef],
-        "FindingProviderFieldsRelatedFindingsId": List[StringFilterOutputTypeDef],
-        "FindingProviderFieldsRelatedFindingsProductArn": List[StringFilterOutputTypeDef],
-        "FindingProviderFieldsSeverityLabel": List[StringFilterOutputTypeDef],
-        "FindingProviderFieldsSeverityOriginal": List[StringFilterOutputTypeDef],
-        "FindingProviderFieldsTypes": List[StringFilterOutputTypeDef],
-        "Sample": List[BooleanFilterOutputTypeDef],
-        "ComplianceSecurityControlId": List[StringFilterOutputTypeDef],
-        "ComplianceAssociatedStandardsId": List[StringFilterOutputTypeDef],
+        "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AutomationRulesFindingFiltersOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersOutputTypeDef",
+    {
+        "ProductArn": List[StringFilterTypeDef],
+        "AwsAccountId": List[StringFilterTypeDef],
+        "Id": List[StringFilterTypeDef],
+        "GeneratorId": List[StringFilterTypeDef],
+        "Type": List[StringFilterTypeDef],
+        "FirstObservedAt": List[DateFilterTypeDef],
+        "LastObservedAt": List[DateFilterTypeDef],
+        "CreatedAt": List[DateFilterTypeDef],
+        "UpdatedAt": List[DateFilterTypeDef],
+        "Confidence": List[NumberFilterTypeDef],
+        "Criticality": List[NumberFilterTypeDef],
+        "Title": List[StringFilterTypeDef],
+        "Description": List[StringFilterTypeDef],
+        "SourceUrl": List[StringFilterTypeDef],
+        "ProductName": List[StringFilterTypeDef],
+        "CompanyName": List[StringFilterTypeDef],
+        "SeverityLabel": List[StringFilterTypeDef],
+        "ResourceType": List[StringFilterTypeDef],
+        "ResourceId": List[StringFilterTypeDef],
+        "ResourcePartition": List[StringFilterTypeDef],
+        "ResourceRegion": List[StringFilterTypeDef],
+        "ResourceTags": List[MapFilterTypeDef],
+        "ResourceDetailsOther": List[MapFilterTypeDef],
+        "ComplianceStatus": List[StringFilterTypeDef],
+        "ComplianceSecurityControlId": List[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": List[StringFilterTypeDef],
+        "VerificationState": List[StringFilterTypeDef],
+        "WorkflowStatus": List[StringFilterTypeDef],
+        "RecordState": List[StringFilterTypeDef],
+        "RelatedFindingsProductArn": List[StringFilterTypeDef],
+        "RelatedFindingsId": List[StringFilterTypeDef],
+        "NoteText": List[StringFilterTypeDef],
+        "NoteUpdatedAt": List[DateFilterTypeDef],
+        "NoteUpdatedBy": List[StringFilterTypeDef],
+        "UserDefinedFields": List[MapFilterTypeDef],
     },
     total=False,
 )
 
 AutomationRulesFindingFiltersTypeDef = TypedDict(
     "AutomationRulesFindingFiltersTypeDef",
     {
@@ -14980,14 +10806,118 @@
         "NoteUpdatedAt": Sequence[DateFilterTypeDef],
         "NoteUpdatedBy": Sequence[StringFilterTypeDef],
         "UserDefinedFields": Sequence[MapFilterTypeDef],
     },
     total=False,
 )
 
+AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
+    "AwsSecurityFindingFiltersOutputTypeDef",
+    {
+        "ProductArn": List[StringFilterTypeDef],
+        "AwsAccountId": List[StringFilterTypeDef],
+        "Id": List[StringFilterTypeDef],
+        "GeneratorId": List[StringFilterTypeDef],
+        "Region": List[StringFilterTypeDef],
+        "Type": List[StringFilterTypeDef],
+        "FirstObservedAt": List[DateFilterTypeDef],
+        "LastObservedAt": List[DateFilterTypeDef],
+        "CreatedAt": List[DateFilterTypeDef],
+        "UpdatedAt": List[DateFilterTypeDef],
+        "SeverityProduct": List[NumberFilterTypeDef],
+        "SeverityNormalized": List[NumberFilterTypeDef],
+        "SeverityLabel": List[StringFilterTypeDef],
+        "Confidence": List[NumberFilterTypeDef],
+        "Criticality": List[NumberFilterTypeDef],
+        "Title": List[StringFilterTypeDef],
+        "Description": List[StringFilterTypeDef],
+        "RecommendationText": List[StringFilterTypeDef],
+        "SourceUrl": List[StringFilterTypeDef],
+        "ProductFields": List[MapFilterTypeDef],
+        "ProductName": List[StringFilterTypeDef],
+        "CompanyName": List[StringFilterTypeDef],
+        "UserDefinedFields": List[MapFilterTypeDef],
+        "MalwareName": List[StringFilterTypeDef],
+        "MalwareType": List[StringFilterTypeDef],
+        "MalwarePath": List[StringFilterTypeDef],
+        "MalwareState": List[StringFilterTypeDef],
+        "NetworkDirection": List[StringFilterTypeDef],
+        "NetworkProtocol": List[StringFilterTypeDef],
+        "NetworkSourceIpV4": List[IpFilterTypeDef],
+        "NetworkSourceIpV6": List[IpFilterTypeDef],
+        "NetworkSourcePort": List[NumberFilterTypeDef],
+        "NetworkSourceDomain": List[StringFilterTypeDef],
+        "NetworkSourceMac": List[StringFilterTypeDef],
+        "NetworkDestinationIpV4": List[IpFilterTypeDef],
+        "NetworkDestinationIpV6": List[IpFilterTypeDef],
+        "NetworkDestinationPort": List[NumberFilterTypeDef],
+        "NetworkDestinationDomain": List[StringFilterTypeDef],
+        "ProcessName": List[StringFilterTypeDef],
+        "ProcessPath": List[StringFilterTypeDef],
+        "ProcessPid": List[NumberFilterTypeDef],
+        "ProcessParentPid": List[NumberFilterTypeDef],
+        "ProcessLaunchedAt": List[DateFilterTypeDef],
+        "ProcessTerminatedAt": List[DateFilterTypeDef],
+        "ThreatIntelIndicatorType": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorValue": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorCategory": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorLastObservedAt": List[DateFilterTypeDef],
+        "ThreatIntelIndicatorSource": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorSourceUrl": List[StringFilterTypeDef],
+        "ResourceType": List[StringFilterTypeDef],
+        "ResourceId": List[StringFilterTypeDef],
+        "ResourcePartition": List[StringFilterTypeDef],
+        "ResourceRegion": List[StringFilterTypeDef],
+        "ResourceTags": List[MapFilterTypeDef],
+        "ResourceAwsEc2InstanceType": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceImageId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceIpV4Addresses": List[IpFilterTypeDef],
+        "ResourceAwsEc2InstanceIpV6Addresses": List[IpFilterTypeDef],
+        "ResourceAwsEc2InstanceKeyName": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceIamInstanceProfileArn": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceVpcId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceSubnetId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceLaunchedAt": List[DateFilterTypeDef],
+        "ResourceAwsS3BucketOwnerId": List[StringFilterTypeDef],
+        "ResourceAwsS3BucketOwnerName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyUserName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyPrincipalName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyStatus": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyCreatedAt": List[DateFilterTypeDef],
+        "ResourceAwsIamUserUserName": List[StringFilterTypeDef],
+        "ResourceContainerName": List[StringFilterTypeDef],
+        "ResourceContainerImageId": List[StringFilterTypeDef],
+        "ResourceContainerImageName": List[StringFilterTypeDef],
+        "ResourceContainerLaunchedAt": List[DateFilterTypeDef],
+        "ResourceDetailsOther": List[MapFilterTypeDef],
+        "ComplianceStatus": List[StringFilterTypeDef],
+        "VerificationState": List[StringFilterTypeDef],
+        "WorkflowState": List[StringFilterTypeDef],
+        "WorkflowStatus": List[StringFilterTypeDef],
+        "RecordState": List[StringFilterTypeDef],
+        "RelatedFindingsProductArn": List[StringFilterTypeDef],
+        "RelatedFindingsId": List[StringFilterTypeDef],
+        "NoteText": List[StringFilterTypeDef],
+        "NoteUpdatedAt": List[DateFilterTypeDef],
+        "NoteUpdatedBy": List[StringFilterTypeDef],
+        "Keyword": List[KeywordFilterTypeDef],
+        "FindingProviderFieldsConfidence": List[NumberFilterTypeDef],
+        "FindingProviderFieldsCriticality": List[NumberFilterTypeDef],
+        "FindingProviderFieldsRelatedFindingsId": List[StringFilterTypeDef],
+        "FindingProviderFieldsRelatedFindingsProductArn": List[StringFilterTypeDef],
+        "FindingProviderFieldsSeverityLabel": List[StringFilterTypeDef],
+        "FindingProviderFieldsSeverityOriginal": List[StringFilterTypeDef],
+        "FindingProviderFieldsTypes": List[StringFilterTypeDef],
+        "Sample": List[BooleanFilterTypeDef],
+        "ComplianceSecurityControlId": List[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": List[StringFilterTypeDef],
+    },
+    total=False,
+)
+
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
         "Id": Sequence[StringFilterTypeDef],
         "GeneratorId": Sequence[StringFilterTypeDef],
@@ -15124,19 +11054,19 @@
     },
     total=False,
 )
 
 OccurrencesOutputTypeDef = TypedDict(
     "OccurrencesOutputTypeDef",
     {
-        "LineRanges": List[RangeOutputTypeDef],
-        "OffsetRanges": List[RangeOutputTypeDef],
-        "Pages": List[PageOutputTypeDef],
-        "Records": List[RecordOutputTypeDef],
-        "Cells": List[CellOutputTypeDef],
+        "LineRanges": List[RangeTypeDef],
+        "OffsetRanges": List[RangeTypeDef],
+        "Pages": List[PageTypeDef],
+        "Records": List[RecordTypeDef],
+        "Cells": List[CellTypeDef],
     },
     total=False,
 )
 
 OccurrencesTypeDef = TypedDict(
     "OccurrencesTypeDef",
     {
@@ -15172,31 +11102,14 @@
     {
         "Standards": List[StandardTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "BatchGetStandardsControlAssociationsResponseTypeDef",
-    {
-        "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
-        "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
-    {
-        "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -15233,40 +11146,29 @@
     },
     total=False,
 )
 
 PortProbeActionOutputTypeDef = TypedDict(
     "PortProbeActionOutputTypeDef",
     {
-        "PortProbeDetails": List[PortProbeDetailOutputTypeDef],
+        "PortProbeDetails": List[PortProbeDetailTypeDef],
         "Blocked": bool,
     },
     total=False,
 )
 
 PortProbeActionTypeDef = TypedDict(
     "PortProbeActionTypeDef",
     {
         "PortProbeDetails": Sequence[PortProbeDetailTypeDef],
         "Blocked": bool,
     },
     total=False,
 )
 
-AwsAthenaWorkGroupDetailsOutputTypeDef = TypedDict(
-    "AwsAthenaWorkGroupDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "State": str,
-        "Configuration": AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsAthenaWorkGroupDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
         "State": str,
         "Configuration": AwsAthenaWorkGroupConfigurationDetailsTypeDef,
@@ -15282,18 +11184,18 @@
         "HealthCheckType": str,
         "HealthCheckGracePeriod": int,
         "CreatedTime": str,
         "MixedInstancesPolicy": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef
         ),
         "AvailabilityZones": List[
-            AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef
+            AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef
         ],
         "LaunchTemplate": (
-            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef
+            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
         ),
         "CapacityRebalance": bool,
     },
     total=False,
 )
 
 AwsAutoScalingAutoScalingGroupDetailsTypeDef = TypedDict(
@@ -15343,25 +11245,25 @@
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": str,
         "DomainName": str,
         "DomainValidationOptions": List[
             AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef
         ],
-        "ExtendedKeyUsages": List[AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef],
+        "ExtendedKeyUsages": List[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef],
         "FailureReason": str,
         "ImportedAt": str,
         "InUseBy": List[str],
         "IssuedAt": str,
         "Issuer": str,
         "KeyAlgorithm": str,
-        "KeyUsages": List[AwsCertificateManagerCertificateKeyUsageOutputTypeDef],
+        "KeyUsages": List[AwsCertificateManagerCertificateKeyUsageTypeDef],
         "NotAfter": str,
         "NotBefore": str,
-        "Options": AwsCertificateManagerCertificateOptionsOutputTypeDef,
+        "Options": AwsCertificateManagerCertificateOptionsTypeDef,
         "RenewalEligibility": str,
         "RenewalSummary": AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef,
         "Serial": str,
         "SignatureAlgorithm": str,
         "Status": str,
         "Subject": str,
         "SubjectAlternativeNames": List[str],
@@ -15433,29 +11335,29 @@
     },
     total=False,
 )
 
 AwsDynamoDbTableDetailsOutputTypeDef = TypedDict(
     "AwsDynamoDbTableDetailsOutputTypeDef",
     {
-        "AttributeDefinitions": List[AwsDynamoDbTableAttributeDefinitionOutputTypeDef],
-        "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryOutputTypeDef,
+        "AttributeDefinitions": List[AwsDynamoDbTableAttributeDefinitionTypeDef],
+        "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryTypeDef,
         "CreationDateTime": str,
         "GlobalSecondaryIndexes": List[AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef],
         "GlobalTableVersion": str,
         "ItemCount": int,
-        "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
         "LatestStreamArn": str,
         "LatestStreamLabel": str,
         "LocalSecondaryIndexes": List[AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef],
-        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
+        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputTypeDef,
         "Replicas": List[AwsDynamoDbTableReplicaOutputTypeDef],
-        "RestoreSummary": AwsDynamoDbTableRestoreSummaryOutputTypeDef,
-        "SseDescription": AwsDynamoDbTableSseDescriptionOutputTypeDef,
-        "StreamSpecification": AwsDynamoDbTableStreamSpecificationOutputTypeDef,
+        "RestoreSummary": AwsDynamoDbTableRestoreSummaryTypeDef,
+        "SseDescription": AwsDynamoDbTableSseDescriptionTypeDef,
+        "StreamSpecification": AwsDynamoDbTableStreamSpecificationTypeDef,
         "TableId": str,
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
     total=False,
 )
@@ -15512,18 +11414,18 @@
 
 AwsEcsClusterDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterDetailsOutputTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
         "CapacityProviders": List[str],
-        "ClusterSettings": List[AwsEcsClusterClusterSettingsDetailsOutputTypeDef],
-        "Configuration": AwsEcsClusterConfigurationDetailsOutputTypeDef,
+        "ClusterSettings": List[AwsEcsClusterClusterSettingsDetailsTypeDef],
+        "Configuration": AwsEcsClusterConfigurationDetailsTypeDef,
         "DefaultCapacityProviderStrategy": List[
-            AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef
+            AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef
         ],
         "ClusterName": str,
         "RegisteredContainerInstancesCount": int,
         "RunningTasksCount": int,
         "Status": str,
     },
     total=False,
@@ -15551,22 +11453,20 @@
 AwsEcsTaskDefinitionDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionDetailsOutputTypeDef",
     {
         "ContainerDefinitions": List[AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef],
         "Cpu": str,
         "ExecutionRoleArn": str,
         "Family": str,
-        "InferenceAccelerators": List[
-            AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef
-        ],
+        "InferenceAccelerators": List[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef],
         "IpcMode": str,
         "Memory": str,
         "NetworkMode": str,
         "PidMode": str,
-        "PlacementConstraints": List[AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef],
+        "PlacementConstraints": List[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef],
         "ProxyConfiguration": AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
         "RequiresCompatibilities": List[str],
         "TaskRoleArn": str,
         "Volumes": List[AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef],
     },
     total=False,
 )
@@ -15588,27 +11488,14 @@
         "RequiresCompatibilities": Sequence[str],
         "TaskRoleArn": str,
         "Volumes": Sequence[AwsEcsTaskDefinitionVolumesDetailsTypeDef],
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef",
-    {
-        "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef,
-        "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef,
-        "FlowLogs": AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef,
-        "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef,
-        "MalwareProtection": AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef,
-        "S3Logs": AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
     {
         "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
         "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
         "FlowLogs": AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
         "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
@@ -15617,70 +11504,70 @@
     },
     total=False,
 )
 
 AwsRdsDbInstanceDetailsOutputTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsOutputTypeDef",
     {
-        "AssociatedRoles": List[AwsRdsDbInstanceAssociatedRoleOutputTypeDef],
+        "AssociatedRoles": List[AwsRdsDbInstanceAssociatedRoleTypeDef],
         "CACertificateIdentifier": str,
         "DBClusterIdentifier": str,
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "DbInstancePort": int,
         "DbiResourceId": str,
         "DBName": str,
         "DeletionProtection": bool,
-        "Endpoint": AwsRdsDbInstanceEndpointOutputTypeDef,
+        "Endpoint": AwsRdsDbInstanceEndpointTypeDef,
         "Engine": str,
         "EngineVersion": str,
         "IAMDatabaseAuthenticationEnabled": bool,
         "InstanceCreateTime": str,
         "KmsKeyId": str,
         "PubliclyAccessible": bool,
         "StorageEncrypted": bool,
         "TdeCredentialArn": str,
-        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef],
+        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupTypeDef],
         "MultiAz": bool,
         "EnhancedMonitoringResourceArn": str,
         "DbInstanceStatus": str,
         "MasterUsername": str,
         "AllocatedStorage": int,
         "PreferredBackupWindow": str,
         "BackupRetentionPeriod": int,
         "DbSecurityGroups": List[str],
-        "DbParameterGroups": List[AwsRdsDbParameterGroupOutputTypeDef],
+        "DbParameterGroups": List[AwsRdsDbParameterGroupTypeDef],
         "AvailabilityZone": str,
         "DbSubnetGroup": AwsRdsDbSubnetGroupOutputTypeDef,
         "PreferredMaintenanceWindow": str,
         "PendingModifiedValues": AwsRdsDbPendingModifiedValuesOutputTypeDef,
         "LatestRestorableTime": str,
         "AutoMinorVersionUpgrade": bool,
         "ReadReplicaSourceDBInstanceIdentifier": str,
         "ReadReplicaDBInstanceIdentifiers": List[str],
         "ReadReplicaDBClusterIdentifiers": List[str],
         "LicenseModel": str,
         "Iops": int,
-        "OptionGroupMemberships": List[AwsRdsDbOptionGroupMembershipOutputTypeDef],
+        "OptionGroupMemberships": List[AwsRdsDbOptionGroupMembershipTypeDef],
         "CharacterSetName": str,
         "SecondaryAvailabilityZone": str,
-        "StatusInfos": List[AwsRdsDbStatusInfoOutputTypeDef],
+        "StatusInfos": List[AwsRdsDbStatusInfoTypeDef],
         "StorageType": str,
-        "DomainMemberships": List[AwsRdsDbDomainMembershipOutputTypeDef],
+        "DomainMemberships": List[AwsRdsDbDomainMembershipTypeDef],
         "CopyTagsToSnapshot": bool,
         "MonitoringInterval": int,
         "MonitoringRoleArn": str,
         "PromotionTier": int,
         "Timezone": str,
         "PerformanceInsightsEnabled": bool,
         "PerformanceInsightsKmsKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "EnabledCloudWatchLogsExports": List[str],
-        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
-        "ListenerEndpoint": AwsRdsDbInstanceEndpointOutputTypeDef,
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
+        "ListenerEndpoint": AwsRdsDbInstanceEndpointTypeDef,
         "MaxAllocatedStorage": int,
     },
     total=False,
 )
 
 AwsRdsDbInstanceDetailsTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsTypeDef",
@@ -15791,15 +11678,15 @@
     {
         "Label": str,
         "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
         "Name": str,
         "RoleArn": str,
         "StateMachineArn": str,
         "Status": str,
-        "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef,
+        "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 AwsStepFunctionStateMachineDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineDetailsTypeDef",
@@ -15870,24 +11757,14 @@
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
-InsightTypeDef = TypedDict(
-    "InsightTypeDef",
-    {
-        "InsightArn": str,
-        "Name": str,
-        "Filters": AwsSecurityFindingFiltersOutputTypeDef,
-        "GroupByAttribute": str,
-    },
-)
-
 _RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutomationRuleRequestRequestTypeDef",
     {
         "RuleOrder": int,
         "RuleName": str,
         "Description": str,
         "Criteria": AutomationRulesFindingFiltersTypeDef,
@@ -15936,14 +11813,24 @@
 class UpdateAutomationRulesRequestItemTypeDef(
     _RequiredUpdateAutomationRulesRequestItemTypeDef,
     _OptionalUpdateAutomationRulesRequestItemTypeDef,
 ):
     pass
 
 
+InsightTypeDef = TypedDict(
+    "InsightTypeDef",
+    {
+        "InsightArn": str,
+        "Name": str,
+        "Filters": AwsSecurityFindingFiltersOutputTypeDef,
+        "GroupByAttribute": str,
+    },
+)
+
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
@@ -16133,17 +12020,17 @@
     total=False,
 )
 
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
         "ActionType": str,
-        "NetworkConnectionAction": NetworkConnectionActionOutputTypeDef,
+        "NetworkConnectionAction": NetworkConnectionActionTypeDef,
         "AwsApiCallAction": AwsApiCallActionOutputTypeDef,
-        "DnsRequestAction": DnsRequestActionOutputTypeDef,
+        "DnsRequestAction": DnsRequestActionTypeDef,
         "PortProbeAction": PortProbeActionOutputTypeDef,
     },
     total=False,
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
@@ -16179,23 +12066,23 @@
     total=False,
 )
 
 AwsCloudFrontDistributionDetailsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionDetailsOutputTypeDef",
     {
         "CacheBehaviors": AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
-        "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef,
+        "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
         "DefaultRootObject": str,
         "DomainName": str,
         "ETag": str,
         "LastModifiedTime": str,
-        "Logging": AwsCloudFrontDistributionLoggingOutputTypeDef,
+        "Logging": AwsCloudFrontDistributionLoggingTypeDef,
         "Origins": AwsCloudFrontDistributionOriginsOutputTypeDef,
         "OriginGroups": AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
-        "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateOutputTypeDef,
+        "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateTypeDef,
         "Status": str,
         "WebAclId": str,
     },
     total=False,
 )
 
 AwsCloudFrontDistributionDetailsTypeDef = TypedDict(
@@ -16216,16 +12103,16 @@
     },
     total=False,
 )
 
 AwsGuardDutyDetectorDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDetailsOutputTypeDef",
     {
-        "DataSources": AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef,
-        "Features": List[AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef],
+        "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+        "Features": List[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
         "FindingPublishingFrequency": str,
         "ServiceRole": str,
         "Status": str,
     },
     total=False,
 )
 
@@ -16240,29 +12127,29 @@
     },
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     {
-        "AbortIncompleteMultipartUpload": AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef,
+        "AbortIncompleteMultipartUpload": (
+            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
+        ),
         "ExpirationDate": str,
         "ExpirationInDays": int,
         "ExpiredObjectDeleteMarker": bool,
         "Filter": AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
         "ID": str,
         "NoncurrentVersionExpirationInDays": int,
         "NoncurrentVersionTransitions": List[
-            AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef
+            AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef
         ],
         "Prefix": str,
         "Status": str,
-        "Transitions": List[
-            AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef
-        ],
+        "Transitions": List[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef],
     },
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
@@ -16306,15 +12193,15 @@
 AwsWafv2RulesDetailsOutputTypeDef = TypedDict(
     "AwsWafv2RulesDetailsOutputTypeDef",
     {
         "Action": AwsWafv2RulesActionDetailsOutputTypeDef,
         "Name": str,
         "OverrideAction": str,
         "Priority": int,
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
     },
     total=False,
 )
 
 AwsWafv2RulesDetailsTypeDef = TypedDict(
     "AwsWafv2RulesDetailsTypeDef",
     {
@@ -16332,30 +12219,30 @@
     {
         "Rules": List[AutomationRulesConfigTypeDef],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchUpdateAutomationRulesRequestRequestTypeDef = TypedDict(
+    "BatchUpdateAutomationRulesRequestRequestTypeDef",
+    {
+        "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
+    },
+)
+
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchUpdateAutomationRulesRequestRequestTypeDef = TypedDict(
-    "BatchUpdateAutomationRulesRequestRequestTypeDef",
-    {
-        "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
-    },
-)
-
 CustomDataIdentifiersResultOutputTypeDef = TypedDict(
     "CustomDataIdentifiersResultOutputTypeDef",
     {
         "Detections": List[CustomDataIdentifiersDetectionsOutputTypeDef],
         "TotalCount": int,
     },
     total=False,
@@ -16390,21 +12277,21 @@
     total=False,
 )
 
 FirewallPolicyDetailsOutputTypeDef = TypedDict(
     "FirewallPolicyDetailsOutputTypeDef",
     {
         "StatefulRuleGroupReferences": List[
-            FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef
+            FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef
         ],
         "StatelessCustomActions": List[FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef],
         "StatelessDefaultActions": List[str],
         "StatelessFragmentDefaultActions": List[str],
         "StatelessRuleGroupReferences": List[
-            FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef
+            FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef
         ],
     },
     total=False,
 )
 
 RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
@@ -16462,32 +12349,32 @@
         "Capacity": int,
         "Description": str,
         "Id": str,
         "Name": str,
         "Arn": str,
         "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
         "Scope": str,
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
     },
     total=False,
 )
 
 AwsWafv2WebAclDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclDetailsOutputTypeDef",
     {
         "Name": str,
         "Arn": str,
         "ManagedbyFirewallManager": bool,
         "Id": str,
         "Capacity": int,
-        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef,
+        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
         "DefaultAction": AwsWafv2WebAclActionDetailsOutputTypeDef,
         "Description": str,
         "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
     },
     total=False,
 )
 
 AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
     "AwsWafv2RuleGroupDetailsTypeDef",
     {
@@ -16522,15 +12409,15 @@
 
 ClassificationResultOutputTypeDef = TypedDict(
     "ClassificationResultOutputTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
-        "Status": ClassificationStatusOutputTypeDef,
+        "Status": ClassificationStatusTypeDef,
         "SensitiveData": List[SensitiveDataResultOutputTypeDef],
         "CustomDataIdentifiers": CustomDataIdentifiersResultOutputTypeDef,
     },
     total=False,
 )
 
 ClassificationResultTypeDef = TypedDict(
@@ -16603,21 +12490,21 @@
         "OwnerName": str,
         "OwnerAccountId": str,
         "CreatedAt": str,
         "ServerSideEncryptionConfiguration": (
             AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef
         ),
         "BucketLifecycleConfiguration": AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef,
-        "PublicAccessBlockConfiguration": AwsS3AccountPublicAccessBlockDetailsOutputTypeDef,
+        "PublicAccessBlockConfiguration": AwsS3AccountPublicAccessBlockDetailsTypeDef,
         "AccessControlList": str,
-        "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationOutputTypeDef,
+        "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationTypeDef,
         "BucketWebsiteConfiguration": AwsS3BucketWebsiteConfigurationOutputTypeDef,
         "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationOutputTypeDef,
-        "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationOutputTypeDef,
-        "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationOutputTypeDef,
+        "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationTypeDef,
+        "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationTypeDef,
     },
     total=False,
 )
 
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
@@ -16709,45 +12596,45 @@
         "AwsCodeBuildProject": AwsCodeBuildProjectDetailsOutputTypeDef,
         "AwsCloudFrontDistribution": AwsCloudFrontDistributionDetailsOutputTypeDef,
         "AwsEc2Instance": AwsEc2InstanceDetailsOutputTypeDef,
         "AwsEc2NetworkInterface": AwsEc2NetworkInterfaceDetailsOutputTypeDef,
         "AwsEc2SecurityGroup": AwsEc2SecurityGroupDetailsOutputTypeDef,
         "AwsEc2Volume": AwsEc2VolumeDetailsOutputTypeDef,
         "AwsEc2Vpc": AwsEc2VpcDetailsOutputTypeDef,
-        "AwsEc2Eip": AwsEc2EipDetailsOutputTypeDef,
+        "AwsEc2Eip": AwsEc2EipDetailsTypeDef,
         "AwsEc2Subnet": AwsEc2SubnetDetailsOutputTypeDef,
         "AwsEc2NetworkAcl": AwsEc2NetworkAclDetailsOutputTypeDef,
         "AwsElbv2LoadBalancer": AwsElbv2LoadBalancerDetailsOutputTypeDef,
         "AwsElasticBeanstalkEnvironment": AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
         "AwsElasticsearchDomain": AwsElasticsearchDomainDetailsOutputTypeDef,
         "AwsS3Bucket": AwsS3BucketDetailsOutputTypeDef,
-        "AwsS3AccountPublicAccessBlock": AwsS3AccountPublicAccessBlockDetailsOutputTypeDef,
-        "AwsS3Object": AwsS3ObjectDetailsOutputTypeDef,
-        "AwsSecretsManagerSecret": AwsSecretsManagerSecretDetailsOutputTypeDef,
-        "AwsIamAccessKey": AwsIamAccessKeyDetailsOutputTypeDef,
+        "AwsS3AccountPublicAccessBlock": AwsS3AccountPublicAccessBlockDetailsTypeDef,
+        "AwsS3Object": AwsS3ObjectDetailsTypeDef,
+        "AwsSecretsManagerSecret": AwsSecretsManagerSecretDetailsTypeDef,
+        "AwsIamAccessKey": AwsIamAccessKeyDetailsTypeDef,
         "AwsIamUser": AwsIamUserDetailsOutputTypeDef,
         "AwsIamPolicy": AwsIamPolicyDetailsOutputTypeDef,
         "AwsApiGatewayV2Stage": AwsApiGatewayV2StageDetailsOutputTypeDef,
         "AwsApiGatewayV2Api": AwsApiGatewayV2ApiDetailsOutputTypeDef,
         "AwsDynamoDbTable": AwsDynamoDbTableDetailsOutputTypeDef,
         "AwsApiGatewayStage": AwsApiGatewayStageDetailsOutputTypeDef,
         "AwsApiGatewayRestApi": AwsApiGatewayRestApiDetailsOutputTypeDef,
-        "AwsCloudTrailTrail": AwsCloudTrailTrailDetailsOutputTypeDef,
-        "AwsSsmPatchCompliance": AwsSsmPatchComplianceDetailsOutputTypeDef,
+        "AwsCloudTrailTrail": AwsCloudTrailTrailDetailsTypeDef,
+        "AwsSsmPatchCompliance": AwsSsmPatchComplianceDetailsTypeDef,
         "AwsCertificateManagerCertificate": AwsCertificateManagerCertificateDetailsOutputTypeDef,
         "AwsRedshiftCluster": AwsRedshiftClusterDetailsOutputTypeDef,
         "AwsElbLoadBalancer": AwsElbLoadBalancerDetailsOutputTypeDef,
         "AwsIamGroup": AwsIamGroupDetailsOutputTypeDef,
         "AwsIamRole": AwsIamRoleDetailsOutputTypeDef,
-        "AwsKmsKey": AwsKmsKeyDetailsOutputTypeDef,
+        "AwsKmsKey": AwsKmsKeyDetailsTypeDef,
         "AwsLambdaFunction": AwsLambdaFunctionDetailsOutputTypeDef,
         "AwsLambdaLayerVersion": AwsLambdaLayerVersionDetailsOutputTypeDef,
         "AwsRdsDbInstance": AwsRdsDbInstanceDetailsOutputTypeDef,
         "AwsSnsTopic": AwsSnsTopicDetailsOutputTypeDef,
-        "AwsSqsQueue": AwsSqsQueueDetailsOutputTypeDef,
+        "AwsSqsQueue": AwsSqsQueueDetailsTypeDef,
         "AwsWafWebAcl": AwsWafWebAclDetailsOutputTypeDef,
         "AwsRdsDbSnapshot": AwsRdsDbSnapshotDetailsOutputTypeDef,
         "AwsRdsDbClusterSnapshot": AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
         "AwsRdsDbCluster": AwsRdsDbClusterDetailsOutputTypeDef,
         "AwsEcsCluster": AwsEcsClusterDetailsOutputTypeDef,
         "AwsEcsContainer": AwsEcsContainerDetailsOutputTypeDef,
         "AwsEcsTaskDefinition": AwsEcsTaskDefinitionDetailsOutputTypeDef,
@@ -16756,49 +12643,49 @@
         "AwsRdsEventSubscription": AwsRdsEventSubscriptionDetailsOutputTypeDef,
         "AwsEcsService": AwsEcsServiceDetailsOutputTypeDef,
         "AwsAutoScalingLaunchConfiguration": AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
         "AwsEc2VpnConnection": AwsEc2VpnConnectionDetailsOutputTypeDef,
         "AwsEcrContainerImage": AwsEcrContainerImageDetailsOutputTypeDef,
         "AwsOpenSearchServiceDomain": AwsOpenSearchServiceDomainDetailsOutputTypeDef,
         "AwsEc2VpcEndpointService": AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
-        "AwsXrayEncryptionConfig": AwsXrayEncryptionConfigDetailsOutputTypeDef,
+        "AwsXrayEncryptionConfig": AwsXrayEncryptionConfigDetailsTypeDef,
         "AwsWafRateBasedRule": AwsWafRateBasedRuleDetailsOutputTypeDef,
         "AwsWafRegionalRateBasedRule": AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
-        "AwsEcrRepository": AwsEcrRepositoryDetailsOutputTypeDef,
+        "AwsEcrRepository": AwsEcrRepositoryDetailsTypeDef,
         "AwsEksCluster": AwsEksClusterDetailsOutputTypeDef,
         "AwsNetworkFirewallFirewallPolicy": AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef,
         "AwsNetworkFirewallFirewall": AwsNetworkFirewallFirewallDetailsOutputTypeDef,
         "AwsNetworkFirewallRuleGroup": AwsNetworkFirewallRuleGroupDetailsOutputTypeDef,
         "AwsRdsDbSecurityGroup": AwsRdsDbSecurityGroupDetailsOutputTypeDef,
-        "AwsKinesisStream": AwsKinesisStreamDetailsOutputTypeDef,
+        "AwsKinesisStream": AwsKinesisStreamDetailsTypeDef,
         "AwsEc2TransitGateway": AwsEc2TransitGatewayDetailsOutputTypeDef,
         "AwsEfsAccessPoint": AwsEfsAccessPointDetailsOutputTypeDef,
         "AwsCloudFormationStack": AwsCloudFormationStackDetailsOutputTypeDef,
         "AwsCloudWatchAlarm": AwsCloudWatchAlarmDetailsOutputTypeDef,
         "AwsEc2VpcPeeringConnection": AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
         "AwsWafRegionalRuleGroup": AwsWafRegionalRuleGroupDetailsOutputTypeDef,
         "AwsWafRegionalRule": AwsWafRegionalRuleDetailsOutputTypeDef,
         "AwsWafRegionalWebAcl": AwsWafRegionalWebAclDetailsOutputTypeDef,
         "AwsWafRule": AwsWafRuleDetailsOutputTypeDef,
         "AwsWafRuleGroup": AwsWafRuleGroupDetailsOutputTypeDef,
         "AwsEcsTask": AwsEcsTaskDetailsOutputTypeDef,
         "AwsBackupBackupVault": AwsBackupBackupVaultDetailsOutputTypeDef,
         "AwsBackupBackupPlan": AwsBackupBackupPlanDetailsOutputTypeDef,
-        "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsOutputTypeDef,
+        "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsTypeDef,
         "AwsEc2LaunchTemplate": AwsEc2LaunchTemplateDetailsOutputTypeDef,
         "AwsSageMakerNotebookInstance": AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
         "AwsWafv2WebAcl": AwsWafv2WebAclDetailsOutputTypeDef,
         "AwsWafv2RuleGroup": AwsWafv2RuleGroupDetailsOutputTypeDef,
         "AwsEc2RouteTable": AwsEc2RouteTableDetailsOutputTypeDef,
         "AwsAmazonMqBroker": AwsAmazonMqBrokerDetailsOutputTypeDef,
         "AwsAppSyncGraphQlApi": AwsAppSyncGraphQlApiDetailsOutputTypeDef,
-        "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsOutputTypeDef,
+        "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsTypeDef,
         "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsOutputTypeDef,
         "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsOutputTypeDef,
-        "AwsAthenaWorkGroup": AwsAthenaWorkGroupDetailsOutputTypeDef,
+        "AwsAthenaWorkGroup": AwsAthenaWorkGroupDetailsTypeDef,
     },
     total=False,
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
@@ -16966,36 +12853,36 @@
     {
         "ProductName": str,
         "CompanyName": str,
         "Region": str,
         "Types": List[str],
         "FirstObservedAt": str,
         "LastObservedAt": str,
-        "Severity": SeverityOutputTypeDef,
+        "Severity": SeverityTypeDef,
         "Confidence": int,
         "Criticality": int,
-        "Remediation": RemediationOutputTypeDef,
+        "Remediation": RemediationTypeDef,
         "SourceUrl": str,
         "ProductFields": Dict[str, str],
         "UserDefinedFields": Dict[str, str],
-        "Malware": List[MalwareOutputTypeDef],
-        "Network": NetworkOutputTypeDef,
+        "Malware": List[MalwareTypeDef],
+        "Network": NetworkTypeDef,
         "NetworkPath": List[NetworkPathComponentOutputTypeDef],
-        "Process": ProcessDetailsOutputTypeDef,
+        "Process": ProcessDetailsTypeDef,
         "Threats": List[ThreatOutputTypeDef],
-        "ThreatIntelIndicators": List[ThreatIntelIndicatorOutputTypeDef],
+        "ThreatIntelIndicators": List[ThreatIntelIndicatorTypeDef],
         "Compliance": ComplianceOutputTypeDef,
         "VerificationState": VerificationStateType,
         "WorkflowState": WorkflowStateType,
-        "Workflow": WorkflowOutputTypeDef,
+        "Workflow": WorkflowTypeDef,
         "RecordState": RecordStateType,
-        "RelatedFindings": List[RelatedFindingOutputTypeDef],
-        "Note": NoteOutputTypeDef,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+        "Note": NoteTypeDef,
         "Vulnerabilities": List[VulnerabilityOutputTypeDef],
-        "PatchSummary": PatchSummaryOutputTypeDef,
+        "PatchSummary": PatchSummaryTypeDef,
         "Action": ActionOutputTypeDef,
         "FindingProviderFields": FindingProviderFieldsOutputTypeDef,
         "Sample": bool,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub/type_defs.pyi` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub/type_defs.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -58,682 +58,388 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AcceptAdministratorInvitationRequestRequestTypeDef",
     "AcceptInvitationRequestRequestTypeDef",
     "AccountDetailsTypeDef",
-    "ActionLocalIpDetailsOutputTypeDef",
     "ActionLocalIpDetailsTypeDef",
-    "ActionLocalPortDetailsOutputTypeDef",
     "ActionLocalPortDetailsTypeDef",
-    "DnsRequestActionOutputTypeDef",
-    "CityOutputTypeDef",
-    "CountryOutputTypeDef",
-    "GeoLocationOutputTypeDef",
-    "IpOrganizationDetailsOutputTypeDef",
+    "DnsRequestActionTypeDef",
     "CityTypeDef",
     "CountryTypeDef",
     "GeoLocationTypeDef",
     "IpOrganizationDetailsTypeDef",
-    "ActionRemotePortDetailsOutputTypeDef",
     "ActionRemotePortDetailsTypeDef",
     "ActionTargetTypeDef",
-    "DnsRequestActionTypeDef",
-    "AdjustmentOutputTypeDef",
     "AdjustmentTypeDef",
     "AdminAccountTypeDef",
-    "AssociatedStandardOutputTypeDef",
     "AssociatedStandardTypeDef",
-    "AssociationStateDetailsOutputTypeDef",
     "AssociationStateDetailsTypeDef",
-    "NoteUpdateOutputTypeDef",
-    "RelatedFindingOutputTypeDef",
-    "SeverityUpdateOutputTypeDef",
-    "WorkflowUpdateOutputTypeDef",
     "NoteUpdateTypeDef",
     "RelatedFindingTypeDef",
     "SeverityUpdateTypeDef",
     "WorkflowUpdateTypeDef",
-    "MapFilterOutputTypeDef",
-    "NumberFilterOutputTypeDef",
-    "StringFilterOutputTypeDef",
     "MapFilterTypeDef",
     "NumberFilterTypeDef",
     "StringFilterTypeDef",
     "AutomationRulesMetadataTypeDef",
-    "AvailabilityZoneOutputTypeDef",
     "AvailabilityZoneTypeDef",
-    "AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef",
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
-    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef",
-    "AwsAmazonMqBrokerUsersDetailsOutputTypeDef",
     "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
-    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef",
     "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
     "AwsAmazonMqBrokerUsersDetailsTypeDef",
-    "AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef",
+    "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
-    "AwsApiCallActionDomainDetailsOutputTypeDef",
     "AwsApiCallActionDomainDetailsTypeDef",
-    "AwsApiGatewayAccessLogSettingsOutputTypeDef",
     "AwsApiGatewayAccessLogSettingsTypeDef",
     "AwsApiGatewayCanarySettingsOutputTypeDef",
     "AwsApiGatewayCanarySettingsTypeDef",
     "AwsApiGatewayEndpointConfigurationOutputTypeDef",
     "AwsApiGatewayEndpointConfigurationTypeDef",
-    "AwsApiGatewayMethodSettingsOutputTypeDef",
     "AwsApiGatewayMethodSettingsTypeDef",
     "AwsCorsConfigurationOutputTypeDef",
     "AwsCorsConfigurationTypeDef",
-    "AwsApiGatewayV2RouteSettingsOutputTypeDef",
     "AwsApiGatewayV2RouteSettingsTypeDef",
-    "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef",
-    "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef",
-    "AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef",
     "AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef",
-    "AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
-    "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef",
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef",
-    "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
-    "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef",
-    "AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef",
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef",
     "AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef",
-    "AwsBackupBackupPlanLifecycleDetailsOutputTypeDef",
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
     "AwsBackupBackupVaultNotificationsDetailsOutputTypeDef",
     "AwsBackupBackupVaultNotificationsDetailsTypeDef",
-    "AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef",
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
-    "AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef",
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
-    "AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef",
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
-    "AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef",
-    "AwsCertificateManagerCertificateKeyUsageOutputTypeDef",
-    "AwsCertificateManagerCertificateOptionsOutputTypeDef",
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     "AwsCertificateManagerCertificateKeyUsageTypeDef",
     "AwsCertificateManagerCertificateOptionsTypeDef",
-    "AwsCertificateManagerCertificateResourceRecordOutputTypeDef",
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
-    "AwsCloudFormationStackDriftInformationDetailsOutputTypeDef",
-    "AwsCloudFormationStackOutputsDetailsOutputTypeDef",
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     "AwsCloudFormationStackOutputsDetailsTypeDef",
-    "AwsCloudFrontDistributionCacheBehaviorOutputTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
-    "AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef",
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
-    "AwsCloudFrontDistributionLoggingOutputTypeDef",
-    "AwsCloudFrontDistributionViewerCertificateOutputTypeDef",
     "AwsCloudFrontDistributionLoggingTypeDef",
     "AwsCloudFrontDistributionViewerCertificateTypeDef",
     "AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef",
     "AwsCloudFrontDistributionOriginSslProtocolsTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef",
-    "AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef",
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
-    "AwsCloudTrailTrailDetailsOutputTypeDef",
     "AwsCloudTrailTrailDetailsTypeDef",
-    "AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef",
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
-    "AwsCodeBuildProjectArtifactsDetailsOutputTypeDef",
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
-    "AwsCodeBuildProjectSourceOutputTypeDef",
-    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     "AwsCodeBuildProjectSourceTypeDef",
+    "AwsCodeBuildProjectVpcConfigOutputTypeDef",
     "AwsCodeBuildProjectVpcConfigTypeDef",
-    "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
-    "AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
-    "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef",
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
-    "AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef",
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
-    "AwsDynamoDbTableAttributeDefinitionOutputTypeDef",
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
-    "AwsDynamoDbTableBillingModeSummaryOutputTypeDef",
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
-    "AwsDynamoDbTableKeySchemaOutputTypeDef",
-    "AwsDynamoDbTableProvisionedThroughputOutputTypeDef",
-    "AwsDynamoDbTableRestoreSummaryOutputTypeDef",
-    "AwsDynamoDbTableSseDescriptionOutputTypeDef",
-    "AwsDynamoDbTableStreamSpecificationOutputTypeDef",
     "AwsDynamoDbTableKeySchemaTypeDef",
     "AwsDynamoDbTableProvisionedThroughputTypeDef",
     "AwsDynamoDbTableRestoreSummaryTypeDef",
     "AwsDynamoDbTableSseDescriptionTypeDef",
     "AwsDynamoDbTableStreamSpecificationTypeDef",
     "AwsDynamoDbTableProjectionOutputTypeDef",
     "AwsDynamoDbTableProjectionTypeDef",
-    "AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef",
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
-    "AwsEc2EipDetailsOutputTypeDef",
     "AwsEc2EipDetailsTypeDef",
-    "AwsEc2InstanceMetadataOptionsOutputTypeDef",
-    "AwsEc2InstanceMonitoringDetailsOutputTypeDef",
-    "AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef",
     "AwsEc2InstanceMetadataOptionsTypeDef",
     "AwsEc2InstanceMonitoringDetailsTypeDef",
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef",
     "AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef",
     "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef",
     "AwsEc2LaunchTemplateDataPlacementDetailsTypeDef",
     "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef",
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef",
-    "AwsEc2NetworkAclAssociationOutputTypeDef",
     "AwsEc2NetworkAclAssociationTypeDef",
-    "IcmpTypeCodeOutputTypeDef",
-    "PortRangeFromToOutputTypeDef",
     "IcmpTypeCodeTypeDef",
     "PortRangeFromToTypeDef",
-    "AwsEc2NetworkInterfaceAttachmentOutputTypeDef",
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
-    "AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef",
-    "AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef",
-    "AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef",
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     "AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef",
     "AwsEc2NetworkInterfaceSecurityGroupTypeDef",
-    "PropagatingVgwSetDetailsOutputTypeDef",
-    "RouteSetDetailsOutputTypeDef",
     "PropagatingVgwSetDetailsTypeDef",
     "RouteSetDetailsTypeDef",
-    "AwsEc2SecurityGroupIpRangeOutputTypeDef",
-    "AwsEc2SecurityGroupIpv6RangeOutputTypeDef",
-    "AwsEc2SecurityGroupPrefixListIdOutputTypeDef",
-    "AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef",
     "AwsEc2SecurityGroupIpRangeTypeDef",
     "AwsEc2SecurityGroupIpv6RangeTypeDef",
     "AwsEc2SecurityGroupPrefixListIdTypeDef",
     "AwsEc2SecurityGroupUserIdGroupPairTypeDef",
-    "Ipv6CidrBlockAssociationOutputTypeDef",
     "Ipv6CidrBlockAssociationTypeDef",
     "AwsEc2TransitGatewayDetailsOutputTypeDef",
     "AwsEc2TransitGatewayDetailsTypeDef",
-    "AwsEc2VolumeAttachmentOutputTypeDef",
     "AwsEc2VolumeAttachmentTypeDef",
-    "CidrBlockAssociationOutputTypeDef",
     "CidrBlockAssociationTypeDef",
-    "AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef",
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
-    "AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
-    "VpcInfoCidrBlockSetDetailsOutputTypeDef",
-    "VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef",
-    "VpcInfoPeeringOptionsDetailsOutputTypeDef",
     "VpcInfoCidrBlockSetDetailsTypeDef",
     "VpcInfoIpv6CidrBlockSetDetailsTypeDef",
     "VpcInfoPeeringOptionsDetailsTypeDef",
-    "AwsEc2VpnConnectionRoutesDetailsOutputTypeDef",
-    "AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef",
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     "AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef",
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef",
     "AwsEcrContainerImageDetailsOutputTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
-    "AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef",
-    "AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef",
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     "AwsEcrRepositoryLifecyclePolicyDetailsTypeDef",
-    "AwsEcsClusterClusterSettingsDetailsOutputTypeDef",
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
-    "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
-    "AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef",
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
-    "AwsMountPointOutputTypeDef",
     "AwsMountPointTypeDef",
-    "AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef",
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
-    "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef",
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
-    "AwsEcsServiceDeploymentControllerDetailsOutputTypeDef",
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
-    "AwsEcsServiceLoadBalancersDetailsOutputTypeDef",
-    "AwsEcsServicePlacementConstraintsDetailsOutputTypeDef",
-    "AwsEcsServicePlacementStrategiesDetailsOutputTypeDef",
-    "AwsEcsServiceServiceRegistriesDetailsOutputTypeDef",
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     "AwsEcsServicePlacementConstraintsDetailsTypeDef",
     "AwsEcsServicePlacementStrategiesDetailsTypeDef",
     "AwsEcsServiceServiceRegistriesDetailsTypeDef",
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
+    "AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef",
-    "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
-    "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     "AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef",
-    "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef",
-    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef",
+    "AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
-    "AwsEcsTaskVolumeHostDetailsOutputTypeDef",
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     "AwsEfsAccessPointPosixUserDetailsOutputTypeDef",
     "AwsEfsAccessPointPosixUserDetailsTypeDef",
-    "AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef",
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
     "AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef",
     "AwsEksClusterResourcesVpcConfigDetailsTypeDef",
     "AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingClusterLoggingDetailsTypeDef",
-    "AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef",
-    "AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef",
-    "AwsElasticBeanstalkEnvironmentTierOutputTypeDef",
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     "AwsElasticBeanstalkEnvironmentOptionSettingTypeDef",
     "AwsElasticBeanstalkEnvironmentTierTypeDef",
-    "AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef",
-    "AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef",
-    "AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef",
-    "AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef",
-    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
     "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
     "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
+    "AwsElasticsearchDomainVPCOptionsOutputTypeDef",
     "AwsElasticsearchDomainVPCOptionsTypeDef",
-    "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
-    "AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
-    "AwsElbAppCookieStickinessPolicyOutputTypeDef",
     "AwsElbAppCookieStickinessPolicyTypeDef",
-    "AwsElbLbCookieStickinessPolicyOutputTypeDef",
     "AwsElbLbCookieStickinessPolicyTypeDef",
-    "AwsElbLoadBalancerAccessLogOutputTypeDef",
     "AwsElbLoadBalancerAccessLogTypeDef",
-    "AwsElbLoadBalancerAdditionalAttributeOutputTypeDef",
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
-    "AwsElbLoadBalancerConnectionDrainingOutputTypeDef",
-    "AwsElbLoadBalancerConnectionSettingsOutputTypeDef",
-    "AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef",
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     "AwsElbLoadBalancerConnectionSettingsTypeDef",
     "AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef",
     "AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerBackendServerDescriptionTypeDef",
-    "AwsElbLoadBalancerHealthCheckOutputTypeDef",
-    "AwsElbLoadBalancerInstanceOutputTypeDef",
-    "AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef",
     "AwsElbLoadBalancerHealthCheckTypeDef",
     "AwsElbLoadBalancerInstanceTypeDef",
     "AwsElbLoadBalancerSourceSecurityGroupTypeDef",
-    "AwsElbLoadBalancerListenerOutputTypeDef",
     "AwsElbLoadBalancerListenerTypeDef",
-    "AwsElbv2LoadBalancerAttributeOutputTypeDef",
     "AwsElbv2LoadBalancerAttributeTypeDef",
-    "LoadBalancerStateOutputTypeDef",
     "LoadBalancerStateTypeDef",
-    "AwsEventSchemasRegistryDetailsOutputTypeDef",
     "AwsEventSchemasRegistryDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef",
-    "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef",
-    "AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef",
     "AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
-    "AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef",
     "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
-    "AwsIamAccessKeySessionContextAttributesOutputTypeDef",
     "AwsIamAccessKeySessionContextAttributesTypeDef",
-    "AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef",
     "AwsIamAccessKeySessionContextSessionIssuerTypeDef",
-    "AwsIamAttachedManagedPolicyOutputTypeDef",
     "AwsIamAttachedManagedPolicyTypeDef",
-    "AwsIamGroupPolicyOutputTypeDef",
     "AwsIamGroupPolicyTypeDef",
-    "AwsIamInstanceProfileRoleOutputTypeDef",
     "AwsIamInstanceProfileRoleTypeDef",
-    "AwsIamPermissionsBoundaryOutputTypeDef",
     "AwsIamPermissionsBoundaryTypeDef",
-    "AwsIamPolicyVersionOutputTypeDef",
     "AwsIamPolicyVersionTypeDef",
-    "AwsIamRolePolicyOutputTypeDef",
     "AwsIamRolePolicyTypeDef",
-    "AwsIamUserPolicyOutputTypeDef",
     "AwsIamUserPolicyTypeDef",
-    "AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef",
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
-    "AwsKmsKeyDetailsOutputTypeDef",
     "AwsKmsKeyDetailsTypeDef",
-    "AwsLambdaFunctionCodeOutputTypeDef",
     "AwsLambdaFunctionCodeTypeDef",
-    "AwsLambdaFunctionDeadLetterConfigOutputTypeDef",
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
-    "AwsLambdaFunctionLayerOutputTypeDef",
-    "AwsLambdaFunctionTracingConfigOutputTypeDef",
-    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     "AwsLambdaFunctionLayerTypeDef",
     "AwsLambdaFunctionTracingConfigTypeDef",
+    "AwsLambdaFunctionVpcConfigOutputTypeDef",
     "AwsLambdaFunctionVpcConfigTypeDef",
-    "AwsLambdaFunctionEnvironmentErrorOutputTypeDef",
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
     "AwsLambdaLayerVersionDetailsOutputTypeDef",
     "AwsLambdaLayerVersionDetailsTypeDef",
-    "AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef",
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
-    "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef",
-    "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef",
-    "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef",
-    "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef",
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef",
     "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef",
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
-    "AwsRdsDbClusterAssociatedRoleOutputTypeDef",
     "AwsRdsDbClusterAssociatedRoleTypeDef",
-    "AwsRdsDbClusterMemberOutputTypeDef",
-    "AwsRdsDbClusterOptionGroupMembershipOutputTypeDef",
-    "AwsRdsDbDomainMembershipOutputTypeDef",
-    "AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef",
     "AwsRdsDbClusterMemberTypeDef",
     "AwsRdsDbClusterOptionGroupMembershipTypeDef",
     "AwsRdsDbDomainMembershipTypeDef",
     "AwsRdsDbInstanceVpcSecurityGroupTypeDef",
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef",
     "AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef",
-    "AwsRdsDbInstanceAssociatedRoleOutputTypeDef",
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
-    "AwsRdsDbInstanceEndpointOutputTypeDef",
-    "AwsRdsDbOptionGroupMembershipOutputTypeDef",
-    "AwsRdsDbParameterGroupOutputTypeDef",
-    "AwsRdsDbProcessorFeatureOutputTypeDef",
-    "AwsRdsDbStatusInfoOutputTypeDef",
     "AwsRdsDbInstanceEndpointTypeDef",
     "AwsRdsDbOptionGroupMembershipTypeDef",
     "AwsRdsDbParameterGroupTypeDef",
     "AwsRdsDbProcessorFeatureTypeDef",
     "AwsRdsDbStatusInfoTypeDef",
     "AwsRdsPendingCloudWatchLogsExportsOutputTypeDef",
     "AwsRdsPendingCloudWatchLogsExportsTypeDef",
-    "AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef",
-    "AwsRdsDbSecurityGroupIpRangeOutputTypeDef",
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     "AwsRdsDbSecurityGroupIpRangeTypeDef",
-    "AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef",
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     "AwsRdsEventSubscriptionDetailsOutputTypeDef",
     "AwsRdsEventSubscriptionDetailsTypeDef",
-    "AwsRedshiftClusterClusterNodeOutputTypeDef",
     "AwsRedshiftClusterClusterNodeTypeDef",
-    "AwsRedshiftClusterClusterParameterStatusOutputTypeDef",
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
-    "AwsRedshiftClusterClusterSecurityGroupOutputTypeDef",
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
-    "AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef",
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
-    "AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef",
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
-    "AwsRedshiftClusterElasticIpStatusOutputTypeDef",
-    "AwsRedshiftClusterEndpointOutputTypeDef",
-    "AwsRedshiftClusterHsmStatusOutputTypeDef",
-    "AwsRedshiftClusterIamRoleOutputTypeDef",
-    "AwsRedshiftClusterLoggingStatusOutputTypeDef",
-    "AwsRedshiftClusterPendingModifiedValuesOutputTypeDef",
-    "AwsRedshiftClusterResizeInfoOutputTypeDef",
-    "AwsRedshiftClusterRestoreStatusOutputTypeDef",
-    "AwsRedshiftClusterVpcSecurityGroupOutputTypeDef",
     "AwsRedshiftClusterElasticIpStatusTypeDef",
     "AwsRedshiftClusterEndpointTypeDef",
     "AwsRedshiftClusterHsmStatusTypeDef",
     "AwsRedshiftClusterIamRoleTypeDef",
     "AwsRedshiftClusterLoggingStatusTypeDef",
     "AwsRedshiftClusterPendingModifiedValuesTypeDef",
     "AwsRedshiftClusterResizeInfoTypeDef",
     "AwsRedshiftClusterRestoreStatusTypeDef",
     "AwsRedshiftClusterVpcSecurityGroupTypeDef",
-    "AwsS3AccountPublicAccessBlockDetailsOutputTypeDef",
     "AwsS3AccountPublicAccessBlockDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef",
-    "AwsS3BucketBucketVersioningConfigurationOutputTypeDef",
     "AwsS3BucketBucketVersioningConfigurationTypeDef",
-    "AwsS3BucketLoggingConfigurationOutputTypeDef",
     "AwsS3BucketLoggingConfigurationTypeDef",
-    "AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
-    "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef",
     "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
-    "AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef",
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
-    "AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
-    "AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
-    "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
-    "AwsS3ObjectDetailsOutputTypeDef",
     "AwsS3ObjectDetailsTypeDef",
-    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
-    "AwsSecretsManagerSecretRotationRulesOutputTypeDef",
     "AwsSecretsManagerSecretRotationRulesTypeDef",
-    "BooleanFilterOutputTypeDef",
-    "IpFilterOutputTypeDef",
-    "KeywordFilterOutputTypeDef",
     "BooleanFilterTypeDef",
     "IpFilterTypeDef",
     "KeywordFilterTypeDef",
-    "AwsSecurityFindingIdentifierOutputTypeDef",
     "AwsSecurityFindingIdentifierTypeDef",
-    "MalwareOutputTypeDef",
-    "NoteOutputTypeDef",
-    "PatchSummaryOutputTypeDef",
-    "ProcessDetailsOutputTypeDef",
-    "SeverityOutputTypeDef",
-    "ThreatIntelIndicatorOutputTypeDef",
-    "WorkflowOutputTypeDef",
     "MalwareTypeDef",
     "NoteTypeDef",
     "PatchSummaryTypeDef",
     "ProcessDetailsTypeDef",
     "SeverityTypeDef",
     "ThreatIntelIndicatorTypeDef",
     "WorkflowTypeDef",
-    "AwsSnsTopicSubscriptionOutputTypeDef",
     "AwsSnsTopicSubscriptionTypeDef",
-    "AwsSqsQueueDetailsOutputTypeDef",
     "AwsSqsQueueDetailsTypeDef",
-    "AwsSsmComplianceSummaryOutputTypeDef",
     "AwsSsmComplianceSummaryTypeDef",
-    "AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
-    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
-    "AwsWafRateBasedRuleMatchPredicateOutputTypeDef",
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
-    "AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef",
     "AwsWafRegionalRateBasedRuleMatchPredicateTypeDef",
-    "AwsWafRegionalRulePredicateListDetailsOutputTypeDef",
     "AwsWafRegionalRulePredicateListDetailsTypeDef",
-    "AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupRulesActionDetailsTypeDef",
-    "AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef",
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
-    "AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef",
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
-    "AwsWafRulePredicateListDetailsOutputTypeDef",
     "AwsWafRulePredicateListDetailsTypeDef",
-    "AwsWafRuleGroupRulesActionDetailsOutputTypeDef",
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
-    "WafActionOutputTypeDef",
-    "WafExcludedRuleOutputTypeDef",
-    "WafOverrideActionOutputTypeDef",
     "WafActionTypeDef",
     "WafExcludedRuleTypeDef",
     "WafOverrideActionTypeDef",
-    "AwsWafv2CustomHttpHeaderOutputTypeDef",
     "AwsWafv2CustomHttpHeaderTypeDef",
-    "AwsWafv2VisibilityConfigDetailsOutputTypeDef",
     "AwsWafv2VisibilityConfigDetailsTypeDef",
-    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef",
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
-    "AwsXrayEncryptionConfigDetailsOutputTypeDef",
     "AwsXrayEncryptionConfigDetailsTypeDef",
     "BatchDeleteAutomationRulesRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedAutomationRuleTypeDef",
     "BatchDisableStandardsRequestRequestTypeDef",
     "StandardsSubscriptionRequestTypeDef",
     "BatchGetAutomationRulesRequestRequestTypeDef",
     "BatchGetSecurityControlsRequestRequestTypeDef",
     "SecurityControlTypeDef",
     "UnprocessedSecurityControlTypeDef",
     "StandardsControlAssociationIdTypeDef",
     "StandardsControlAssociationDetailTypeDef",
     "ImportFindingsErrorTypeDef",
     "StandardsControlAssociationUpdateTypeDef",
-    "CellOutputTypeDef",
     "CellTypeDef",
-    "ClassificationStatusOutputTypeDef",
     "ClassificationStatusTypeDef",
-    "StatusReasonOutputTypeDef",
     "StatusReasonTypeDef",
-    "VolumeMountOutputTypeDef",
     "VolumeMountTypeDef",
     "CreateActionTargetRequestRequestTypeDef",
     "CreateFindingAggregatorRequestRequestTypeDef",
     "ResultTypeDef",
-    "DateRangeOutputTypeDef",
     "DateRangeTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteActionTargetRequestRequestTypeDef",
     "DeleteFindingAggregatorRequestRequestTypeDef",
     "DeleteInsightRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
@@ -747,23 +453,19 @@
     "DescribeStandardsRequestRequestTypeDef",
     "DisableImportFindingsForProductRequestRequestTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMembersRequestRequestTypeDef",
     "EnableImportFindingsForProductRequestRequestTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "EnableSecurityHubRequestRequestTypeDef",
-    "FilePathsOutputTypeDef",
     "FilePathsTypeDef",
     "FindingAggregatorTypeDef",
     "FindingHistoryUpdateSourceTypeDef",
     "FindingHistoryUpdateTypeDef",
-    "FindingProviderSeverityOutputTypeDef",
     "FindingProviderSeverityTypeDef",
-    "FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef",
-    "FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef",
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     "FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef",
     "InvitationTypeDef",
     "GetEnabledStandardsRequestRequestTypeDef",
     "GetFindingAggregatorRequestRequestTypeDef",
     "SortCriterionTypeDef",
     "GetInsightResultsRequestRequestTypeDef",
@@ -779,91 +481,69 @@
     "ListMembersRequestRequestTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListSecurityControlDefinitionsRequestRequestTypeDef",
     "SecurityControlDefinitionTypeDef",
     "ListStandardsControlAssociationsRequestRequestTypeDef",
     "StandardsControlAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PortRangeOutputTypeDef",
     "PortRangeTypeDef",
-    "RangeOutputTypeDef",
-    "RecordOutputTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "RecommendationOutputTypeDef",
     "RecommendationTypeDef",
     "RuleGroupSourceListDetailsOutputTypeDef",
     "RuleGroupSourceListDetailsTypeDef",
-    "RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef",
-    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
+    "RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef",
-    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
+    "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     "RuleGroupVariablesIpSetsDetailsOutputTypeDef",
     "RuleGroupVariablesIpSetsDetailsTypeDef",
     "RuleGroupVariablesPortSetsDetailsOutputTypeDef",
     "RuleGroupVariablesPortSetsDetailsTypeDef",
-    "SoftwarePackageOutputTypeDef",
     "SoftwarePackageTypeDef",
     "StandardsManagedByTypeDef",
-    "StandardsControlAssociationIdOutputTypeDef",
-    "StandardsControlAssociationUpdateOutputTypeDef",
     "StandardsStatusReasonTypeDef",
-    "StatelessCustomPublishMetricActionDimensionOutputTypeDef",
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateActionTargetRequestRequestTypeDef",
     "UpdateFindingAggregatorRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateSecurityHubConfigurationRequestRequestTypeDef",
     "UpdateStandardsControlRequestRequestTypeDef",
-    "VulnerabilityVendorOutputTypeDef",
     "VulnerabilityVendorTypeDef",
     "CreateMembersRequestRequestTypeDef",
-    "ActionRemoteIpDetailsOutputTypeDef",
     "ActionRemoteIpDetailsTypeDef",
     "CvssOutputTypeDef",
     "CvssTypeDef",
-    "AssociationSetDetailsOutputTypeDef",
     "AssociationSetDetailsTypeDef",
     "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     "AutomationRulesFindingFieldsUpdateTypeDef",
-    "AwsAmazonMqBrokerLogsDetailsOutputTypeDef",
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     "AwsApiGatewayRestApiDetailsOutputTypeDef",
     "AwsApiGatewayRestApiDetailsTypeDef",
     "AwsApiGatewayStageDetailsOutputTypeDef",
     "AwsApiGatewayStageDetailsTypeDef",
     "AwsApiGatewayV2ApiDetailsOutputTypeDef",
     "AwsApiGatewayV2ApiDetailsTypeDef",
     "AwsApiGatewayV2StageDetailsOutputTypeDef",
     "AwsApiGatewayV2StageDetailsTypeDef",
-    "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
-    "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef",
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
-    "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
-    "AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef",
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     "AwsBackupBackupVaultDetailsOutputTypeDef",
     "AwsBackupBackupVaultDetailsTypeDef",
-    "AwsBackupRecoveryPointDetailsOutputTypeDef",
     "AwsBackupRecoveryPointDetailsTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     "AwsCertificateManagerCertificateDomainValidationOptionTypeDef",
     "AwsCloudFormationStackDetailsOutputTypeDef",
     "AwsCloudFormationStackDetailsTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
@@ -871,35 +551,29 @@
     "AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef",
     "AwsCloudFrontDistributionOriginGroupFailoverTypeDef",
     "AwsCloudWatchAlarmDetailsOutputTypeDef",
     "AwsCloudWatchAlarmDetailsTypeDef",
     "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     "AwsCodeBuildProjectEnvironmentTypeDef",
-    "AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef",
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
     "AwsDynamoDbTableLocalSecondaryIndexTypeDef",
-    "AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef",
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     "AwsEc2InstanceDetailsOutputTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef",
-    "AwsEc2NetworkAclEntryOutputTypeDef",
     "AwsEc2NetworkAclEntryTypeDef",
     "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     "AwsEc2NetworkInterfaceDetailsTypeDef",
     "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     "AwsEc2SubnetDetailsOutputTypeDef",
     "AwsEc2SubnetDetailsTypeDef",
@@ -909,136 +583,109 @@
     "AwsEc2VpcDetailsTypeDef",
     "AwsEc2VpcEndpointServiceDetailsOutputTypeDef",
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef",
     "AwsEc2VpnConnectionOptionsDetailsOutputTypeDef",
     "AwsEc2VpnConnectionOptionsDetailsTypeDef",
-    "AwsEcrRepositoryDetailsOutputTypeDef",
     "AwsEcrRepositoryDetailsTypeDef",
-    "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef",
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     "AwsEcsContainerDetailsOutputTypeDef",
     "AwsEcsContainerDetailsTypeDef",
-    "AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     "AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef",
     "AwsEcsServiceNetworkConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef",
-    "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
-    "AwsEcsTaskVolumeDetailsOutputTypeDef",
     "AwsEcsTaskVolumeDetailsTypeDef",
-    "AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef",
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
     "AwsEksClusterLoggingDetailsOutputTypeDef",
     "AwsEksClusterLoggingDetailsTypeDef",
     "AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef",
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
-    "AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef",
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
-    "AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef",
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     "AwsElbLoadBalancerPoliciesOutputTypeDef",
     "AwsElbLoadBalancerPoliciesTypeDef",
     "AwsElbLoadBalancerAttributesOutputTypeDef",
     "AwsElbLoadBalancerAttributesTypeDef",
     "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
     "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     "AwsElbv2LoadBalancerDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
-    "AwsIamAccessKeySessionContextOutputTypeDef",
     "AwsIamAccessKeySessionContextTypeDef",
     "AwsIamGroupDetailsOutputTypeDef",
     "AwsIamGroupDetailsTypeDef",
     "AwsIamInstanceProfileOutputTypeDef",
     "AwsIamInstanceProfileTypeDef",
     "AwsIamPolicyDetailsOutputTypeDef",
     "AwsIamPolicyDetailsTypeDef",
     "AwsIamUserDetailsOutputTypeDef",
     "AwsIamUserDetailsTypeDef",
-    "AwsKinesisStreamDetailsOutputTypeDef",
     "AwsKinesisStreamDetailsTypeDef",
     "AwsLambdaFunctionEnvironmentOutputTypeDef",
     "AwsLambdaFunctionEnvironmentTypeDef",
     "AwsNetworkFirewallFirewallDetailsOutputTypeDef",
     "AwsNetworkFirewallFirewallDetailsTypeDef",
-    "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
-    "AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
-    "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
     "AwsRdsDbClusterDetailsOutputTypeDef",
     "AwsRdsDbClusterDetailsTypeDef",
     "AwsRdsDbClusterSnapshotDetailsOutputTypeDef",
     "AwsRdsDbClusterSnapshotDetailsTypeDef",
     "AwsRdsDbSnapshotDetailsOutputTypeDef",
     "AwsRdsDbSnapshotDetailsTypeDef",
     "AwsRdsDbPendingModifiedValuesOutputTypeDef",
     "AwsRdsDbPendingModifiedValuesTypeDef",
     "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     "AwsRdsDbSecurityGroupDetailsTypeDef",
-    "AwsRdsDbSubnetGroupSubnetOutputTypeDef",
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     "AwsRedshiftClusterClusterParameterGroupTypeDef",
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
-    "AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef",
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
-    "AwsS3BucketServerSideEncryptionRuleOutputTypeDef",
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
-    "AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     "AwsSageMakerNotebookInstanceDetailsOutputTypeDef",
     "AwsSageMakerNotebookInstanceDetailsTypeDef",
-    "AwsSecretsManagerSecretDetailsOutputTypeDef",
     "AwsSecretsManagerSecretDetailsTypeDef",
-    "BatchUpdateFindingsUnprocessedFindingTypeDef",
     "BatchUpdateFindingsRequestRequestTypeDef",
+    "BatchUpdateFindingsUnprocessedFindingTypeDef",
     "GetFindingHistoryRequestRequestTypeDef",
     "AwsSnsTopicDetailsOutputTypeDef",
     "AwsSnsTopicDetailsTypeDef",
-    "AwsSsmPatchOutputTypeDef",
     "AwsSsmPatchTypeDef",
-    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     "AwsWafRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     "AwsWafRegionalRuleDetailsOutputTypeDef",
     "AwsWafRegionalRuleDetailsTypeDef",
-    "AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
-    "AwsWafRegionalWebAclRulesListDetailsOutputTypeDef",
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     "AwsWafRuleDetailsOutputTypeDef",
     "AwsWafRuleDetailsTypeDef",
-    "AwsWafRuleGroupRulesDetailsOutputTypeDef",
     "AwsWafRuleGroupRulesDetailsTypeDef",
     "AwsWafWebAclRuleOutputTypeDef",
     "AwsWafWebAclRuleTypeDef",
     "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
-    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     "AwsWafv2CustomResponseDetailsTypeDef",
-    "AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef",
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     "CreateActionTargetResponseTypeDef",
     "CreateAutomationRuleResponseTypeDef",
     "CreateFindingAggregatorResponseTypeDef",
     "CreateInsightResponseTypeDef",
     "DeleteActionTargetResponseTypeDef",
     "DeleteInsightResponseTypeDef",
@@ -1054,26 +701,27 @@
     "ListTagsForResourceResponseTypeDef",
     "UpdateFindingAggregatorResponseTypeDef",
     "BatchDeleteAutomationRulesResponseTypeDef",
     "BatchUpdateAutomationRulesResponseTypeDef",
     "BatchEnableStandardsRequestRequestTypeDef",
     "BatchGetSecurityControlsResponseTypeDef",
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
+    "UnprocessedStandardsControlAssociationTypeDef",
     "BatchImportFindingsResponseTypeDef",
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
+    "UnprocessedStandardsControlAssociationUpdateTypeDef",
     "ComplianceOutputTypeDef",
     "ComplianceTypeDef",
     "ContainerDetailsOutputTypeDef",
     "ContainerDetailsTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
-    "DateFilterOutputTypeDef",
     "DateFilterTypeDef",
     "DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef",
     "DescribeProductsRequestDescribeProductsPaginateTypeDef",
     "DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef",
     "DescribeStandardsRequestDescribeStandardsPaginateTypeDef",
     "GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef",
     "GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef",
@@ -1097,51 +745,43 @@
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetMembersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "InsightResultsTypeDef",
     "ListSecurityControlDefinitionsResponseTypeDef",
     "ListStandardsControlAssociationsResponseTypeDef",
-    "NetworkOutputTypeDef",
     "NetworkPathComponentDetailsOutputTypeDef",
     "NetworkPathComponentDetailsTypeDef",
     "NetworkTypeDef",
-    "PageOutputTypeDef",
     "PageTypeDef",
-    "RemediationOutputTypeDef",
     "RemediationTypeDef",
     "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
     "RuleGroupVariablesOutputTypeDef",
     "RuleGroupVariablesTypeDef",
     "StandardTypeDef",
-    "UnprocessedStandardsControlAssociationTypeDef",
-    "UnprocessedStandardsControlAssociationUpdateTypeDef",
     "StandardsSubscriptionTypeDef",
     "StatelessCustomPublishMetricActionOutputTypeDef",
     "StatelessCustomPublishMetricActionTypeDef",
     "AwsApiCallActionOutputTypeDef",
-    "NetworkConnectionActionOutputTypeDef",
-    "PortProbeDetailOutputTypeDef",
     "AwsApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "VulnerabilityOutputTypeDef",
     "VulnerabilityTypeDef",
     "AwsEc2RouteTableDetailsOutputTypeDef",
     "AwsEc2RouteTableDetailsTypeDef",
     "AutomationRulesActionOutputTypeDef",
     "AutomationRulesActionTypeDef",
     "AwsAmazonMqBrokerDetailsOutputTypeDef",
     "AwsAmazonMqBrokerDetailsTypeDef",
     "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     "AwsAppSyncGraphQlApiDetailsTypeDef",
-    "AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef",
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     "AwsBackupBackupPlanRuleDetailsOutputTypeDef",
     "AwsBackupBackupPlanRuleDetailsTypeDef",
@@ -1161,15 +801,14 @@
     "AwsEc2NetworkAclDetailsTypeDef",
     "AwsEc2SecurityGroupDetailsOutputTypeDef",
     "AwsEc2SecurityGroupDetailsTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
     "AwsEc2VpnConnectionDetailsOutputTypeDef",
     "AwsEc2VpnConnectionDetailsTypeDef",
-    "AwsEcsClusterConfigurationDetailsOutputTypeDef",
     "AwsEcsClusterConfigurationDetailsTypeDef",
     "AwsEcsServiceDetailsOutputTypeDef",
     "AwsEcsServiceDetailsTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
@@ -1179,17 +818,15 @@
     "AwsEfsAccessPointDetailsTypeDef",
     "AwsEksClusterDetailsOutputTypeDef",
     "AwsEksClusterDetailsTypeDef",
     "AwsElasticsearchDomainDetailsOutputTypeDef",
     "AwsElasticsearchDomainDetailsTypeDef",
     "AwsElbLoadBalancerDetailsOutputTypeDef",
     "AwsElbLoadBalancerDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
-    "AwsIamAccessKeyDetailsOutputTypeDef",
     "AwsIamAccessKeyDetailsTypeDef",
     "AwsIamRoleDetailsOutputTypeDef",
     "AwsIamRoleDetailsTypeDef",
     "AwsLambdaFunctionDetailsOutputTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "AwsOpenSearchServiceDomainDetailsOutputTypeDef",
     "AwsOpenSearchServiceDomainDetailsTypeDef",
@@ -1197,64 +834,61 @@
     "AwsRdsDbSubnetGroupTypeDef",
     "AwsRedshiftClusterDetailsOutputTypeDef",
     "AwsRedshiftClusterDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationFilterOutputTypeDef",
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
-    "AwsS3BucketObjectLockConfigurationOutputTypeDef",
     "AwsS3BucketObjectLockConfigurationTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     "AwsS3BucketWebsiteConfigurationTypeDef",
     "BatchUpdateFindingsResponseTypeDef",
-    "AwsSsmPatchComplianceDetailsOutputTypeDef",
     "AwsSsmPatchComplianceDetailsTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef",
     "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     "AwsWafRegionalWebAclDetailsOutputTypeDef",
     "AwsWafRegionalWebAclDetailsTypeDef",
     "AwsWafRuleGroupDetailsOutputTypeDef",
     "AwsWafRuleGroupDetailsTypeDef",
     "AwsWafWebAclDetailsOutputTypeDef",
     "AwsWafWebAclDetailsTypeDef",
     "AwsWafv2ActionAllowDetailsOutputTypeDef",
     "AwsWafv2RulesActionCaptchaDetailsOutputTypeDef",
     "AwsWafv2RulesActionCountDetailsOutputTypeDef",
-    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     "AwsWafv2ActionAllowDetailsTypeDef",
     "AwsWafv2RulesActionCaptchaDetailsTypeDef",
     "AwsWafv2RulesActionCountDetailsTypeDef",
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
     "AwsWafv2ActionBlockDetailsTypeDef",
+    "BatchGetStandardsControlAssociationsResponseTypeDef",
+    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     "AutomationRulesFindingFiltersOutputTypeDef",
-    "AwsSecurityFindingFiltersOutputTypeDef",
     "AutomationRulesFindingFiltersTypeDef",
+    "AwsSecurityFindingFiltersOutputTypeDef",
     "AwsSecurityFindingFiltersTypeDef",
     "GetFindingHistoryResponseTypeDef",
     "GetInsightResultsResponseTypeDef",
     "NetworkHeaderOutputTypeDef",
     "NetworkHeaderTypeDef",
     "OccurrencesOutputTypeDef",
     "OccurrencesTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionOutputTypeDef",
     "RuleGroupSourceStatelessRuleDefinitionTypeDef",
     "DescribeStandardsResponseTypeDef",
-    "BatchGetStandardsControlAssociationsResponseTypeDef",
-    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     "BatchDisableStandardsResponseTypeDef",
     "BatchEnableStandardsResponseTypeDef",
     "GetEnabledStandardsResponseTypeDef",
     "StatelessCustomActionDefinitionOutputTypeDef",
     "StatelessCustomActionDefinitionTypeDef",
     "PortProbeActionOutputTypeDef",
     "PortProbeActionTypeDef",
-    "AwsAthenaWorkGroupDetailsOutputTypeDef",
     "AwsAthenaWorkGroupDetailsTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef",
     "AwsAutoScalingAutoScalingGroupDetailsTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef",
     "AwsBackupBackupPlanBackupPlanDetailsTypeDef",
     "AwsCertificateManagerCertificateDetailsOutputTypeDef",
     "AwsCertificateManagerCertificateDetailsTypeDef",
@@ -1266,32 +900,31 @@
     "AwsDynamoDbTableDetailsTypeDef",
     "AwsEc2LaunchTemplateDetailsOutputTypeDef",
     "AwsEc2LaunchTemplateDetailsTypeDef",
     "AwsEcsClusterDetailsOutputTypeDef",
     "AwsEcsClusterDetailsTypeDef",
     "AwsEcsTaskDefinitionDetailsOutputTypeDef",
     "AwsEcsTaskDefinitionDetailsTypeDef",
-    "AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef",
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
     "AwsRdsDbInstanceDetailsOutputTypeDef",
     "AwsRdsDbInstanceDetailsTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationDetailOutputTypeDef",
     "AwsS3BucketNotificationConfigurationDetailTypeDef",
     "AwsStepFunctionStateMachineDetailsOutputTypeDef",
     "AwsStepFunctionStateMachineDetailsTypeDef",
     "AwsWafv2RulesActionDetailsOutputTypeDef",
     "AwsWafv2WebAclActionDetailsOutputTypeDef",
     "AwsWafv2RulesActionDetailsTypeDef",
     "AwsWafv2WebAclActionDetailsTypeDef",
     "AutomationRulesConfigTypeDef",
-    "InsightTypeDef",
     "CreateAutomationRuleRequestRequestTypeDef",
     "UpdateAutomationRulesRequestItemTypeDef",
+    "InsightTypeDef",
     "CreateInsightRequestRequestTypeDef",
     "GetFindingsRequestGetFindingsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "UpdateFindingsRequestRequestTypeDef",
     "UpdateInsightRequestRequestTypeDef",
     "NetworkPathComponentOutputTypeDef",
     "NetworkPathComponentTypeDef",
@@ -1316,16 +949,16 @@
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     "AwsS3BucketNotificationConfigurationOutputTypeDef",
     "AwsS3BucketNotificationConfigurationTypeDef",
     "AwsWafv2RulesDetailsOutputTypeDef",
     "AwsWafv2RulesDetailsTypeDef",
     "BatchGetAutomationRulesResponseTypeDef",
-    "GetInsightsResponseTypeDef",
     "BatchUpdateAutomationRulesRequestRequestTypeDef",
+    "GetInsightsResponseTypeDef",
     "CustomDataIdentifiersResultOutputTypeDef",
     "SensitiveDataResultOutputTypeDef",
     "CustomDataIdentifiersResultTypeDef",
     "SensitiveDataResultTypeDef",
     "FirewallPolicyDetailsOutputTypeDef",
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
     "FirewallPolicyDetailsTypeDef",
@@ -1389,95 +1022,41 @@
     },
     total=False,
 )
 
 class AccountDetailsTypeDef(_RequiredAccountDetailsTypeDef, _OptionalAccountDetailsTypeDef):
     pass
 
-ActionLocalIpDetailsOutputTypeDef = TypedDict(
-    "ActionLocalIpDetailsOutputTypeDef",
-    {
-        "IpAddressV4": str,
-    },
-    total=False,
-)
-
 ActionLocalIpDetailsTypeDef = TypedDict(
     "ActionLocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
 
-ActionLocalPortDetailsOutputTypeDef = TypedDict(
-    "ActionLocalPortDetailsOutputTypeDef",
-    {
-        "Port": int,
-        "PortName": str,
-    },
-    total=False,
-)
-
 ActionLocalPortDetailsTypeDef = TypedDict(
     "ActionLocalPortDetailsTypeDef",
     {
         "Port": int,
         "PortName": str,
     },
     total=False,
 )
 
-DnsRequestActionOutputTypeDef = TypedDict(
-    "DnsRequestActionOutputTypeDef",
+DnsRequestActionTypeDef = TypedDict(
+    "DnsRequestActionTypeDef",
     {
         "Domain": str,
         "Protocol": str,
         "Blocked": bool,
     },
     total=False,
 )
 
-CityOutputTypeDef = TypedDict(
-    "CityOutputTypeDef",
-    {
-        "CityName": str,
-    },
-    total=False,
-)
-
-CountryOutputTypeDef = TypedDict(
-    "CountryOutputTypeDef",
-    {
-        "CountryCode": str,
-        "CountryName": str,
-    },
-    total=False,
-)
-
-GeoLocationOutputTypeDef = TypedDict(
-    "GeoLocationOutputTypeDef",
-    {
-        "Lon": float,
-        "Lat": float,
-    },
-    total=False,
-)
-
-IpOrganizationDetailsOutputTypeDef = TypedDict(
-    "IpOrganizationDetailsOutputTypeDef",
-    {
-        "Asn": int,
-        "AsnOrg": str,
-        "Isp": str,
-        "Org": str,
-    },
-    total=False,
-)
-
 CityTypeDef = TypedDict(
     "CityTypeDef",
     {
         "CityName": str,
     },
     total=False,
 )
@@ -1507,23 +1086,14 @@
         "AsnOrg": str,
         "Isp": str,
         "Org": str,
     },
     total=False,
 )
 
-ActionRemotePortDetailsOutputTypeDef = TypedDict(
-    "ActionRemotePortDetailsOutputTypeDef",
-    {
-        "Port": int,
-        "PortName": str,
-    },
-    total=False,
-)
-
 ActionRemotePortDetailsTypeDef = TypedDict(
     "ActionRemotePortDetailsTypeDef",
     {
         "Port": int,
         "PortName": str,
     },
     total=False,
@@ -1534,33 +1104,14 @@
     {
         "ActionTargetArn": str,
         "Name": str,
         "Description": str,
     },
 )
 
-DnsRequestActionTypeDef = TypedDict(
-    "DnsRequestActionTypeDef",
-    {
-        "Domain": str,
-        "Protocol": str,
-        "Blocked": bool,
-    },
-    total=False,
-)
-
-AdjustmentOutputTypeDef = TypedDict(
-    "AdjustmentOutputTypeDef",
-    {
-        "Metric": str,
-        "Reason": str,
-    },
-    total=False,
-)
-
 AdjustmentTypeDef = TypedDict(
     "AdjustmentTypeDef",
     {
         "Metric": str,
         "Reason": str,
     },
     total=False,
@@ -1571,82 +1122,31 @@
     {
         "AccountId": str,
         "Status": AdminStatusType,
     },
     total=False,
 )
 
-AssociatedStandardOutputTypeDef = TypedDict(
-    "AssociatedStandardOutputTypeDef",
-    {
-        "StandardsId": str,
-    },
-    total=False,
-)
-
 AssociatedStandardTypeDef = TypedDict(
     "AssociatedStandardTypeDef",
     {
         "StandardsId": str,
     },
     total=False,
 )
 
-AssociationStateDetailsOutputTypeDef = TypedDict(
-    "AssociationStateDetailsOutputTypeDef",
-    {
-        "State": str,
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
 AssociationStateDetailsTypeDef = TypedDict(
     "AssociationStateDetailsTypeDef",
     {
         "State": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-NoteUpdateOutputTypeDef = TypedDict(
-    "NoteUpdateOutputTypeDef",
-    {
-        "Text": str,
-        "UpdatedBy": str,
-    },
-)
-
-RelatedFindingOutputTypeDef = TypedDict(
-    "RelatedFindingOutputTypeDef",
-    {
-        "ProductArn": str,
-        "Id": str,
-    },
-)
-
-SeverityUpdateOutputTypeDef = TypedDict(
-    "SeverityUpdateOutputTypeDef",
-    {
-        "Normalized": int,
-        "Product": float,
-        "Label": SeverityLabelType,
-    },
-    total=False,
-)
-
-WorkflowUpdateOutputTypeDef = TypedDict(
-    "WorkflowUpdateOutputTypeDef",
-    {
-        "Status": WorkflowStatusType,
-    },
-    total=False,
-)
-
 NoteUpdateTypeDef = TypedDict(
     "NoteUpdateTypeDef",
     {
         "Text": str,
         "UpdatedBy": str,
     },
 )
@@ -1673,43 +1173,14 @@
     "WorkflowUpdateTypeDef",
     {
         "Status": WorkflowStatusType,
     },
     total=False,
 )
 
-MapFilterOutputTypeDef = TypedDict(
-    "MapFilterOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-        "Comparison": MapFilterComparisonType,
-    },
-    total=False,
-)
-
-NumberFilterOutputTypeDef = TypedDict(
-    "NumberFilterOutputTypeDef",
-    {
-        "Gte": float,
-        "Lte": float,
-        "Eq": float,
-    },
-    total=False,
-)
-
-StringFilterOutputTypeDef = TypedDict(
-    "StringFilterOutputTypeDef",
-    {
-        "Value": str,
-        "Comparison": StringFilterComparisonType,
-    },
-    total=False,
-)
-
 MapFilterTypeDef = TypedDict(
     "MapFilterTypeDef",
     {
         "Key": str,
         "Value": str,
         "Comparison": MapFilterComparisonType,
     },
@@ -1747,34 +1218,25 @@
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
-AvailabilityZoneOutputTypeDef = TypedDict(
-    "AvailabilityZoneOutputTypeDef",
-    {
-        "ZoneName": str,
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AvailabilityZoneTypeDef = TypedDict(
     "AvailabilityZoneTypeDef",
     {
         "ZoneName": str,
         "SubnetId": str,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef",
+AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
     {
         "KmsKeyId": str,
         "UseAwsOwnedKey": bool,
     },
     total=False,
 )
 
@@ -1791,42 +1253,33 @@
         "UserRoleName": str,
         "UserSearchMatching": str,
         "UserSearchSubtree": bool,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef",
+AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
     {
         "DayOfWeek": str,
         "TimeOfDay": str,
         "TimeZone": str,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerUsersDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerUsersDetailsOutputTypeDef",
+AwsAmazonMqBrokerUsersDetailsTypeDef = TypedDict(
+    "AwsAmazonMqBrokerUsersDetailsTypeDef",
     {
         "PendingChange": str,
         "Username": str,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef = TypedDict(
-    "AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef",
-    {
-        "KmsKeyId": str,
-        "UseAwsOwnedKey": bool,
-    },
-    total=False,
-)
-
 AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef",
     {
         "Hosts": Sequence[str],
         "RoleBase": str,
         "RoleName": str,
         "RoleSearchMatching": str,
@@ -1836,76 +1289,31 @@
         "UserRoleName": str,
         "UserSearchMatching": str,
         "UserSearchSubtree": bool,
     },
     total=False,
 )
 
-AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef = TypedDict(
-    "AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef",
-    {
-        "DayOfWeek": str,
-        "TimeOfDay": str,
-        "TimeZone": str,
-    },
-    total=False,
-)
-
-AwsAmazonMqBrokerUsersDetailsTypeDef = TypedDict(
-    "AwsAmazonMqBrokerUsersDetailsTypeDef",
-    {
-        "PendingChange": str,
-        "Username": str,
-    },
-    total=False,
-)
-
-AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef",
-    {
-        "Audit": bool,
-        "General": bool,
-    },
-    total=False,
-)
-
 AwsAmazonMqBrokerLogsPendingDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsPendingDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
     },
     total=False,
 )
 
-AwsApiCallActionDomainDetailsOutputTypeDef = TypedDict(
-    "AwsApiCallActionDomainDetailsOutputTypeDef",
-    {
-        "Domain": str,
-    },
-    total=False,
-)
-
 AwsApiCallActionDomainDetailsTypeDef = TypedDict(
     "AwsApiCallActionDomainDetailsTypeDef",
     {
         "Domain": str,
     },
     total=False,
 )
 
-AwsApiGatewayAccessLogSettingsOutputTypeDef = TypedDict(
-    "AwsApiGatewayAccessLogSettingsOutputTypeDef",
-    {
-        "Format": str,
-        "DestinationArn": str,
-    },
-    total=False,
-)
-
 AwsApiGatewayAccessLogSettingsTypeDef = TypedDict(
     "AwsApiGatewayAccessLogSettingsTypeDef",
     {
         "Format": str,
         "DestinationArn": str,
     },
     total=False,
@@ -1945,33 +1353,14 @@
     "AwsApiGatewayEndpointConfigurationTypeDef",
     {
         "Types": Sequence[str],
     },
     total=False,
 )
 
-AwsApiGatewayMethodSettingsOutputTypeDef = TypedDict(
-    "AwsApiGatewayMethodSettingsOutputTypeDef",
-    {
-        "MetricsEnabled": bool,
-        "LoggingLevel": str,
-        "DataTraceEnabled": bool,
-        "ThrottlingBurstLimit": int,
-        "ThrottlingRateLimit": float,
-        "CachingEnabled": bool,
-        "CacheTtlInSeconds": int,
-        "CacheDataEncrypted": bool,
-        "RequireAuthorizationForCacheControl": bool,
-        "UnauthorizedCacheControlHeaderStrategy": str,
-        "HttpMethod": str,
-        "ResourcePath": str,
-    },
-    total=False,
-)
-
 AwsApiGatewayMethodSettingsTypeDef = TypedDict(
     "AwsApiGatewayMethodSettingsTypeDef",
     {
         "MetricsEnabled": bool,
         "LoggingLevel": str,
         "DataTraceEnabled": bool,
         "ThrottlingBurstLimit": int,
@@ -2009,70 +1398,26 @@
         "MaxAge": int,
         "AllowMethods": Sequence[str],
         "AllowHeaders": Sequence[str],
     },
     total=False,
 )
 
-AwsApiGatewayV2RouteSettingsOutputTypeDef = TypedDict(
-    "AwsApiGatewayV2RouteSettingsOutputTypeDef",
-    {
-        "DetailedMetricsEnabled": bool,
-        "LoggingLevel": str,
-        "DataTraceEnabled": bool,
-        "ThrottlingBurstLimit": int,
-        "ThrottlingRateLimit": float,
-    },
-    total=False,
-)
-
 AwsApiGatewayV2RouteSettingsTypeDef = TypedDict(
     "AwsApiGatewayV2RouteSettingsTypeDef",
     {
         "DetailedMetricsEnabled": bool,
         "LoggingLevel": str,
         "DataTraceEnabled": bool,
         "ThrottlingBurstLimit": int,
         "ThrottlingRateLimit": float,
     },
     total=False,
 )
 
-AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef",
-    {
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerUri": str,
-        "IdentityValidationExpression": str,
-    },
-    total=False,
-)
-
-AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef",
-    {
-        "AuthTtL": int,
-        "ClientId": str,
-        "IatTtL": int,
-        "Issuer": str,
-    },
-    total=False,
-)
-
-AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef",
-    {
-        "AppIdClientRegex": str,
-        "AwsRegion": str,
-        "DefaultAction": str,
-        "UserPoolId": str,
-    },
-    total=False,
-)
-
 AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef",
     {
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerUri": str,
         "IdentityValidationExpression": str,
     },
@@ -2097,133 +1442,64 @@
         "AwsRegion": str,
         "DefaultAction": str,
         "UserPoolId": str,
     },
     total=False,
 )
 
-AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef",
-    {
-        "CloudWatchLogsRoleArn": str,
-        "ExcludeVerboseContent": bool,
-        "FieldLogLevel": str,
-    },
-    total=False,
-)
-
 AwsAppSyncGraphQlApiLogConfigDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiLogConfigDetailsTypeDef",
     {
         "CloudWatchLogsRoleArn": str,
         "ExcludeVerboseContent": bool,
         "FieldLogLevel": str,
     },
     total=False,
 )
 
-AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef",
-    {
-        "EncryptionOption": str,
-        "KmsKey": str,
-    },
-    total=False,
-)
-
 AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef",
     {
         "EncryptionOption": str,
         "KmsKey": str,
     },
     total=False,
 )
 
-AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
-    {
-        "LaunchTemplateId": str,
-        "LaunchTemplateName": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
     total=False,
 )
 
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef",
-    {
-        "OnDemandAllocationStrategy": str,
-        "OnDemandBaseCapacity": int,
-        "OnDemandPercentageAboveBaseCapacity": int,
-        "SpotAllocationStrategy": str,
-        "SpotInstancePools": int,
-        "SpotMaxPrice": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef",
     {
         "OnDemandAllocationStrategy": str,
         "OnDemandBaseCapacity": int,
         "OnDemandPercentageAboveBaseCapacity": int,
         "SpotAllocationStrategy": str,
         "SpotInstancePools": int,
         "SpotMaxPrice": str,
     },
     total=False,
 )
 
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef",
-    {
-        "LaunchTemplateId": str,
-        "LaunchTemplateName": str,
-        "Version": str,
-    },
-    total=False,
-)
-
-AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef",
-    {
-        "InstanceType": str,
-        "WeightedCapacity": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef",
     {
         "LaunchTemplateId": str,
         "LaunchTemplateName": str,
         "Version": str,
     },
@@ -2235,58 +1511,27 @@
     {
         "InstanceType": str,
         "WeightedCapacity": str,
     },
     total=False,
 )
 
-AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef",
-    {
-        "DeleteOnTermination": bool,
-        "Encrypted": bool,
-        "Iops": int,
-        "SnapshotId": str,
-        "VolumeSize": int,
-        "VolumeType": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
         "Iops": int,
         "SnapshotId": str,
         "VolumeSize": int,
         "VolumeType": str,
     },
     total=False,
 )
 
-AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef",
-    {
-        "HttpEndpoint": str,
-        "HttpPutResponseHopLimit": int,
-        "HttpTokens": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -2315,23 +1560,14 @@
     {
         "BackupOptions": Mapping[str, str],
         "ResourceType": str,
     },
     total=False,
 )
 
-AwsBackupBackupPlanLifecycleDetailsOutputTypeDef = TypedDict(
-    "AwsBackupBackupPlanLifecycleDetailsOutputTypeDef",
-    {
-        "DeleteAfterDays": int,
-        "MoveToColdStorageAfterDays": int,
-    },
-    total=False,
-)
-
 AwsBackupBackupPlanLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
     total=False,
@@ -2351,97 +1587,43 @@
     {
         "BackupVaultEvents": Sequence[str],
         "SnsTopicArn": str,
     },
     total=False,
 )
 
-AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef = TypedDict(
-    "AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef",
-    {
-        "DeleteAt": str,
-        "MoveToColdStorageAt": str,
-    },
-    total=False,
-)
-
 AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef",
     {
         "DeleteAt": str,
         "MoveToColdStorageAt": str,
     },
     total=False,
 )
 
-AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef = TypedDict(
-    "AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef",
-    {
-        "BackupPlanArn": str,
-        "BackupPlanId": str,
-        "BackupPlanVersion": str,
-        "BackupRuleId": str,
-    },
-    total=False,
-)
-
 AwsBackupRecoveryPointCreatedByDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointCreatedByDetailsTypeDef",
     {
         "BackupPlanArn": str,
         "BackupPlanId": str,
         "BackupPlanVersion": str,
         "BackupRuleId": str,
     },
     total=False,
 )
 
-AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef = TypedDict(
-    "AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef",
-    {
-        "DeleteAfterDays": int,
-        "MoveToColdStorageAfterDays": int,
-    },
-    total=False,
-)
-
 AwsBackupRecoveryPointLifecycleDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointLifecycleDetailsTypeDef",
     {
         "DeleteAfterDays": int,
         "MoveToColdStorageAfterDays": int,
     },
     total=False,
 )
 
-AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef",
-    {
-        "Name": str,
-        "OId": str,
-    },
-    total=False,
-)
-
-AwsCertificateManagerCertificateKeyUsageOutputTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateKeyUsageOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-AwsCertificateManagerCertificateOptionsOutputTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateOptionsOutputTypeDef",
-    {
-        "CertificateTransparencyLoggingPreference": str,
-    },
-    total=False,
-)
-
 AwsCertificateManagerCertificateExtendedKeyUsageTypeDef = TypedDict(
     "AwsCertificateManagerCertificateExtendedKeyUsageTypeDef",
     {
         "Name": str,
         "OId": str,
     },
     total=False,
@@ -2459,52 +1641,24 @@
     "AwsCertificateManagerCertificateOptionsTypeDef",
     {
         "CertificateTransparencyLoggingPreference": str,
     },
     total=False,
 )
 
-AwsCertificateManagerCertificateResourceRecordOutputTypeDef = TypedDict(
-    "AwsCertificateManagerCertificateResourceRecordOutputTypeDef",
-    {
-        "Name": str,
-        "Type": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsCertificateManagerCertificateResourceRecordTypeDef = TypedDict(
     "AwsCertificateManagerCertificateResourceRecordTypeDef",
     {
         "Name": str,
         "Type": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsCloudFormationStackDriftInformationDetailsOutputTypeDef = TypedDict(
-    "AwsCloudFormationStackDriftInformationDetailsOutputTypeDef",
-    {
-        "StackDriftStatus": str,
-    },
-    total=False,
-)
-
-AwsCloudFormationStackOutputsDetailsOutputTypeDef = TypedDict(
-    "AwsCloudFormationStackOutputsDetailsOutputTypeDef",
-    {
-        "Description": str,
-        "OutputKey": str,
-        "OutputValue": str,
-    },
-    total=False,
-)
-
 AwsCloudFormationStackDriftInformationDetailsTypeDef = TypedDict(
     "AwsCloudFormationStackDriftInformationDetailsTypeDef",
     {
         "StackDriftStatus": str,
     },
     total=False,
 )
@@ -2515,71 +1669,30 @@
         "Description": str,
         "OutputKey": str,
         "OutputValue": str,
     },
     total=False,
 )
 
-AwsCloudFrontDistributionCacheBehaviorOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionCacheBehaviorOutputTypeDef",
-    {
-        "ViewerProtocolPolicy": str,
-    },
-    total=False,
-)
-
 AwsCloudFrontDistributionCacheBehaviorTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
     total=False,
 )
 
-AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef",
-    {
-        "ViewerProtocolPolicy": str,
-    },
-    total=False,
-)
-
 AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef = TypedDict(
     "AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef",
     {
         "ViewerProtocolPolicy": str,
     },
     total=False,
 )
 
-AwsCloudFrontDistributionLoggingOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionLoggingOutputTypeDef",
-    {
-        "Bucket": str,
-        "Enabled": bool,
-        "IncludeCookies": bool,
-        "Prefix": str,
-    },
-    total=False,
-)
-
-AwsCloudFrontDistributionViewerCertificateOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionViewerCertificateOutputTypeDef",
-    {
-        "AcmCertificateArn": str,
-        "Certificate": str,
-        "CertificateSource": str,
-        "CloudFrontDefaultCertificate": bool,
-        "IamCertificateId": str,
-        "MinimumProtocolVersion": str,
-        "SslSupportMethod": str,
-    },
-    total=False,
-)
-
 AwsCloudFrontDistributionLoggingTypeDef = TypedDict(
     "AwsCloudFrontDistributionLoggingTypeDef",
     {
         "Bucket": str,
         "Enabled": bool,
         "IncludeCookies": bool,
         "Prefix": str,
@@ -2633,52 +1746,22 @@
     {
         "Items": Sequence[int],
         "Quantity": int,
     },
     total=False,
 )
 
-AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef = TypedDict(
-    "AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef",
-    {
-        "OriginAccessIdentity": str,
-    },
-    total=False,
-)
-
 AwsCloudFrontDistributionOriginS3OriginConfigTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginS3OriginConfigTypeDef",
     {
         "OriginAccessIdentity": str,
     },
     total=False,
 )
 
-AwsCloudTrailTrailDetailsOutputTypeDef = TypedDict(
-    "AwsCloudTrailTrailDetailsOutputTypeDef",
-    {
-        "CloudWatchLogsLogGroupArn": str,
-        "CloudWatchLogsRoleArn": str,
-        "HasCustomEventSelectors": bool,
-        "HomeRegion": str,
-        "IncludeGlobalServiceEvents": bool,
-        "IsMultiRegionTrail": bool,
-        "IsOrganizationTrail": bool,
-        "KmsKeyId": str,
-        "LogFileValidationEnabled": bool,
-        "Name": str,
-        "S3BucketName": str,
-        "S3KeyPrefix": str,
-        "SnsTopicArn": str,
-        "SnsTopicName": str,
-        "TrailArn": str,
-    },
-    total=False,
-)
-
 AwsCloudTrailTrailDetailsTypeDef = TypedDict(
     "AwsCloudTrailTrailDetailsTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "CloudWatchLogsRoleArn": str,
         "HasCustomEventSelectors": bool,
         "HomeRegion": str,
@@ -2693,48 +1776,23 @@
         "SnsTopicArn": str,
         "SnsTopicName": str,
         "TrailArn": str,
     },
     total=False,
 )
 
-AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef = TypedDict(
-    "AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsCloudWatchAlarmDimensionsDetailsTypeDef = TypedDict(
     "AwsCloudWatchAlarmDimensionsDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectArtifactsDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectArtifactsDetailsOutputTypeDef",
-    {
-        "ArtifactIdentifier": str,
-        "EncryptionDisabled": bool,
-        "Location": str,
-        "Name": str,
-        "NamespaceType": str,
-        "OverrideArtifactName": bool,
-        "Packaging": str,
-        "Path": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectArtifactsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectArtifactsDetailsTypeDef",
     {
         "ArtifactIdentifier": str,
         "EncryptionDisabled": bool,
         "Location": str,
         "Name": str,
@@ -2743,16 +1801,16 @@
         "Packaging": str,
         "Path": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectSourceOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectSourceOutputTypeDef",
+AwsCodeBuildProjectSourceTypeDef = TypedDict(
+    "AwsCodeBuildProjectSourceTypeDef",
     {
         "Type": str,
         "Location": str,
         "GitCloneDepth": int,
         "InsecureSsl": bool,
     },
     total=False,
@@ -2764,201 +1822,81 @@
         "VpcId": str,
         "Subnets": List[str],
         "SecurityGroupIds": List[str],
     },
     total=False,
 )
 
-AwsCodeBuildProjectSourceTypeDef = TypedDict(
-    "AwsCodeBuildProjectSourceTypeDef",
-    {
-        "Type": str,
-        "Location": str,
-        "GitCloneDepth": int,
-        "InsecureSsl": bool,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectVpcConfigTypeDef = TypedDict(
     "AwsCodeBuildProjectVpcConfigTypeDef",
     {
         "VpcId": str,
         "Subnets": Sequence[str],
         "SecurityGroupIds": Sequence[str],
     },
     total=False,
 )
 
-AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Type": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef",
     {
         "Name": str,
         "Type": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef",
-    {
-        "Credential": str,
-        "CredentialProvider": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef",
     {
         "Credential": str,
         "CredentialProvider": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef",
-    {
-        "GroupName": str,
-        "Status": str,
-        "StreamName": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef",
     {
         "GroupName": str,
         "Status": str,
         "StreamName": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef",
-    {
-        "EncryptionDisabled": bool,
-        "Location": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef",
     {
         "EncryptionDisabled": bool,
         "Location": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsDynamoDbTableAttributeDefinitionOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableAttributeDefinitionOutputTypeDef",
-    {
-        "AttributeName": str,
-        "AttributeType": str,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableAttributeDefinitionTypeDef = TypedDict(
     "AwsDynamoDbTableAttributeDefinitionTypeDef",
     {
         "AttributeName": str,
         "AttributeType": str,
     },
     total=False,
 )
 
-AwsDynamoDbTableBillingModeSummaryOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableBillingModeSummaryOutputTypeDef",
-    {
-        "BillingMode": str,
-        "LastUpdateToPayPerRequestDateTime": str,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableBillingModeSummaryTypeDef = TypedDict(
     "AwsDynamoDbTableBillingModeSummaryTypeDef",
     {
         "BillingMode": str,
         "LastUpdateToPayPerRequestDateTime": str,
     },
     total=False,
 )
 
-AwsDynamoDbTableKeySchemaOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableKeySchemaOutputTypeDef",
-    {
-        "AttributeName": str,
-        "KeyType": str,
-    },
-    total=False,
-)
-
-AwsDynamoDbTableProvisionedThroughputOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableProvisionedThroughputOutputTypeDef",
-    {
-        "LastDecreaseDateTime": str,
-        "LastIncreaseDateTime": str,
-        "NumberOfDecreasesToday": int,
-        "ReadCapacityUnits": int,
-        "WriteCapacityUnits": int,
-    },
-    total=False,
-)
-
-AwsDynamoDbTableRestoreSummaryOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableRestoreSummaryOutputTypeDef",
-    {
-        "SourceBackupArn": str,
-        "SourceTableArn": str,
-        "RestoreDateTime": str,
-        "RestoreInProgress": bool,
-    },
-    total=False,
-)
-
-AwsDynamoDbTableSseDescriptionOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableSseDescriptionOutputTypeDef",
-    {
-        "InaccessibleEncryptionDateTime": str,
-        "Status": str,
-        "SseType": str,
-        "KmsMasterKeyArn": str,
-    },
-    total=False,
-)
-
-AwsDynamoDbTableStreamSpecificationOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableStreamSpecificationOutputTypeDef",
-    {
-        "StreamEnabled": bool,
-        "StreamViewType": str,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableKeySchemaTypeDef = TypedDict(
     "AwsDynamoDbTableKeySchemaTypeDef",
     {
         "AttributeName": str,
         "KeyType": str,
     },
     total=False,
@@ -3021,47 +1959,22 @@
     {
         "NonKeyAttributes": Sequence[str],
         "ProjectionType": str,
     },
     total=False,
 )
 
-AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef",
-    {
-        "ReadCapacityUnits": int,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableProvisionedThroughputOverrideTypeDef = TypedDict(
     "AwsDynamoDbTableProvisionedThroughputOverrideTypeDef",
     {
         "ReadCapacityUnits": int,
     },
     total=False,
 )
 
-AwsEc2EipDetailsOutputTypeDef = TypedDict(
-    "AwsEc2EipDetailsOutputTypeDef",
-    {
-        "InstanceId": str,
-        "PublicIp": str,
-        "AllocationId": str,
-        "AssociationId": str,
-        "Domain": str,
-        "PublicIpv4Pool": str,
-        "NetworkBorderGroup": str,
-        "NetworkInterfaceId": str,
-        "NetworkInterfaceOwnerId": str,
-        "PrivateIpAddress": str,
-    },
-    total=False,
-)
-
 AwsEc2EipDetailsTypeDef = TypedDict(
     "AwsEc2EipDetailsTypeDef",
     {
         "InstanceId": str,
         "PublicIp": str,
         "AllocationId": str,
         "AssociationId": str,
@@ -3071,42 +1984,14 @@
         "NetworkInterfaceId": str,
         "NetworkInterfaceOwnerId": str,
         "PrivateIpAddress": str,
     },
     total=False,
 )
 
-AwsEc2InstanceMetadataOptionsOutputTypeDef = TypedDict(
-    "AwsEc2InstanceMetadataOptionsOutputTypeDef",
-    {
-        "HttpEndpoint": str,
-        "HttpProtocolIpv6": str,
-        "HttpPutResponseHopLimit": int,
-        "HttpTokens": str,
-        "InstanceMetadataTags": str,
-    },
-    total=False,
-)
-
-AwsEc2InstanceMonitoringDetailsOutputTypeDef = TypedDict(
-    "AwsEc2InstanceMonitoringDetailsOutputTypeDef",
-    {
-        "State": str,
-    },
-    total=False,
-)
-
-AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef",
-    {
-        "NetworkInterfaceId": str,
-    },
-    total=False,
-)
-
 AwsEc2InstanceMetadataOptionsTypeDef = TypedDict(
     "AwsEc2InstanceMetadataOptionsTypeDef",
     {
         "HttpEndpoint": str,
         "HttpProtocolIpv6": str,
         "HttpPutResponseHopLimit": int,
         "HttpTokens": str,
@@ -3127,29 +2012,14 @@
     "AwsEc2InstanceNetworkInterfacesDetailsTypeDef",
     {
         "NetworkInterfaceId": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef",
-    {
-        "DeleteOnTermination": bool,
-        "Encrypted": bool,
-        "Iops": int,
-        "KmsKeyId": str,
-        "SnapshotId": str,
-        "Throughput": int,
-        "VolumeSize": int,
-        "VolumeType": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef",
     {
         "DeleteOnTermination": bool,
         "Encrypted": bool,
         "Iops": int,
         "KmsKeyId": str,
@@ -3157,169 +2027,40 @@
         "Throughput": int,
         "VolumeSize": int,
         "VolumeType": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef",
-    {
-        "CapacityReservationId": str,
-        "CapacityReservationResourceGroupArn": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef",
     {
         "CapacityReservationId": str,
         "CapacityReservationResourceGroupArn": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef",
-    {
-        "CoreCount": int,
-        "ThreadsPerCore": int,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef",
     {
         "CoreCount": int,
         "ThreadsPerCore": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef",
-    {
-        "CpuCredits": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef",
     {
         "CpuCredits": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef",
-    {
-        "Count": int,
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef",
-    {
-        "Configured": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef",
-    {
-        "Arn": str,
-        "Name": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef",
-    {
-        "AutoRecovery": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef",
-    {
-        "HttpEndpoint": str,
-        "HttpProtocolIpv6": str,
-        "HttpTokens": str,
-        "HttpPutResponseHopLimit": int,
-        "InstanceMetadataTags": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef",
-    {
-        "Affinity": str,
-        "AvailabilityZone": str,
-        "GroupName": str,
-        "HostId": str,
-        "HostResourceGroupArn": str,
-        "PartitionNumber": int,
-        "SpreadDomain": str,
-        "Tenancy": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef",
-    {
-        "EnableResourceNameDnsAAAARecord": bool,
-        "EnableResourceNameDnsARecord": bool,
-        "HostnameType": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
@@ -3415,141 +2156,53 @@
         "EnableResourceNameDnsAAAARecord": bool,
         "EnableResourceNameDnsARecord": bool,
         "HostnameType": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef",
-    {
-        "BlockDurationMinutes": int,
-        "InstanceInterruptionBehavior": str,
-        "MaxPrice": str,
-        "SpotInstanceType": str,
-        "ValidUntil": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef",
     {
         "BlockDurationMinutes": int,
         "InstanceInterruptionBehavior": str,
         "MaxPrice": str,
         "SpotInstanceType": str,
         "ValidUntil": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef",
     {
         "Max": int,
         "Min": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef",
-        {
-            "Max": int,
-            "Min": int,
-        },
-        total=False,
-    )
-)
-
 AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef",
     {
         "Max": int,
         "Min": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef",
-        {
-            "Max": int,
-            "Min": int,
-        },
-        total=False,
-    )
-)
-
 AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef",
     {
         "Max": int,
         "Min": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef",
-    {
-        "Max": float,
-        "Min": float,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef",
-    {
-        "Max": float,
-        "Min": float,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef",
-    {
-        "Max": int,
-        "Min": int,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef",
     {
         "Max": float,
         "Min": float,
     },
     total=False,
@@ -3587,47 +2240,14 @@
     {
         "Max": int,
         "Min": int,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef",
-    {
-        "Ipv4Prefix": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef",
-    {
-        "Ipv6Address": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef",
-    {
-        "Ipv6Prefix": str,
-    },
-    total=False,
-)
-
-AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef",
-    {
-        "Primary": bool,
-        "PrivateIpAddress": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef",
     {
         "Ipv4Prefix": str,
     },
     total=False,
 )
@@ -3653,52 +2273,24 @@
     {
         "Primary": bool,
         "PrivateIpAddress": str,
     },
     total=False,
 )
 
-AwsEc2NetworkAclAssociationOutputTypeDef = TypedDict(
-    "AwsEc2NetworkAclAssociationOutputTypeDef",
-    {
-        "NetworkAclAssociationId": str,
-        "NetworkAclId": str,
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclAssociationTypeDef = TypedDict(
     "AwsEc2NetworkAclAssociationTypeDef",
     {
         "NetworkAclAssociationId": str,
         "NetworkAclId": str,
         "SubnetId": str,
     },
     total=False,
 )
 
-IcmpTypeCodeOutputTypeDef = TypedDict(
-    "IcmpTypeCodeOutputTypeDef",
-    {
-        "Code": int,
-        "Type": int,
-    },
-    total=False,
-)
-
-PortRangeFromToOutputTypeDef = TypedDict(
-    "PortRangeFromToOutputTypeDef",
-    {
-        "From": int,
-        "To": int,
-    },
-    total=False,
-)
-
 IcmpTypeCodeTypeDef = TypedDict(
     "IcmpTypeCodeTypeDef",
     {
         "Code": int,
         "Type": int,
     },
     total=False,
@@ -3709,68 +2301,28 @@
     {
         "From": int,
         "To": int,
     },
     total=False,
 )
 
-AwsEc2NetworkInterfaceAttachmentOutputTypeDef = TypedDict(
-    "AwsEc2NetworkInterfaceAttachmentOutputTypeDef",
-    {
-        "AttachTime": str,
-        "AttachmentId": str,
-        "DeleteOnTermination": bool,
-        "DeviceIndex": int,
-        "InstanceId": str,
-        "InstanceOwnerId": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkInterfaceAttachmentTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceAttachmentTypeDef",
     {
         "AttachTime": str,
         "AttachmentId": str,
         "DeleteOnTermination": bool,
         "DeviceIndex": int,
         "InstanceId": str,
         "InstanceOwnerId": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef = TypedDict(
-    "AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef",
-    {
-        "IpV6Address": str,
-    },
-    total=False,
-)
-
-AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef = TypedDict(
-    "AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef",
-    {
-        "PrivateIpAddress": str,
-        "PrivateDnsName": str,
-    },
-    total=False,
-)
-
-AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef = TypedDict(
-    "AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef",
-    {
-        "GroupName": str,
-        "GroupId": str,
-    },
-    total=False,
-)
-
 AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef",
     {
         "IpV6Address": str,
     },
     total=False,
 )
@@ -3789,45 +2341,14 @@
     {
         "GroupName": str,
         "GroupId": str,
     },
     total=False,
 )
 
-PropagatingVgwSetDetailsOutputTypeDef = TypedDict(
-    "PropagatingVgwSetDetailsOutputTypeDef",
-    {
-        "GatewayId": str,
-    },
-    total=False,
-)
-
-RouteSetDetailsOutputTypeDef = TypedDict(
-    "RouteSetDetailsOutputTypeDef",
-    {
-        "CarrierGatewayId": str,
-        "CoreNetworkArn": str,
-        "DestinationCidrBlock": str,
-        "DestinationIpv6CidrBlock": str,
-        "DestinationPrefixListId": str,
-        "EgressOnlyInternetGatewayId": str,
-        "GatewayId": str,
-        "InstanceId": str,
-        "InstanceOwnerId": str,
-        "LocalGatewayId": str,
-        "NatGatewayId": str,
-        "NetworkInterfaceId": str,
-        "Origin": str,
-        "State": str,
-        "TransitGatewayId": str,
-        "VpcPeeringConnectionId": str,
-    },
-    total=False,
-)
-
 PropagatingVgwSetDetailsTypeDef = TypedDict(
     "PropagatingVgwSetDetailsTypeDef",
     {
         "GatewayId": str,
     },
     total=False,
 )
@@ -3851,51 +2372,14 @@
         "State": str,
         "TransitGatewayId": str,
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
-AwsEc2SecurityGroupIpRangeOutputTypeDef = TypedDict(
-    "AwsEc2SecurityGroupIpRangeOutputTypeDef",
-    {
-        "CidrIp": str,
-    },
-    total=False,
-)
-
-AwsEc2SecurityGroupIpv6RangeOutputTypeDef = TypedDict(
-    "AwsEc2SecurityGroupIpv6RangeOutputTypeDef",
-    {
-        "CidrIpv6": str,
-    },
-    total=False,
-)
-
-AwsEc2SecurityGroupPrefixListIdOutputTypeDef = TypedDict(
-    "AwsEc2SecurityGroupPrefixListIdOutputTypeDef",
-    {
-        "PrefixListId": str,
-    },
-    total=False,
-)
-
-AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef = TypedDict(
-    "AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef",
-    {
-        "GroupId": str,
-        "GroupName": str,
-        "PeeringStatus": str,
-        "UserId": str,
-        "VpcId": str,
-        "VpcPeeringConnectionId": str,
-    },
-    total=False,
-)
-
 AwsEc2SecurityGroupIpRangeTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpRangeTypeDef",
     {
         "CidrIp": str,
     },
     total=False,
 )
@@ -3925,24 +2409,14 @@
         "UserId": str,
         "VpcId": str,
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
-Ipv6CidrBlockAssociationOutputTypeDef = TypedDict(
-    "Ipv6CidrBlockAssociationOutputTypeDef",
-    {
-        "AssociationId": str,
-        "Ipv6CidrBlock": str,
-        "CidrBlockState": str,
-    },
-    total=False,
-)
-
 Ipv6CidrBlockAssociationTypeDef = TypedDict(
     "Ipv6CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "Ipv6CidrBlock": str,
         "CidrBlockState": str,
     },
@@ -3983,116 +2457,52 @@
         "DnsSupport": str,
         "MulticastSupport": str,
         "AmazonSideAsn": int,
     },
     total=False,
 )
 
-AwsEc2VolumeAttachmentOutputTypeDef = TypedDict(
-    "AwsEc2VolumeAttachmentOutputTypeDef",
-    {
-        "AttachTime": str,
-        "DeleteOnTermination": bool,
-        "InstanceId": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsEc2VolumeAttachmentTypeDef = TypedDict(
     "AwsEc2VolumeAttachmentTypeDef",
     {
         "AttachTime": str,
         "DeleteOnTermination": bool,
         "InstanceId": str,
         "Status": str,
     },
     total=False,
 )
 
-CidrBlockAssociationOutputTypeDef = TypedDict(
-    "CidrBlockAssociationOutputTypeDef",
-    {
-        "AssociationId": str,
-        "CidrBlock": str,
-        "CidrBlockState": str,
-    },
-    total=False,
-)
-
 CidrBlockAssociationTypeDef = TypedDict(
     "CidrBlockAssociationTypeDef",
     {
         "AssociationId": str,
         "CidrBlock": str,
         "CidrBlockState": str,
     },
     total=False,
 )
 
-AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef = TypedDict(
-    "AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef",
-    {
-        "ServiceType": str,
-    },
-    total=False,
-)
-
 AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef",
     {
         "ServiceType": str,
     },
     total=False,
 )
 
-AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef = TypedDict(
-    "AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef",
-    {
-        "Code": str,
-        "Message": str,
-    },
-    total=False,
-)
-
 AwsEc2VpcPeeringConnectionStatusDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionStatusDetailsTypeDef",
     {
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-VpcInfoCidrBlockSetDetailsOutputTypeDef = TypedDict(
-    "VpcInfoCidrBlockSetDetailsOutputTypeDef",
-    {
-        "CidrBlock": str,
-    },
-    total=False,
-)
-
-VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef = TypedDict(
-    "VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef",
-    {
-        "Ipv6CidrBlock": str,
-    },
-    total=False,
-)
-
-VpcInfoPeeringOptionsDetailsOutputTypeDef = TypedDict(
-    "VpcInfoPeeringOptionsDetailsOutputTypeDef",
-    {
-        "AllowDnsResolutionFromRemoteVpc": bool,
-        "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
-        "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
-    },
-    total=False,
-)
-
 VpcInfoCidrBlockSetDetailsTypeDef = TypedDict(
     "VpcInfoCidrBlockSetDetailsTypeDef",
     {
         "CidrBlock": str,
     },
     total=False,
 )
@@ -4111,36 +2521,14 @@
         "AllowDnsResolutionFromRemoteVpc": bool,
         "AllowEgressFromLocalClassicLinkToRemoteVpc": bool,
         "AllowEgressFromLocalVpcToRemoteClassicLink": bool,
     },
     total=False,
 )
 
-AwsEc2VpnConnectionRoutesDetailsOutputTypeDef = TypedDict(
-    "AwsEc2VpnConnectionRoutesDetailsOutputTypeDef",
-    {
-        "DestinationCidrBlock": str,
-        "State": str,
-    },
-    total=False,
-)
-
-AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef = TypedDict(
-    "AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef",
-    {
-        "AcceptedRouteCount": int,
-        "CertificateArn": str,
-        "LastStatusChange": str,
-        "OutsideIpAddress": str,
-        "Status": str,
-        "StatusMessage": str,
-    },
-    total=False,
-)
-
 AwsEc2VpnConnectionRoutesDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionRoutesDetailsTypeDef",
     {
         "DestinationCidrBlock": str,
         "State": str,
     },
     total=False,
@@ -4227,31 +2615,14 @@
         "ImageDigest": str,
         "ImageTags": Sequence[str],
         "ImagePublishedAt": str,
     },
     total=False,
 )
 
-AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef",
-    {
-        "ScanOnPush": bool,
-    },
-    total=False,
-)
-
-AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef = TypedDict(
-    "AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef",
-    {
-        "LifecyclePolicyText": str,
-        "RegistryId": str,
-    },
-    total=False,
-)
-
 AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef = TypedDict(
     "AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef",
     {
         "ScanOnPush": bool,
     },
     total=False,
 )
@@ -4261,190 +2632,81 @@
     {
         "LifecyclePolicyText": str,
         "RegistryId": str,
     },
     total=False,
 )
 
-AwsEcsClusterClusterSettingsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsClusterClusterSettingsDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsEcsClusterClusterSettingsDetailsTypeDef = TypedDict(
     "AwsEcsClusterClusterSettingsDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef",
-        {
-            "CloudWatchEncryptionEnabled": bool,
-            "CloudWatchLogGroupName": str,
-            "S3BucketName": str,
-            "S3EncryptionEnabled": bool,
-            "S3KeyPrefix": str,
-        },
-        total=False,
-    )
-)
-
 AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef",
     {
         "CloudWatchEncryptionEnabled": bool,
         "CloudWatchLogGroupName": str,
         "S3BucketName": str,
         "S3EncryptionEnabled": bool,
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef = TypedDict(
-    "AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef",
-    {
-        "Base": int,
-        "CapacityProvider": str,
-        "Weight": int,
-    },
-    total=False,
-)
-
 AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef = TypedDict(
     "AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
         "Weight": int,
     },
     total=False,
 )
 
-AwsMountPointOutputTypeDef = TypedDict(
-    "AwsMountPointOutputTypeDef",
-    {
-        "SourceVolume": str,
-        "ContainerPath": str,
-    },
-    total=False,
-)
-
 AwsMountPointTypeDef = TypedDict(
     "AwsMountPointTypeDef",
     {
         "SourceVolume": str,
         "ContainerPath": str,
     },
     total=False,
 )
 
-AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef",
-    {
-        "Base": int,
-        "CapacityProvider": str,
-        "Weight": int,
-    },
-    total=False,
-)
-
 AwsEcsServiceCapacityProviderStrategyDetailsTypeDef = TypedDict(
     "AwsEcsServiceCapacityProviderStrategyDetailsTypeDef",
     {
         "Base": int,
         "CapacityProvider": str,
         "Weight": int,
     },
     total=False,
 )
 
-AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef",
-    {
-        "Enable": bool,
-        "Rollback": bool,
-    },
-    total=False,
-)
-
 AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef",
     {
         "Enable": bool,
         "Rollback": bool,
     },
     total=False,
 )
 
-AwsEcsServiceDeploymentControllerDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceDeploymentControllerDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsEcsServiceDeploymentControllerDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentControllerDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsEcsServiceLoadBalancersDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceLoadBalancersDetailsOutputTypeDef",
-    {
-        "ContainerName": str,
-        "ContainerPort": int,
-        "LoadBalancerName": str,
-        "TargetGroupArn": str,
-    },
-    total=False,
-)
-
-AwsEcsServicePlacementConstraintsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServicePlacementConstraintsDetailsOutputTypeDef",
-    {
-        "Expression": str,
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEcsServicePlacementStrategiesDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServicePlacementStrategiesDetailsOutputTypeDef",
-    {
-        "Field": str,
-        "Type": str,
-    },
-    total=False,
-)
-
-AwsEcsServiceServiceRegistriesDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceServiceRegistriesDetailsOutputTypeDef",
-    {
-        "ContainerName": str,
-        "ContainerPort": int,
-        "Port": int,
-        "RegistryArn": str,
-    },
-    total=False,
-)
-
 AwsEcsServiceLoadBalancersDetailsTypeDef = TypedDict(
     "AwsEcsServiceLoadBalancersDetailsTypeDef",
     {
         "ContainerName": str,
         "ContainerPort": int,
         "LoadBalancerName": str,
         "TargetGroupArn": str,
@@ -4497,52 +2759,43 @@
         "AssignPublicIp": str,
         "SecurityGroups": Sequence[str],
         "Subnets": Sequence[str],
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef",
-    {
-        "Condition": str,
-        "ContainerName": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef",
     {
         "Condition": str,
         "ContainerName": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
     {
         "Type": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
     {
         "Hostname": str,
         "IpAddress": str,
     },
     total=False,
 )
 
@@ -4563,115 +2816,88 @@
         "Retries": int,
         "StartPeriod": int,
         "Timeout": int,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
     {
         "ContainerPath": str,
         "ReadOnly": bool,
         "SourceVolume": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
     {
         "ContainerPort": int,
         "HostPort": int,
         "Protocol": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
     {
         "CredentialsParameter": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
     {
         "Type": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
     {
         "Name": str,
         "ValueFrom": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
     {
         "Namespace": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
     {
         "HardLimit": int,
         "Name": str,
         "SoftLimit": int,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef",
+AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
     {
         "ReadOnly": bool,
         "SourceContainer": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef",
-    {
-        "Type": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef",
-    {
-        "Hostname": str,
-        "IpAddress": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef",
     {
         "Options": Mapping[str, str],
         "Type": str,
     },
     total=False,
@@ -4685,88 +2911,14 @@
         "Retries": int,
         "StartPeriod": int,
         "Timeout": int,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef",
-    {
-        "ContainerPath": str,
-        "ReadOnly": bool,
-        "SourceVolume": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef",
-    {
-        "ContainerPort": int,
-        "HostPort": int,
-        "Protocol": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef",
-    {
-        "CredentialsParameter": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef",
-    {
-        "Type": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef",
-    {
-        "Name": str,
-        "ValueFrom": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef",
-    {
-        "Namespace": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef",
-    {
-        "HardLimit": int,
-        "Name": str,
-        "SoftLimit": int,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef",
-    {
-        "ReadOnly": bool,
-        "SourceContainer": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef",
     {
         "Add": List[str],
         "Drop": List[str],
     },
     total=False,
@@ -4817,52 +2969,23 @@
         "ContainerPath": str,
         "MountOptions": Sequence[str],
         "Size": int,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef",
-        {
-            "Name": str,
-            "ValueFrom": str,
-        },
-        total=False,
-    )
-)
-
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef",
     {
         "Name": str,
         "ValueFrom": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef",
-    {
-        "DeviceName": str,
-        "DeviceType": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef",
-    {
-        "Expression": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef",
     {
         "DeviceName": str,
         "DeviceType": str,
     },
     total=False,
@@ -4873,23 +2996,14 @@
     {
         "Expression": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -4903,16 +3017,16 @@
         "DriverOpts": Dict[str, str],
         "Labels": Dict[str, str],
         "Scope": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef",
+AwsEcsTaskDefinitionVolumesHostDetailsTypeDef = TypedDict(
+    "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef = TypedDict(
@@ -4923,50 +3037,23 @@
         "DriverOpts": Mapping[str, str],
         "Labels": Mapping[str, str],
         "Scope": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionVolumesHostDetailsTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesHostDetailsTypeDef",
-    {
-        "SourcePath": str,
-    },
-    total=False,
-)
-
-AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef = (
-    TypedDict(
-        "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef",
-        {
-            "AccessPointId": str,
-            "Iam": str,
-        },
-        total=False,
-    )
-)
-
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef",
     {
         "AccessPointId": str,
         "Iam": str,
     },
     total=False,
 )
 
-AwsEcsTaskVolumeHostDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskVolumeHostDetailsOutputTypeDef",
-    {
-        "SourcePath": str,
-    },
-    total=False,
-)
-
 AwsEcsTaskVolumeHostDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeHostDetailsTypeDef",
     {
         "SourcePath": str,
     },
     total=False,
 )
@@ -4987,24 +3074,14 @@
         "Gid": str,
         "SecondaryGids": Sequence[str],
         "Uid": str,
     },
     total=False,
 )
 
-AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef = TypedDict(
-    "AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef",
-    {
-        "OwnerGid": str,
-        "OwnerUid": str,
-        "Permissions": str,
-    },
-    total=False,
-)
-
 AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef",
     {
         "OwnerGid": str,
         "OwnerUid": str,
         "Permissions": str,
     },
@@ -5045,44 +3122,14 @@
     {
         "Enabled": bool,
         "Types": Sequence[str],
     },
     total=False,
 )
 
-AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef = TypedDict(
-    "AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef",
-    {
-        "EnvironmentName": str,
-        "LinkName": str,
-    },
-    total=False,
-)
-
-AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef = TypedDict(
-    "AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef",
-    {
-        "Namespace": str,
-        "OptionName": str,
-        "ResourceName": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsElasticBeanstalkEnvironmentTierOutputTypeDef = TypedDict(
-    "AwsElasticBeanstalkEnvironmentTierOutputTypeDef",
-    {
-        "Name": str,
-        "Type": str,
-        "Version": str,
-    },
-    total=False,
-)
-
 AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef",
     {
         "EnvironmentName": str,
         "LinkName": str,
     },
     total=False,
@@ -5105,42 +3152,42 @@
         "Name": str,
         "Type": str,
         "Version": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef",
+AwsElasticsearchDomainDomainEndpointOptionsTypeDef = TypedDict(
+    "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
     {
         "EnforceHTTPS": bool,
         "TLSSecurityPolicy": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef",
+AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef = TypedDict(
+    "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
     {
         "Enabled": bool,
         "KmsKeyId": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef",
+AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef = TypedDict(
+    "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef",
+AwsElasticsearchDomainServiceSoftwareOptionsTypeDef = TypedDict(
+    "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
     {
         "AutomatedUpdateDate": str,
         "Cancellable": bool,
         "CurrentVersion": str,
         "Description": str,
         "NewVersion": str,
         "UpdateAvailable": bool,
@@ -5156,200 +3203,80 @@
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "VPCId": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainDomainEndpointOptionsTypeDef = TypedDict(
-    "AwsElasticsearchDomainDomainEndpointOptionsTypeDef",
-    {
-        "EnforceHTTPS": bool,
-        "TLSSecurityPolicy": str,
-    },
-    total=False,
-)
-
-AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef = TypedDict(
-    "AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef",
-    {
-        "Enabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef = TypedDict(
-    "AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsElasticsearchDomainServiceSoftwareOptionsTypeDef = TypedDict(
-    "AwsElasticsearchDomainServiceSoftwareOptionsTypeDef",
-    {
-        "AutomatedUpdateDate": str,
-        "Cancellable": bool,
-        "CurrentVersion": str,
-        "Description": str,
-        "NewVersion": str,
-        "UpdateAvailable": bool,
-        "UpdateStatus": str,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainVPCOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainVPCOptionsTypeDef",
     {
         "AvailabilityZones": Sequence[str],
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VPCId": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
-    {
-        "AvailabilityZoneCount": int,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
     total=False,
 )
 
-AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef",
-    {
-        "CloudWatchLogsLogGroupArn": str,
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
     },
     total=False,
 )
 
-AwsElbAppCookieStickinessPolicyOutputTypeDef = TypedDict(
-    "AwsElbAppCookieStickinessPolicyOutputTypeDef",
-    {
-        "CookieName": str,
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsElbAppCookieStickinessPolicyTypeDef = TypedDict(
     "AwsElbAppCookieStickinessPolicyTypeDef",
     {
         "CookieName": str,
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsElbLbCookieStickinessPolicyOutputTypeDef = TypedDict(
-    "AwsElbLbCookieStickinessPolicyOutputTypeDef",
-    {
-        "CookieExpirationPeriod": int,
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsElbLbCookieStickinessPolicyTypeDef = TypedDict(
     "AwsElbLbCookieStickinessPolicyTypeDef",
     {
         "CookieExpirationPeriod": int,
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsElbLoadBalancerAccessLogOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerAccessLogOutputTypeDef",
-    {
-        "EmitInterval": int,
-        "Enabled": bool,
-        "S3BucketName": str,
-        "S3BucketPrefix": str,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerAccessLogTypeDef = TypedDict(
     "AwsElbLoadBalancerAccessLogTypeDef",
     {
         "EmitInterval": int,
         "Enabled": bool,
         "S3BucketName": str,
         "S3BucketPrefix": str,
     },
     total=False,
 )
 
-AwsElbLoadBalancerAdditionalAttributeOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerAdditionalAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerAdditionalAttributeTypeDef = TypedDict(
     "AwsElbLoadBalancerAdditionalAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsElbLoadBalancerConnectionDrainingOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerConnectionDrainingOutputTypeDef",
-    {
-        "Enabled": bool,
-        "Timeout": int,
-    },
-    total=False,
-)
-
-AwsElbLoadBalancerConnectionSettingsOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerConnectionSettingsOutputTypeDef",
-    {
-        "IdleTimeout": int,
-    },
-    total=False,
-)
-
-AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerConnectionDrainingTypeDef = TypedDict(
     "AwsElbLoadBalancerConnectionDrainingTypeDef",
     {
         "Enabled": bool,
         "Timeout": int,
     },
     total=False,
@@ -5385,43 +3312,14 @@
     {
         "InstancePort": int,
         "PolicyNames": Sequence[str],
     },
     total=False,
 )
 
-AwsElbLoadBalancerHealthCheckOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerHealthCheckOutputTypeDef",
-    {
-        "HealthyThreshold": int,
-        "Interval": int,
-        "Target": str,
-        "Timeout": int,
-        "UnhealthyThreshold": int,
-    },
-    total=False,
-)
-
-AwsElbLoadBalancerInstanceOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerInstanceOutputTypeDef",
-    {
-        "InstanceId": str,
-    },
-    total=False,
-)
-
-AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef",
-    {
-        "GroupName": str,
-        "OwnerAlias": str,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerHealthCheckTypeDef = TypedDict(
     "AwsElbLoadBalancerHealthCheckTypeDef",
     {
         "HealthyThreshold": int,
         "Interval": int,
         "Target": str,
         "Timeout": int,
@@ -5443,134 +3341,62 @@
     {
         "GroupName": str,
         "OwnerAlias": str,
     },
     total=False,
 )
 
-AwsElbLoadBalancerListenerOutputTypeDef = TypedDict(
-    "AwsElbLoadBalancerListenerOutputTypeDef",
-    {
-        "InstancePort": int,
-        "InstanceProtocol": str,
-        "LoadBalancerPort": int,
-        "Protocol": str,
-        "SslCertificateId": str,
-    },
-    total=False,
-)
-
 AwsElbLoadBalancerListenerTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerTypeDef",
     {
         "InstancePort": int,
         "InstanceProtocol": str,
         "LoadBalancerPort": int,
         "Protocol": str,
         "SslCertificateId": str,
     },
     total=False,
 )
 
-AwsElbv2LoadBalancerAttributeOutputTypeDef = TypedDict(
-    "AwsElbv2LoadBalancerAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsElbv2LoadBalancerAttributeTypeDef = TypedDict(
     "AwsElbv2LoadBalancerAttributeTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-LoadBalancerStateOutputTypeDef = TypedDict(
-    "LoadBalancerStateOutputTypeDef",
-    {
-        "Code": str,
-        "Reason": str,
-    },
-    total=False,
-)
-
 LoadBalancerStateTypeDef = TypedDict(
     "LoadBalancerStateTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
     total=False,
 )
 
-AwsEventSchemasRegistryDetailsOutputTypeDef = TypedDict(
-    "AwsEventSchemasRegistryDetailsOutputTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-    },
-    total=False,
-)
-
 AwsEventSchemasRegistryDetailsTypeDef = TypedDict(
     "AwsEventSchemasRegistryDetailsTypeDef",
     {
         "Description": str,
         "RegistryArn": str,
         "RegistryName": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
@@ -5587,271 +3413,135 @@
     "AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef",
-    {
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef",
     {
         "Status": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef",
-    {
-        "Reason": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef",
     {
         "Reason": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorFeaturesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorFeaturesDetailsTypeDef",
     {
         "Name": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsIamAccessKeySessionContextAttributesOutputTypeDef = TypedDict(
-    "AwsIamAccessKeySessionContextAttributesOutputTypeDef",
-    {
-        "MfaAuthenticated": bool,
-        "CreationDate": str,
-    },
-    total=False,
-)
-
 AwsIamAccessKeySessionContextAttributesTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextAttributesTypeDef",
     {
         "MfaAuthenticated": bool,
         "CreationDate": str,
     },
     total=False,
 )
 
-AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef = TypedDict(
-    "AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef",
-    {
-        "Type": str,
-        "PrincipalId": str,
-        "Arn": str,
-        "AccountId": str,
-        "UserName": str,
-    },
-    total=False,
-)
-
 AwsIamAccessKeySessionContextSessionIssuerTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextSessionIssuerTypeDef",
     {
         "Type": str,
         "PrincipalId": str,
         "Arn": str,
         "AccountId": str,
         "UserName": str,
     },
     total=False,
 )
 
-AwsIamAttachedManagedPolicyOutputTypeDef = TypedDict(
-    "AwsIamAttachedManagedPolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-        "PolicyArn": str,
-    },
-    total=False,
-)
-
 AwsIamAttachedManagedPolicyTypeDef = TypedDict(
     "AwsIamAttachedManagedPolicyTypeDef",
     {
         "PolicyName": str,
         "PolicyArn": str,
     },
     total=False,
 )
 
-AwsIamGroupPolicyOutputTypeDef = TypedDict(
-    "AwsIamGroupPolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsIamGroupPolicyTypeDef = TypedDict(
     "AwsIamGroupPolicyTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsIamInstanceProfileRoleOutputTypeDef = TypedDict(
-    "AwsIamInstanceProfileRoleOutputTypeDef",
-    {
-        "Arn": str,
-        "AssumeRolePolicyDocument": str,
-        "CreateDate": str,
-        "Path": str,
-        "RoleId": str,
-        "RoleName": str,
-    },
-    total=False,
-)
-
 AwsIamInstanceProfileRoleTypeDef = TypedDict(
     "AwsIamInstanceProfileRoleTypeDef",
     {
         "Arn": str,
         "AssumeRolePolicyDocument": str,
         "CreateDate": str,
         "Path": str,
         "RoleId": str,
         "RoleName": str,
     },
     total=False,
 )
 
-AwsIamPermissionsBoundaryOutputTypeDef = TypedDict(
-    "AwsIamPermissionsBoundaryOutputTypeDef",
-    {
-        "PermissionsBoundaryArn": str,
-        "PermissionsBoundaryType": str,
-    },
-    total=False,
-)
-
 AwsIamPermissionsBoundaryTypeDef = TypedDict(
     "AwsIamPermissionsBoundaryTypeDef",
     {
         "PermissionsBoundaryArn": str,
         "PermissionsBoundaryType": str,
     },
     total=False,
 )
 
-AwsIamPolicyVersionOutputTypeDef = TypedDict(
-    "AwsIamPolicyVersionOutputTypeDef",
-    {
-        "VersionId": str,
-        "IsDefaultVersion": bool,
-        "CreateDate": str,
-    },
-    total=False,
-)
-
 AwsIamPolicyVersionTypeDef = TypedDict(
     "AwsIamPolicyVersionTypeDef",
     {
         "VersionId": str,
         "IsDefaultVersion": bool,
         "CreateDate": str,
     },
     total=False,
 )
 
-AwsIamRolePolicyOutputTypeDef = TypedDict(
-    "AwsIamRolePolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsIamRolePolicyTypeDef = TypedDict(
     "AwsIamRolePolicyTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsIamUserPolicyOutputTypeDef = TypedDict(
-    "AwsIamUserPolicyOutputTypeDef",
-    {
-        "PolicyName": str,
-    },
-    total=False,
-)
-
 AwsIamUserPolicyTypeDef = TypedDict(
     "AwsIamUserPolicyTypeDef",
     {
         "PolicyName": str,
     },
     total=False,
 )
 
-AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef = TypedDict(
-    "AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef",
-    {
-        "EncryptionType": str,
-        "KeyId": str,
-    },
-    total=False,
-)
-
 AwsKinesisStreamStreamEncryptionDetailsTypeDef = TypedDict(
     "AwsKinesisStreamStreamEncryptionDetailsTypeDef",
     {
         "EncryptionType": str,
         "KeyId": str,
     },
     total=False,
 )
 
-AwsKmsKeyDetailsOutputTypeDef = TypedDict(
-    "AwsKmsKeyDetailsOutputTypeDef",
-    {
-        "AWSAccountId": str,
-        "CreationDate": float,
-        "KeyId": str,
-        "KeyManager": str,
-        "KeyState": str,
-        "Origin": str,
-        "Description": str,
-        "KeyRotationStatus": bool,
-    },
-    total=False,
-)
-
 AwsKmsKeyDetailsTypeDef = TypedDict(
     "AwsKmsKeyDetailsTypeDef",
     {
         "AWSAccountId": str,
         "CreationDate": float,
         "KeyId": str,
         "KeyManager": str,
@@ -5859,63 +3549,44 @@
         "Origin": str,
         "Description": str,
         "KeyRotationStatus": bool,
     },
     total=False,
 )
 
-AwsLambdaFunctionCodeOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionCodeOutputTypeDef",
-    {
-        "S3Bucket": str,
-        "S3Key": str,
-        "S3ObjectVersion": str,
-        "ZipFile": str,
-    },
-    total=False,
-)
-
 AwsLambdaFunctionCodeTypeDef = TypedDict(
     "AwsLambdaFunctionCodeTypeDef",
     {
         "S3Bucket": str,
         "S3Key": str,
         "S3ObjectVersion": str,
         "ZipFile": str,
     },
     total=False,
 )
 
-AwsLambdaFunctionDeadLetterConfigOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionDeadLetterConfigOutputTypeDef",
-    {
-        "TargetArn": str,
-    },
-    total=False,
-)
-
 AwsLambdaFunctionDeadLetterConfigTypeDef = TypedDict(
     "AwsLambdaFunctionDeadLetterConfigTypeDef",
     {
         "TargetArn": str,
     },
     total=False,
 )
 
-AwsLambdaFunctionLayerOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionLayerOutputTypeDef",
+AwsLambdaFunctionLayerTypeDef = TypedDict(
+    "AwsLambdaFunctionLayerTypeDef",
     {
         "Arn": str,
         "CodeSize": int,
     },
     total=False,
 )
 
-AwsLambdaFunctionTracingConfigOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionTracingConfigOutputTypeDef",
+AwsLambdaFunctionTracingConfigTypeDef = TypedDict(
+    "AwsLambdaFunctionTracingConfigTypeDef",
     {
         "Mode": str,
     },
     total=False,
 )
 
 AwsLambdaFunctionVpcConfigOutputTypeDef = TypedDict(
@@ -5924,50 +3595,24 @@
         "SecurityGroupIds": List[str],
         "SubnetIds": List[str],
         "VpcId": str,
     },
     total=False,
 )
 
-AwsLambdaFunctionLayerTypeDef = TypedDict(
-    "AwsLambdaFunctionLayerTypeDef",
-    {
-        "Arn": str,
-        "CodeSize": int,
-    },
-    total=False,
-)
-
-AwsLambdaFunctionTracingConfigTypeDef = TypedDict(
-    "AwsLambdaFunctionTracingConfigTypeDef",
-    {
-        "Mode": str,
-    },
-    total=False,
-)
-
 AwsLambdaFunctionVpcConfigTypeDef = TypedDict(
     "AwsLambdaFunctionVpcConfigTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VpcId": str,
     },
     total=False,
 )
 
-AwsLambdaFunctionEnvironmentErrorOutputTypeDef = TypedDict(
-    "AwsLambdaFunctionEnvironmentErrorOutputTypeDef",
-    {
-        "ErrorCode": str,
-        "Message": str,
-    },
-    total=False,
-)
-
 AwsLambdaFunctionEnvironmentErrorTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentErrorTypeDef",
     {
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
@@ -5989,119 +3634,40 @@
         "Version": int,
         "CompatibleRuntimes": Sequence[str],
         "CreatedDate": str,
     },
     total=False,
 )
 
-AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef = TypedDict(
-    "AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef",
-    {
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef",
     {
         "SubnetId": str,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef",
-    {
-        "MasterUserArn": str,
-        "MasterUserName": str,
-        "MasterUserPassword": str,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef",
     {
         "MasterUserArn": str,
         "MasterUserName": str,
         "MasterUserPassword": str,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef",
-    {
-        "AvailabilityZoneCount": int,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef",
     {
         "AvailabilityZoneCount": int,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef",
-    {
-        "CustomEndpointCertificateArn": str,
-        "CustomEndpointEnabled": bool,
-        "EnforceHTTPS": bool,
-        "CustomEndpoint": str,
-        "TLSSecurityPolicy": str,
-    },
-    total=False,
-)
-
-AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
-AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef",
-    {
-        "AutomatedUpdateDate": str,
-        "Cancellable": bool,
-        "CurrentVersion": str,
-        "Description": str,
-        "NewVersion": str,
-        "UpdateAvailable": bool,
-        "UpdateStatus": str,
-        "OptionalDeployment": bool,
-    },
-    total=False,
-)
-
-AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef",
     {
         "CustomEndpointCertificateArn": str,
         "CustomEndpointEnabled": bool,
         "EnforceHTTPS": bool,
         "CustomEndpoint": str,
@@ -6138,99 +3704,50 @@
         "UpdateAvailable": bool,
         "UpdateStatus": str,
         "OptionalDeployment": bool,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
+AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef",
     {
-        "SecurityGroupIds": Sequence[str],
-        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef",
+AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef = TypedDict(
+    "AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef",
     {
-        "CloudWatchLogsLogGroupArn": str,
-        "Enabled": bool,
+        "SecurityGroupIds": Sequence[str],
+        "SubnetIds": Sequence[str],
     },
     total=False,
 )
 
 AwsOpenSearchServiceDomainLogPublishingOptionTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionTypeDef",
     {
         "CloudWatchLogsLogGroupArn": str,
         "Enabled": bool,
     },
     total=False,
 )
 
-AwsRdsDbClusterAssociatedRoleOutputTypeDef = TypedDict(
-    "AwsRdsDbClusterAssociatedRoleOutputTypeDef",
-    {
-        "RoleArn": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRdsDbClusterAssociatedRoleTypeDef = TypedDict(
     "AwsRdsDbClusterAssociatedRoleTypeDef",
     {
         "RoleArn": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsRdsDbClusterMemberOutputTypeDef = TypedDict(
-    "AwsRdsDbClusterMemberOutputTypeDef",
-    {
-        "IsClusterWriter": bool,
-        "PromotionTier": int,
-        "DbInstanceIdentifier": str,
-        "DbClusterParameterGroupStatus": str,
-    },
-    total=False,
-)
-
-AwsRdsDbClusterOptionGroupMembershipOutputTypeDef = TypedDict(
-    "AwsRdsDbClusterOptionGroupMembershipOutputTypeDef",
-    {
-        "DbClusterOptionGroupName": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRdsDbDomainMembershipOutputTypeDef = TypedDict(
-    "AwsRdsDbDomainMembershipOutputTypeDef",
-    {
-        "Domain": str,
-        "Status": str,
-        "Fqdn": str,
-        "IamRoleName": str,
-    },
-    total=False,
-)
-
-AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef = TypedDict(
-    "AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef",
-    {
-        "VpcSecurityGroupId": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRdsDbClusterMemberTypeDef = TypedDict(
     "AwsRdsDbClusterMemberTypeDef",
     {
         "IsClusterWriter": bool,
         "PromotionTier": int,
         "DbInstanceIdentifier": str,
         "DbClusterParameterGroupStatus": str,
@@ -6281,82 +3798,24 @@
     {
         "AttributeName": str,
         "AttributeValues": Sequence[str],
     },
     total=False,
 )
 
-AwsRdsDbInstanceAssociatedRoleOutputTypeDef = TypedDict(
-    "AwsRdsDbInstanceAssociatedRoleOutputTypeDef",
-    {
-        "RoleArn": str,
-        "FeatureName": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRdsDbInstanceAssociatedRoleTypeDef = TypedDict(
     "AwsRdsDbInstanceAssociatedRoleTypeDef",
     {
         "RoleArn": str,
         "FeatureName": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsRdsDbInstanceEndpointOutputTypeDef = TypedDict(
-    "AwsRdsDbInstanceEndpointOutputTypeDef",
-    {
-        "Address": str,
-        "Port": int,
-        "HostedZoneId": str,
-    },
-    total=False,
-)
-
-AwsRdsDbOptionGroupMembershipOutputTypeDef = TypedDict(
-    "AwsRdsDbOptionGroupMembershipOutputTypeDef",
-    {
-        "OptionGroupName": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRdsDbParameterGroupOutputTypeDef = TypedDict(
-    "AwsRdsDbParameterGroupOutputTypeDef",
-    {
-        "DbParameterGroupName": str,
-        "ParameterApplyStatus": str,
-    },
-    total=False,
-)
-
-AwsRdsDbProcessorFeatureOutputTypeDef = TypedDict(
-    "AwsRdsDbProcessorFeatureOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
-AwsRdsDbStatusInfoOutputTypeDef = TypedDict(
-    "AwsRdsDbStatusInfoOutputTypeDef",
-    {
-        "StatusType": str,
-        "Normal": bool,
-        "Status": str,
-        "Message": str,
-    },
-    total=False,
-)
-
 AwsRdsDbInstanceEndpointTypeDef = TypedDict(
     "AwsRdsDbInstanceEndpointTypeDef",
     {
         "Address": str,
         "Port": int,
         "HostedZoneId": str,
     },
@@ -6415,34 +3874,14 @@
     {
         "LogTypesToEnable": Sequence[str],
         "LogTypesToDisable": Sequence[str],
     },
     total=False,
 )
 
-AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef = TypedDict(
-    "AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef",
-    {
-        "Ec2SecurityGroupId": str,
-        "Ec2SecurityGroupName": str,
-        "Ec2SecurityGroupOwnerId": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRdsDbSecurityGroupIpRangeOutputTypeDef = TypedDict(
-    "AwsRdsDbSecurityGroupIpRangeOutputTypeDef",
-    {
-        "CidrIp": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef",
     {
         "Ec2SecurityGroupId": str,
         "Ec2SecurityGroupName": str,
         "Ec2SecurityGroupOwnerId": str,
         "Status": str,
@@ -6455,22 +3894,14 @@
     {
         "CidrIp": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef = TypedDict(
-    "AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
 AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
@@ -6505,213 +3936,64 @@
         "SourceType": str,
         "Status": str,
         "SubscriptionCreationTime": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterClusterNodeOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterNodeOutputTypeDef",
-    {
-        "NodeRole": str,
-        "PrivateIpAddress": str,
-        "PublicIpAddress": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterClusterNodeTypeDef = TypedDict(
     "AwsRedshiftClusterClusterNodeTypeDef",
     {
         "NodeRole": str,
         "PrivateIpAddress": str,
         "PublicIpAddress": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterClusterParameterStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterParameterStatusOutputTypeDef",
-    {
-        "ParameterName": str,
-        "ParameterApplyStatus": str,
-        "ParameterApplyErrorDescription": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterClusterParameterStatusTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterStatusTypeDef",
     {
         "ParameterName": str,
         "ParameterApplyStatus": str,
         "ParameterApplyErrorDescription": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterClusterSecurityGroupOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterSecurityGroupOutputTypeDef",
-    {
-        "ClusterSecurityGroupName": str,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterClusterSecurityGroupTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSecurityGroupTypeDef",
     {
         "ClusterSecurityGroupName": str,
         "Status": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef",
-    {
-        "DestinationRegion": str,
-        "ManualSnapshotRetentionPeriod": int,
-        "RetentionPeriod": int,
-        "SnapshotCopyGrantName": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef = TypedDict(
     "AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef",
     {
         "DestinationRegion": str,
         "ManualSnapshotRetentionPeriod": int,
         "RetentionPeriod": int,
         "SnapshotCopyGrantName": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef",
-    {
-        "DeferMaintenanceEndTime": str,
-        "DeferMaintenanceIdentifier": str,
-        "DeferMaintenanceStartTime": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterDeferredMaintenanceWindowTypeDef = TypedDict(
     "AwsRedshiftClusterDeferredMaintenanceWindowTypeDef",
     {
         "DeferMaintenanceEndTime": str,
         "DeferMaintenanceIdentifier": str,
         "DeferMaintenanceStartTime": str,
     },
     total=False,
 )
 
-AwsRedshiftClusterElasticIpStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterElasticIpStatusOutputTypeDef",
-    {
-        "ElasticIp": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterEndpointOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterEndpointOutputTypeDef",
-    {
-        "Address": str,
-        "Port": int,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterHsmStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterHsmStatusOutputTypeDef",
-    {
-        "HsmClientCertificateIdentifier": str,
-        "HsmConfigurationIdentifier": str,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterIamRoleOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterIamRoleOutputTypeDef",
-    {
-        "ApplyStatus": str,
-        "IamRoleArn": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterLoggingStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterLoggingStatusOutputTypeDef",
-    {
-        "BucketName": str,
-        "LastFailureMessage": str,
-        "LastFailureTime": str,
-        "LastSuccessfulDeliveryTime": str,
-        "LoggingEnabled": bool,
-        "S3KeyPrefix": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterPendingModifiedValuesOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterPendingModifiedValuesOutputTypeDef",
-    {
-        "AutomatedSnapshotRetentionPeriod": int,
-        "ClusterIdentifier": str,
-        "ClusterType": str,
-        "ClusterVersion": str,
-        "EncryptionType": str,
-        "EnhancedVpcRouting": bool,
-        "MaintenanceTrackName": str,
-        "MasterUserPassword": str,
-        "NodeType": str,
-        "NumberOfNodes": int,
-        "PubliclyAccessible": bool,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterResizeInfoOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterResizeInfoOutputTypeDef",
-    {
-        "AllowCancelResize": bool,
-        "ResizeType": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterRestoreStatusOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterRestoreStatusOutputTypeDef",
-    {
-        "CurrentRestoreRateInMegaBytesPerSecond": float,
-        "ElapsedTimeInSeconds": int,
-        "EstimatedTimeToCompletionInSeconds": int,
-        "ProgressInMegaBytes": int,
-        "SnapshotSizeInMegaBytes": int,
-        "Status": str,
-    },
-    total=False,
-)
-
-AwsRedshiftClusterVpcSecurityGroupOutputTypeDef = TypedDict(
-    "AwsRedshiftClusterVpcSecurityGroupOutputTypeDef",
-    {
-        "Status": str,
-        "VpcSecurityGroupId": str,
-    },
-    total=False,
-)
-
 AwsRedshiftClusterElasticIpStatusTypeDef = TypedDict(
     "AwsRedshiftClusterElasticIpStatusTypeDef",
     {
         "ElasticIp": str,
         "Status": str,
     },
     total=False,
@@ -6803,73 +4085,35 @@
     {
         "Status": str,
         "VpcSecurityGroupId": str,
     },
     total=False,
 )
 
-AwsS3AccountPublicAccessBlockDetailsOutputTypeDef = TypedDict(
-    "AwsS3AccountPublicAccessBlockDetailsOutputTypeDef",
-    {
-        "BlockPublicAcls": bool,
-        "BlockPublicPolicy": bool,
-        "IgnorePublicAcls": bool,
-        "RestrictPublicBuckets": bool,
-    },
-    total=False,
-)
-
 AwsS3AccountPublicAccessBlockDetailsTypeDef = TypedDict(
     "AwsS3AccountPublicAccessBlockDetailsTypeDef",
     {
         "BlockPublicAcls": bool,
         "BlockPublicPolicy": bool,
         "IgnorePublicAcls": bool,
         "RestrictPublicBuckets": bool,
     },
     total=False,
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef",
-    {
-        "DaysAfterInitiation": int,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef = (
     TypedDict(
         "AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef",
         {
             "DaysAfterInitiation": int,
         },
         total=False,
     )
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef",
-    {
-        "Days": int,
-        "StorageClass": str,
-    },
-    total=False,
-)
-
-AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef",
-    {
-        "Date": str,
-        "Days": int,
-        "StorageClass": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef",
     {
         "Days": int,
         "StorageClass": str,
     },
     total=False,
@@ -6881,284 +4125,137 @@
         "Date": str,
         "Days": int,
         "StorageClass": str,
     },
     total=False,
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsS3BucketBucketVersioningConfigurationOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketVersioningConfigurationOutputTypeDef",
-    {
-        "IsMfaDeleteEnabled": bool,
-        "Status": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketVersioningConfigurationTypeDef = TypedDict(
     "AwsS3BucketBucketVersioningConfigurationTypeDef",
     {
         "IsMfaDeleteEnabled": bool,
         "Status": str,
     },
     total=False,
 )
 
-AwsS3BucketLoggingConfigurationOutputTypeDef = TypedDict(
-    "AwsS3BucketLoggingConfigurationOutputTypeDef",
-    {
-        "DestinationBucketName": str,
-        "LogFilePrefix": str,
-    },
-    total=False,
-)
-
 AwsS3BucketLoggingConfigurationTypeDef = TypedDict(
     "AwsS3BucketLoggingConfigurationTypeDef",
     {
         "DestinationBucketName": str,
         "LogFilePrefix": str,
     },
     total=False,
 )
 
-AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef = TypedDict(
-    "AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef",
-    {
-        "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef",
     {
         "Name": AwsS3BucketNotificationConfigurationS3KeyFilterRuleNameType,
         "Value": str,
     },
     total=False,
 )
 
-AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef",
-    {
-        "Days": int,
-        "Mode": str,
-        "Years": int,
-    },
-    total=False,
-)
-
 AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef",
     {
         "Days": int,
         "Mode": str,
         "Years": int,
     },
     total=False,
 )
 
-AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef = TypedDict(
-    "AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef",
-    {
-        "SSEAlgorithm": str,
-        "KMSMasterKeyID": str,
-    },
-    total=False,
-)
-
 AwsS3BucketServerSideEncryptionByDefaultTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionByDefaultTypeDef",
     {
         "SSEAlgorithm": str,
         "KMSMasterKeyID": str,
     },
     total=False,
 )
 
-AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef",
-    {
-        "Hostname": str,
-        "Protocol": str,
-    },
-    total=False,
-)
-
 AwsS3BucketWebsiteConfigurationRedirectToTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRedirectToTypeDef",
     {
         "Hostname": str,
         "Protocol": str,
     },
     total=False,
 )
 
-AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef",
-    {
-        "HttpErrorCodeReturnedEquals": str,
-        "KeyPrefixEquals": str,
-    },
-    total=False,
-)
-
 AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef",
     {
         "HttpErrorCodeReturnedEquals": str,
         "KeyPrefixEquals": str,
     },
     total=False,
 )
 
-AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef",
-    {
-        "Hostname": str,
-        "HttpRedirectCode": str,
-        "Protocol": str,
-        "ReplaceKeyPrefixWith": str,
-        "ReplaceKeyWith": str,
-    },
-    total=False,
-)
-
 AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef",
     {
         "Hostname": str,
         "HttpRedirectCode": str,
         "Protocol": str,
         "ReplaceKeyPrefixWith": str,
         "ReplaceKeyWith": str,
     },
     total=False,
 )
 
-AwsS3ObjectDetailsOutputTypeDef = TypedDict(
-    "AwsS3ObjectDetailsOutputTypeDef",
-    {
-        "LastModified": str,
-        "ETag": str,
-        "VersionId": str,
-        "ContentType": str,
-        "ServerSideEncryption": str,
-        "SSEKMSKeyId": str,
-    },
-    total=False,
-)
-
 AwsS3ObjectDetailsTypeDef = TypedDict(
     "AwsS3ObjectDetailsTypeDef",
     {
         "LastModified": str,
         "ETag": str,
         "VersionId": str,
         "ContentType": str,
         "ServerSideEncryption": str,
         "SSEKMSKeyId": str,
     },
     total=False,
 )
 
-AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef",
-    {
-        "MinimumInstanceMetadataServiceVersion": str,
-    },
-    total=False,
-)
-
 AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef = TypedDict(
     "AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef",
     {
         "MinimumInstanceMetadataServiceVersion": str,
     },
     total=False,
 )
 
-AwsSecretsManagerSecretRotationRulesOutputTypeDef = TypedDict(
-    "AwsSecretsManagerSecretRotationRulesOutputTypeDef",
-    {
-        "AutomaticallyAfterDays": int,
-    },
-    total=False,
-)
-
 AwsSecretsManagerSecretRotationRulesTypeDef = TypedDict(
     "AwsSecretsManagerSecretRotationRulesTypeDef",
     {
         "AutomaticallyAfterDays": int,
     },
     total=False,
 )
 
-BooleanFilterOutputTypeDef = TypedDict(
-    "BooleanFilterOutputTypeDef",
-    {
-        "Value": bool,
-    },
-    total=False,
-)
-
-IpFilterOutputTypeDef = TypedDict(
-    "IpFilterOutputTypeDef",
-    {
-        "Cidr": str,
-    },
-    total=False,
-)
-
-KeywordFilterOutputTypeDef = TypedDict(
-    "KeywordFilterOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
 BooleanFilterTypeDef = TypedDict(
     "BooleanFilterTypeDef",
     {
         "Value": bool,
     },
     total=False,
 )
@@ -7175,131 +4272,22 @@
     "KeywordFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-AwsSecurityFindingIdentifierOutputTypeDef = TypedDict(
-    "AwsSecurityFindingIdentifierOutputTypeDef",
-    {
-        "Id": str,
-        "ProductArn": str,
-    },
-)
-
 AwsSecurityFindingIdentifierTypeDef = TypedDict(
     "AwsSecurityFindingIdentifierTypeDef",
     {
         "Id": str,
         "ProductArn": str,
     },
 )
 
-_RequiredMalwareOutputTypeDef = TypedDict(
-    "_RequiredMalwareOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalMalwareOutputTypeDef = TypedDict(
-    "_OptionalMalwareOutputTypeDef",
-    {
-        "Type": MalwareTypeType,
-        "Path": str,
-        "State": MalwareStateType,
-    },
-    total=False,
-)
-
-class MalwareOutputTypeDef(_RequiredMalwareOutputTypeDef, _OptionalMalwareOutputTypeDef):
-    pass
-
-NoteOutputTypeDef = TypedDict(
-    "NoteOutputTypeDef",
-    {
-        "Text": str,
-        "UpdatedBy": str,
-        "UpdatedAt": str,
-    },
-)
-
-_RequiredPatchSummaryOutputTypeDef = TypedDict(
-    "_RequiredPatchSummaryOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalPatchSummaryOutputTypeDef = TypedDict(
-    "_OptionalPatchSummaryOutputTypeDef",
-    {
-        "InstalledCount": int,
-        "MissingCount": int,
-        "FailedCount": int,
-        "InstalledOtherCount": int,
-        "InstalledRejectedCount": int,
-        "InstalledPendingReboot": int,
-        "OperationStartTime": str,
-        "OperationEndTime": str,
-        "RebootOption": str,
-        "Operation": str,
-    },
-    total=False,
-)
-
-class PatchSummaryOutputTypeDef(
-    _RequiredPatchSummaryOutputTypeDef, _OptionalPatchSummaryOutputTypeDef
-):
-    pass
-
-ProcessDetailsOutputTypeDef = TypedDict(
-    "ProcessDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Path": str,
-        "Pid": int,
-        "ParentPid": int,
-        "LaunchedAt": str,
-        "TerminatedAt": str,
-    },
-    total=False,
-)
-
-SeverityOutputTypeDef = TypedDict(
-    "SeverityOutputTypeDef",
-    {
-        "Product": float,
-        "Label": SeverityLabelType,
-        "Normalized": int,
-        "Original": str,
-    },
-    total=False,
-)
-
-ThreatIntelIndicatorOutputTypeDef = TypedDict(
-    "ThreatIntelIndicatorOutputTypeDef",
-    {
-        "Type": ThreatIntelIndicatorTypeType,
-        "Value": str,
-        "Category": ThreatIntelIndicatorCategoryType,
-        "LastObservedAt": str,
-        "Source": str,
-        "SourceUrl": str,
-    },
-    total=False,
-)
-
-WorkflowOutputTypeDef = TypedDict(
-    "WorkflowOutputTypeDef",
-    {
-        "Status": WorkflowStatusType,
-    },
-    total=False,
-)
-
 _RequiredMalwareTypeDef = TypedDict(
     "_RequiredMalwareTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalMalwareTypeDef = TypedDict(
@@ -7391,79 +4379,34 @@
     "WorkflowTypeDef",
     {
         "Status": WorkflowStatusType,
     },
     total=False,
 )
 
-AwsSnsTopicSubscriptionOutputTypeDef = TypedDict(
-    "AwsSnsTopicSubscriptionOutputTypeDef",
-    {
-        "Endpoint": str,
-        "Protocol": str,
-    },
-    total=False,
-)
-
 AwsSnsTopicSubscriptionTypeDef = TypedDict(
     "AwsSnsTopicSubscriptionTypeDef",
     {
         "Endpoint": str,
         "Protocol": str,
     },
     total=False,
 )
 
-AwsSqsQueueDetailsOutputTypeDef = TypedDict(
-    "AwsSqsQueueDetailsOutputTypeDef",
-    {
-        "KmsDataKeyReusePeriodSeconds": int,
-        "KmsMasterKeyId": str,
-        "QueueName": str,
-        "DeadLetterTargetArn": str,
-    },
-    total=False,
-)
-
 AwsSqsQueueDetailsTypeDef = TypedDict(
     "AwsSqsQueueDetailsTypeDef",
     {
         "KmsDataKeyReusePeriodSeconds": int,
         "KmsMasterKeyId": str,
         "QueueName": str,
         "DeadLetterTargetArn": str,
     },
     total=False,
 )
 
-AwsSsmComplianceSummaryOutputTypeDef = TypedDict(
-    "AwsSsmComplianceSummaryOutputTypeDef",
-    {
-        "Status": str,
-        "CompliantCriticalCount": int,
-        "CompliantHighCount": int,
-        "CompliantMediumCount": int,
-        "ExecutionType": str,
-        "NonCompliantCriticalCount": int,
-        "CompliantInformationalCount": int,
-        "NonCompliantInformationalCount": int,
-        "CompliantUnspecifiedCount": int,
-        "NonCompliantLowCount": int,
-        "NonCompliantHighCount": int,
-        "CompliantLowCount": int,
-        "ComplianceType": str,
-        "PatchBaselineId": str,
-        "OverallSeverity": str,
-        "NonCompliantMediumCount": int,
-        "NonCompliantUnspecifiedCount": int,
-        "PatchGroup": str,
-    },
-    total=False,
-)
-
 AwsSsmComplianceSummaryTypeDef = TypedDict(
     "AwsSsmComplianceSummaryTypeDef",
     {
         "Status": str,
         "CompliantCriticalCount": int,
         "CompliantHighCount": int,
         "CompliantMediumCount": int,
@@ -7481,214 +4424,102 @@
         "NonCompliantMediumCount": int,
         "NonCompliantUnspecifiedCount": int,
         "PatchGroup": str,
     },
     total=False,
 )
 
-AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef",
-    {
-        "LogGroupArn": str,
-    },
-    total=False,
-)
-
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef",
     {
         "LogGroupArn": str,
     },
     total=False,
 )
 
-AwsWafRateBasedRuleMatchPredicateOutputTypeDef = TypedDict(
-    "AwsWafRateBasedRuleMatchPredicateOutputTypeDef",
-    {
-        "DataId": str,
-        "Negated": bool,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef = TypedDict(
-    "AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef",
-    {
-        "DataId": str,
-        "Negated": bool,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalRateBasedRuleMatchPredicateTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleMatchPredicateTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalRulePredicateListDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalRulePredicateListDetailsOutputTypeDef",
-    {
-        "DataId": str,
-        "Negated": bool,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalRulePredicateListDetailsTypeDef = TypedDict(
     "AwsWafRegionalRulePredicateListDetailsTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalRuleGroupRulesActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesActionDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalWebAclRulesListActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListActionDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRulePredicateListDetailsOutputTypeDef = TypedDict(
-    "AwsWafRulePredicateListDetailsOutputTypeDef",
-    {
-        "DataId": str,
-        "Negated": bool,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRulePredicateListDetailsTypeDef = TypedDict(
     "AwsWafRulePredicateListDetailsTypeDef",
     {
         "DataId": str,
         "Negated": bool,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRuleGroupRulesActionDetailsOutputTypeDef = TypedDict(
-    "AwsWafRuleGroupRulesActionDetailsOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRuleGroupRulesActionDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupRulesActionDetailsTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-WafActionOutputTypeDef = TypedDict(
-    "WafActionOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
-WafExcludedRuleOutputTypeDef = TypedDict(
-    "WafExcludedRuleOutputTypeDef",
-    {
-        "RuleId": str,
-    },
-    total=False,
-)
-
-WafOverrideActionOutputTypeDef = TypedDict(
-    "WafOverrideActionOutputTypeDef",
-    {
-        "Type": str,
-    },
-    total=False,
-)
-
 WafActionTypeDef = TypedDict(
     "WafActionTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
@@ -7705,78 +4536,41 @@
     "WafOverrideActionTypeDef",
     {
         "Type": str,
     },
     total=False,
 )
 
-AwsWafv2CustomHttpHeaderOutputTypeDef = TypedDict(
-    "AwsWafv2CustomHttpHeaderOutputTypeDef",
-    {
-        "Name": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 AwsWafv2CustomHttpHeaderTypeDef = TypedDict(
     "AwsWafv2CustomHttpHeaderTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AwsWafv2VisibilityConfigDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2VisibilityConfigDetailsOutputTypeDef",
-    {
-        "CloudWatchMetricsEnabled": bool,
-        "MetricName": str,
-        "SampledRequestsEnabled": bool,
-    },
-    total=False,
-)
-
 AwsWafv2VisibilityConfigDetailsTypeDef = TypedDict(
     "AwsWafv2VisibilityConfigDetailsTypeDef",
     {
         "CloudWatchMetricsEnabled": bool,
         "MetricName": str,
         "SampledRequestsEnabled": bool,
     },
     total=False,
 )
 
-AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef",
-    {
-        "ImmunityTime": int,
-    },
-    total=False,
-)
-
 AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef",
     {
         "ImmunityTime": int,
     },
     total=False,
 )
 
-AwsXrayEncryptionConfigDetailsOutputTypeDef = TypedDict(
-    "AwsXrayEncryptionConfigDetailsOutputTypeDef",
-    {
-        "KeyId": str,
-        "Status": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsXrayEncryptionConfigDetailsTypeDef = TypedDict(
     "AwsXrayEncryptionConfigDetailsTypeDef",
     {
         "KeyId": str,
         "Status": str,
         "Type": str,
     },
@@ -7947,73 +4741,34 @@
 
 class StandardsControlAssociationUpdateTypeDef(
     _RequiredStandardsControlAssociationUpdateTypeDef,
     _OptionalStandardsControlAssociationUpdateTypeDef,
 ):
     pass
 
-CellOutputTypeDef = TypedDict(
-    "CellOutputTypeDef",
-    {
-        "Column": int,
-        "Row": int,
-        "ColumnName": str,
-        "CellReference": str,
-    },
-    total=False,
-)
-
 CellTypeDef = TypedDict(
     "CellTypeDef",
     {
         "Column": int,
         "Row": int,
         "ColumnName": str,
         "CellReference": str,
     },
     total=False,
 )
 
-ClassificationStatusOutputTypeDef = TypedDict(
-    "ClassificationStatusOutputTypeDef",
-    {
-        "Code": str,
-        "Reason": str,
-    },
-    total=False,
-)
-
 ClassificationStatusTypeDef = TypedDict(
     "ClassificationStatusTypeDef",
     {
         "Code": str,
         "Reason": str,
     },
     total=False,
 )
 
-_RequiredStatusReasonOutputTypeDef = TypedDict(
-    "_RequiredStatusReasonOutputTypeDef",
-    {
-        "ReasonCode": str,
-    },
-)
-_OptionalStatusReasonOutputTypeDef = TypedDict(
-    "_OptionalStatusReasonOutputTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class StatusReasonOutputTypeDef(
-    _RequiredStatusReasonOutputTypeDef, _OptionalStatusReasonOutputTypeDef
-):
-    pass
-
 _RequiredStatusReasonTypeDef = TypedDict(
     "_RequiredStatusReasonTypeDef",
     {
         "ReasonCode": str,
     },
 )
 _OptionalStatusReasonTypeDef = TypedDict(
@@ -8023,23 +4778,14 @@
     },
     total=False,
 )
 
 class StatusReasonTypeDef(_RequiredStatusReasonTypeDef, _OptionalStatusReasonTypeDef):
     pass
 
-VolumeMountOutputTypeDef = TypedDict(
-    "VolumeMountOutputTypeDef",
-    {
-        "Name": str,
-        "MountPath": str,
-    },
-    total=False,
-)
-
 VolumeMountTypeDef = TypedDict(
     "VolumeMountTypeDef",
     {
         "Name": str,
         "MountPath": str,
     },
     total=False,
@@ -8079,23 +4825,14 @@
     {
         "AccountId": str,
         "ProcessingResult": str,
     },
     total=False,
 )
 
-DateRangeOutputTypeDef = TypedDict(
-    "DateRangeOutputTypeDef",
-    {
-        "Value": int,
-        "Unit": Literal["DAYS"],
-    },
-    total=False,
-)
-
 DateRangeTypeDef = TypedDict(
     "DateRangeTypeDef",
     {
         "Value": int,
         "Unit": Literal["DAYS"],
     },
     total=False,
@@ -8293,25 +5030,14 @@
         "Tags": Mapping[str, str],
         "EnableDefaultStandards": bool,
         "ControlFindingGenerator": ControlFindingGeneratorType,
     },
     total=False,
 )
 
-FilePathsOutputTypeDef = TypedDict(
-    "FilePathsOutputTypeDef",
-    {
-        "FilePath": str,
-        "FileName": str,
-        "ResourceId": str,
-        "Hash": str,
-    },
-    total=False,
-)
-
 FilePathsTypeDef = TypedDict(
     "FilePathsTypeDef",
     {
         "FilePath": str,
         "FileName": str,
         "ResourceId": str,
         "Hash": str,
@@ -8342,49 +5068,23 @@
         "UpdatedField": str,
         "OldValue": str,
         "NewValue": str,
     },
     total=False,
 )
 
-FindingProviderSeverityOutputTypeDef = TypedDict(
-    "FindingProviderSeverityOutputTypeDef",
-    {
-        "Label": SeverityLabelType,
-        "Original": str,
-    },
-    total=False,
-)
-
 FindingProviderSeverityTypeDef = TypedDict(
     "FindingProviderSeverityTypeDef",
     {
         "Label": SeverityLabelType,
         "Original": str,
     },
     total=False,
 )
 
-FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef = TypedDict(
-    "FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef",
-    {
-        "ResourceArn": str,
-    },
-    total=False,
-)
-
-FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef = TypedDict(
-    "FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef",
-    {
-        "Priority": int,
-        "ResourceArn": str,
-    },
-    total=False,
-)
-
 FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef = TypedDict(
     "FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef",
     {
         "ResourceArn": str,
     },
     total=False,
 )
@@ -8616,51 +5316,23 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-PortRangeOutputTypeDef = TypedDict(
-    "PortRangeOutputTypeDef",
-    {
-        "Begin": int,
-        "End": int,
-    },
-    total=False,
-)
-
 PortRangeTypeDef = TypedDict(
     "PortRangeTypeDef",
     {
         "Begin": int,
         "End": int,
     },
     total=False,
 )
 
-RangeOutputTypeDef = TypedDict(
-    "RangeOutputTypeDef",
-    {
-        "Start": int,
-        "End": int,
-        "StartColumn": int,
-    },
-    total=False,
-)
-
-RecordOutputTypeDef = TypedDict(
-    "RecordOutputTypeDef",
-    {
-        "JsonPath": str,
-        "RecordIndex": int,
-    },
-    total=False,
-)
-
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "Start": int,
         "End": int,
         "StartColumn": int,
     },
@@ -8672,23 +5344,14 @@
     {
         "JsonPath": str,
         "RecordIndex": int,
     },
     total=False,
 )
 
-RecommendationOutputTypeDef = TypedDict(
-    "RecommendationOutputTypeDef",
-    {
-        "Text": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Text": str,
         "Url": str,
     },
     total=False,
@@ -8710,16 +5373,16 @@
         "GeneratedRulesType": str,
         "TargetTypes": Sequence[str],
         "Targets": Sequence[str],
     },
     total=False,
 )
 
-RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef",
+RuleGroupSourceStatefulRulesHeaderDetailsTypeDef = TypedDict(
+    "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
     {
         "Destination": str,
         "DestinationPort": str,
         "Direction": str,
         "Protocol": str,
         "Source": str,
         "SourcePort": str,
@@ -8732,81 +5395,51 @@
     {
         "Keyword": str,
         "Settings": List[str],
     },
     total=False,
 )
 
-RuleGroupSourceStatefulRulesHeaderDetailsTypeDef = TypedDict(
-    "RuleGroupSourceStatefulRulesHeaderDetailsTypeDef",
-    {
-        "Destination": str,
-        "DestinationPort": str,
-        "Direction": str,
-        "Protocol": str,
-        "Source": str,
-        "SourcePort": str,
-    },
-    total=False,
-)
-
 RuleGroupSourceStatefulRulesOptionsDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesOptionsDetailsTypeDef",
     {
         "Keyword": str,
         "Settings": Sequence[str],
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef",
-    {
-        "FromPort": int,
-        "ToPort": int,
-    },
-    total=False,
-)
-
 RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef",
-    {
-        "AddressDefinition": str,
-    },
-    total=False,
-)
-
 RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef",
     {
         "AddressDefinition": str,
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef",
+RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
     {
         "FromPort": int,
         "ToPort": int,
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef",
+RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef = TypedDict(
+    "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
     {
         "AddressDefinition": str,
     },
     total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef = TypedDict(
@@ -8814,31 +5447,14 @@
     {
         "Flags": List[str],
         "Masks": List[str],
     },
     total=False,
 )
 
-RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef",
-    {
-        "FromPort": int,
-        "ToPort": int,
-    },
-    total=False,
-)
-
-RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef = TypedDict(
-    "RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef",
-    {
-        "AddressDefinition": str,
-    },
-    total=False,
-)
-
 RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef",
     {
         "Flags": Sequence[str],
         "Masks": Sequence[str],
     },
     total=False,
@@ -8872,32 +5488,14 @@
     "RuleGroupVariablesPortSetsDetailsTypeDef",
     {
         "Definition": Sequence[str],
     },
     total=False,
 )
 
-SoftwarePackageOutputTypeDef = TypedDict(
-    "SoftwarePackageOutputTypeDef",
-    {
-        "Name": str,
-        "Version": str,
-        "Epoch": str,
-        "Release": str,
-        "Architecture": str,
-        "PackageManager": str,
-        "FilePath": str,
-        "FixedInVersion": str,
-        "Remediation": str,
-        "SourceLayerHash": str,
-        "SourceLayerArn": str,
-    },
-    total=False,
-)
-
 SoftwarePackageTypeDef = TypedDict(
     "SoftwarePackageTypeDef",
     {
         "Name": str,
         "Version": str,
         "Epoch": str,
         "Release": str,
@@ -8917,59 +5515,21 @@
     {
         "Company": str,
         "Product": str,
     },
     total=False,
 )
 
-StandardsControlAssociationIdOutputTypeDef = TypedDict(
-    "StandardsControlAssociationIdOutputTypeDef",
-    {
-        "SecurityControlId": str,
-        "StandardsArn": str,
-    },
-)
-
-_RequiredStandardsControlAssociationUpdateOutputTypeDef = TypedDict(
-    "_RequiredStandardsControlAssociationUpdateOutputTypeDef",
-    {
-        "StandardsArn": str,
-        "SecurityControlId": str,
-        "AssociationStatus": AssociationStatusType,
-    },
-)
-_OptionalStandardsControlAssociationUpdateOutputTypeDef = TypedDict(
-    "_OptionalStandardsControlAssociationUpdateOutputTypeDef",
-    {
-        "UpdatedReason": str,
-    },
-    total=False,
-)
-
-class StandardsControlAssociationUpdateOutputTypeDef(
-    _RequiredStandardsControlAssociationUpdateOutputTypeDef,
-    _OptionalStandardsControlAssociationUpdateOutputTypeDef,
-):
-    pass
-
 StandardsStatusReasonTypeDef = TypedDict(
     "StandardsStatusReasonTypeDef",
     {
         "StatusReasonCode": StatusReasonCodeType,
     },
 )
 
-StatelessCustomPublishMetricActionDimensionOutputTypeDef = TypedDict(
-    "StatelessCustomPublishMetricActionDimensionOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
 StatelessCustomPublishMetricActionDimensionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionDimensionTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
@@ -9078,36 +5638,14 @@
 
 class UpdateStandardsControlRequestRequestTypeDef(
     _RequiredUpdateStandardsControlRequestRequestTypeDef,
     _OptionalUpdateStandardsControlRequestRequestTypeDef,
 ):
     pass
 
-_RequiredVulnerabilityVendorOutputTypeDef = TypedDict(
-    "_RequiredVulnerabilityVendorOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalVulnerabilityVendorOutputTypeDef = TypedDict(
-    "_OptionalVulnerabilityVendorOutputTypeDef",
-    {
-        "Url": str,
-        "VendorSeverity": str,
-        "VendorCreatedAt": str,
-        "VendorUpdatedAt": str,
-    },
-    total=False,
-)
-
-class VulnerabilityVendorOutputTypeDef(
-    _RequiredVulnerabilityVendorOutputTypeDef, _OptionalVulnerabilityVendorOutputTypeDef
-):
-    pass
-
 _RequiredVulnerabilityVendorTypeDef = TypedDict(
     "_RequiredVulnerabilityVendorTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalVulnerabilityVendorTypeDef = TypedDict(
@@ -9129,26 +5667,14 @@
 CreateMembersRequestRequestTypeDef = TypedDict(
     "CreateMembersRequestRequestTypeDef",
     {
         "AccountDetails": Sequence[AccountDetailsTypeDef],
     },
 )
 
-ActionRemoteIpDetailsOutputTypeDef = TypedDict(
-    "ActionRemoteIpDetailsOutputTypeDef",
-    {
-        "IpAddressV4": str,
-        "Organization": IpOrganizationDetailsOutputTypeDef,
-        "Country": CountryOutputTypeDef,
-        "City": CityOutputTypeDef,
-        "GeoLocation": GeoLocationOutputTypeDef,
-    },
-    total=False,
-)
-
 ActionRemoteIpDetailsTypeDef = TypedDict(
     "ActionRemoteIpDetailsTypeDef",
     {
         "IpAddressV4": str,
         "Organization": IpOrganizationDetailsTypeDef,
         "Country": CountryTypeDef,
         "City": CityTypeDef,
@@ -9160,15 +5686,15 @@
 CvssOutputTypeDef = TypedDict(
     "CvssOutputTypeDef",
     {
         "Version": str,
         "BaseScore": float,
         "BaseVector": str,
         "Source": str,
-        "Adjustments": List[AdjustmentOutputTypeDef],
+        "Adjustments": List[AdjustmentTypeDef],
     },
     total=False,
 )
 
 CvssTypeDef = TypedDict(
     "CvssTypeDef",
     {
@@ -9177,27 +5703,14 @@
         "BaseVector": str,
         "Source": str,
         "Adjustments": Sequence[AdjustmentTypeDef],
     },
     total=False,
 )
 
-AssociationSetDetailsOutputTypeDef = TypedDict(
-    "AssociationSetDetailsOutputTypeDef",
-    {
-        "AssociationState": AssociationStateDetailsOutputTypeDef,
-        "GatewayId": str,
-        "Main": bool,
-        "RouteTableAssociationId": str,
-        "RouteTableId": str,
-        "SubnetId": str,
-    },
-    total=False,
-)
-
 AssociationSetDetailsTypeDef = TypedDict(
     "AssociationSetDetailsTypeDef",
     {
         "AssociationState": AssociationStateDetailsTypeDef,
         "GatewayId": str,
         "Main": bool,
         "RouteTableAssociationId": str,
@@ -9206,23 +5719,23 @@
     },
     total=False,
 )
 
 AutomationRulesFindingFieldsUpdateOutputTypeDef = TypedDict(
     "AutomationRulesFindingFieldsUpdateOutputTypeDef",
     {
-        "Note": NoteUpdateOutputTypeDef,
-        "Severity": SeverityUpdateOutputTypeDef,
+        "Note": NoteUpdateTypeDef,
+        "Severity": SeverityUpdateTypeDef,
         "VerificationState": VerificationStateType,
         "Confidence": int,
         "Criticality": int,
         "Types": List[str],
         "UserDefinedFields": Dict[str, str],
-        "Workflow": WorkflowUpdateOutputTypeDef,
-        "RelatedFindings": List[RelatedFindingOutputTypeDef],
+        "Workflow": WorkflowUpdateTypeDef,
+        "RelatedFindings": List[RelatedFindingTypeDef],
     },
     total=False,
 )
 
 AutomationRulesFindingFieldsUpdateTypeDef = TypedDict(
     "AutomationRulesFindingFieldsUpdateTypeDef",
     {
@@ -9235,26 +5748,14 @@
         "UserDefinedFields": Mapping[str, str],
         "Workflow": WorkflowUpdateTypeDef,
         "RelatedFindings": Sequence[RelatedFindingTypeDef],
     },
     total=False,
 )
 
-AwsAmazonMqBrokerLogsDetailsOutputTypeDef = TypedDict(
-    "AwsAmazonMqBrokerLogsDetailsOutputTypeDef",
-    {
-        "Audit": bool,
-        "General": bool,
-        "AuditLogGroup": str,
-        "GeneralLogGroup": str,
-        "Pending": AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsAmazonMqBrokerLogsDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerLogsDetailsTypeDef",
     {
         "Audit": bool,
         "General": bool,
         "AuditLogGroup": str,
         "GeneralLogGroup": str,
@@ -9301,18 +5802,18 @@
         "DeploymentId": str,
         "ClientCertificateId": str,
         "StageName": str,
         "Description": str,
         "CacheClusterEnabled": bool,
         "CacheClusterSize": str,
         "CacheClusterStatus": str,
-        "MethodSettings": List[AwsApiGatewayMethodSettingsOutputTypeDef],
+        "MethodSettings": List[AwsApiGatewayMethodSettingsTypeDef],
         "Variables": Dict[str, str],
         "DocumentationVersion": str,
-        "AccessLogSettings": AwsApiGatewayAccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AwsApiGatewayAccessLogSettingsTypeDef,
         "CanarySettings": AwsApiGatewayCanarySettingsOutputTypeDef,
         "TracingEnabled": bool,
         "CreatedDate": str,
         "LastUpdatedDate": str,
         "WebAclArn": str,
     },
     total=False,
@@ -9377,21 +5878,21 @@
 
 AwsApiGatewayV2StageDetailsOutputTypeDef = TypedDict(
     "AwsApiGatewayV2StageDetailsOutputTypeDef",
     {
         "ClientCertificateId": str,
         "CreatedDate": str,
         "Description": str,
-        "DefaultRouteSettings": AwsApiGatewayV2RouteSettingsOutputTypeDef,
+        "DefaultRouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
         "DeploymentId": str,
         "LastUpdatedDate": str,
-        "RouteSettings": AwsApiGatewayV2RouteSettingsOutputTypeDef,
+        "RouteSettings": AwsApiGatewayV2RouteSettingsTypeDef,
         "StageName": str,
         "StageVariables": Dict[str, str],
-        "AccessLogSettings": AwsApiGatewayAccessLogSettingsOutputTypeDef,
+        "AccessLogSettings": AwsApiGatewayAccessLogSettingsTypeDef,
         "AutoDeploy": bool,
         "LastDeploymentStatusMessage": str,
         "ApiGatewayManaged": bool,
     },
     total=False,
 )
 
@@ -9411,60 +5912,41 @@
         "AutoDeploy": bool,
         "LastDeploymentStatusMessage": str,
         "ApiGatewayManaged": bool,
     },
     total=False,
 )
 
-AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef = TypedDict(
-    "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef",
-    {
-        "AuthenticationType": str,
-        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
-        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
-        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef",
     {
         "AuthenticationType": str,
         "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
         "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
         "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
     },
     total=False,
 )
 
-AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef",
-    {
-        "EncryptionConfiguration": AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef",
     {
         "EncryptionConfiguration": (
             AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef
         ),
     },
     total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef",
     {
-        "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
+        "LaunchTemplateSpecification": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
         "Overrides": List[
-            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
         ],
     },
     total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef",
@@ -9473,45 +5955,25 @@
         "Overrides": Sequence[
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef
         ],
     },
     total=False,
 )
 
-AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef = TypedDict(
-    "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef",
-    {
-        "DeviceName": str,
-        "Ebs": AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef,
-        "NoDevice": bool,
-        "VirtualName": str,
-    },
-    total=False,
-)
-
 AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
         "NoDevice": bool,
         "VirtualName": str,
     },
     total=False,
 )
 
-AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef = TypedDict(
-    "AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef",
-    {
-        "DestinationBackupVaultArn": str,
-        "Lifecycle": AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef",
     {
         "DestinationBackupVaultArn": str,
         "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
     },
     total=False,
@@ -9537,40 +5999,14 @@
         "EncryptionKeyArn": str,
         "Notifications": AwsBackupBackupVaultNotificationsDetailsTypeDef,
         "AccessPolicy": str,
     },
     total=False,
 )
 
-AwsBackupRecoveryPointDetailsOutputTypeDef = TypedDict(
-    "AwsBackupRecoveryPointDetailsOutputTypeDef",
-    {
-        "BackupSizeInBytes": int,
-        "BackupVaultArn": str,
-        "BackupVaultName": str,
-        "CalculatedLifecycle": AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef,
-        "CompletionDate": str,
-        "CreatedBy": AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef,
-        "CreationDate": str,
-        "EncryptionKeyArn": str,
-        "IamRoleArn": str,
-        "IsEncrypted": bool,
-        "LastRestoreTime": str,
-        "Lifecycle": AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef,
-        "RecoveryPointArn": str,
-        "ResourceArn": str,
-        "ResourceType": str,
-        "SourceBackupVaultArn": str,
-        "Status": str,
-        "StatusMessage": str,
-        "StorageClass": str,
-    },
-    total=False,
-)
-
 AwsBackupRecoveryPointDetailsTypeDef = TypedDict(
     "AwsBackupRecoveryPointDetailsTypeDef",
     {
         "BackupSizeInBytes": int,
         "BackupVaultArn": str,
         "BackupVaultName": str,
         "CalculatedLifecycle": AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef,
@@ -9593,15 +6029,15 @@
     total=False,
 )
 
 AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef = TypedDict(
     "AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef",
     {
         "DomainName": str,
-        "ResourceRecord": AwsCertificateManagerCertificateResourceRecordOutputTypeDef,
+        "ResourceRecord": AwsCertificateManagerCertificateResourceRecordTypeDef,
         "ValidationDomain": str,
         "ValidationEmails": List[str],
         "ValidationMethod": str,
         "ValidationStatus": str,
     },
     total=False,
 )
@@ -9622,19 +6058,19 @@
 AwsCloudFormationStackDetailsOutputTypeDef = TypedDict(
     "AwsCloudFormationStackDetailsOutputTypeDef",
     {
         "Capabilities": List[str],
         "CreationTime": str,
         "Description": str,
         "DisableRollback": bool,
-        "DriftInformation": AwsCloudFormationStackDriftInformationDetailsOutputTypeDef,
+        "DriftInformation": AwsCloudFormationStackDriftInformationDetailsTypeDef,
         "EnableTerminationProtection": bool,
         "LastUpdatedTime": str,
         "NotificationArns": List[str],
-        "Outputs": List[AwsCloudFormationStackOutputsDetailsOutputTypeDef],
+        "Outputs": List[AwsCloudFormationStackOutputsDetailsTypeDef],
         "RoleArn": str,
         "StackId": str,
         "StackName": str,
         "StackStatus": str,
         "StackStatusReason": str,
         "TimeoutInMinutes": int,
     },
@@ -9662,15 +6098,15 @@
     },
     total=False,
 )
 
 AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef",
     {
-        "Items": List[AwsCloudFrontDistributionCacheBehaviorOutputTypeDef],
+        "Items": List[AwsCloudFrontDistributionCacheBehaviorTypeDef],
     },
     total=False,
 )
 
 AwsCloudFrontDistributionCacheBehaviorsTypeDef = TypedDict(
     "AwsCloudFrontDistributionCacheBehaviorsTypeDef",
     {
@@ -9728,15 +6164,15 @@
         "AlarmActions": List[str],
         "AlarmArn": str,
         "AlarmConfigurationUpdatedTimestamp": str,
         "AlarmDescription": str,
         "AlarmName": str,
         "ComparisonOperator": str,
         "DatapointsToAlarm": int,
-        "Dimensions": List[AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef],
+        "Dimensions": List[AwsCloudWatchAlarmDimensionsDetailsTypeDef],
         "EvaluateLowSampleCountPercentile": str,
         "EvaluationPeriods": int,
         "ExtendedStatistic": str,
         "InsufficientDataActions": List[str],
         "MetricName": str,
         "Namespace": str,
         "OkActions": List[str],
@@ -9780,19 +6216,19 @@
 )
 
 AwsCodeBuildProjectEnvironmentOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentOutputTypeDef",
     {
         "Certificate": str,
         "EnvironmentVariables": List[
-            AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef
+            AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef
         ],
         "PrivilegedMode": bool,
         "ImagePullCredentialsType": str,
-        "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef,
+        "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 AwsCodeBuildProjectEnvironmentTypeDef = TypedDict(
     "AwsCodeBuildProjectEnvironmentTypeDef",
@@ -9805,23 +6241,14 @@
         "ImagePullCredentialsType": str,
         "RegistryCredential": AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
         "Type": str,
     },
     total=False,
 )
 
-AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef = TypedDict(
-    "AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef",
-    {
-        "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef,
-        "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsCodeBuildProjectLogsConfigDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectLogsConfigDetailsTypeDef",
     {
         "CloudWatchLogs": AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
         "S3Logs": AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
     },
     total=False,
@@ -9832,27 +6259,27 @@
     {
         "Backfilling": bool,
         "IndexArn": str,
         "IndexName": str,
         "IndexSizeBytes": int,
         "IndexStatus": str,
         "ItemCount": int,
-        "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
         "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
-        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
+        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputTypeDef,
     },
     total=False,
 )
 
 AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef = TypedDict(
     "AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef",
     {
         "IndexArn": str,
         "IndexName": str,
-        "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
         "Projection": AwsDynamoDbTableProjectionOutputTypeDef,
     },
     total=False,
 )
 
 AwsDynamoDbTableGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableGlobalSecondaryIndexTypeDef",
@@ -9877,23 +6304,14 @@
         "IndexName": str,
         "KeySchema": Sequence[AwsDynamoDbTableKeySchemaTypeDef],
         "Projection": AwsDynamoDbTableProjectionTypeDef,
     },
     total=False,
 )
 
-AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef = TypedDict(
-    "AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef",
-    {
-        "IndexName": str,
-        "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef",
     {
         "IndexName": str,
         "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
     },
     total=False,
@@ -9907,18 +6325,18 @@
         "IpV4Addresses": List[str],
         "IpV6Addresses": List[str],
         "KeyName": str,
         "IamInstanceProfileArn": str,
         "VpcId": str,
         "SubnetId": str,
         "LaunchedAt": str,
-        "NetworkInterfaces": List[AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef],
+        "NetworkInterfaces": List[AwsEc2InstanceNetworkInterfacesDetailsTypeDef],
         "VirtualizationType": str,
-        "MetadataOptions": AwsEc2InstanceMetadataOptionsOutputTypeDef,
-        "Monitoring": AwsEc2InstanceMonitoringDetailsOutputTypeDef,
+        "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
+        "Monitoring": AwsEc2InstanceMonitoringDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEc2InstanceDetailsTypeDef = TypedDict(
     "AwsEc2InstanceDetailsTypeDef",
     {
@@ -9935,106 +6353,79 @@
         "VirtualizationType": str,
         "MetadataOptions": AwsEc2InstanceMetadataOptionsTypeDef,
         "Monitoring": AwsEc2InstanceMonitoringDetailsTypeDef,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef",
-    {
-        "DeviceName": str,
-        "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef,
-        "NoDevice": str,
-        "VirtualName": str,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef",
     {
         "DeviceName": str,
         "Ebs": AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
         "NoDevice": str,
         "VirtualName": str,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef",
-    {
-        "CapacityReservationPreference": str,
-        "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef",
     {
         "CapacityReservationPreference": str,
         "CapacityReservationTarget": AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
     },
     total=False,
 )
 
-AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef",
-    {
-        "MarketType": str,
-        "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef",
     {
         "MarketType": str,
         "SpotOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef",
     {
         "AcceleratorCount": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef
         ),
         "AcceleratorManufacturers": List[str],
         "AcceleratorNames": List[str],
-        "AcceleratorTotalMemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef,
+        "AcceleratorTotalMemoryMiB": (
+            AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef
+        ),
         "AcceleratorTypes": List[str],
         "BareMetal": str,
         "BaselineEbsBandwidthMbps": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef
         ),
         "BurstablePerformance": str,
         "CpuManufacturers": List[str],
         "ExcludedInstanceTypes": List[str],
         "InstanceGenerations": List[str],
         "LocalStorage": str,
         "LocalStorageTypes": List[str],
         "MemoryGiBPerVCpu": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef
         ),
-        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef,
+        "MemoryMiB": AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
         "NetworkInterfaceCount": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef
         ),
         "OnDemandMaxPricePercentageOverLowestPrice": int,
         "RequireHibernateSupport": bool,
         "SpotMaxPricePercentageOverLowestPrice": int,
         "TotalLocalStorageGB": (
-            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef
         ),
-        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef,
+        "VCpuCount": AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef",
     {
@@ -10082,30 +6473,26 @@
         "AssociatePublicIpAddress": bool,
         "DeleteOnTermination": bool,
         "Description": str,
         "DeviceIndex": int,
         "Groups": List[str],
         "InterfaceType": str,
         "Ipv4PrefixCount": int,
-        "Ipv4Prefixes": List[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef
-        ],
+        "Ipv4Prefixes": List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef],
         "Ipv6AddressCount": int,
         "Ipv6Addresses": List[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef
         ],
         "Ipv6PrefixCount": int,
-        "Ipv6Prefixes": List[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef
-        ],
+        "Ipv6Prefixes": List[AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef],
         "NetworkCardIndex": int,
         "NetworkInterfaceId": str,
         "PrivateIpAddress": str,
         "PrivateIpAddresses": List[
-            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef
         ],
         "SecondaryPrivateIpAddressCount": int,
         "SubnetId": str,
     },
     total=False,
 )
 
@@ -10139,29 +6526,14 @@
         ],
         "SecondaryPrivateIpAddressCount": int,
         "SubnetId": str,
     },
     total=False,
 )
 
-AwsEc2NetworkAclEntryOutputTypeDef = TypedDict(
-    "AwsEc2NetworkAclEntryOutputTypeDef",
-    {
-        "CidrBlock": str,
-        "Egress": bool,
-        "IcmpTypeCode": IcmpTypeCodeOutputTypeDef,
-        "Ipv6CidrBlock": str,
-        "PortRange": PortRangeFromToOutputTypeDef,
-        "Protocol": str,
-        "RuleAction": str,
-        "RuleNumber": int,
-    },
-    total=False,
-)
-
 AwsEc2NetworkAclEntryTypeDef = TypedDict(
     "AwsEc2NetworkAclEntryTypeDef",
     {
         "CidrBlock": str,
         "Egress": bool,
         "IcmpTypeCode": IcmpTypeCodeTypeDef,
         "Ipv6CidrBlock": str,
@@ -10172,20 +6544,20 @@
     },
     total=False,
 )
 
 AwsEc2NetworkInterfaceDetailsOutputTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceDetailsOutputTypeDef",
     {
-        "Attachment": AwsEc2NetworkInterfaceAttachmentOutputTypeDef,
+        "Attachment": AwsEc2NetworkInterfaceAttachmentTypeDef,
         "NetworkInterfaceId": str,
-        "SecurityGroups": List[AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef],
+        "SecurityGroups": List[AwsEc2NetworkInterfaceSecurityGroupTypeDef],
         "SourceDestCheck": bool,
-        "IpV6Addresses": List[AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef],
-        "PrivateIpAddresses": List[AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef],
+        "IpV6Addresses": List[AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef],
+        "PrivateIpAddresses": List[AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef],
         "PublicDnsName": str,
         "PublicIp": str,
     },
     total=False,
 )
 
 AwsEc2NetworkInterfaceDetailsTypeDef = TypedDict(
@@ -10205,18 +6577,18 @@
 
 AwsEc2SecurityGroupIpPermissionOutputTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpPermissionOutputTypeDef",
     {
         "IpProtocol": str,
         "FromPort": int,
         "ToPort": int,
-        "UserIdGroupPairs": List[AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef],
-        "IpRanges": List[AwsEc2SecurityGroupIpRangeOutputTypeDef],
-        "Ipv6Ranges": List[AwsEc2SecurityGroupIpv6RangeOutputTypeDef],
-        "PrefixListIds": List[AwsEc2SecurityGroupPrefixListIdOutputTypeDef],
+        "UserIdGroupPairs": List[AwsEc2SecurityGroupUserIdGroupPairTypeDef],
+        "IpRanges": List[AwsEc2SecurityGroupIpRangeTypeDef],
+        "Ipv6Ranges": List[AwsEc2SecurityGroupIpv6RangeTypeDef],
+        "PrefixListIds": List[AwsEc2SecurityGroupPrefixListIdTypeDef],
     },
     total=False,
 )
 
 AwsEc2SecurityGroupIpPermissionTypeDef = TypedDict(
     "AwsEc2SecurityGroupIpPermissionTypeDef",
     {
@@ -10242,15 +6614,15 @@
         "DefaultForAz": bool,
         "MapPublicIpOnLaunch": bool,
         "OwnerId": str,
         "State": str,
         "SubnetArn": str,
         "SubnetId": str,
         "VpcId": str,
-        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationOutputTypeDef],
+        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationTypeDef],
     },
     total=False,
 )
 
 AwsEc2SubnetDetailsTypeDef = TypedDict(
     "AwsEc2SubnetDetailsTypeDef",
     {
@@ -10277,15 +6649,15 @@
         "CreateTime": str,
         "DeviceName": str,
         "Encrypted": bool,
         "Size": int,
         "SnapshotId": str,
         "Status": str,
         "KmsKeyId": str,
-        "Attachments": List[AwsEc2VolumeAttachmentOutputTypeDef],
+        "Attachments": List[AwsEc2VolumeAttachmentTypeDef],
         "VolumeId": str,
         "VolumeType": str,
         "VolumeScanStatus": str,
     },
     total=False,
 )
 
@@ -10306,16 +6678,16 @@
     },
     total=False,
 )
 
 AwsEc2VpcDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcDetailsOutputTypeDef",
     {
-        "CidrBlockAssociationSet": List[CidrBlockAssociationOutputTypeDef],
-        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationOutputTypeDef],
+        "CidrBlockAssociationSet": List[CidrBlockAssociationTypeDef],
+        "Ipv6CidrBlockAssociationSet": List[Ipv6CidrBlockAssociationTypeDef],
         "DhcpOptionsId": str,
         "State": str,
     },
     total=False,
 )
 
 AwsEc2VpcDetailsTypeDef = TypedDict(
@@ -10338,15 +6710,15 @@
         "ManagesVpcEndpoints": bool,
         "GatewayLoadBalancerArns": List[str],
         "NetworkLoadBalancerArns": List[str],
         "PrivateDnsName": str,
         "ServiceId": str,
         "ServiceName": str,
         "ServiceState": str,
-        "ServiceType": List[AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef],
+        "ServiceType": List[AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef],
     },
     total=False,
 )
 
 AwsEc2VpcEndpointServiceDetailsTypeDef = TypedDict(
     "AwsEc2VpcEndpointServiceDetailsTypeDef",
     {
@@ -10365,18 +6737,18 @@
     total=False,
 )
 
 AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef",
     {
         "CidrBlock": str,
-        "CidrBlockSet": List[VpcInfoCidrBlockSetDetailsOutputTypeDef],
-        "Ipv6CidrBlockSet": List[VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef],
+        "CidrBlockSet": List[VpcInfoCidrBlockSetDetailsTypeDef],
+        "Ipv6CidrBlockSet": List[VpcInfoIpv6CidrBlockSetDetailsTypeDef],
         "OwnerId": str,
-        "PeeringOptions": VpcInfoPeeringOptionsDetailsOutputTypeDef,
+        "PeeringOptions": VpcInfoPeeringOptionsDetailsTypeDef,
         "Region": str,
         "VpcId": str,
     },
     total=False,
 )
 
 AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef = TypedDict(
@@ -10407,52 +6779,27 @@
     {
         "StaticRoutesOnly": bool,
         "TunnelOptions": Sequence[AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef],
     },
     total=False,
 )
 
-AwsEcrRepositoryDetailsOutputTypeDef = TypedDict(
-    "AwsEcrRepositoryDetailsOutputTypeDef",
-    {
-        "Arn": str,
-        "ImageScanningConfiguration": (
-            AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef
-        ),
-        "ImageTagMutability": str,
-        "LifecyclePolicy": AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef,
-        "RepositoryName": str,
-        "RepositoryPolicyText": str,
-    },
-    total=False,
-)
-
 AwsEcrRepositoryDetailsTypeDef = TypedDict(
     "AwsEcrRepositoryDetailsTypeDef",
     {
         "Arn": str,
         "ImageScanningConfiguration": AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
         "ImageTagMutability": str,
         "LifecyclePolicy": AwsEcrRepositoryLifecyclePolicyDetailsTypeDef,
         "RepositoryName": str,
         "RepositoryPolicyText": str,
     },
     total=False,
 )
 
-AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef",
-    {
-        "KmsKeyId": str,
-        "LogConfiguration": AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef,
-        "Logging": str,
-    },
-    total=False,
-)
-
 AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef",
     {
         "KmsKeyId": str,
         "LogConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef
         ),
@@ -10462,15 +6809,15 @@
 )
 
 AwsEcsContainerDetailsOutputTypeDef = TypedDict(
     "AwsEcsContainerDetailsOutputTypeDef",
     {
         "Name": str,
         "Image": str,
-        "MountPoints": List[AwsMountPointOutputTypeDef],
+        "MountPoints": List[AwsMountPointTypeDef],
         "Privileged": bool,
     },
     total=False,
 )
 
 AwsEcsContainerDetailsTypeDef = TypedDict(
     "AwsEcsContainerDetailsTypeDef",
@@ -10479,26 +6826,14 @@
         "Image": str,
         "MountPoints": Sequence[AwsMountPointTypeDef],
         "Privileged": bool,
     },
     total=False,
 )
 
-AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef",
-    {
-        "DeploymentCircuitBreaker": (
-            AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef
-        ),
-        "MaximumPercent": int,
-        "MinimumHealthyPercent": int,
-    },
-    total=False,
-)
-
 AwsEcsServiceDeploymentConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsServiceDeploymentConfigurationDetailsTypeDef",
     {
         "DeploymentCircuitBreaker": (
             AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef
         ),
         "MaximumPercent": int,
@@ -10567,15 +6902,15 @@
 
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef",
     {
         "LogDriver": str,
         "Options": Dict[str, str],
         "SecretOptions": List[
-            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef
         ],
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef",
@@ -10590,15 +6925,15 @@
 )
 
 AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef",
     {
         "ContainerName": str,
         "ProxyConfigurationProperties": List[
-            AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef
+            AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef
         ],
         "Type": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef = TypedDict(
@@ -10609,69 +6944,37 @@
             AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef
         ],
         "Type": str,
     },
     total=False,
 )
 
-AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef",
-    {
-        "AuthorizationConfig": (
-            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef
-        ),
-        "FilesystemId": str,
-        "RootDirectory": str,
-        "TransitEncryption": str,
-        "TransitEncryptionPort": int,
-    },
-    total=False,
-)
-
 AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef",
     {
         "AuthorizationConfig": (
             AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef
         ),
         "FilesystemId": str,
         "RootDirectory": str,
         "TransitEncryption": str,
         "TransitEncryptionPort": int,
     },
     total=False,
 )
 
-AwsEcsTaskVolumeDetailsOutputTypeDef = TypedDict(
-    "AwsEcsTaskVolumeDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Host": AwsEcsTaskVolumeHostDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsEcsTaskVolumeDetailsTypeDef = TypedDict(
     "AwsEcsTaskVolumeDetailsTypeDef",
     {
         "Name": str,
         "Host": AwsEcsTaskVolumeHostDetailsTypeDef,
     },
     total=False,
 )
 
-AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef = TypedDict(
-    "AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef",
-    {
-        "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef,
-        "Path": str,
-    },
-    total=False,
-)
-
 AwsEfsAccessPointRootDirectoryDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointRootDirectoryDetailsTypeDef",
     {
         "CreationInfo": AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
         "Path": str,
     },
     total=False,
@@ -10700,21 +7003,21 @@
         "Cname": str,
         "DateCreated": str,
         "DateUpdated": str,
         "Description": str,
         "EndpointUrl": str,
         "EnvironmentArn": str,
         "EnvironmentId": str,
-        "EnvironmentLinks": List[AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef],
+        "EnvironmentLinks": List[AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef],
         "EnvironmentName": str,
-        "OptionSettings": List[AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef],
+        "OptionSettings": List[AwsElasticBeanstalkEnvironmentOptionSettingTypeDef],
         "PlatformArn": str,
         "SolutionStackName": str,
         "Status": str,
-        "Tier": AwsElasticBeanstalkEnvironmentTierOutputTypeDef,
+        "Tier": AwsElasticBeanstalkEnvironmentTierTypeDef,
         "VersionLabel": str,
     },
     total=False,
 )
 
 AwsElasticBeanstalkEnvironmentDetailsTypeDef = TypedDict(
     "AwsElasticBeanstalkEnvironmentDetailsTypeDef",
@@ -10735,30 +7038,14 @@
         "Status": str,
         "Tier": AwsElasticBeanstalkEnvironmentTierTypeDef,
         "VersionLabel": str,
     },
     total=False,
 )
 
-AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef",
-    {
-        "DedicatedMasterCount": int,
-        "DedicatedMasterEnabled": bool,
-        "DedicatedMasterType": str,
-        "InstanceCount": int,
-        "InstanceType": str,
-        "ZoneAwarenessConfig": (
-            AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef
-        ),
-        "ZoneAwarenessEnabled": bool,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef",
     {
         "DedicatedMasterCount": int,
         "DedicatedMasterEnabled": bool,
         "DedicatedMasterType": str,
         "InstanceCount": int,
@@ -10767,39 +7054,29 @@
             AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef
         ),
         "ZoneAwarenessEnabled": bool,
     },
     total=False,
 )
 
-AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef = TypedDict(
-    "AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef",
-    {
-        "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
-        "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
-        "AuditLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsElasticsearchDomainLogPublishingOptionsTypeDef = TypedDict(
     "AwsElasticsearchDomainLogPublishingOptionsTypeDef",
     {
         "IndexSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "SearchSlowLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
         "AuditLogs": AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
     },
     total=False,
 )
 
 AwsElbLoadBalancerPoliciesOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesOutputTypeDef",
     {
-        "AppCookieStickinessPolicies": List[AwsElbAppCookieStickinessPolicyOutputTypeDef],
-        "LbCookieStickinessPolicies": List[AwsElbLbCookieStickinessPolicyOutputTypeDef],
+        "AppCookieStickinessPolicies": List[AwsElbAppCookieStickinessPolicyTypeDef],
+        "LbCookieStickinessPolicies": List[AwsElbLbCookieStickinessPolicyTypeDef],
         "OtherPolicies": List[str],
     },
     total=False,
 )
 
 AwsElbLoadBalancerPoliciesTypeDef = TypedDict(
     "AwsElbLoadBalancerPoliciesTypeDef",
@@ -10810,19 +7087,19 @@
     },
     total=False,
 )
 
 AwsElbLoadBalancerAttributesOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerAttributesOutputTypeDef",
     {
-        "AccessLog": AwsElbLoadBalancerAccessLogOutputTypeDef,
-        "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingOutputTypeDef,
-        "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsOutputTypeDef,
-        "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef,
-        "AdditionalAttributes": List[AwsElbLoadBalancerAdditionalAttributeOutputTypeDef],
+        "AccessLog": AwsElbLoadBalancerAccessLogTypeDef,
+        "ConnectionDraining": AwsElbLoadBalancerConnectionDrainingTypeDef,
+        "ConnectionSettings": AwsElbLoadBalancerConnectionSettingsTypeDef,
+        "CrossZoneLoadBalancing": AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
+        "AdditionalAttributes": List[AwsElbLoadBalancerAdditionalAttributeTypeDef],
     },
     total=False,
 )
 
 AwsElbLoadBalancerAttributesTypeDef = TypedDict(
     "AwsElbLoadBalancerAttributesTypeDef",
     {
@@ -10834,15 +7111,15 @@
     },
     total=False,
 )
 
 AwsElbLoadBalancerListenerDescriptionOutputTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionOutputTypeDef",
     {
-        "Listener": AwsElbLoadBalancerListenerOutputTypeDef,
+        "Listener": AwsElbLoadBalancerListenerTypeDef,
         "PolicyNames": List[str],
     },
     total=False,
 )
 
 AwsElbLoadBalancerListenerDescriptionTypeDef = TypedDict(
     "AwsElbLoadBalancerListenerDescriptionTypeDef",
@@ -10852,25 +7129,25 @@
     },
     total=False,
 )
 
 AwsElbv2LoadBalancerDetailsOutputTypeDef = TypedDict(
     "AwsElbv2LoadBalancerDetailsOutputTypeDef",
     {
-        "AvailabilityZones": List[AvailabilityZoneOutputTypeDef],
+        "AvailabilityZones": List[AvailabilityZoneTypeDef],
         "CanonicalHostedZoneId": str,
         "CreatedTime": str,
         "DNSName": str,
         "IpAddressType": str,
         "Scheme": str,
         "SecurityGroups": List[str],
-        "State": LoadBalancerStateOutputTypeDef,
+        "State": LoadBalancerStateTypeDef,
         "Type": str,
         "VpcId": str,
-        "LoadBalancerAttributes": List[AwsElbv2LoadBalancerAttributeOutputTypeDef],
+        "LoadBalancerAttributes": List[AwsElbv2LoadBalancerAttributeTypeDef],
     },
     total=False,
 )
 
 AwsElbv2LoadBalancerDetailsTypeDef = TypedDict(
     "AwsElbv2LoadBalancerDetailsTypeDef",
     {
@@ -10885,72 +7162,47 @@
         "Type": str,
         "VpcId": str,
         "LoadBalancerAttributes": Sequence[AwsElbv2LoadBalancerAttributeTypeDef],
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef",
-    {
-        "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef",
     {
         "AuditLogs": AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef",
-    {
-        "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef",
     {
         "EbsVolumes": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
     },
     total=False,
 )
 
-AwsIamAccessKeySessionContextOutputTypeDef = TypedDict(
-    "AwsIamAccessKeySessionContextOutputTypeDef",
-    {
-        "Attributes": AwsIamAccessKeySessionContextAttributesOutputTypeDef,
-        "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsIamAccessKeySessionContextTypeDef = TypedDict(
     "AwsIamAccessKeySessionContextTypeDef",
     {
         "Attributes": AwsIamAccessKeySessionContextAttributesTypeDef,
         "SessionIssuer": AwsIamAccessKeySessionContextSessionIssuerTypeDef,
     },
     total=False,
 )
 
 AwsIamGroupDetailsOutputTypeDef = TypedDict(
     "AwsIamGroupDetailsOutputTypeDef",
     {
-        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyOutputTypeDef],
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "GroupId": str,
         "GroupName": str,
-        "GroupPolicyList": List[AwsIamGroupPolicyOutputTypeDef],
+        "GroupPolicyList": List[AwsIamGroupPolicyTypeDef],
         "Path": str,
     },
     total=False,
 )
 
 AwsIamGroupDetailsTypeDef = TypedDict(
     "AwsIamGroupDetailsTypeDef",
@@ -10969,15 +7221,15 @@
     "AwsIamInstanceProfileOutputTypeDef",
     {
         "Arn": str,
         "CreateDate": str,
         "InstanceProfileId": str,
         "InstanceProfileName": str,
         "Path": str,
-        "Roles": List[AwsIamInstanceProfileRoleOutputTypeDef],
+        "Roles": List[AwsIamInstanceProfileRoleTypeDef],
     },
     total=False,
 )
 
 AwsIamInstanceProfileTypeDef = TypedDict(
     "AwsIamInstanceProfileTypeDef",
     {
@@ -10999,15 +7251,15 @@
         "DefaultVersionId": str,
         "Description": str,
         "IsAttachable": bool,
         "Path": str,
         "PermissionsBoundaryUsageCount": int,
         "PolicyId": str,
         "PolicyName": str,
-        "PolicyVersionList": List[AwsIamPolicyVersionOutputTypeDef],
+        "PolicyVersionList": List[AwsIamPolicyVersionTypeDef],
         "UpdateDate": str,
     },
     total=False,
 )
 
 AwsIamPolicyDetailsTypeDef = TypedDict(
     "AwsIamPolicyDetailsTypeDef",
@@ -11026,22 +7278,22 @@
     },
     total=False,
 )
 
 AwsIamUserDetailsOutputTypeDef = TypedDict(
     "AwsIamUserDetailsOutputTypeDef",
     {
-        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyOutputTypeDef],
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "GroupList": List[str],
         "Path": str,
-        "PermissionsBoundary": AwsIamPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AwsIamPermissionsBoundaryTypeDef,
         "UserId": str,
         "UserName": str,
-        "UserPolicyList": List[AwsIamUserPolicyOutputTypeDef],
+        "UserPolicyList": List[AwsIamUserPolicyTypeDef],
     },
     total=False,
 )
 
 AwsIamUserDetailsTypeDef = TypedDict(
     "AwsIamUserDetailsTypeDef",
     {
@@ -11053,26 +7305,14 @@
         "UserId": str,
         "UserName": str,
         "UserPolicyList": Sequence[AwsIamUserPolicyTypeDef],
     },
     total=False,
 )
 
-AwsKinesisStreamDetailsOutputTypeDef = TypedDict(
-    "AwsKinesisStreamDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Arn": str,
-        "StreamEncryption": AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef,
-        "ShardCount": int,
-        "RetentionPeriodHours": int,
-    },
-    total=False,
-)
-
 AwsKinesisStreamDetailsTypeDef = TypedDict(
     "AwsKinesisStreamDetailsTypeDef",
     {
         "Name": str,
         "Arn": str,
         "StreamEncryption": AwsKinesisStreamStreamEncryptionDetailsTypeDef,
         "ShardCount": int,
@@ -11081,15 +7321,15 @@
     total=False,
 )
 
 AwsLambdaFunctionEnvironmentOutputTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentOutputTypeDef",
     {
         "Variables": Dict[str, str],
-        "Error": AwsLambdaFunctionEnvironmentErrorOutputTypeDef,
+        "Error": AwsLambdaFunctionEnvironmentErrorTypeDef,
     },
     total=False,
 )
 
 AwsLambdaFunctionEnvironmentTypeDef = TypedDict(
     "AwsLambdaFunctionEnvironmentTypeDef",
     {
@@ -11106,15 +7346,15 @@
         "Description": str,
         "FirewallArn": str,
         "FirewallId": str,
         "FirewallName": str,
         "FirewallPolicyArn": str,
         "FirewallPolicyChangeProtection": bool,
         "SubnetChangeProtection": bool,
-        "SubnetMappings": List[AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef],
+        "SubnetMappings": List[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
 AwsNetworkFirewallFirewallDetailsTypeDef = TypedDict(
     "AwsNetworkFirewallFirewallDetailsTypeDef",
@@ -11129,53 +7369,24 @@
         "SubnetChangeProtection": bool,
         "SubnetMappings": Sequence[AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef",
-    {
-        "Enabled": bool,
-        "InternalUserDatabaseEnabled": bool,
-        "MasterUserOptions": AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef",
     {
         "Enabled": bool,
         "InternalUserDatabaseEnabled": bool,
         "MasterUserOptions": AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef",
-    {
-        "InstanceCount": int,
-        "WarmEnabled": bool,
-        "WarmCount": int,
-        "DedicatedMasterEnabled": bool,
-        "ZoneAwarenessConfig": (
-            AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef
-        ),
-        "DedicatedMasterCount": int,
-        "InstanceType": str,
-        "WarmType": str,
-        "ZoneAwarenessEnabled": bool,
-        "DedicatedMasterType": str,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef",
     {
         "InstanceCount": int,
         "WarmEnabled": bool,
         "WarmCount": int,
         "DedicatedMasterEnabled": bool,
@@ -11187,24 +7398,14 @@
         "WarmType": str,
         "ZoneAwarenessEnabled": bool,
         "DedicatedMasterType": str,
     },
     total=False,
 )
 
-AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef = TypedDict(
-    "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef",
-    {
-        "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
-        "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
-        "AuditLogs": AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef",
     {
         "IndexSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "SearchSlowLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
         "AuditLogs": AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
     },
@@ -11226,34 +7427,34 @@
         "Engine": str,
         "EngineVersion": str,
         "Port": int,
         "MasterUsername": str,
         "PreferredBackupWindow": str,
         "PreferredMaintenanceWindow": str,
         "ReadReplicaIdentifiers": List[str],
-        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef],
+        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupTypeDef],
         "HostedZoneId": str,
         "StorageEncrypted": bool,
         "KmsKeyId": str,
         "DbClusterResourceId": str,
-        "AssociatedRoles": List[AwsRdsDbClusterAssociatedRoleOutputTypeDef],
+        "AssociatedRoles": List[AwsRdsDbClusterAssociatedRoleTypeDef],
         "ClusterCreateTime": str,
         "EnabledCloudWatchLogsExports": List[str],
         "EngineMode": str,
         "DeletionProtection": bool,
         "HttpEndpointEnabled": bool,
         "ActivityStreamStatus": str,
         "CopyTagsToSnapshot": bool,
         "CrossAccountClone": bool,
-        "DomainMemberships": List[AwsRdsDbDomainMembershipOutputTypeDef],
+        "DomainMemberships": List[AwsRdsDbDomainMembershipTypeDef],
         "DbClusterParameterGroup": str,
         "DbSubnetGroup": str,
-        "DbClusterOptionGroupMemberships": List[AwsRdsDbClusterOptionGroupMembershipOutputTypeDef],
+        "DbClusterOptionGroupMemberships": List[AwsRdsDbClusterOptionGroupMembershipTypeDef],
         "DbClusterIdentifier": str,
-        "DbClusterMembers": List[AwsRdsDbClusterMemberOutputTypeDef],
+        "DbClusterMembers": List[AwsRdsDbClusterMemberTypeDef],
         "IamDatabaseAuthenticationEnabled": bool,
     },
     total=False,
 )
 
 AwsRdsDbClusterDetailsTypeDef = TypedDict(
     "AwsRdsDbClusterDetailsTypeDef",
@@ -11379,15 +7580,15 @@
         "SourceDbSnapshotIdentifier": str,
         "StorageType": str,
         "TdeCredentialArn": str,
         "Encrypted": bool,
         "KmsKeyId": str,
         "Timezone": str,
         "IamDatabaseAuthenticationEnabled": bool,
-        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
         "DbiResourceId": str,
     },
     total=False,
 )
 
 AwsRdsDbSnapshotDetailsTypeDef = TypedDict(
     "AwsRdsDbSnapshotDetailsTypeDef",
@@ -11436,15 +7637,15 @@
         "LicenseModel": str,
         "Iops": int,
         "DbInstanceIdentifier": str,
         "StorageType": str,
         "CaCertificateIdentifier": str,
         "DbSubnetGroupName": str,
         "PendingCloudWatchLogsExports": AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
-        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
     },
     total=False,
 )
 
 AwsRdsDbPendingModifiedValuesTypeDef = TypedDict(
     "AwsRdsDbPendingModifiedValuesTypeDef",
     {
@@ -11469,16 +7670,16 @@
 
 AwsRdsDbSecurityGroupDetailsOutputTypeDef = TypedDict(
     "AwsRdsDbSecurityGroupDetailsOutputTypeDef",
     {
         "DbSecurityGroupArn": str,
         "DbSecurityGroupDescription": str,
         "DbSecurityGroupName": str,
-        "Ec2SecurityGroups": List[AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef],
-        "IpRanges": List[AwsRdsDbSecurityGroupIpRangeOutputTypeDef],
+        "Ec2SecurityGroups": List[AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef],
+        "IpRanges": List[AwsRdsDbSecurityGroupIpRangeTypeDef],
         "OwnerId": str,
         "VpcId": str,
     },
     total=False,
 )
 
 AwsRdsDbSecurityGroupDetailsTypeDef = TypedDict(
@@ -11491,38 +7692,28 @@
         "IpRanges": Sequence[AwsRdsDbSecurityGroupIpRangeTypeDef],
         "OwnerId": str,
         "VpcId": str,
     },
     total=False,
 )
 
-AwsRdsDbSubnetGroupSubnetOutputTypeDef = TypedDict(
-    "AwsRdsDbSubnetGroupSubnetOutputTypeDef",
-    {
-        "SubnetIdentifier": str,
-        "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef,
-        "SubnetStatus": str,
-    },
-    total=False,
-)
-
 AwsRdsDbSubnetGroupSubnetTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupSubnetTypeDef",
     {
         "SubnetIdentifier": str,
         "SubnetAvailabilityZone": AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
         "SubnetStatus": str,
     },
     total=False,
 )
 
 AwsRedshiftClusterClusterParameterGroupOutputTypeDef = TypedDict(
     "AwsRedshiftClusterClusterParameterGroupOutputTypeDef",
     {
-        "ClusterParameterStatusList": List[AwsRedshiftClusterClusterParameterStatusOutputTypeDef],
+        "ClusterParameterStatusList": List[AwsRedshiftClusterClusterParameterStatusTypeDef],
         "ParameterApplyStatus": str,
         "ParameterGroupName": str,
     },
     total=False,
 )
 
 AwsRedshiftClusterClusterParameterGroupTypeDef = TypedDict(
@@ -11531,93 +7722,56 @@
         "ClusterParameterStatusList": Sequence[AwsRedshiftClusterClusterParameterStatusTypeDef],
         "ParameterApplyStatus": str,
         "ParameterGroupName": str,
     },
     total=False,
 )
 
-AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef",
-    {
-        "Prefix": str,
-        "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef",
     {
         "Prefix": str,
         "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef",
     {
-        "FilterRules": List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef],
+        "FilterRules": List[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
     total=False,
 )
 
 AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef = TypedDict(
     "AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef",
     {
         "FilterRules": Sequence[AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef],
     },
     total=False,
 )
 
-AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef = TypedDict(
-    "AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef",
-    {
-        "DefaultRetention": (
-            AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
 AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef",
     {
         "DefaultRetention": AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
     },
     total=False,
 )
 
-AwsS3BucketServerSideEncryptionRuleOutputTypeDef = TypedDict(
-    "AwsS3BucketServerSideEncryptionRuleOutputTypeDef",
-    {
-        "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsS3BucketServerSideEncryptionRuleTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionRuleTypeDef",
     {
         "ApplyServerSideEncryptionByDefault": AwsS3BucketServerSideEncryptionByDefaultTypeDef,
     },
     total=False,
 )
 
-AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef = TypedDict(
-    "AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef",
-    {
-        "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef,
-        "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef",
     {
         "Condition": AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
         "Redirect": AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
     },
     total=False,
@@ -11628,15 +7782,15 @@
     {
         "AcceleratorTypes": List[str],
         "AdditionalCodeRepositories": List[str],
         "DefaultCodeRepository": str,
         "DirectInternetAccess": str,
         "FailureReason": str,
         "InstanceMetadataServiceConfiguration": (
-            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef
+            AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef
         ),
         "InstanceType": str,
         "KmsKeyId": str,
         "NetworkInterfaceId": str,
         "NotebookInstanceArn": str,
         "NotebookInstanceLifecycleConfigName": str,
         "NotebookInstanceName": str,
@@ -11677,29 +7831,14 @@
         "SubnetId": str,
         "Url": str,
         "VolumeSizeInGB": int,
     },
     total=False,
 )
 
-AwsSecretsManagerSecretDetailsOutputTypeDef = TypedDict(
-    "AwsSecretsManagerSecretDetailsOutputTypeDef",
-    {
-        "RotationRules": AwsSecretsManagerSecretRotationRulesOutputTypeDef,
-        "RotationOccurredWithinFrequency": bool,
-        "KmsKeyId": str,
-        "RotationEnabled": bool,
-        "RotationLambdaArn": str,
-        "Deleted": bool,
-        "Name": str,
-        "Description": str,
-    },
-    total=False,
-)
-
 AwsSecretsManagerSecretDetailsTypeDef = TypedDict(
     "AwsSecretsManagerSecretDetailsTypeDef",
     {
         "RotationRules": AwsSecretsManagerSecretRotationRulesTypeDef,
         "RotationOccurredWithinFrequency": bool,
         "KmsKeyId": str,
         "RotationEnabled": bool,
@@ -11707,23 +7846,14 @@
         "Deleted": bool,
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-BatchUpdateFindingsUnprocessedFindingTypeDef = TypedDict(
-    "BatchUpdateFindingsUnprocessedFindingTypeDef",
-    {
-        "FindingIdentifier": AwsSecurityFindingIdentifierOutputTypeDef,
-        "ErrorCode": str,
-        "ErrorMessage": str,
-    },
-)
-
 _RequiredBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchUpdateFindingsRequestRequestTypeDef",
     {
         "FindingIdentifiers": Sequence[AwsSecurityFindingIdentifierTypeDef],
     },
 )
 _OptionalBatchUpdateFindingsRequestRequestTypeDef = TypedDict(
@@ -11744,14 +7874,23 @@
 
 class BatchUpdateFindingsRequestRequestTypeDef(
     _RequiredBatchUpdateFindingsRequestRequestTypeDef,
     _OptionalBatchUpdateFindingsRequestRequestTypeDef,
 ):
     pass
 
+BatchUpdateFindingsUnprocessedFindingTypeDef = TypedDict(
+    "BatchUpdateFindingsUnprocessedFindingTypeDef",
+    {
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
+        "ErrorCode": str,
+        "ErrorMessage": str,
+    },
+)
+
 _RequiredGetFindingHistoryRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingHistoryRequestRequestTypeDef",
     {
         "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
     },
 )
 _OptionalGetFindingHistoryRequestRequestTypeDef = TypedDict(
@@ -11770,15 +7909,15 @@
 ):
     pass
 
 AwsSnsTopicDetailsOutputTypeDef = TypedDict(
     "AwsSnsTopicDetailsOutputTypeDef",
     {
         "KmsMasterKeyId": str,
-        "Subscription": List[AwsSnsTopicSubscriptionOutputTypeDef],
+        "Subscription": List[AwsSnsTopicSubscriptionTypeDef],
         "TopicName": str,
         "Owner": str,
         "SqsSuccessFeedbackRoleArn": str,
         "SqsFailureFeedbackRoleArn": str,
         "ApplicationSuccessFeedbackRoleArn": str,
         "FirehoseSuccessFeedbackRoleArn": str,
         "FirehoseFailureFeedbackRoleArn": str,
@@ -11802,38 +7941,22 @@
         "FirehoseFailureFeedbackRoleArn": str,
         "HttpSuccessFeedbackRoleArn": str,
         "HttpFailureFeedbackRoleArn": str,
     },
     total=False,
 )
 
-AwsSsmPatchOutputTypeDef = TypedDict(
-    "AwsSsmPatchOutputTypeDef",
-    {
-        "ComplianceSummary": AwsSsmComplianceSummaryOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsSsmPatchTypeDef = TypedDict(
     "AwsSsmPatchTypeDef",
     {
         "ComplianceSummary": AwsSsmComplianceSummaryTypeDef,
     },
     total=False,
 )
 
-AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef = TypedDict(
-    "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef",
-    {
-        "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef",
     {
         "CloudWatchLogsLogGroup": AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
     },
     total=False,
 )
@@ -11842,15 +7965,15 @@
     "AwsWafRateBasedRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
-        "MatchPredicates": List[AwsWafRateBasedRuleMatchPredicateOutputTypeDef],
+        "MatchPredicates": List[AwsWafRateBasedRuleMatchPredicateTypeDef],
     },
     total=False,
 )
 
 AwsWafRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRateBasedRuleDetailsTypeDef",
     {
@@ -11868,15 +7991,15 @@
     "AwsWafRegionalRateBasedRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RateKey": str,
         "RateLimit": int,
         "RuleId": str,
-        "MatchPredicates": List[AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef],
+        "MatchPredicates": List[AwsWafRegionalRateBasedRuleMatchPredicateTypeDef],
     },
     total=False,
 )
 
 AwsWafRegionalRateBasedRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRateBasedRuleDetailsTypeDef",
     {
@@ -11891,15 +8014,15 @@
 )
 
 AwsWafRegionalRuleDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
-        "PredicateList": List[AwsWafRegionalRulePredicateListDetailsOutputTypeDef],
+        "PredicateList": List[AwsWafRegionalRulePredicateListDetailsTypeDef],
         "RuleId": str,
     },
     total=False,
 )
 
 AwsWafRegionalRuleDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleDetailsTypeDef",
@@ -11908,48 +8031,25 @@
         "Name": str,
         "PredicateList": Sequence[AwsWafRegionalRulePredicateListDetailsTypeDef],
         "RuleId": str,
     },
     total=False,
 )
 
-AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef",
-    {
-        "Action": AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef,
-        "Priority": int,
-        "RuleId": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalRuleGroupRulesDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupRulesDetailsTypeDef",
     {
         "Action": AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
-AwsWafRegionalWebAclRulesListDetailsOutputTypeDef = TypedDict(
-    "AwsWafRegionalWebAclRulesListDetailsOutputTypeDef",
-    {
-        "Action": AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef,
-        "OverrideAction": AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef,
-        "Priority": int,
-        "RuleId": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRegionalWebAclRulesListDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclRulesListDetailsTypeDef",
     {
         "Action": AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
         "OverrideAction": AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
         "Priority": int,
         "RuleId": str,
@@ -11959,15 +8059,15 @@
 )
 
 AwsWafRuleDetailsOutputTypeDef = TypedDict(
     "AwsWafRuleDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
-        "PredicateList": List[AwsWafRulePredicateListDetailsOutputTypeDef],
+        "PredicateList": List[AwsWafRulePredicateListDetailsTypeDef],
         "RuleId": str,
     },
     total=False,
 )
 
 AwsWafRuleDetailsTypeDef = TypedDict(
     "AwsWafRuleDetailsTypeDef",
@@ -11976,42 +8076,31 @@
         "Name": str,
         "PredicateList": Sequence[AwsWafRulePredicateListDetailsTypeDef],
         "RuleId": str,
     },
     total=False,
 )
 
-AwsWafRuleGroupRulesDetailsOutputTypeDef = TypedDict(
-    "AwsWafRuleGroupRulesDetailsOutputTypeDef",
-    {
-        "Action": AwsWafRuleGroupRulesActionDetailsOutputTypeDef,
-        "Priority": int,
-        "RuleId": str,
-        "Type": str,
-    },
-    total=False,
-)
-
 AwsWafRuleGroupRulesDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupRulesDetailsTypeDef",
     {
         "Action": AwsWafRuleGroupRulesActionDetailsTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
 AwsWafWebAclRuleOutputTypeDef = TypedDict(
     "AwsWafWebAclRuleOutputTypeDef",
     {
-        "Action": WafActionOutputTypeDef,
-        "ExcludedRules": List[WafExcludedRuleOutputTypeDef],
-        "OverrideAction": WafOverrideActionOutputTypeDef,
+        "Action": WafActionTypeDef,
+        "ExcludedRules": List[WafExcludedRuleTypeDef],
+        "OverrideAction": WafOverrideActionTypeDef,
         "Priority": int,
         "RuleId": str,
         "Type": str,
     },
     total=False,
 )
 
@@ -12027,51 +8116,43 @@
     },
     total=False,
 )
 
 AwsWafv2CustomRequestHandlingDetailsOutputTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsOutputTypeDef",
     {
-        "InsertHeaders": List[AwsWafv2CustomHttpHeaderOutputTypeDef],
-    },
-    total=False,
-)
-
-AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2CustomResponseDetailsOutputTypeDef",
-    {
-        "CustomResponseBodyKey": str,
-        "ResponseCode": int,
-        "ResponseHeaders": List[AwsWafv2CustomHttpHeaderOutputTypeDef],
+        "InsertHeaders": List[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
 AwsWafv2CustomRequestHandlingDetailsTypeDef = TypedDict(
     "AwsWafv2CustomRequestHandlingDetailsTypeDef",
     {
         "InsertHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
-AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
-    "AwsWafv2CustomResponseDetailsTypeDef",
+AwsWafv2CustomResponseDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsOutputTypeDef",
     {
         "CustomResponseBodyKey": str,
         "ResponseCode": int,
-        "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
+        "ResponseHeaders": List[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
-AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef",
+AwsWafv2CustomResponseDetailsTypeDef = TypedDict(
+    "AwsWafv2CustomResponseDetailsTypeDef",
     {
-        "ImmunityTimeProperty": AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef,
+        "CustomResponseBodyKey": str,
+        "ResponseCode": int,
+        "ResponseHeaders": Sequence[AwsWafv2CustomHttpHeaderTypeDef],
     },
     total=False,
 )
 
 AwsWafv2WebAclCaptchaConfigDetailsTypeDef = TypedDict(
     "AwsWafv2WebAclCaptchaConfigDetailsTypeDef",
     {
@@ -12271,14 +8352,35 @@
 BatchGetStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchGetStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationIds": Sequence[StandardsControlAssociationIdTypeDef],
     },
 )
 
+_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
+    {
+        "StandardsControlAssociationId": StandardsControlAssociationIdTypeDef,
+        "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
+    {
+        "ErrorReason": str,
+    },
+    total=False,
+)
+
+class UnprocessedStandardsControlAssociationTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationTypeDef,
+):
+    pass
+
 BatchImportFindingsResponseTypeDef = TypedDict(
     "BatchImportFindingsResponseTypeDef",
     {
         "FailedCount": int,
         "SuccessCount": int,
         "FailedFindings": List[ImportFindingsErrorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -12288,22 +8390,43 @@
 BatchUpdateStandardsControlAssociationsRequestRequestTypeDef = TypedDict(
     "BatchUpdateStandardsControlAssociationsRequestRequestTypeDef",
     {
         "StandardsControlAssociationUpdates": Sequence[StandardsControlAssociationUpdateTypeDef],
     },
 )
 
+_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
+    {
+        "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateTypeDef,
+        "ErrorCode": UnprocessedErrorCodeType,
+    },
+)
+_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
+    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
+    {
+        "ErrorReason": str,
+    },
+    total=False,
+)
+
+class UnprocessedStandardsControlAssociationUpdateTypeDef(
+    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
+    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
+):
+    pass
+
 ComplianceOutputTypeDef = TypedDict(
     "ComplianceOutputTypeDef",
     {
         "Status": ComplianceStatusType,
         "RelatedRequirements": List[str],
-        "StatusReasons": List[StatusReasonOutputTypeDef],
+        "StatusReasons": List[StatusReasonTypeDef],
         "SecurityControlId": str,
-        "AssociatedStandards": List[AssociatedStandardOutputTypeDef],
+        "AssociatedStandards": List[AssociatedStandardTypeDef],
     },
     total=False,
 )
 
 ComplianceTypeDef = TypedDict(
     "ComplianceTypeDef",
     {
@@ -12320,15 +8443,15 @@
     "ContainerDetailsOutputTypeDef",
     {
         "ContainerRuntime": str,
         "Name": str,
         "ImageId": str,
         "ImageName": str,
         "LaunchedAt": str,
-        "VolumeMounts": List[VolumeMountOutputTypeDef],
+        "VolumeMounts": List[VolumeMountTypeDef],
         "Privileged": bool,
     },
     total=False,
 )
 
 ContainerDetailsTypeDef = TypedDict(
     "ContainerDetailsTypeDef",
@@ -12380,24 +8503,14 @@
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[ResultTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DateFilterOutputTypeDef = TypedDict(
-    "DateFilterOutputTypeDef",
-    {
-        "Start": str,
-        "End": str,
-        "DateRange": DateRangeOutputTypeDef,
-    },
-    total=False,
-)
-
 DateFilterTypeDef = TypedDict(
     "DateFilterTypeDef",
     {
         "Start": str,
         "End": str,
         "DateRange": DateRangeTypeDef,
     },
@@ -12580,15 +8693,15 @@
 
 ThreatOutputTypeDef = TypedDict(
     "ThreatOutputTypeDef",
     {
         "Name": str,
         "Severity": str,
         "ItemCount": int,
-        "FilePaths": List[FilePathsOutputTypeDef],
+        "FilePaths": List[FilePathsTypeDef],
     },
     total=False,
 )
 
 ThreatTypeDef = TypedDict(
     "ThreatTypeDef",
     {
@@ -12608,31 +8721,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FindingHistoryRecordTypeDef = TypedDict(
     "FindingHistoryRecordTypeDef",
     {
-        "FindingIdentifier": AwsSecurityFindingIdentifierOutputTypeDef,
+        "FindingIdentifier": AwsSecurityFindingIdentifierTypeDef,
         "UpdateTime": datetime,
         "FindingCreated": bool,
         "UpdateSource": FindingHistoryUpdateSourceTypeDef,
         "Updates": List[FindingHistoryUpdateTypeDef],
         "NextToken": str,
     },
     total=False,
 )
 
 FindingProviderFieldsOutputTypeDef = TypedDict(
     "FindingProviderFieldsOutputTypeDef",
     {
         "Confidence": int,
         "Criticality": int,
-        "RelatedFindings": List[RelatedFindingOutputTypeDef],
-        "Severity": FindingProviderSeverityOutputTypeDef,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+        "Severity": FindingProviderSeverityTypeDef,
         "Types": List[str],
     },
     total=False,
 )
 
 FindingProviderFieldsTypeDef = TypedDict(
     "FindingProviderFieldsTypeDef",
@@ -12712,38 +8825,19 @@
     {
         "StandardsControlAssociationSummaries": List[StandardsControlAssociationSummaryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-NetworkOutputTypeDef = TypedDict(
-    "NetworkOutputTypeDef",
-    {
-        "Direction": NetworkDirectionType,
-        "Protocol": str,
-        "OpenPortRange": PortRangeOutputTypeDef,
-        "SourceIpV4": str,
-        "SourceIpV6": str,
-        "SourcePort": int,
-        "SourceDomain": str,
-        "SourceMac": str,
-        "DestinationIpV4": str,
-        "DestinationIpV6": str,
-        "DestinationPort": int,
-        "DestinationDomain": str,
-    },
-    total=False,
-)
-
 NetworkPathComponentDetailsOutputTypeDef = TypedDict(
     "NetworkPathComponentDetailsOutputTypeDef",
     {
         "Address": List[str],
-        "PortRanges": List[PortRangeOutputTypeDef],
+        "PortRanges": List[PortRangeTypeDef],
     },
     total=False,
 )
 
 NetworkPathComponentDetailsTypeDef = TypedDict(
     "NetworkPathComponentDetailsTypeDef",
     {
@@ -12768,55 +8862,37 @@
         "DestinationIpV6": str,
         "DestinationPort": int,
         "DestinationDomain": str,
     },
     total=False,
 )
 
-PageOutputTypeDef = TypedDict(
-    "PageOutputTypeDef",
-    {
-        "PageNumber": int,
-        "LineRange": RangeOutputTypeDef,
-        "OffsetRange": RangeOutputTypeDef,
-    },
-    total=False,
-)
-
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
         "PageNumber": int,
         "LineRange": RangeTypeDef,
         "OffsetRange": RangeTypeDef,
     },
     total=False,
 )
 
-RemediationOutputTypeDef = TypedDict(
-    "RemediationOutputTypeDef",
-    {
-        "Recommendation": RecommendationOutputTypeDef,
-    },
-    total=False,
-)
-
 RemediationTypeDef = TypedDict(
     "RemediationTypeDef",
     {
         "Recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
 RuleGroupSourceStatefulRulesDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsOutputTypeDef",
     {
         "Action": str,
-        "Header": RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef,
+        "Header": RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
         "RuleOptions": List[RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef],
     },
     total=False,
 )
 
 RuleGroupSourceStatefulRulesDetailsTypeDef = TypedDict(
     "RuleGroupSourceStatefulRulesDetailsTypeDef",
@@ -12828,20 +8904,20 @@
     total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef",
     {
         "DestinationPorts": List[
-            RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef
+            RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef
         ],
-        "Destinations": List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef],
+        "Destinations": List[RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef],
         "Protocols": List[int],
-        "SourcePorts": List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef],
-        "Sources": List[RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef],
+        "SourcePorts": List[RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef],
+        "Sources": List[RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef],
         "TcpFlags": List[RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef],
     },
     total=False,
 )
 
 RuleGroupSourceStatelessRuleMatchAttributesTypeDef = TypedDict(
     "RuleGroupSourceStatelessRuleMatchAttributesTypeDef",
@@ -12884,56 +8960,14 @@
         "Description": str,
         "EnabledByDefault": bool,
         "StandardsManagedBy": StandardsManagedByTypeDef,
     },
     total=False,
 )
 
-_RequiredUnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "_RequiredUnprocessedStandardsControlAssociationTypeDef",
-    {
-        "StandardsControlAssociationId": StandardsControlAssociationIdOutputTypeDef,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedStandardsControlAssociationTypeDef = TypedDict(
-    "_OptionalUnprocessedStandardsControlAssociationTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-class UnprocessedStandardsControlAssociationTypeDef(
-    _RequiredUnprocessedStandardsControlAssociationTypeDef,
-    _OptionalUnprocessedStandardsControlAssociationTypeDef,
-):
-    pass
-
-_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_RequiredUnprocessedStandardsControlAssociationUpdateTypeDef",
-    {
-        "StandardsControlAssociationUpdate": StandardsControlAssociationUpdateOutputTypeDef,
-        "ErrorCode": UnprocessedErrorCodeType,
-    },
-)
-_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef = TypedDict(
-    "_OptionalUnprocessedStandardsControlAssociationUpdateTypeDef",
-    {
-        "ErrorReason": str,
-    },
-    total=False,
-)
-
-class UnprocessedStandardsControlAssociationUpdateTypeDef(
-    _RequiredUnprocessedStandardsControlAssociationUpdateTypeDef,
-    _OptionalUnprocessedStandardsControlAssociationUpdateTypeDef,
-):
-    pass
-
 _RequiredStandardsSubscriptionTypeDef = TypedDict(
     "_RequiredStandardsSubscriptionTypeDef",
     {
         "StandardsSubscriptionArn": str,
         "StandardsArn": str,
         "StandardsInput": Dict[str, str],
         "StandardsStatus": StandardsStatusType,
@@ -12951,15 +8985,15 @@
     _RequiredStandardsSubscriptionTypeDef, _OptionalStandardsSubscriptionTypeDef
 ):
     pass
 
 StatelessCustomPublishMetricActionOutputTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionOutputTypeDef",
     {
-        "Dimensions": List[StatelessCustomPublishMetricActionDimensionOutputTypeDef],
+        "Dimensions": List[StatelessCustomPublishMetricActionDimensionTypeDef],
     },
     total=False,
 )
 
 StatelessCustomPublishMetricActionTypeDef = TypedDict(
     "StatelessCustomPublishMetricActionTypeDef",
     {
@@ -12970,46 +9004,23 @@
 
 AwsApiCallActionOutputTypeDef = TypedDict(
     "AwsApiCallActionOutputTypeDef",
     {
         "Api": str,
         "ServiceName": str,
         "CallerType": str,
-        "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
-        "DomainDetails": AwsApiCallActionDomainDetailsOutputTypeDef,
+        "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
+        "DomainDetails": AwsApiCallActionDomainDetailsTypeDef,
         "AffectedResources": Dict[str, str],
         "FirstSeen": str,
         "LastSeen": str,
     },
     total=False,
 )
 
-NetworkConnectionActionOutputTypeDef = TypedDict(
-    "NetworkConnectionActionOutputTypeDef",
-    {
-        "ConnectionDirection": str,
-        "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
-        "RemotePortDetails": ActionRemotePortDetailsOutputTypeDef,
-        "LocalPortDetails": ActionLocalPortDetailsOutputTypeDef,
-        "Protocol": str,
-        "Blocked": bool,
-    },
-    total=False,
-)
-
-PortProbeDetailOutputTypeDef = TypedDict(
-    "PortProbeDetailOutputTypeDef",
-    {
-        "LocalPortDetails": ActionLocalPortDetailsOutputTypeDef,
-        "LocalIpDetails": ActionLocalIpDetailsOutputTypeDef,
-        "RemoteIpDetails": ActionRemoteIpDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsApiCallActionTypeDef = TypedDict(
     "AwsApiCallActionTypeDef",
     {
         "Api": str,
         "ServiceName": str,
         "CallerType": str,
         "RemoteIpDetails": ActionRemoteIpDetailsTypeDef,
@@ -13049,18 +9060,18 @@
     {
         "Id": str,
     },
 )
 _OptionalVulnerabilityOutputTypeDef = TypedDict(
     "_OptionalVulnerabilityOutputTypeDef",
     {
-        "VulnerablePackages": List[SoftwarePackageOutputTypeDef],
+        "VulnerablePackages": List[SoftwarePackageTypeDef],
         "Cvss": List[CvssOutputTypeDef],
         "RelatedVulnerabilities": List[str],
-        "Vendor": VulnerabilityVendorOutputTypeDef,
+        "Vendor": VulnerabilityVendorTypeDef,
         "ReferenceUrls": List[str],
         "FixAvailable": VulnerabilityFixAvailableType,
     },
     total=False,
 )
 
 class VulnerabilityOutputTypeDef(
@@ -13089,19 +9100,19 @@
 
 class VulnerabilityTypeDef(_RequiredVulnerabilityTypeDef, _OptionalVulnerabilityTypeDef):
     pass
 
 AwsEc2RouteTableDetailsOutputTypeDef = TypedDict(
     "AwsEc2RouteTableDetailsOutputTypeDef",
     {
-        "AssociationSet": List[AssociationSetDetailsOutputTypeDef],
+        "AssociationSet": List[AssociationSetDetailsTypeDef],
         "OwnerId": str,
-        "PropagatingVgwSet": List[PropagatingVgwSetDetailsOutputTypeDef],
+        "PropagatingVgwSet": List[PropagatingVgwSetDetailsTypeDef],
         "RouteTableId": str,
-        "RouteSet": List[RouteSetDetailsOutputTypeDef],
+        "RouteSet": List[RouteSetDetailsTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
 AwsEc2RouteTableDetailsTypeDef = TypedDict(
     "AwsEc2RouteTableDetailsTypeDef",
@@ -13138,29 +9149,27 @@
     "AwsAmazonMqBrokerDetailsOutputTypeDef",
     {
         "AuthenticationStrategy": str,
         "AutoMinorVersionUpgrade": bool,
         "BrokerArn": str,
         "BrokerName": str,
         "DeploymentMode": str,
-        "EncryptionOptions": AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef,
+        "EncryptionOptions": AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
         "EngineType": str,
         "EngineVersion": str,
         "HostInstanceType": str,
         "BrokerId": str,
         "LdapServerMetadata": AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
-        "Logs": AwsAmazonMqBrokerLogsDetailsOutputTypeDef,
-        "MaintenanceWindowStartTime": (
-            AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef
-        ),
+        "Logs": AwsAmazonMqBrokerLogsDetailsTypeDef,
+        "MaintenanceWindowStartTime": AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
         "PubliclyAccessible": bool,
         "SecurityGroups": List[str],
         "StorageType": str,
         "SubnetIds": List[str],
-        "Users": List[AwsAmazonMqBrokerUsersDetailsOutputTypeDef],
+        "Users": List[AwsAmazonMqBrokerUsersDetailsTypeDef],
     },
     total=False,
 )
 
 AwsAmazonMqBrokerDetailsTypeDef = TypedDict(
     "AwsAmazonMqBrokerDetailsTypeDef",
     {
@@ -13187,24 +9196,24 @@
 )
 
 AwsAppSyncGraphQlApiDetailsOutputTypeDef = TypedDict(
     "AwsAppSyncGraphQlApiDetailsOutputTypeDef",
     {
         "ApiId": str,
         "Id": str,
-        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
+        "OpenIdConnectConfig": AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
         "Name": str,
-        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
+        "LambdaAuthorizerConfig": AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
         "XrayEnabled": bool,
         "Arn": str,
-        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
+        "UserPoolConfig": AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
         "AuthenticationType": str,
-        "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef,
+        "LogConfig": AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
         "AdditionalAuthenticationProviders": List[
-            AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef
+            AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
         ],
         "WafWebAclArn": str,
     },
     total=False,
 )
 
 AwsAppSyncGraphQlApiDetailsTypeDef = TypedDict(
@@ -13224,36 +9233,28 @@
             AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef
         ],
         "WafWebAclArn": str,
     },
     total=False,
 )
 
-AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef",
-    {
-        "ResultConfiguration": (
-            AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
 AwsAthenaWorkGroupConfigurationDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupConfigurationDetailsTypeDef",
     {
         "ResultConfiguration": AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef,
     },
     total=False,
 )
 
 AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef",
     {
-        "InstancesDistribution": AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef,
+        "InstancesDistribution": (
+            AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef
+        ),
         "LaunchTemplate": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef
         ),
     },
     total=False,
 )
 
@@ -13271,35 +9272,33 @@
 )
 
 AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BlockDeviceMappings": List[
-            AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef
+            AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef
         ],
         "ClassicLinkVpcId": str,
         "ClassicLinkVpcSecurityGroups": List[str],
         "CreatedTime": str,
         "EbsOptimized": bool,
         "IamInstanceProfile": str,
         "ImageId": str,
-        "InstanceMonitoring": (
-            AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef
-        ),
+        "InstanceMonitoring": AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
         "InstanceType": str,
         "KernelId": str,
         "KeyName": str,
         "LaunchConfigurationName": str,
         "PlacementTenancy": str,
         "RamdiskId": str,
         "SecurityGroups": List[str],
         "SpotPrice": str,
         "UserData": str,
-        "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef,
+        "MetadataOptions": AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
     },
     total=False,
 )
 
 AwsAutoScalingLaunchConfigurationDetailsTypeDef = TypedDict(
     "AwsAutoScalingLaunchConfigurationDetailsTypeDef",
     {
@@ -13334,16 +9333,16 @@
         "TargetBackupVault": str,
         "StartWindowMinutes": int,
         "ScheduleExpression": str,
         "RuleName": str,
         "RuleId": str,
         "EnableContinuousBackup": bool,
         "CompletionWindowMinutes": int,
-        "CopyActions": List[AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef],
-        "Lifecycle": AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
+        "CopyActions": List[AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef],
+        "Lifecycle": AwsBackupBackupPlanLifecycleDetailsTypeDef,
     },
     total=False,
 )
 
 AwsBackupBackupPlanRuleDetailsTypeDef = TypedDict(
     "AwsBackupBackupPlanRuleDetailsTypeDef",
     {
@@ -13388,15 +9387,15 @@
 
 AwsCloudFrontDistributionOriginItemOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemOutputTypeDef",
     {
         "DomainName": str,
         "Id": str,
         "OriginPath": str,
-        "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef,
+        "S3OriginConfig": AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
         "CustomOriginConfig": AwsCloudFrontDistributionOriginCustomOriginConfigOutputTypeDef,
     },
     total=False,
 )
 
 AwsCloudFrontDistributionOriginItemTypeDef = TypedDict(
     "AwsCloudFrontDistributionOriginItemTypeDef",
@@ -13426,22 +9425,22 @@
     total=False,
 )
 
 AwsCodeBuildProjectDetailsOutputTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsOutputTypeDef",
     {
         "EncryptionKey": str,
-        "Artifacts": List[AwsCodeBuildProjectArtifactsDetailsOutputTypeDef],
+        "Artifacts": List[AwsCodeBuildProjectArtifactsDetailsTypeDef],
         "Environment": AwsCodeBuildProjectEnvironmentOutputTypeDef,
         "Name": str,
-        "Source": AwsCodeBuildProjectSourceOutputTypeDef,
+        "Source": AwsCodeBuildProjectSourceTypeDef,
         "ServiceRole": str,
-        "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef,
+        "LogsConfig": AwsCodeBuildProjectLogsConfigDetailsTypeDef,
         "VpcConfig": AwsCodeBuildProjectVpcConfigOutputTypeDef,
-        "SecondaryArtifacts": List[AwsCodeBuildProjectArtifactsDetailsOutputTypeDef],
+        "SecondaryArtifacts": List[AwsCodeBuildProjectArtifactsDetailsTypeDef],
     },
     total=False,
 )
 
 AwsCodeBuildProjectDetailsTypeDef = TypedDict(
     "AwsCodeBuildProjectDetailsTypeDef",
     {
@@ -13457,17 +9456,17 @@
     },
     total=False,
 )
 
 AwsDynamoDbTableReplicaOutputTypeDef = TypedDict(
     "AwsDynamoDbTableReplicaOutputTypeDef",
     {
-        "GlobalSecondaryIndexes": List[AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef],
+        "GlobalSecondaryIndexes": List[AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef],
         "KmsMasterKeyId": str,
-        "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
+        "ProvisionedThroughputOverride": AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
         "RegionName": str,
         "ReplicaStatus": str,
         "ReplicaStatusDescription": str,
     },
     total=False,
 )
 
@@ -13483,50 +9482,48 @@
     },
     total=False,
 )
 
 AwsEc2LaunchTemplateDataDetailsOutputTypeDef = TypedDict(
     "AwsEc2LaunchTemplateDataDetailsOutputTypeDef",
     {
-        "BlockDeviceMappingSet": List[
-            AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef
-        ],
+        "BlockDeviceMappingSet": List[AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef],
         "CapacityReservationSpecification": (
-            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef
         ),
-        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef,
-        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef,
+        "CpuOptions": AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
+        "CreditSpecification": AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
         "DisableApiStop": bool,
         "DisableApiTermination": bool,
         "EbsOptimized": bool,
         "ElasticGpuSpecificationSet": List[
-            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef
         ],
         "ElasticInferenceAcceleratorSet": List[
-            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef
+            AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef
         ],
-        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef,
-        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef,
-        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef,
+        "EnclaveOptions": AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
+        "HibernationOptions": AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
+        "IamInstanceProfile": AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
         "ImageId": str,
         "InstanceInitiatedShutdownBehavior": str,
-        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef,
+        "InstanceMarketOptions": AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
         "InstanceRequirements": AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
         "InstanceType": str,
         "KernelId": str,
         "KeyName": str,
-        "LicenseSet": List[AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef],
-        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef,
-        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef,
-        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef,
+        "LicenseSet": List[AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef],
+        "MaintenanceOptions": AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
+        "MetadataOptions": AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
+        "Monitoring": AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
         "NetworkInterfaceSet": List[
             AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef
         ],
-        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef,
-        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef,
+        "Placement": AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
+        "PrivateDnsNameOptions": AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
         "RamDiskId": str,
         "SecurityGroupIdSet": List[str],
         "SecurityGroupSet": List[str],
         "UserData": str,
     },
     total=False,
 )
@@ -13579,16 +9576,16 @@
 AwsEc2NetworkAclDetailsOutputTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsOutputTypeDef",
     {
         "IsDefault": bool,
         "NetworkAclId": str,
         "OwnerId": str,
         "VpcId": str,
-        "Associations": List[AwsEc2NetworkAclAssociationOutputTypeDef],
-        "Entries": List[AwsEc2NetworkAclEntryOutputTypeDef],
+        "Associations": List[AwsEc2NetworkAclAssociationTypeDef],
+        "Entries": List[AwsEc2NetworkAclEntryTypeDef],
     },
     total=False,
 )
 
 AwsEc2NetworkAclDetailsTypeDef = TypedDict(
     "AwsEc2NetworkAclDetailsTypeDef",
     {
@@ -13630,15 +9627,15 @@
 
 AwsEc2VpcPeeringConnectionDetailsOutputTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsOutputTypeDef",
     {
         "AccepterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
         "ExpirationTime": str,
         "RequesterVpcInfo": AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
-        "Status": AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef,
+        "Status": AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
 AwsEc2VpcPeeringConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpcPeeringConnectionDetailsTypeDef",
@@ -13658,17 +9655,17 @@
         "VpnConnectionId": str,
         "State": str,
         "CustomerGatewayId": str,
         "CustomerGatewayConfiguration": str,
         "Type": str,
         "VpnGatewayId": str,
         "Category": str,
-        "VgwTelemetry": List[AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef],
+        "VgwTelemetry": List[AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef],
         "Options": AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
-        "Routes": List[AwsEc2VpnConnectionRoutesDetailsOutputTypeDef],
+        "Routes": List[AwsEc2VpnConnectionRoutesDetailsTypeDef],
         "TransitGatewayId": str,
     },
     total=False,
 )
 
 AwsEc2VpnConnectionDetailsTypeDef = TypedDict(
     "AwsEc2VpnConnectionDetailsTypeDef",
@@ -13684,58 +9681,48 @@
         "Options": AwsEc2VpnConnectionOptionsDetailsTypeDef,
         "Routes": Sequence[AwsEc2VpnConnectionRoutesDetailsTypeDef],
         "TransitGatewayId": str,
     },
     total=False,
 )
 
-AwsEcsClusterConfigurationDetailsOutputTypeDef = TypedDict(
-    "AwsEcsClusterConfigurationDetailsOutputTypeDef",
-    {
-        "ExecuteCommandConfiguration": (
-            AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef
-        ),
-    },
-    total=False,
-)
-
 AwsEcsClusterConfigurationDetailsTypeDef = TypedDict(
     "AwsEcsClusterConfigurationDetailsTypeDef",
     {
         "ExecuteCommandConfiguration": (
             AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef
         ),
     },
     total=False,
 )
 
 AwsEcsServiceDetailsOutputTypeDef = TypedDict(
     "AwsEcsServiceDetailsOutputTypeDef",
     {
-        "CapacityProviderStrategy": List[AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef],
+        "CapacityProviderStrategy": List[AwsEcsServiceCapacityProviderStrategyDetailsTypeDef],
         "Cluster": str,
-        "DeploymentConfiguration": AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef,
-        "DeploymentController": AwsEcsServiceDeploymentControllerDetailsOutputTypeDef,
+        "DeploymentConfiguration": AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
+        "DeploymentController": AwsEcsServiceDeploymentControllerDetailsTypeDef,
         "DesiredCount": int,
         "EnableEcsManagedTags": bool,
         "EnableExecuteCommand": bool,
         "HealthCheckGracePeriodSeconds": int,
         "LaunchType": str,
-        "LoadBalancers": List[AwsEcsServiceLoadBalancersDetailsOutputTypeDef],
+        "LoadBalancers": List[AwsEcsServiceLoadBalancersDetailsTypeDef],
         "Name": str,
         "NetworkConfiguration": AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
-        "PlacementConstraints": List[AwsEcsServicePlacementConstraintsDetailsOutputTypeDef],
-        "PlacementStrategies": List[AwsEcsServicePlacementStrategiesDetailsOutputTypeDef],
+        "PlacementConstraints": List[AwsEcsServicePlacementConstraintsDetailsTypeDef],
+        "PlacementStrategies": List[AwsEcsServicePlacementStrategiesDetailsTypeDef],
         "PlatformVersion": str,
         "PropagateTags": str,
         "Role": str,
         "SchedulingStrategy": str,
         "ServiceArn": str,
         "ServiceName": str,
-        "ServiceRegistries": List[AwsEcsServiceServiceRegistriesDetailsOutputTypeDef],
+        "ServiceRegistries": List[AwsEcsServiceServiceRegistriesDetailsTypeDef],
         "TaskDefinition": str,
     },
     total=False,
 )
 
 AwsEcsServiceDetailsTypeDef = TypedDict(
     "AwsEcsServiceDetailsTypeDef",
@@ -13767,29 +9754,27 @@
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef",
     {
         "Command": List[str],
         "Cpu": int,
-        "DependsOn": List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef],
+        "DependsOn": List[AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef],
         "DisableNetworking": bool,
         "DnsSearchDomains": List[str],
         "DnsServers": List[str],
         "DockerLabels": Dict[str, str],
         "DockerSecurityOptions": List[str],
         "EntryPoint": List[str],
-        "Environment": List[
-            AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef
-        ],
+        "Environment": List[AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef],
         "EnvironmentFiles": List[
-            AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef
         ],
         "Essential": bool,
-        "ExtraHosts": List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef],
+        "ExtraHosts": List[AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef],
         "FirelensConfiguration": (
             AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef
         ),
         "HealthCheck": AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
         "Hostname": str,
         "Image": str,
         "Interactive": bool,
@@ -13798,41 +9783,35 @@
             AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef
         ),
         "LogConfiguration": (
             AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef
         ),
         "Memory": int,
         "MemoryReservation": int,
-        "MountPoints": List[
-            AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef
-        ],
+        "MountPoints": List[AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef],
         "Name": str,
-        "PortMappings": List[
-            AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef
-        ],
+        "PortMappings": List[AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef],
         "Privileged": bool,
         "PseudoTerminal": bool,
         "ReadonlyRootFilesystem": bool,
         "RepositoryCredentials": (
-            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef
         ),
         "ResourceRequirements": List[
-            AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef
         ],
-        "Secrets": List[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef],
+        "Secrets": List[AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef],
         "StartTimeout": int,
         "StopTimeout": int,
         "SystemControls": List[
-            AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef
+            AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef
         ],
-        "Ulimits": List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef],
+        "Ulimits": List[AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef],
         "User": str,
-        "VolumesFrom": List[
-            AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef
-        ],
+        "VolumesFrom": List[AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef],
         "WorkingDirectory": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef",
@@ -13894,18 +9873,16 @@
 
 AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef",
     {
         "DockerVolumeConfiguration": (
             AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef
         ),
-        "EfsVolumeConfiguration": (
-            AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef
-        ),
-        "Host": AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef,
+        "EfsVolumeConfiguration": AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
+        "Host": AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
         "Name": str,
     },
     total=False,
 )
 
 AwsEcsTaskDefinitionVolumesDetailsTypeDef = TypedDict(
     "AwsEcsTaskDefinitionVolumesDetailsTypeDef",
@@ -13926,15 +9903,15 @@
         "ClusterArn": str,
         "TaskDefinitionArn": str,
         "Version": str,
         "CreatedAt": str,
         "StartedAt": str,
         "StartedBy": str,
         "Group": str,
-        "Volumes": List[AwsEcsTaskVolumeDetailsOutputTypeDef],
+        "Volumes": List[AwsEcsTaskVolumeDetailsTypeDef],
         "Containers": List[AwsEcsContainerDetailsOutputTypeDef],
     },
     total=False,
 )
 
 AwsEcsTaskDetailsTypeDef = TypedDict(
     "AwsEcsTaskDetailsTypeDef",
@@ -13956,15 +9933,15 @@
     "AwsEfsAccessPointDetailsOutputTypeDef",
     {
         "AccessPointId": str,
         "Arn": str,
         "ClientToken": str,
         "FileSystemId": str,
         "PosixUser": AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
-        "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef,
+        "RootDirectory": AwsEfsAccessPointRootDirectoryDetailsTypeDef,
     },
     total=False,
 )
 
 AwsEfsAccessPointDetailsTypeDef = TypedDict(
     "AwsEfsAccessPointDetailsTypeDef",
     {
@@ -14010,29 +9987,27 @@
     total=False,
 )
 
 AwsElasticsearchDomainDetailsOutputTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsOutputTypeDef",
     {
         "AccessPolicies": str,
-        "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef,
+        "DomainEndpointOptions": AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
         "DomainId": str,
         "DomainName": str,
         "Endpoint": str,
         "Endpoints": Dict[str, str],
         "ElasticsearchVersion": str,
         "ElasticsearchClusterConfig": (
-            AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef
-        ),
-        "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef,
-        "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef,
-        "NodeToNodeEncryptionOptions": (
-            AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef
+            AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef
         ),
-        "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef,
+        "EncryptionAtRestOptions": AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
+        "LogPublishingOptions": AwsElasticsearchDomainLogPublishingOptionsTypeDef,
+        "NodeToNodeEncryptionOptions": AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
+        "ServiceSoftwareOptions": AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
         "VPCOptions": AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     },
     total=False,
 )
 
 AwsElasticsearchDomainDetailsTypeDef = TypedDict(
     "AwsElasticsearchDomainDetailsTypeDef",
@@ -14061,23 +10036,23 @@
     {
         "AvailabilityZones": List[str],
         "BackendServerDescriptions": List[AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef],
         "CanonicalHostedZoneName": str,
         "CanonicalHostedZoneNameID": str,
         "CreatedTime": str,
         "DnsName": str,
-        "HealthCheck": AwsElbLoadBalancerHealthCheckOutputTypeDef,
-        "Instances": List[AwsElbLoadBalancerInstanceOutputTypeDef],
+        "HealthCheck": AwsElbLoadBalancerHealthCheckTypeDef,
+        "Instances": List[AwsElbLoadBalancerInstanceTypeDef],
         "ListenerDescriptions": List[AwsElbLoadBalancerListenerDescriptionOutputTypeDef],
         "LoadBalancerAttributes": AwsElbLoadBalancerAttributesOutputTypeDef,
         "LoadBalancerName": str,
         "Policies": AwsElbLoadBalancerPoliciesOutputTypeDef,
         "Scheme": str,
         "SecurityGroups": List[str],
-        "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef,
+        "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupTypeDef,
         "Subnets": List[str],
         "VpcId": str,
     },
     total=False,
 )
 
 AwsElbLoadBalancerDetailsTypeDef = TypedDict(
@@ -14100,48 +10075,23 @@
         "SourceSecurityGroup": AwsElbLoadBalancerSourceSecurityGroupTypeDef,
         "Subnets": Sequence[str],
         "VpcId": str,
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef",
-    {
-        "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef,
-        "ServiceRole": str,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef",
     {
         "ScanEc2InstanceWithFindings": AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
         "ServiceRole": str,
     },
     total=False,
 )
 
-AwsIamAccessKeyDetailsOutputTypeDef = TypedDict(
-    "AwsIamAccessKeyDetailsOutputTypeDef",
-    {
-        "UserName": str,
-        "Status": AwsIamAccessKeyStatusType,
-        "CreatedAt": str,
-        "PrincipalId": str,
-        "PrincipalType": str,
-        "PrincipalName": str,
-        "AccountId": str,
-        "AccessKeyId": str,
-        "SessionContext": AwsIamAccessKeySessionContextOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsIamAccessKeyDetailsTypeDef = TypedDict(
     "AwsIamAccessKeyDetailsTypeDef",
     {
         "UserName": str,
         "Status": AwsIamAccessKeyStatusType,
         "CreatedAt": str,
         "PrincipalId": str,
@@ -14154,21 +10104,21 @@
     total=False,
 )
 
 AwsIamRoleDetailsOutputTypeDef = TypedDict(
     "AwsIamRoleDetailsOutputTypeDef",
     {
         "AssumeRolePolicyDocument": str,
-        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyOutputTypeDef],
+        "AttachedManagedPolicies": List[AwsIamAttachedManagedPolicyTypeDef],
         "CreateDate": str,
         "InstanceProfileList": List[AwsIamInstanceProfileOutputTypeDef],
-        "PermissionsBoundary": AwsIamPermissionsBoundaryOutputTypeDef,
+        "PermissionsBoundary": AwsIamPermissionsBoundaryTypeDef,
         "RoleId": str,
         "RoleName": str,
-        "RolePolicyList": List[AwsIamRolePolicyOutputTypeDef],
+        "RolePolicyList": List[AwsIamRolePolicyTypeDef],
         "MaxSessionDuration": int,
         "Path": str,
     },
     total=False,
 )
 
 AwsIamRoleDetailsTypeDef = TypedDict(
@@ -14187,30 +10137,30 @@
     },
     total=False,
 )
 
 AwsLambdaFunctionDetailsOutputTypeDef = TypedDict(
     "AwsLambdaFunctionDetailsOutputTypeDef",
     {
-        "Code": AwsLambdaFunctionCodeOutputTypeDef,
+        "Code": AwsLambdaFunctionCodeTypeDef,
         "CodeSha256": str,
-        "DeadLetterConfig": AwsLambdaFunctionDeadLetterConfigOutputTypeDef,
+        "DeadLetterConfig": AwsLambdaFunctionDeadLetterConfigTypeDef,
         "Environment": AwsLambdaFunctionEnvironmentOutputTypeDef,
         "FunctionName": str,
         "Handler": str,
         "KmsKeyArn": str,
         "LastModified": str,
-        "Layers": List[AwsLambdaFunctionLayerOutputTypeDef],
+        "Layers": List[AwsLambdaFunctionLayerTypeDef],
         "MasterArn": str,
         "MemorySize": int,
         "RevisionId": str,
         "Role": str,
         "Runtime": str,
         "Timeout": int,
-        "TracingConfig": AwsLambdaFunctionTracingConfigOutputTypeDef,
+        "TracingConfig": AwsLambdaFunctionTracingConfigTypeDef,
         "VpcConfig": AwsLambdaFunctionVpcConfigOutputTypeDef,
         "Version": str,
         "Architectures": List[str],
         "PackageType": str,
     },
     total=False,
 )
@@ -14247,33 +10197,25 @@
     {
         "Arn": str,
         "AccessPolicies": str,
         "DomainName": str,
         "Id": str,
         "DomainEndpoint": str,
         "EngineVersion": str,
-        "EncryptionAtRestOptions": (
-            AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef
-        ),
+        "EncryptionAtRestOptions": AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
         "NodeToNodeEncryptionOptions": (
-            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef
-        ),
-        "ServiceSoftwareOptions": (
-            AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef
-        ),
-        "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef,
-        "DomainEndpointOptions": (
-            AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef
+            AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef
         ),
+        "ServiceSoftwareOptions": AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+        "ClusterConfig": AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
+        "DomainEndpointOptions": AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
         "VpcOptions": AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
-        "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef,
+        "LogPublishingOptions": AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
         "DomainEndpoints": Dict[str, str],
-        "AdvancedSecurityOptions": (
-            AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef
-        ),
+        "AdvancedSecurityOptions": AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
     },
     total=False,
 )
 
 AwsOpenSearchServiceDomainDetailsTypeDef = TypedDict(
     "AwsOpenSearchServiceDomainDetailsTypeDef",
     {
@@ -14301,15 +10243,15 @@
 AwsRdsDbSubnetGroupOutputTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupOutputTypeDef",
     {
         "DbSubnetGroupName": str,
         "DbSubnetGroupDescription": str,
         "VpcId": str,
         "SubnetGroupStatus": str,
-        "Subnets": List[AwsRdsDbSubnetGroupSubnetOutputTypeDef],
+        "Subnets": List[AwsRdsDbSubnetGroupSubnetTypeDef],
         "DbSubnetGroupArn": str,
     },
     total=False,
 )
 
 AwsRdsDbSubnetGroupTypeDef = TypedDict(
     "AwsRdsDbSubnetGroupTypeDef",
@@ -14329,54 +10271,52 @@
     {
         "AllowVersionUpgrade": bool,
         "AutomatedSnapshotRetentionPeriod": int,
         "AvailabilityZone": str,
         "ClusterAvailabilityStatus": str,
         "ClusterCreateTime": str,
         "ClusterIdentifier": str,
-        "ClusterNodes": List[AwsRedshiftClusterClusterNodeOutputTypeDef],
+        "ClusterNodes": List[AwsRedshiftClusterClusterNodeTypeDef],
         "ClusterParameterGroups": List[AwsRedshiftClusterClusterParameterGroupOutputTypeDef],
         "ClusterPublicKey": str,
         "ClusterRevisionNumber": str,
-        "ClusterSecurityGroups": List[AwsRedshiftClusterClusterSecurityGroupOutputTypeDef],
-        "ClusterSnapshotCopyStatus": AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef,
+        "ClusterSecurityGroups": List[AwsRedshiftClusterClusterSecurityGroupTypeDef],
+        "ClusterSnapshotCopyStatus": AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
         "ClusterStatus": str,
         "ClusterSubnetGroupName": str,
         "ClusterVersion": str,
         "DBName": str,
-        "DeferredMaintenanceWindows": List[
-            AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef
-        ],
-        "ElasticIpStatus": AwsRedshiftClusterElasticIpStatusOutputTypeDef,
+        "DeferredMaintenanceWindows": List[AwsRedshiftClusterDeferredMaintenanceWindowTypeDef],
+        "ElasticIpStatus": AwsRedshiftClusterElasticIpStatusTypeDef,
         "ElasticResizeNumberOfNodeOptions": str,
         "Encrypted": bool,
-        "Endpoint": AwsRedshiftClusterEndpointOutputTypeDef,
+        "Endpoint": AwsRedshiftClusterEndpointTypeDef,
         "EnhancedVpcRouting": bool,
         "ExpectedNextSnapshotScheduleTime": str,
         "ExpectedNextSnapshotScheduleTimeStatus": str,
-        "HsmStatus": AwsRedshiftClusterHsmStatusOutputTypeDef,
-        "IamRoles": List[AwsRedshiftClusterIamRoleOutputTypeDef],
+        "HsmStatus": AwsRedshiftClusterHsmStatusTypeDef,
+        "IamRoles": List[AwsRedshiftClusterIamRoleTypeDef],
         "KmsKeyId": str,
         "MaintenanceTrackName": str,
         "ManualSnapshotRetentionPeriod": int,
         "MasterUsername": str,
         "NextMaintenanceWindowStartTime": str,
         "NodeType": str,
         "NumberOfNodes": int,
         "PendingActions": List[str],
-        "PendingModifiedValues": AwsRedshiftClusterPendingModifiedValuesOutputTypeDef,
+        "PendingModifiedValues": AwsRedshiftClusterPendingModifiedValuesTypeDef,
         "PreferredMaintenanceWindow": str,
         "PubliclyAccessible": bool,
-        "ResizeInfo": AwsRedshiftClusterResizeInfoOutputTypeDef,
-        "RestoreStatus": AwsRedshiftClusterRestoreStatusOutputTypeDef,
+        "ResizeInfo": AwsRedshiftClusterResizeInfoTypeDef,
+        "RestoreStatus": AwsRedshiftClusterRestoreStatusTypeDef,
         "SnapshotScheduleIdentifier": str,
         "SnapshotScheduleState": str,
         "VpcId": str,
-        "VpcSecurityGroups": List[AwsRedshiftClusterVpcSecurityGroupOutputTypeDef],
-        "LoggingStatus": AwsRedshiftClusterLoggingStatusOutputTypeDef,
+        "VpcSecurityGroups": List[AwsRedshiftClusterVpcSecurityGroupTypeDef],
+        "LoggingStatus": AwsRedshiftClusterLoggingStatusTypeDef,
     },
     total=False,
 )
 
 AwsRedshiftClusterDetailsTypeDef = TypedDict(
     "AwsRedshiftClusterDetailsTypeDef",
     {
@@ -14428,18 +10368,18 @@
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef",
     {
         "Operands": List[
-            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef
+            AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef
         ],
         "Prefix": str,
-        "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef,
+        "Tag": AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef",
@@ -14466,36 +10406,27 @@
     "AwsS3BucketNotificationConfigurationFilterTypeDef",
     {
         "S3KeyFilter": AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
     },
     total=False,
 )
 
-AwsS3BucketObjectLockConfigurationOutputTypeDef = TypedDict(
-    "AwsS3BucketObjectLockConfigurationOutputTypeDef",
-    {
-        "ObjectLockEnabled": str,
-        "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsS3BucketObjectLockConfigurationTypeDef = TypedDict(
     "AwsS3BucketObjectLockConfigurationTypeDef",
     {
         "ObjectLockEnabled": str,
         "Rule": AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
     },
     total=False,
 )
 
 AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef",
     {
-        "Rules": List[AwsS3BucketServerSideEncryptionRuleOutputTypeDef],
+        "Rules": List[AwsS3BucketServerSideEncryptionRuleTypeDef],
     },
     total=False,
 )
 
 AwsS3BucketServerSideEncryptionConfigurationTypeDef = TypedDict(
     "AwsS3BucketServerSideEncryptionConfigurationTypeDef",
     {
@@ -14505,16 +10436,16 @@
 )
 
 AwsS3BucketWebsiteConfigurationOutputTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationOutputTypeDef",
     {
         "ErrorDocument": str,
         "IndexDocumentSuffix": str,
-        "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef,
-        "RoutingRules": List[AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef],
+        "RedirectAllRequestsTo": AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
+        "RoutingRules": List[AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef],
     },
     total=False,
 )
 
 AwsS3BucketWebsiteConfigurationTypeDef = TypedDict(
     "AwsS3BucketWebsiteConfigurationTypeDef",
     {
@@ -14525,41 +10456,33 @@
     },
     total=False,
 )
 
 BatchUpdateFindingsResponseTypeDef = TypedDict(
     "BatchUpdateFindingsResponseTypeDef",
     {
-        "ProcessedFindings": List[AwsSecurityFindingIdentifierOutputTypeDef],
+        "ProcessedFindings": List[AwsSecurityFindingIdentifierTypeDef],
         "UnprocessedFindings": List[BatchUpdateFindingsUnprocessedFindingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AwsSsmPatchComplianceDetailsOutputTypeDef = TypedDict(
-    "AwsSsmPatchComplianceDetailsOutputTypeDef",
-    {
-        "Patch": AwsSsmPatchOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsSsmPatchComplianceDetailsTypeDef = TypedDict(
     "AwsSsmPatchComplianceDetailsTypeDef",
     {
         "Patch": AwsSsmPatchTypeDef,
     },
     total=False,
 )
 
 AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef = TypedDict(
     "AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef",
     {
         "Destinations": List[
-            AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef
+            AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef
         ],
         "IncludeExecutionData": bool,
         "Level": str,
     },
     total=False,
 )
 
@@ -14577,15 +10500,15 @@
 
 AwsWafRegionalRuleGroupDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
-        "Rules": List[AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef],
+        "Rules": List[AwsWafRegionalRuleGroupRulesDetailsTypeDef],
     },
     total=False,
 )
 
 AwsWafRegionalRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRegionalRuleGroupDetailsTypeDef",
     {
@@ -14599,15 +10522,15 @@
 
 AwsWafRegionalWebAclDetailsOutputTypeDef = TypedDict(
     "AwsWafRegionalWebAclDetailsOutputTypeDef",
     {
         "DefaultAction": str,
         "MetricName": str,
         "Name": str,
-        "RulesList": List[AwsWafRegionalWebAclRulesListDetailsOutputTypeDef],
+        "RulesList": List[AwsWafRegionalWebAclRulesListDetailsTypeDef],
         "WebAclId": str,
     },
     total=False,
 )
 
 AwsWafRegionalWebAclDetailsTypeDef = TypedDict(
     "AwsWafRegionalWebAclDetailsTypeDef",
@@ -14623,15 +10546,15 @@
 
 AwsWafRuleGroupDetailsOutputTypeDef = TypedDict(
     "AwsWafRuleGroupDetailsOutputTypeDef",
     {
         "MetricName": str,
         "Name": str,
         "RuleGroupId": str,
-        "Rules": List[AwsWafRuleGroupRulesDetailsOutputTypeDef],
+        "Rules": List[AwsWafRuleGroupRulesDetailsTypeDef],
     },
     total=False,
 )
 
 AwsWafRuleGroupDetailsTypeDef = TypedDict(
     "AwsWafRuleGroupDetailsTypeDef",
     {
@@ -14685,22 +10608,14 @@
     "AwsWafv2RulesActionCountDetailsOutputTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
     },
     total=False,
 )
 
-AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
-    "AwsWafv2ActionBlockDetailsOutputTypeDef",
-    {
-        "CustomResponse": AwsWafv2CustomResponseDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsWafv2ActionAllowDetailsTypeDef = TypedDict(
     "AwsWafv2ActionAllowDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
     total=False,
 )
@@ -14717,164 +10632,85 @@
     "AwsWafv2RulesActionCountDetailsTypeDef",
     {
         "CustomRequestHandling": AwsWafv2CustomRequestHandlingDetailsTypeDef,
     },
     total=False,
 )
 
+AwsWafv2ActionBlockDetailsOutputTypeDef = TypedDict(
+    "AwsWafv2ActionBlockDetailsOutputTypeDef",
+    {
+        "CustomResponse": AwsWafv2CustomResponseDetailsOutputTypeDef,
+    },
+    total=False,
+)
+
 AwsWafv2ActionBlockDetailsTypeDef = TypedDict(
     "AwsWafv2ActionBlockDetailsTypeDef",
     {
         "CustomResponse": AwsWafv2CustomResponseDetailsTypeDef,
     },
     total=False,
 )
 
-AutomationRulesFindingFiltersOutputTypeDef = TypedDict(
-    "AutomationRulesFindingFiltersOutputTypeDef",
+BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "BatchGetStandardsControlAssociationsResponseTypeDef",
     {
-        "ProductArn": List[StringFilterOutputTypeDef],
-        "AwsAccountId": List[StringFilterOutputTypeDef],
-        "Id": List[StringFilterOutputTypeDef],
-        "GeneratorId": List[StringFilterOutputTypeDef],
-        "Type": List[StringFilterOutputTypeDef],
-        "FirstObservedAt": List[DateFilterOutputTypeDef],
-        "LastObservedAt": List[DateFilterOutputTypeDef],
-        "CreatedAt": List[DateFilterOutputTypeDef],
-        "UpdatedAt": List[DateFilterOutputTypeDef],
-        "Confidence": List[NumberFilterOutputTypeDef],
-        "Criticality": List[NumberFilterOutputTypeDef],
-        "Title": List[StringFilterOutputTypeDef],
-        "Description": List[StringFilterOutputTypeDef],
-        "SourceUrl": List[StringFilterOutputTypeDef],
-        "ProductName": List[StringFilterOutputTypeDef],
-        "CompanyName": List[StringFilterOutputTypeDef],
-        "SeverityLabel": List[StringFilterOutputTypeDef],
-        "ResourceType": List[StringFilterOutputTypeDef],
-        "ResourceId": List[StringFilterOutputTypeDef],
-        "ResourcePartition": List[StringFilterOutputTypeDef],
-        "ResourceRegion": List[StringFilterOutputTypeDef],
-        "ResourceTags": List[MapFilterOutputTypeDef],
-        "ResourceDetailsOther": List[MapFilterOutputTypeDef],
-        "ComplianceStatus": List[StringFilterOutputTypeDef],
-        "ComplianceSecurityControlId": List[StringFilterOutputTypeDef],
-        "ComplianceAssociatedStandardsId": List[StringFilterOutputTypeDef],
-        "VerificationState": List[StringFilterOutputTypeDef],
-        "WorkflowStatus": List[StringFilterOutputTypeDef],
-        "RecordState": List[StringFilterOutputTypeDef],
-        "RelatedFindingsProductArn": List[StringFilterOutputTypeDef],
-        "RelatedFindingsId": List[StringFilterOutputTypeDef],
-        "NoteText": List[StringFilterOutputTypeDef],
-        "NoteUpdatedAt": List[DateFilterOutputTypeDef],
-        "NoteUpdatedBy": List[StringFilterOutputTypeDef],
-        "UserDefinedFields": List[MapFilterOutputTypeDef],
+        "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
+        "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
-    "AwsSecurityFindingFiltersOutputTypeDef",
+BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
+    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
     {
-        "ProductArn": List[StringFilterOutputTypeDef],
-        "AwsAccountId": List[StringFilterOutputTypeDef],
-        "Id": List[StringFilterOutputTypeDef],
-        "GeneratorId": List[StringFilterOutputTypeDef],
-        "Region": List[StringFilterOutputTypeDef],
-        "Type": List[StringFilterOutputTypeDef],
-        "FirstObservedAt": List[DateFilterOutputTypeDef],
-        "LastObservedAt": List[DateFilterOutputTypeDef],
-        "CreatedAt": List[DateFilterOutputTypeDef],
-        "UpdatedAt": List[DateFilterOutputTypeDef],
-        "SeverityProduct": List[NumberFilterOutputTypeDef],
-        "SeverityNormalized": List[NumberFilterOutputTypeDef],
-        "SeverityLabel": List[StringFilterOutputTypeDef],
-        "Confidence": List[NumberFilterOutputTypeDef],
-        "Criticality": List[NumberFilterOutputTypeDef],
-        "Title": List[StringFilterOutputTypeDef],
-        "Description": List[StringFilterOutputTypeDef],
-        "RecommendationText": List[StringFilterOutputTypeDef],
-        "SourceUrl": List[StringFilterOutputTypeDef],
-        "ProductFields": List[MapFilterOutputTypeDef],
-        "ProductName": List[StringFilterOutputTypeDef],
-        "CompanyName": List[StringFilterOutputTypeDef],
-        "UserDefinedFields": List[MapFilterOutputTypeDef],
-        "MalwareName": List[StringFilterOutputTypeDef],
-        "MalwareType": List[StringFilterOutputTypeDef],
-        "MalwarePath": List[StringFilterOutputTypeDef],
-        "MalwareState": List[StringFilterOutputTypeDef],
-        "NetworkDirection": List[StringFilterOutputTypeDef],
-        "NetworkProtocol": List[StringFilterOutputTypeDef],
-        "NetworkSourceIpV4": List[IpFilterOutputTypeDef],
-        "NetworkSourceIpV6": List[IpFilterOutputTypeDef],
-        "NetworkSourcePort": List[NumberFilterOutputTypeDef],
-        "NetworkSourceDomain": List[StringFilterOutputTypeDef],
-        "NetworkSourceMac": List[StringFilterOutputTypeDef],
-        "NetworkDestinationIpV4": List[IpFilterOutputTypeDef],
-        "NetworkDestinationIpV6": List[IpFilterOutputTypeDef],
-        "NetworkDestinationPort": List[NumberFilterOutputTypeDef],
-        "NetworkDestinationDomain": List[StringFilterOutputTypeDef],
-        "ProcessName": List[StringFilterOutputTypeDef],
-        "ProcessPath": List[StringFilterOutputTypeDef],
-        "ProcessPid": List[NumberFilterOutputTypeDef],
-        "ProcessParentPid": List[NumberFilterOutputTypeDef],
-        "ProcessLaunchedAt": List[DateFilterOutputTypeDef],
-        "ProcessTerminatedAt": List[DateFilterOutputTypeDef],
-        "ThreatIntelIndicatorType": List[StringFilterOutputTypeDef],
-        "ThreatIntelIndicatorValue": List[StringFilterOutputTypeDef],
-        "ThreatIntelIndicatorCategory": List[StringFilterOutputTypeDef],
-        "ThreatIntelIndicatorLastObservedAt": List[DateFilterOutputTypeDef],
-        "ThreatIntelIndicatorSource": List[StringFilterOutputTypeDef],
-        "ThreatIntelIndicatorSourceUrl": List[StringFilterOutputTypeDef],
-        "ResourceType": List[StringFilterOutputTypeDef],
-        "ResourceId": List[StringFilterOutputTypeDef],
-        "ResourcePartition": List[StringFilterOutputTypeDef],
-        "ResourceRegion": List[StringFilterOutputTypeDef],
-        "ResourceTags": List[MapFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceType": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceImageId": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceIpV4Addresses": List[IpFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceIpV6Addresses": List[IpFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceKeyName": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceIamInstanceProfileArn": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceVpcId": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceSubnetId": List[StringFilterOutputTypeDef],
-        "ResourceAwsEc2InstanceLaunchedAt": List[DateFilterOutputTypeDef],
-        "ResourceAwsS3BucketOwnerId": List[StringFilterOutputTypeDef],
-        "ResourceAwsS3BucketOwnerName": List[StringFilterOutputTypeDef],
-        "ResourceAwsIamAccessKeyUserName": List[StringFilterOutputTypeDef],
-        "ResourceAwsIamAccessKeyPrincipalName": List[StringFilterOutputTypeDef],
-        "ResourceAwsIamAccessKeyStatus": List[StringFilterOutputTypeDef],
-        "ResourceAwsIamAccessKeyCreatedAt": List[DateFilterOutputTypeDef],
-        "ResourceAwsIamUserUserName": List[StringFilterOutputTypeDef],
-        "ResourceContainerName": List[StringFilterOutputTypeDef],
-        "ResourceContainerImageId": List[StringFilterOutputTypeDef],
-        "ResourceContainerImageName": List[StringFilterOutputTypeDef],
-        "ResourceContainerLaunchedAt": List[DateFilterOutputTypeDef],
-        "ResourceDetailsOther": List[MapFilterOutputTypeDef],
-        "ComplianceStatus": List[StringFilterOutputTypeDef],
-        "VerificationState": List[StringFilterOutputTypeDef],
-        "WorkflowState": List[StringFilterOutputTypeDef],
-        "WorkflowStatus": List[StringFilterOutputTypeDef],
-        "RecordState": List[StringFilterOutputTypeDef],
-        "RelatedFindingsProductArn": List[StringFilterOutputTypeDef],
-        "RelatedFindingsId": List[StringFilterOutputTypeDef],
-        "NoteText": List[StringFilterOutputTypeDef],
-        "NoteUpdatedAt": List[DateFilterOutputTypeDef],
-        "NoteUpdatedBy": List[StringFilterOutputTypeDef],
-        "Keyword": List[KeywordFilterOutputTypeDef],
-        "FindingProviderFieldsConfidence": List[NumberFilterOutputTypeDef],
-        "FindingProviderFieldsCriticality": List[NumberFilterOutputTypeDef],
-        "FindingProviderFieldsRelatedFindingsId": List[StringFilterOutputTypeDef],
-        "FindingProviderFieldsRelatedFindingsProductArn": List[StringFilterOutputTypeDef],
-        "FindingProviderFieldsSeverityLabel": List[StringFilterOutputTypeDef],
-        "FindingProviderFieldsSeverityOriginal": List[StringFilterOutputTypeDef],
-        "FindingProviderFieldsTypes": List[StringFilterOutputTypeDef],
-        "Sample": List[BooleanFilterOutputTypeDef],
-        "ComplianceSecurityControlId": List[StringFilterOutputTypeDef],
-        "ComplianceAssociatedStandardsId": List[StringFilterOutputTypeDef],
+        "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AutomationRulesFindingFiltersOutputTypeDef = TypedDict(
+    "AutomationRulesFindingFiltersOutputTypeDef",
+    {
+        "ProductArn": List[StringFilterTypeDef],
+        "AwsAccountId": List[StringFilterTypeDef],
+        "Id": List[StringFilterTypeDef],
+        "GeneratorId": List[StringFilterTypeDef],
+        "Type": List[StringFilterTypeDef],
+        "FirstObservedAt": List[DateFilterTypeDef],
+        "LastObservedAt": List[DateFilterTypeDef],
+        "CreatedAt": List[DateFilterTypeDef],
+        "UpdatedAt": List[DateFilterTypeDef],
+        "Confidence": List[NumberFilterTypeDef],
+        "Criticality": List[NumberFilterTypeDef],
+        "Title": List[StringFilterTypeDef],
+        "Description": List[StringFilterTypeDef],
+        "SourceUrl": List[StringFilterTypeDef],
+        "ProductName": List[StringFilterTypeDef],
+        "CompanyName": List[StringFilterTypeDef],
+        "SeverityLabel": List[StringFilterTypeDef],
+        "ResourceType": List[StringFilterTypeDef],
+        "ResourceId": List[StringFilterTypeDef],
+        "ResourcePartition": List[StringFilterTypeDef],
+        "ResourceRegion": List[StringFilterTypeDef],
+        "ResourceTags": List[MapFilterTypeDef],
+        "ResourceDetailsOther": List[MapFilterTypeDef],
+        "ComplianceStatus": List[StringFilterTypeDef],
+        "ComplianceSecurityControlId": List[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": List[StringFilterTypeDef],
+        "VerificationState": List[StringFilterTypeDef],
+        "WorkflowStatus": List[StringFilterTypeDef],
+        "RecordState": List[StringFilterTypeDef],
+        "RelatedFindingsProductArn": List[StringFilterTypeDef],
+        "RelatedFindingsId": List[StringFilterTypeDef],
+        "NoteText": List[StringFilterTypeDef],
+        "NoteUpdatedAt": List[DateFilterTypeDef],
+        "NoteUpdatedBy": List[StringFilterTypeDef],
+        "UserDefinedFields": List[MapFilterTypeDef],
     },
     total=False,
 )
 
 AutomationRulesFindingFiltersTypeDef = TypedDict(
     "AutomationRulesFindingFiltersTypeDef",
     {
@@ -14913,14 +10749,118 @@
         "NoteUpdatedAt": Sequence[DateFilterTypeDef],
         "NoteUpdatedBy": Sequence[StringFilterTypeDef],
         "UserDefinedFields": Sequence[MapFilterTypeDef],
     },
     total=False,
 )
 
+AwsSecurityFindingFiltersOutputTypeDef = TypedDict(
+    "AwsSecurityFindingFiltersOutputTypeDef",
+    {
+        "ProductArn": List[StringFilterTypeDef],
+        "AwsAccountId": List[StringFilterTypeDef],
+        "Id": List[StringFilterTypeDef],
+        "GeneratorId": List[StringFilterTypeDef],
+        "Region": List[StringFilterTypeDef],
+        "Type": List[StringFilterTypeDef],
+        "FirstObservedAt": List[DateFilterTypeDef],
+        "LastObservedAt": List[DateFilterTypeDef],
+        "CreatedAt": List[DateFilterTypeDef],
+        "UpdatedAt": List[DateFilterTypeDef],
+        "SeverityProduct": List[NumberFilterTypeDef],
+        "SeverityNormalized": List[NumberFilterTypeDef],
+        "SeverityLabel": List[StringFilterTypeDef],
+        "Confidence": List[NumberFilterTypeDef],
+        "Criticality": List[NumberFilterTypeDef],
+        "Title": List[StringFilterTypeDef],
+        "Description": List[StringFilterTypeDef],
+        "RecommendationText": List[StringFilterTypeDef],
+        "SourceUrl": List[StringFilterTypeDef],
+        "ProductFields": List[MapFilterTypeDef],
+        "ProductName": List[StringFilterTypeDef],
+        "CompanyName": List[StringFilterTypeDef],
+        "UserDefinedFields": List[MapFilterTypeDef],
+        "MalwareName": List[StringFilterTypeDef],
+        "MalwareType": List[StringFilterTypeDef],
+        "MalwarePath": List[StringFilterTypeDef],
+        "MalwareState": List[StringFilterTypeDef],
+        "NetworkDirection": List[StringFilterTypeDef],
+        "NetworkProtocol": List[StringFilterTypeDef],
+        "NetworkSourceIpV4": List[IpFilterTypeDef],
+        "NetworkSourceIpV6": List[IpFilterTypeDef],
+        "NetworkSourcePort": List[NumberFilterTypeDef],
+        "NetworkSourceDomain": List[StringFilterTypeDef],
+        "NetworkSourceMac": List[StringFilterTypeDef],
+        "NetworkDestinationIpV4": List[IpFilterTypeDef],
+        "NetworkDestinationIpV6": List[IpFilterTypeDef],
+        "NetworkDestinationPort": List[NumberFilterTypeDef],
+        "NetworkDestinationDomain": List[StringFilterTypeDef],
+        "ProcessName": List[StringFilterTypeDef],
+        "ProcessPath": List[StringFilterTypeDef],
+        "ProcessPid": List[NumberFilterTypeDef],
+        "ProcessParentPid": List[NumberFilterTypeDef],
+        "ProcessLaunchedAt": List[DateFilterTypeDef],
+        "ProcessTerminatedAt": List[DateFilterTypeDef],
+        "ThreatIntelIndicatorType": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorValue": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorCategory": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorLastObservedAt": List[DateFilterTypeDef],
+        "ThreatIntelIndicatorSource": List[StringFilterTypeDef],
+        "ThreatIntelIndicatorSourceUrl": List[StringFilterTypeDef],
+        "ResourceType": List[StringFilterTypeDef],
+        "ResourceId": List[StringFilterTypeDef],
+        "ResourcePartition": List[StringFilterTypeDef],
+        "ResourceRegion": List[StringFilterTypeDef],
+        "ResourceTags": List[MapFilterTypeDef],
+        "ResourceAwsEc2InstanceType": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceImageId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceIpV4Addresses": List[IpFilterTypeDef],
+        "ResourceAwsEc2InstanceIpV6Addresses": List[IpFilterTypeDef],
+        "ResourceAwsEc2InstanceKeyName": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceIamInstanceProfileArn": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceVpcId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceSubnetId": List[StringFilterTypeDef],
+        "ResourceAwsEc2InstanceLaunchedAt": List[DateFilterTypeDef],
+        "ResourceAwsS3BucketOwnerId": List[StringFilterTypeDef],
+        "ResourceAwsS3BucketOwnerName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyUserName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyPrincipalName": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyStatus": List[StringFilterTypeDef],
+        "ResourceAwsIamAccessKeyCreatedAt": List[DateFilterTypeDef],
+        "ResourceAwsIamUserUserName": List[StringFilterTypeDef],
+        "ResourceContainerName": List[StringFilterTypeDef],
+        "ResourceContainerImageId": List[StringFilterTypeDef],
+        "ResourceContainerImageName": List[StringFilterTypeDef],
+        "ResourceContainerLaunchedAt": List[DateFilterTypeDef],
+        "ResourceDetailsOther": List[MapFilterTypeDef],
+        "ComplianceStatus": List[StringFilterTypeDef],
+        "VerificationState": List[StringFilterTypeDef],
+        "WorkflowState": List[StringFilterTypeDef],
+        "WorkflowStatus": List[StringFilterTypeDef],
+        "RecordState": List[StringFilterTypeDef],
+        "RelatedFindingsProductArn": List[StringFilterTypeDef],
+        "RelatedFindingsId": List[StringFilterTypeDef],
+        "NoteText": List[StringFilterTypeDef],
+        "NoteUpdatedAt": List[DateFilterTypeDef],
+        "NoteUpdatedBy": List[StringFilterTypeDef],
+        "Keyword": List[KeywordFilterTypeDef],
+        "FindingProviderFieldsConfidence": List[NumberFilterTypeDef],
+        "FindingProviderFieldsCriticality": List[NumberFilterTypeDef],
+        "FindingProviderFieldsRelatedFindingsId": List[StringFilterTypeDef],
+        "FindingProviderFieldsRelatedFindingsProductArn": List[StringFilterTypeDef],
+        "FindingProviderFieldsSeverityLabel": List[StringFilterTypeDef],
+        "FindingProviderFieldsSeverityOriginal": List[StringFilterTypeDef],
+        "FindingProviderFieldsTypes": List[StringFilterTypeDef],
+        "Sample": List[BooleanFilterTypeDef],
+        "ComplianceSecurityControlId": List[StringFilterTypeDef],
+        "ComplianceAssociatedStandardsId": List[StringFilterTypeDef],
+    },
+    total=False,
+)
+
 AwsSecurityFindingFiltersTypeDef = TypedDict(
     "AwsSecurityFindingFiltersTypeDef",
     {
         "ProductArn": Sequence[StringFilterTypeDef],
         "AwsAccountId": Sequence[StringFilterTypeDef],
         "Id": Sequence[StringFilterTypeDef],
         "GeneratorId": Sequence[StringFilterTypeDef],
@@ -15057,19 +10997,19 @@
     },
     total=False,
 )
 
 OccurrencesOutputTypeDef = TypedDict(
     "OccurrencesOutputTypeDef",
     {
-        "LineRanges": List[RangeOutputTypeDef],
-        "OffsetRanges": List[RangeOutputTypeDef],
-        "Pages": List[PageOutputTypeDef],
-        "Records": List[RecordOutputTypeDef],
-        "Cells": List[CellOutputTypeDef],
+        "LineRanges": List[RangeTypeDef],
+        "OffsetRanges": List[RangeTypeDef],
+        "Pages": List[PageTypeDef],
+        "Records": List[RecordTypeDef],
+        "Cells": List[CellTypeDef],
     },
     total=False,
 )
 
 OccurrencesTypeDef = TypedDict(
     "OccurrencesTypeDef",
     {
@@ -15105,31 +11045,14 @@
     {
         "Standards": List[StandardTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "BatchGetStandardsControlAssociationsResponseTypeDef",
-    {
-        "StandardsControlAssociationDetails": List[StandardsControlAssociationDetailTypeDef],
-        "UnprocessedAssociations": List[UnprocessedStandardsControlAssociationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-BatchUpdateStandardsControlAssociationsResponseTypeDef = TypedDict(
-    "BatchUpdateStandardsControlAssociationsResponseTypeDef",
-    {
-        "UnprocessedAssociationUpdates": List[UnprocessedStandardsControlAssociationUpdateTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 BatchDisableStandardsResponseTypeDef = TypedDict(
     "BatchDisableStandardsResponseTypeDef",
     {
         "StandardsSubscriptions": List[StandardsSubscriptionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -15166,40 +11089,29 @@
     },
     total=False,
 )
 
 PortProbeActionOutputTypeDef = TypedDict(
     "PortProbeActionOutputTypeDef",
     {
-        "PortProbeDetails": List[PortProbeDetailOutputTypeDef],
+        "PortProbeDetails": List[PortProbeDetailTypeDef],
         "Blocked": bool,
     },
     total=False,
 )
 
 PortProbeActionTypeDef = TypedDict(
     "PortProbeActionTypeDef",
     {
         "PortProbeDetails": Sequence[PortProbeDetailTypeDef],
         "Blocked": bool,
     },
     total=False,
 )
 
-AwsAthenaWorkGroupDetailsOutputTypeDef = TypedDict(
-    "AwsAthenaWorkGroupDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "State": str,
-        "Configuration": AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsAthenaWorkGroupDetailsTypeDef = TypedDict(
     "AwsAthenaWorkGroupDetailsTypeDef",
     {
         "Name": str,
         "Description": str,
         "State": str,
         "Configuration": AwsAthenaWorkGroupConfigurationDetailsTypeDef,
@@ -15215,18 +11127,18 @@
         "HealthCheckType": str,
         "HealthCheckGracePeriod": int,
         "CreatedTime": str,
         "MixedInstancesPolicy": (
             AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef
         ),
         "AvailabilityZones": List[
-            AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef
+            AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef
         ],
         "LaunchTemplate": (
-            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef
+            AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef
         ),
         "CapacityRebalance": bool,
     },
     total=False,
 )
 
 AwsAutoScalingAutoScalingGroupDetailsTypeDef = TypedDict(
@@ -15276,25 +11188,25 @@
     {
         "CertificateAuthorityArn": str,
         "CreatedAt": str,
         "DomainName": str,
         "DomainValidationOptions": List[
             AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef
         ],
-        "ExtendedKeyUsages": List[AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef],
+        "ExtendedKeyUsages": List[AwsCertificateManagerCertificateExtendedKeyUsageTypeDef],
         "FailureReason": str,
         "ImportedAt": str,
         "InUseBy": List[str],
         "IssuedAt": str,
         "Issuer": str,
         "KeyAlgorithm": str,
-        "KeyUsages": List[AwsCertificateManagerCertificateKeyUsageOutputTypeDef],
+        "KeyUsages": List[AwsCertificateManagerCertificateKeyUsageTypeDef],
         "NotAfter": str,
         "NotBefore": str,
-        "Options": AwsCertificateManagerCertificateOptionsOutputTypeDef,
+        "Options": AwsCertificateManagerCertificateOptionsTypeDef,
         "RenewalEligibility": str,
         "RenewalSummary": AwsCertificateManagerCertificateRenewalSummaryOutputTypeDef,
         "Serial": str,
         "SignatureAlgorithm": str,
         "Status": str,
         "Subject": str,
         "SubjectAlternativeNames": List[str],
@@ -15366,29 +11278,29 @@
     },
     total=False,
 )
 
 AwsDynamoDbTableDetailsOutputTypeDef = TypedDict(
     "AwsDynamoDbTableDetailsOutputTypeDef",
     {
-        "AttributeDefinitions": List[AwsDynamoDbTableAttributeDefinitionOutputTypeDef],
-        "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryOutputTypeDef,
+        "AttributeDefinitions": List[AwsDynamoDbTableAttributeDefinitionTypeDef],
+        "BillingModeSummary": AwsDynamoDbTableBillingModeSummaryTypeDef,
         "CreationDateTime": str,
         "GlobalSecondaryIndexes": List[AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef],
         "GlobalTableVersion": str,
         "ItemCount": int,
-        "KeySchema": List[AwsDynamoDbTableKeySchemaOutputTypeDef],
+        "KeySchema": List[AwsDynamoDbTableKeySchemaTypeDef],
         "LatestStreamArn": str,
         "LatestStreamLabel": str,
         "LocalSecondaryIndexes": List[AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef],
-        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
+        "ProvisionedThroughput": AwsDynamoDbTableProvisionedThroughputTypeDef,
         "Replicas": List[AwsDynamoDbTableReplicaOutputTypeDef],
-        "RestoreSummary": AwsDynamoDbTableRestoreSummaryOutputTypeDef,
-        "SseDescription": AwsDynamoDbTableSseDescriptionOutputTypeDef,
-        "StreamSpecification": AwsDynamoDbTableStreamSpecificationOutputTypeDef,
+        "RestoreSummary": AwsDynamoDbTableRestoreSummaryTypeDef,
+        "SseDescription": AwsDynamoDbTableSseDescriptionTypeDef,
+        "StreamSpecification": AwsDynamoDbTableStreamSpecificationTypeDef,
         "TableId": str,
         "TableName": str,
         "TableSizeBytes": int,
         "TableStatus": str,
     },
     total=False,
 )
@@ -15445,18 +11357,18 @@
 
 AwsEcsClusterDetailsOutputTypeDef = TypedDict(
     "AwsEcsClusterDetailsOutputTypeDef",
     {
         "ClusterArn": str,
         "ActiveServicesCount": int,
         "CapacityProviders": List[str],
-        "ClusterSettings": List[AwsEcsClusterClusterSettingsDetailsOutputTypeDef],
-        "Configuration": AwsEcsClusterConfigurationDetailsOutputTypeDef,
+        "ClusterSettings": List[AwsEcsClusterClusterSettingsDetailsTypeDef],
+        "Configuration": AwsEcsClusterConfigurationDetailsTypeDef,
         "DefaultCapacityProviderStrategy": List[
-            AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef
+            AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef
         ],
         "ClusterName": str,
         "RegisteredContainerInstancesCount": int,
         "RunningTasksCount": int,
         "Status": str,
     },
     total=False,
@@ -15484,22 +11396,20 @@
 AwsEcsTaskDefinitionDetailsOutputTypeDef = TypedDict(
     "AwsEcsTaskDefinitionDetailsOutputTypeDef",
     {
         "ContainerDefinitions": List[AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef],
         "Cpu": str,
         "ExecutionRoleArn": str,
         "Family": str,
-        "InferenceAccelerators": List[
-            AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef
-        ],
+        "InferenceAccelerators": List[AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef],
         "IpcMode": str,
         "Memory": str,
         "NetworkMode": str,
         "PidMode": str,
-        "PlacementConstraints": List[AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef],
+        "PlacementConstraints": List[AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef],
         "ProxyConfiguration": AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
         "RequiresCompatibilities": List[str],
         "TaskRoleArn": str,
         "Volumes": List[AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef],
     },
     total=False,
 )
@@ -15521,27 +11431,14 @@
         "RequiresCompatibilities": Sequence[str],
         "TaskRoleArn": str,
         "Volumes": Sequence[AwsEcsTaskDefinitionVolumesDetailsTypeDef],
     },
     total=False,
 )
 
-AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef = TypedDict(
-    "AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef",
-    {
-        "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef,
-        "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef,
-        "FlowLogs": AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef,
-        "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef,
-        "MalwareProtection": AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef,
-        "S3Logs": AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsGuardDutyDetectorDataSourcesDetailsTypeDef = TypedDict(
     "AwsGuardDutyDetectorDataSourcesDetailsTypeDef",
     {
         "CloudTrail": AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
         "DnsLogs": AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
         "FlowLogs": AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
         "Kubernetes": AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
@@ -15550,70 +11447,70 @@
     },
     total=False,
 )
 
 AwsRdsDbInstanceDetailsOutputTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsOutputTypeDef",
     {
-        "AssociatedRoles": List[AwsRdsDbInstanceAssociatedRoleOutputTypeDef],
+        "AssociatedRoles": List[AwsRdsDbInstanceAssociatedRoleTypeDef],
         "CACertificateIdentifier": str,
         "DBClusterIdentifier": str,
         "DBInstanceIdentifier": str,
         "DBInstanceClass": str,
         "DbInstancePort": int,
         "DbiResourceId": str,
         "DBName": str,
         "DeletionProtection": bool,
-        "Endpoint": AwsRdsDbInstanceEndpointOutputTypeDef,
+        "Endpoint": AwsRdsDbInstanceEndpointTypeDef,
         "Engine": str,
         "EngineVersion": str,
         "IAMDatabaseAuthenticationEnabled": bool,
         "InstanceCreateTime": str,
         "KmsKeyId": str,
         "PubliclyAccessible": bool,
         "StorageEncrypted": bool,
         "TdeCredentialArn": str,
-        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef],
+        "VpcSecurityGroups": List[AwsRdsDbInstanceVpcSecurityGroupTypeDef],
         "MultiAz": bool,
         "EnhancedMonitoringResourceArn": str,
         "DbInstanceStatus": str,
         "MasterUsername": str,
         "AllocatedStorage": int,
         "PreferredBackupWindow": str,
         "BackupRetentionPeriod": int,
         "DbSecurityGroups": List[str],
-        "DbParameterGroups": List[AwsRdsDbParameterGroupOutputTypeDef],
+        "DbParameterGroups": List[AwsRdsDbParameterGroupTypeDef],
         "AvailabilityZone": str,
         "DbSubnetGroup": AwsRdsDbSubnetGroupOutputTypeDef,
         "PreferredMaintenanceWindow": str,
         "PendingModifiedValues": AwsRdsDbPendingModifiedValuesOutputTypeDef,
         "LatestRestorableTime": str,
         "AutoMinorVersionUpgrade": bool,
         "ReadReplicaSourceDBInstanceIdentifier": str,
         "ReadReplicaDBInstanceIdentifiers": List[str],
         "ReadReplicaDBClusterIdentifiers": List[str],
         "LicenseModel": str,
         "Iops": int,
-        "OptionGroupMemberships": List[AwsRdsDbOptionGroupMembershipOutputTypeDef],
+        "OptionGroupMemberships": List[AwsRdsDbOptionGroupMembershipTypeDef],
         "CharacterSetName": str,
         "SecondaryAvailabilityZone": str,
-        "StatusInfos": List[AwsRdsDbStatusInfoOutputTypeDef],
+        "StatusInfos": List[AwsRdsDbStatusInfoTypeDef],
         "StorageType": str,
-        "DomainMemberships": List[AwsRdsDbDomainMembershipOutputTypeDef],
+        "DomainMemberships": List[AwsRdsDbDomainMembershipTypeDef],
         "CopyTagsToSnapshot": bool,
         "MonitoringInterval": int,
         "MonitoringRoleArn": str,
         "PromotionTier": int,
         "Timezone": str,
         "PerformanceInsightsEnabled": bool,
         "PerformanceInsightsKmsKeyId": str,
         "PerformanceInsightsRetentionPeriod": int,
         "EnabledCloudWatchLogsExports": List[str],
-        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureOutputTypeDef],
-        "ListenerEndpoint": AwsRdsDbInstanceEndpointOutputTypeDef,
+        "ProcessorFeatures": List[AwsRdsDbProcessorFeatureTypeDef],
+        "ListenerEndpoint": AwsRdsDbInstanceEndpointTypeDef,
         "MaxAllocatedStorage": int,
     },
     total=False,
 )
 
 AwsRdsDbInstanceDetailsTypeDef = TypedDict(
     "AwsRdsDbInstanceDetailsTypeDef",
@@ -15724,15 +11621,15 @@
     {
         "Label": str,
         "LoggingConfiguration": AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
         "Name": str,
         "RoleArn": str,
         "StateMachineArn": str,
         "Status": str,
-        "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef,
+        "TracingConfiguration": AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
         "Type": str,
     },
     total=False,
 )
 
 AwsStepFunctionStateMachineDetailsTypeDef = TypedDict(
     "AwsStepFunctionStateMachineDetailsTypeDef",
@@ -15803,24 +11700,14 @@
         "CreatedAt": datetime,
         "UpdatedAt": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
-InsightTypeDef = TypedDict(
-    "InsightTypeDef",
-    {
-        "InsightArn": str,
-        "Name": str,
-        "Filters": AwsSecurityFindingFiltersOutputTypeDef,
-        "GroupByAttribute": str,
-    },
-)
-
 _RequiredCreateAutomationRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutomationRuleRequestRequestTypeDef",
     {
         "RuleOrder": int,
         "RuleName": str,
         "Description": str,
         "Criteria": AutomationRulesFindingFiltersTypeDef,
@@ -15865,14 +11752,24 @@
 
 class UpdateAutomationRulesRequestItemTypeDef(
     _RequiredUpdateAutomationRulesRequestItemTypeDef,
     _OptionalUpdateAutomationRulesRequestItemTypeDef,
 ):
     pass
 
+InsightTypeDef = TypedDict(
+    "InsightTypeDef",
+    {
+        "InsightArn": str,
+        "Name": str,
+        "Filters": AwsSecurityFindingFiltersOutputTypeDef,
+        "GroupByAttribute": str,
+    },
+)
+
 CreateInsightRequestRequestTypeDef = TypedDict(
     "CreateInsightRequestRequestTypeDef",
     {
         "Name": str,
         "Filters": AwsSecurityFindingFiltersTypeDef,
         "GroupByAttribute": str,
     },
@@ -16058,17 +11955,17 @@
     total=False,
 )
 
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
         "ActionType": str,
-        "NetworkConnectionAction": NetworkConnectionActionOutputTypeDef,
+        "NetworkConnectionAction": NetworkConnectionActionTypeDef,
         "AwsApiCallAction": AwsApiCallActionOutputTypeDef,
-        "DnsRequestAction": DnsRequestActionOutputTypeDef,
+        "DnsRequestAction": DnsRequestActionTypeDef,
         "PortProbeAction": PortProbeActionOutputTypeDef,
     },
     total=False,
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
@@ -16104,23 +12001,23 @@
     total=False,
 )
 
 AwsCloudFrontDistributionDetailsOutputTypeDef = TypedDict(
     "AwsCloudFrontDistributionDetailsOutputTypeDef",
     {
         "CacheBehaviors": AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
-        "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef,
+        "DefaultCacheBehavior": AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
         "DefaultRootObject": str,
         "DomainName": str,
         "ETag": str,
         "LastModifiedTime": str,
-        "Logging": AwsCloudFrontDistributionLoggingOutputTypeDef,
+        "Logging": AwsCloudFrontDistributionLoggingTypeDef,
         "Origins": AwsCloudFrontDistributionOriginsOutputTypeDef,
         "OriginGroups": AwsCloudFrontDistributionOriginGroupsOutputTypeDef,
-        "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateOutputTypeDef,
+        "ViewerCertificate": AwsCloudFrontDistributionViewerCertificateTypeDef,
         "Status": str,
         "WebAclId": str,
     },
     total=False,
 )
 
 AwsCloudFrontDistributionDetailsTypeDef = TypedDict(
@@ -16141,16 +12038,16 @@
     },
     total=False,
 )
 
 AwsGuardDutyDetectorDetailsOutputTypeDef = TypedDict(
     "AwsGuardDutyDetectorDetailsOutputTypeDef",
     {
-        "DataSources": AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef,
-        "Features": List[AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef],
+        "DataSources": AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
+        "Features": List[AwsGuardDutyDetectorFeaturesDetailsTypeDef],
         "FindingPublishingFrequency": str,
         "ServiceRole": str,
         "Status": str,
     },
     total=False,
 )
 
@@ -16165,29 +12062,29 @@
     },
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef",
     {
-        "AbortIncompleteMultipartUpload": AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef,
+        "AbortIncompleteMultipartUpload": (
+            AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef
+        ),
         "ExpirationDate": str,
         "ExpirationInDays": int,
         "ExpiredObjectDeleteMarker": bool,
         "Filter": AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
         "ID": str,
         "NoncurrentVersionExpirationInDays": int,
         "NoncurrentVersionTransitions": List[
-            AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef
+            AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef
         ],
         "Prefix": str,
         "Status": str,
-        "Transitions": List[
-            AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef
-        ],
+        "Transitions": List[AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef],
     },
     total=False,
 )
 
 AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef = TypedDict(
     "AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef",
     {
@@ -16231,15 +12128,15 @@
 AwsWafv2RulesDetailsOutputTypeDef = TypedDict(
     "AwsWafv2RulesDetailsOutputTypeDef",
     {
         "Action": AwsWafv2RulesActionDetailsOutputTypeDef,
         "Name": str,
         "OverrideAction": str,
         "Priority": int,
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
     },
     total=False,
 )
 
 AwsWafv2RulesDetailsTypeDef = TypedDict(
     "AwsWafv2RulesDetailsTypeDef",
     {
@@ -16257,30 +12154,30 @@
     {
         "Rules": List[AutomationRulesConfigTypeDef],
         "UnprocessedAutomationRules": List[UnprocessedAutomationRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchUpdateAutomationRulesRequestRequestTypeDef = TypedDict(
+    "BatchUpdateAutomationRulesRequestRequestTypeDef",
+    {
+        "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
+    },
+)
+
 GetInsightsResponseTypeDef = TypedDict(
     "GetInsightsResponseTypeDef",
     {
         "Insights": List[InsightTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchUpdateAutomationRulesRequestRequestTypeDef = TypedDict(
-    "BatchUpdateAutomationRulesRequestRequestTypeDef",
-    {
-        "UpdateAutomationRulesRequestItems": Sequence[UpdateAutomationRulesRequestItemTypeDef],
-    },
-)
-
 CustomDataIdentifiersResultOutputTypeDef = TypedDict(
     "CustomDataIdentifiersResultOutputTypeDef",
     {
         "Detections": List[CustomDataIdentifiersDetectionsOutputTypeDef],
         "TotalCount": int,
     },
     total=False,
@@ -16315,21 +12212,21 @@
     total=False,
 )
 
 FirewallPolicyDetailsOutputTypeDef = TypedDict(
     "FirewallPolicyDetailsOutputTypeDef",
     {
         "StatefulRuleGroupReferences": List[
-            FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef
+            FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef
         ],
         "StatelessCustomActions": List[FirewallPolicyStatelessCustomActionsDetailsOutputTypeDef],
         "StatelessDefaultActions": List[str],
         "StatelessFragmentDefaultActions": List[str],
         "StatelessRuleGroupReferences": List[
-            FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef
+            FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef
         ],
     },
     total=False,
 )
 
 RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef = TypedDict(
     "RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef",
@@ -16387,32 +12284,32 @@
         "Capacity": int,
         "Description": str,
         "Id": str,
         "Name": str,
         "Arn": str,
         "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
         "Scope": str,
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
     },
     total=False,
 )
 
 AwsWafv2WebAclDetailsOutputTypeDef = TypedDict(
     "AwsWafv2WebAclDetailsOutputTypeDef",
     {
         "Name": str,
         "Arn": str,
         "ManagedbyFirewallManager": bool,
         "Id": str,
         "Capacity": int,
-        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef,
+        "CaptchaConfig": AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
         "DefaultAction": AwsWafv2WebAclActionDetailsOutputTypeDef,
         "Description": str,
         "Rules": List[AwsWafv2RulesDetailsOutputTypeDef],
-        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsOutputTypeDef,
+        "VisibilityConfig": AwsWafv2VisibilityConfigDetailsTypeDef,
     },
     total=False,
 )
 
 AwsWafv2RuleGroupDetailsTypeDef = TypedDict(
     "AwsWafv2RuleGroupDetailsTypeDef",
     {
@@ -16447,15 +12344,15 @@
 
 ClassificationResultOutputTypeDef = TypedDict(
     "ClassificationResultOutputTypeDef",
     {
         "MimeType": str,
         "SizeClassified": int,
         "AdditionalOccurrences": bool,
-        "Status": ClassificationStatusOutputTypeDef,
+        "Status": ClassificationStatusTypeDef,
         "SensitiveData": List[SensitiveDataResultOutputTypeDef],
         "CustomDataIdentifiers": CustomDataIdentifiersResultOutputTypeDef,
     },
     total=False,
 )
 
 ClassificationResultTypeDef = TypedDict(
@@ -16528,21 +12425,21 @@
         "OwnerName": str,
         "OwnerAccountId": str,
         "CreatedAt": str,
         "ServerSideEncryptionConfiguration": (
             AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef
         ),
         "BucketLifecycleConfiguration": AwsS3BucketBucketLifecycleConfigurationDetailsOutputTypeDef,
-        "PublicAccessBlockConfiguration": AwsS3AccountPublicAccessBlockDetailsOutputTypeDef,
+        "PublicAccessBlockConfiguration": AwsS3AccountPublicAccessBlockDetailsTypeDef,
         "AccessControlList": str,
-        "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationOutputTypeDef,
+        "BucketLoggingConfiguration": AwsS3BucketLoggingConfigurationTypeDef,
         "BucketWebsiteConfiguration": AwsS3BucketWebsiteConfigurationOutputTypeDef,
         "BucketNotificationConfiguration": AwsS3BucketNotificationConfigurationOutputTypeDef,
-        "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationOutputTypeDef,
-        "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationOutputTypeDef,
+        "BucketVersioningConfiguration": AwsS3BucketBucketVersioningConfigurationTypeDef,
+        "ObjectLockConfiguration": AwsS3BucketObjectLockConfigurationTypeDef,
     },
     total=False,
 )
 
 AwsS3BucketDetailsTypeDef = TypedDict(
     "AwsS3BucketDetailsTypeDef",
     {
@@ -16634,45 +12531,45 @@
         "AwsCodeBuildProject": AwsCodeBuildProjectDetailsOutputTypeDef,
         "AwsCloudFrontDistribution": AwsCloudFrontDistributionDetailsOutputTypeDef,
         "AwsEc2Instance": AwsEc2InstanceDetailsOutputTypeDef,
         "AwsEc2NetworkInterface": AwsEc2NetworkInterfaceDetailsOutputTypeDef,
         "AwsEc2SecurityGroup": AwsEc2SecurityGroupDetailsOutputTypeDef,
         "AwsEc2Volume": AwsEc2VolumeDetailsOutputTypeDef,
         "AwsEc2Vpc": AwsEc2VpcDetailsOutputTypeDef,
-        "AwsEc2Eip": AwsEc2EipDetailsOutputTypeDef,
+        "AwsEc2Eip": AwsEc2EipDetailsTypeDef,
         "AwsEc2Subnet": AwsEc2SubnetDetailsOutputTypeDef,
         "AwsEc2NetworkAcl": AwsEc2NetworkAclDetailsOutputTypeDef,
         "AwsElbv2LoadBalancer": AwsElbv2LoadBalancerDetailsOutputTypeDef,
         "AwsElasticBeanstalkEnvironment": AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
         "AwsElasticsearchDomain": AwsElasticsearchDomainDetailsOutputTypeDef,
         "AwsS3Bucket": AwsS3BucketDetailsOutputTypeDef,
-        "AwsS3AccountPublicAccessBlock": AwsS3AccountPublicAccessBlockDetailsOutputTypeDef,
-        "AwsS3Object": AwsS3ObjectDetailsOutputTypeDef,
-        "AwsSecretsManagerSecret": AwsSecretsManagerSecretDetailsOutputTypeDef,
-        "AwsIamAccessKey": AwsIamAccessKeyDetailsOutputTypeDef,
+        "AwsS3AccountPublicAccessBlock": AwsS3AccountPublicAccessBlockDetailsTypeDef,
+        "AwsS3Object": AwsS3ObjectDetailsTypeDef,
+        "AwsSecretsManagerSecret": AwsSecretsManagerSecretDetailsTypeDef,
+        "AwsIamAccessKey": AwsIamAccessKeyDetailsTypeDef,
         "AwsIamUser": AwsIamUserDetailsOutputTypeDef,
         "AwsIamPolicy": AwsIamPolicyDetailsOutputTypeDef,
         "AwsApiGatewayV2Stage": AwsApiGatewayV2StageDetailsOutputTypeDef,
         "AwsApiGatewayV2Api": AwsApiGatewayV2ApiDetailsOutputTypeDef,
         "AwsDynamoDbTable": AwsDynamoDbTableDetailsOutputTypeDef,
         "AwsApiGatewayStage": AwsApiGatewayStageDetailsOutputTypeDef,
         "AwsApiGatewayRestApi": AwsApiGatewayRestApiDetailsOutputTypeDef,
-        "AwsCloudTrailTrail": AwsCloudTrailTrailDetailsOutputTypeDef,
-        "AwsSsmPatchCompliance": AwsSsmPatchComplianceDetailsOutputTypeDef,
+        "AwsCloudTrailTrail": AwsCloudTrailTrailDetailsTypeDef,
+        "AwsSsmPatchCompliance": AwsSsmPatchComplianceDetailsTypeDef,
         "AwsCertificateManagerCertificate": AwsCertificateManagerCertificateDetailsOutputTypeDef,
         "AwsRedshiftCluster": AwsRedshiftClusterDetailsOutputTypeDef,
         "AwsElbLoadBalancer": AwsElbLoadBalancerDetailsOutputTypeDef,
         "AwsIamGroup": AwsIamGroupDetailsOutputTypeDef,
         "AwsIamRole": AwsIamRoleDetailsOutputTypeDef,
-        "AwsKmsKey": AwsKmsKeyDetailsOutputTypeDef,
+        "AwsKmsKey": AwsKmsKeyDetailsTypeDef,
         "AwsLambdaFunction": AwsLambdaFunctionDetailsOutputTypeDef,
         "AwsLambdaLayerVersion": AwsLambdaLayerVersionDetailsOutputTypeDef,
         "AwsRdsDbInstance": AwsRdsDbInstanceDetailsOutputTypeDef,
         "AwsSnsTopic": AwsSnsTopicDetailsOutputTypeDef,
-        "AwsSqsQueue": AwsSqsQueueDetailsOutputTypeDef,
+        "AwsSqsQueue": AwsSqsQueueDetailsTypeDef,
         "AwsWafWebAcl": AwsWafWebAclDetailsOutputTypeDef,
         "AwsRdsDbSnapshot": AwsRdsDbSnapshotDetailsOutputTypeDef,
         "AwsRdsDbClusterSnapshot": AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
         "AwsRdsDbCluster": AwsRdsDbClusterDetailsOutputTypeDef,
         "AwsEcsCluster": AwsEcsClusterDetailsOutputTypeDef,
         "AwsEcsContainer": AwsEcsContainerDetailsOutputTypeDef,
         "AwsEcsTaskDefinition": AwsEcsTaskDefinitionDetailsOutputTypeDef,
@@ -16681,49 +12578,49 @@
         "AwsRdsEventSubscription": AwsRdsEventSubscriptionDetailsOutputTypeDef,
         "AwsEcsService": AwsEcsServiceDetailsOutputTypeDef,
         "AwsAutoScalingLaunchConfiguration": AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
         "AwsEc2VpnConnection": AwsEc2VpnConnectionDetailsOutputTypeDef,
         "AwsEcrContainerImage": AwsEcrContainerImageDetailsOutputTypeDef,
         "AwsOpenSearchServiceDomain": AwsOpenSearchServiceDomainDetailsOutputTypeDef,
         "AwsEc2VpcEndpointService": AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
-        "AwsXrayEncryptionConfig": AwsXrayEncryptionConfigDetailsOutputTypeDef,
+        "AwsXrayEncryptionConfig": AwsXrayEncryptionConfigDetailsTypeDef,
         "AwsWafRateBasedRule": AwsWafRateBasedRuleDetailsOutputTypeDef,
         "AwsWafRegionalRateBasedRule": AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
-        "AwsEcrRepository": AwsEcrRepositoryDetailsOutputTypeDef,
+        "AwsEcrRepository": AwsEcrRepositoryDetailsTypeDef,
         "AwsEksCluster": AwsEksClusterDetailsOutputTypeDef,
         "AwsNetworkFirewallFirewallPolicy": AwsNetworkFirewallFirewallPolicyDetailsOutputTypeDef,
         "AwsNetworkFirewallFirewall": AwsNetworkFirewallFirewallDetailsOutputTypeDef,
         "AwsNetworkFirewallRuleGroup": AwsNetworkFirewallRuleGroupDetailsOutputTypeDef,
         "AwsRdsDbSecurityGroup": AwsRdsDbSecurityGroupDetailsOutputTypeDef,
-        "AwsKinesisStream": AwsKinesisStreamDetailsOutputTypeDef,
+        "AwsKinesisStream": AwsKinesisStreamDetailsTypeDef,
         "AwsEc2TransitGateway": AwsEc2TransitGatewayDetailsOutputTypeDef,
         "AwsEfsAccessPoint": AwsEfsAccessPointDetailsOutputTypeDef,
         "AwsCloudFormationStack": AwsCloudFormationStackDetailsOutputTypeDef,
         "AwsCloudWatchAlarm": AwsCloudWatchAlarmDetailsOutputTypeDef,
         "AwsEc2VpcPeeringConnection": AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
         "AwsWafRegionalRuleGroup": AwsWafRegionalRuleGroupDetailsOutputTypeDef,
         "AwsWafRegionalRule": AwsWafRegionalRuleDetailsOutputTypeDef,
         "AwsWafRegionalWebAcl": AwsWafRegionalWebAclDetailsOutputTypeDef,
         "AwsWafRule": AwsWafRuleDetailsOutputTypeDef,
         "AwsWafRuleGroup": AwsWafRuleGroupDetailsOutputTypeDef,
         "AwsEcsTask": AwsEcsTaskDetailsOutputTypeDef,
         "AwsBackupBackupVault": AwsBackupBackupVaultDetailsOutputTypeDef,
         "AwsBackupBackupPlan": AwsBackupBackupPlanDetailsOutputTypeDef,
-        "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsOutputTypeDef,
+        "AwsBackupRecoveryPoint": AwsBackupRecoveryPointDetailsTypeDef,
         "AwsEc2LaunchTemplate": AwsEc2LaunchTemplateDetailsOutputTypeDef,
         "AwsSageMakerNotebookInstance": AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
         "AwsWafv2WebAcl": AwsWafv2WebAclDetailsOutputTypeDef,
         "AwsWafv2RuleGroup": AwsWafv2RuleGroupDetailsOutputTypeDef,
         "AwsEc2RouteTable": AwsEc2RouteTableDetailsOutputTypeDef,
         "AwsAmazonMqBroker": AwsAmazonMqBrokerDetailsOutputTypeDef,
         "AwsAppSyncGraphQlApi": AwsAppSyncGraphQlApiDetailsOutputTypeDef,
-        "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsOutputTypeDef,
+        "AwsEventSchemasRegistry": AwsEventSchemasRegistryDetailsTypeDef,
         "AwsGuardDutyDetector": AwsGuardDutyDetectorDetailsOutputTypeDef,
         "AwsStepFunctionStateMachine": AwsStepFunctionStateMachineDetailsOutputTypeDef,
-        "AwsAthenaWorkGroup": AwsAthenaWorkGroupDetailsOutputTypeDef,
+        "AwsAthenaWorkGroup": AwsAthenaWorkGroupDetailsTypeDef,
     },
     total=False,
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
@@ -16887,36 +12784,36 @@
     {
         "ProductName": str,
         "CompanyName": str,
         "Region": str,
         "Types": List[str],
         "FirstObservedAt": str,
         "LastObservedAt": str,
-        "Severity": SeverityOutputTypeDef,
+        "Severity": SeverityTypeDef,
         "Confidence": int,
         "Criticality": int,
-        "Remediation": RemediationOutputTypeDef,
+        "Remediation": RemediationTypeDef,
         "SourceUrl": str,
         "ProductFields": Dict[str, str],
         "UserDefinedFields": Dict[str, str],
-        "Malware": List[MalwareOutputTypeDef],
-        "Network": NetworkOutputTypeDef,
+        "Malware": List[MalwareTypeDef],
+        "Network": NetworkTypeDef,
         "NetworkPath": List[NetworkPathComponentOutputTypeDef],
-        "Process": ProcessDetailsOutputTypeDef,
+        "Process": ProcessDetailsTypeDef,
         "Threats": List[ThreatOutputTypeDef],
-        "ThreatIntelIndicators": List[ThreatIntelIndicatorOutputTypeDef],
+        "ThreatIntelIndicators": List[ThreatIntelIndicatorTypeDef],
         "Compliance": ComplianceOutputTypeDef,
         "VerificationState": VerificationStateType,
         "WorkflowState": WorkflowStateType,
-        "Workflow": WorkflowOutputTypeDef,
+        "Workflow": WorkflowTypeDef,
         "RecordState": RecordStateType,
-        "RelatedFindings": List[RelatedFindingOutputTypeDef],
-        "Note": NoteOutputTypeDef,
+        "RelatedFindings": List[RelatedFindingTypeDef],
+        "Note": NoteTypeDef,
         "Vulnerabilities": List[VulnerabilityOutputTypeDef],
-        "PatchSummary": PatchSummaryOutputTypeDef,
+        "PatchSummary": PatchSummaryTypeDef,
         "Action": ActionOutputTypeDef,
         "FindingProviderFields": FindingProviderFieldsOutputTypeDef,
         "Sample": bool,
     },
     total=False,
 )
```

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/PKG-INFO` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-securityhub
-Version: 1.28.12
-Summary: Type annotations for boto3.SecurityHub 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-securityhub.svg?color=blue)](https://pypi.org/project/mypy-boto3-securityhub)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-securityhub)](https://pepy.tech/project/mypy-boto3-securityhub)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SecurityHub 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
+[boto3.SecurityHub 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/securityhub.html#SecurityHub)
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
 [mypy-boto3-securityhub docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_securityhub/).
 
 See how it helps to find and fix potential bugs:
 
@@ -418,682 +418,388 @@
 assembled to typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_securityhub.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccountDetailsTypeDef,
-    ActionLocalIpDetailsOutputTypeDef,
     ActionLocalIpDetailsTypeDef,
-    ActionLocalPortDetailsOutputTypeDef,
     ActionLocalPortDetailsTypeDef,
-    DnsRequestActionOutputTypeDef,
-    CityOutputTypeDef,
-    CountryOutputTypeDef,
-    GeoLocationOutputTypeDef,
-    IpOrganizationDetailsOutputTypeDef,
+    DnsRequestActionTypeDef,
     CityTypeDef,
     CountryTypeDef,
     GeoLocationTypeDef,
     IpOrganizationDetailsTypeDef,
-    ActionRemotePortDetailsOutputTypeDef,
     ActionRemotePortDetailsTypeDef,
     ActionTargetTypeDef,
-    DnsRequestActionTypeDef,
-    AdjustmentOutputTypeDef,
     AdjustmentTypeDef,
     AdminAccountTypeDef,
-    AssociatedStandardOutputTypeDef,
     AssociatedStandardTypeDef,
-    AssociationStateDetailsOutputTypeDef,
     AssociationStateDetailsTypeDef,
-    NoteUpdateOutputTypeDef,
-    RelatedFindingOutputTypeDef,
-    SeverityUpdateOutputTypeDef,
-    WorkflowUpdateOutputTypeDef,
     NoteUpdateTypeDef,
     RelatedFindingTypeDef,
     SeverityUpdateTypeDef,
     WorkflowUpdateTypeDef,
-    MapFilterOutputTypeDef,
-    NumberFilterOutputTypeDef,
-    StringFilterOutputTypeDef,
     MapFilterTypeDef,
     NumberFilterTypeDef,
     StringFilterTypeDef,
     AutomationRulesMetadataTypeDef,
-    AvailabilityZoneOutputTypeDef,
     AvailabilityZoneTypeDef,
-    AwsAmazonMqBrokerEncryptionOptionsDetailsOutputTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
-    AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsOutputTypeDef,
-    AwsAmazonMqBrokerUsersDetailsOutputTypeDef,
     AwsAmazonMqBrokerEncryptionOptionsDetailsTypeDef,
-    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsOutputTypeDef,
     AwsAmazonMqBrokerMaintenanceWindowStartTimeDetailsTypeDef,
     AwsAmazonMqBrokerUsersDetailsTypeDef,
-    AwsAmazonMqBrokerLogsPendingDetailsOutputTypeDef,
+    AwsAmazonMqBrokerLdapServerMetadataDetailsTypeDef,
     AwsAmazonMqBrokerLogsPendingDetailsTypeDef,
-    AwsApiCallActionDomainDetailsOutputTypeDef,
     AwsApiCallActionDomainDetailsTypeDef,
-    AwsApiGatewayAccessLogSettingsOutputTypeDef,
     AwsApiGatewayAccessLogSettingsTypeDef,
     AwsApiGatewayCanarySettingsOutputTypeDef,
     AwsApiGatewayCanarySettingsTypeDef,
     AwsApiGatewayEndpointConfigurationOutputTypeDef,
     AwsApiGatewayEndpointConfigurationTypeDef,
-    AwsApiGatewayMethodSettingsOutputTypeDef,
     AwsApiGatewayMethodSettingsTypeDef,
     AwsCorsConfigurationOutputTypeDef,
     AwsCorsConfigurationTypeDef,
-    AwsApiGatewayV2RouteSettingsOutputTypeDef,
     AwsApiGatewayV2RouteSettingsTypeDef,
-    AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsOutputTypeDef,
-    AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsOutputTypeDef,
-    AwsAppSyncGraphQlApiUserPoolConfigDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiLambdaAuthorizerConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiOpenIdConnectConfigDetailsTypeDef,
     AwsAppSyncGraphQlApiUserPoolConfigDetailsTypeDef,
-    AwsAppSyncGraphQlApiLogConfigDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiLogConfigDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationResultConfigurationEncryptionConfigurationDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupAvailabilityZonesListDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
     AwsAutoScalingAutoScalingGroupLaunchTemplateLaunchTemplateSpecificationTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyInstancesDistributionDetailsTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationOutputTypeDef,
-    AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateLaunchTemplateSpecificationTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateOverridesListDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsEbsDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsOutputTypeDef,
-    AwsAutoScalingLaunchConfigurationMetadataOptionsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationInstanceMonitoringDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationMetadataOptionsTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsOutputTypeDef,
     AwsBackupBackupPlanAdvancedBackupSettingsDetailsTypeDef,
-    AwsBackupBackupPlanLifecycleDetailsOutputTypeDef,
     AwsBackupBackupPlanLifecycleDetailsTypeDef,
     AwsBackupBackupVaultNotificationsDetailsOutputTypeDef,
     AwsBackupBackupVaultNotificationsDetailsTypeDef,
-    AwsBackupRecoveryPointCalculatedLifecycleDetailsOutputTypeDef,
     AwsBackupRecoveryPointCalculatedLifecycleDetailsTypeDef,
-    AwsBackupRecoveryPointCreatedByDetailsOutputTypeDef,
     AwsBackupRecoveryPointCreatedByDetailsTypeDef,
-    AwsBackupRecoveryPointLifecycleDetailsOutputTypeDef,
     AwsBackupRecoveryPointLifecycleDetailsTypeDef,
-    AwsCertificateManagerCertificateExtendedKeyUsageOutputTypeDef,
-    AwsCertificateManagerCertificateKeyUsageOutputTypeDef,
-    AwsCertificateManagerCertificateOptionsOutputTypeDef,
     AwsCertificateManagerCertificateExtendedKeyUsageTypeDef,
     AwsCertificateManagerCertificateKeyUsageTypeDef,
     AwsCertificateManagerCertificateOptionsTypeDef,
-    AwsCertificateManagerCertificateResourceRecordOutputTypeDef,
     AwsCertificateManagerCertificateResourceRecordTypeDef,
-    AwsCloudFormationStackDriftInformationDetailsOutputTypeDef,
-    AwsCloudFormationStackOutputsDetailsOutputTypeDef,
     AwsCloudFormationStackDriftInformationDetailsTypeDef,
     AwsCloudFormationStackOutputsDetailsTypeDef,
-    AwsCloudFrontDistributionCacheBehaviorOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorTypeDef,
-    AwsCloudFrontDistributionDefaultCacheBehaviorOutputTypeDef,
     AwsCloudFrontDistributionDefaultCacheBehaviorTypeDef,
-    AwsCloudFrontDistributionLoggingOutputTypeDef,
-    AwsCloudFrontDistributionViewerCertificateOutputTypeDef,
     AwsCloudFrontDistributionLoggingTypeDef,
     AwsCloudFrontDistributionViewerCertificateTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsOutputTypeDef,
     AwsCloudFrontDistributionOriginSslProtocolsTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverStatusCodesTypeDef,
-    AwsCloudFrontDistributionOriginS3OriginConfigOutputTypeDef,
     AwsCloudFrontDistributionOriginS3OriginConfigTypeDef,
-    AwsCloudTrailTrailDetailsOutputTypeDef,
     AwsCloudTrailTrailDetailsTypeDef,
-    AwsCloudWatchAlarmDimensionsDetailsOutputTypeDef,
     AwsCloudWatchAlarmDimensionsDetailsTypeDef,
-    AwsCodeBuildProjectArtifactsDetailsOutputTypeDef,
     AwsCodeBuildProjectArtifactsDetailsTypeDef,
-    AwsCodeBuildProjectSourceOutputTypeDef,
-    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectSourceTypeDef,
+    AwsCodeBuildProjectVpcConfigOutputTypeDef,
     AwsCodeBuildProjectVpcConfigTypeDef,
-    AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsOutputTypeDef,
     AwsCodeBuildProjectEnvironmentEnvironmentVariablesDetailsTypeDef,
-    AwsCodeBuildProjectEnvironmentRegistryCredentialOutputTypeDef,
     AwsCodeBuildProjectEnvironmentRegistryCredentialTypeDef,
-    AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigCloudWatchLogsDetailsTypeDef,
-    AwsCodeBuildProjectLogsConfigS3LogsDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigS3LogsDetailsTypeDef,
-    AwsDynamoDbTableAttributeDefinitionOutputTypeDef,
     AwsDynamoDbTableAttributeDefinitionTypeDef,
-    AwsDynamoDbTableBillingModeSummaryOutputTypeDef,
     AwsDynamoDbTableBillingModeSummaryTypeDef,
-    AwsDynamoDbTableKeySchemaOutputTypeDef,
-    AwsDynamoDbTableProvisionedThroughputOutputTypeDef,
-    AwsDynamoDbTableRestoreSummaryOutputTypeDef,
-    AwsDynamoDbTableSseDescriptionOutputTypeDef,
-    AwsDynamoDbTableStreamSpecificationOutputTypeDef,
     AwsDynamoDbTableKeySchemaTypeDef,
     AwsDynamoDbTableProvisionedThroughputTypeDef,
     AwsDynamoDbTableRestoreSummaryTypeDef,
     AwsDynamoDbTableSseDescriptionTypeDef,
     AwsDynamoDbTableStreamSpecificationTypeDef,
     AwsDynamoDbTableProjectionOutputTypeDef,
     AwsDynamoDbTableProjectionTypeDef,
-    AwsDynamoDbTableProvisionedThroughputOverrideOutputTypeDef,
     AwsDynamoDbTableProvisionedThroughputOverrideTypeDef,
-    AwsEc2EipDetailsOutputTypeDef,
     AwsEc2EipDetailsTypeDef,
-    AwsEc2InstanceMetadataOptionsOutputTypeDef,
-    AwsEc2InstanceMonitoringDetailsOutputTypeDef,
-    AwsEc2InstanceNetworkInterfacesDetailsOutputTypeDef,
     AwsEc2InstanceMetadataOptionsTypeDef,
     AwsEc2InstanceMonitoringDetailsTypeDef,
     AwsEc2InstanceNetworkInterfacesDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetEbsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationCapacityReservationTargetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCpuOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCpuOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCreditSpecificationDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCreditSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataEnclaveOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataHibernationOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataIamInstanceProfileDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataLicenseSetDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMetadataOptionsDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataMonitoringDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataPlacementDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataElasticGpuSpecificationSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataElasticInferenceAcceleratorSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataEnclaveOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataHibernationOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataIamInstanceProfileDetailsTypeDef,
     AwsEc2LaunchTemplateDataLicenseSetDetailsTypeDef,
     AwsEc2LaunchTemplateDataMaintenanceOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataMetadataOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataMonitoringDetailsTypeDef,
     AwsEc2LaunchTemplateDataPlacementDetailsTypeDef,
     AwsEc2LaunchTemplateDataPrivateDnsNameOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsSpotOptionsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsAcceleratorTotalMemoryMiBDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsBaselineEbsBandwidthMbpsDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsMemoryGiBPerVCpuDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsMemoryMiBDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsNetworkInterfaceCountDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsTotalLocalStorageGBDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsVCpuCountDetailsTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsOutputTypeDef,
-    AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv4PrefixesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6AddressesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetIpv6PrefixesDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetPrivateIpAddressesDetailsTypeDef,
-    AwsEc2NetworkAclAssociationOutputTypeDef,
     AwsEc2NetworkAclAssociationTypeDef,
-    IcmpTypeCodeOutputTypeDef,
-    PortRangeFromToOutputTypeDef,
     IcmpTypeCodeTypeDef,
     PortRangeFromToTypeDef,
-    AwsEc2NetworkInterfaceAttachmentOutputTypeDef,
     AwsEc2NetworkInterfaceAttachmentTypeDef,
-    AwsEc2NetworkInterfaceIpV6AddressDetailOutputTypeDef,
-    AwsEc2NetworkInterfacePrivateIpAddressDetailOutputTypeDef,
-    AwsEc2NetworkInterfaceSecurityGroupOutputTypeDef,
     AwsEc2NetworkInterfaceIpV6AddressDetailTypeDef,
     AwsEc2NetworkInterfacePrivateIpAddressDetailTypeDef,
     AwsEc2NetworkInterfaceSecurityGroupTypeDef,
-    PropagatingVgwSetDetailsOutputTypeDef,
-    RouteSetDetailsOutputTypeDef,
     PropagatingVgwSetDetailsTypeDef,
     RouteSetDetailsTypeDef,
-    AwsEc2SecurityGroupIpRangeOutputTypeDef,
-    AwsEc2SecurityGroupIpv6RangeOutputTypeDef,
-    AwsEc2SecurityGroupPrefixListIdOutputTypeDef,
-    AwsEc2SecurityGroupUserIdGroupPairOutputTypeDef,
     AwsEc2SecurityGroupIpRangeTypeDef,
     AwsEc2SecurityGroupIpv6RangeTypeDef,
     AwsEc2SecurityGroupPrefixListIdTypeDef,
     AwsEc2SecurityGroupUserIdGroupPairTypeDef,
-    Ipv6CidrBlockAssociationOutputTypeDef,
     Ipv6CidrBlockAssociationTypeDef,
     AwsEc2TransitGatewayDetailsOutputTypeDef,
     AwsEc2TransitGatewayDetailsTypeDef,
-    AwsEc2VolumeAttachmentOutputTypeDef,
     AwsEc2VolumeAttachmentTypeDef,
-    CidrBlockAssociationOutputTypeDef,
     CidrBlockAssociationTypeDef,
-    AwsEc2VpcEndpointServiceServiceTypeDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceServiceTypeDetailsTypeDef,
-    AwsEc2VpcPeeringConnectionStatusDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionStatusDetailsTypeDef,
-    VpcInfoCidrBlockSetDetailsOutputTypeDef,
-    VpcInfoIpv6CidrBlockSetDetailsOutputTypeDef,
-    VpcInfoPeeringOptionsDetailsOutputTypeDef,
     VpcInfoCidrBlockSetDetailsTypeDef,
     VpcInfoIpv6CidrBlockSetDetailsTypeDef,
     VpcInfoPeeringOptionsDetailsTypeDef,
-    AwsEc2VpnConnectionRoutesDetailsOutputTypeDef,
-    AwsEc2VpnConnectionVgwTelemetryDetailsOutputTypeDef,
     AwsEc2VpnConnectionRoutesDetailsTypeDef,
     AwsEc2VpnConnectionVgwTelemetryDetailsTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsTunnelOptionsDetailsTypeDef,
     AwsEcrContainerImageDetailsOutputTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
-    AwsEcrRepositoryImageScanningConfigurationDetailsOutputTypeDef,
-    AwsEcrRepositoryLifecyclePolicyDetailsOutputTypeDef,
     AwsEcrRepositoryImageScanningConfigurationDetailsTypeDef,
     AwsEcrRepositoryLifecyclePolicyDetailsTypeDef,
-    AwsEcsClusterClusterSettingsDetailsOutputTypeDef,
     AwsEcsClusterClusterSettingsDetailsTypeDef,
-    AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationLogConfigurationDetailsTypeDef,
-    AwsEcsClusterDefaultCapacityProviderStrategyDetailsOutputTypeDef,
     AwsEcsClusterDefaultCapacityProviderStrategyDetailsTypeDef,
-    AwsMountPointOutputTypeDef,
     AwsMountPointTypeDef,
-    AwsEcsServiceCapacityProviderStrategyDetailsOutputTypeDef,
     AwsEcsServiceCapacityProviderStrategyDetailsTypeDef,
-    AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsOutputTypeDef,
     AwsEcsServiceDeploymentConfigurationDeploymentCircuitBreakerDetailsTypeDef,
-    AwsEcsServiceDeploymentControllerDetailsOutputTypeDef,
     AwsEcsServiceDeploymentControllerDetailsTypeDef,
-    AwsEcsServiceLoadBalancersDetailsOutputTypeDef,
-    AwsEcsServicePlacementConstraintsDetailsOutputTypeDef,
-    AwsEcsServicePlacementStrategiesDetailsOutputTypeDef,
-    AwsEcsServiceServiceRegistriesDetailsOutputTypeDef,
     AwsEcsServiceLoadBalancersDetailsTypeDef,
     AwsEcsServicePlacementConstraintsDetailsTypeDef,
     AwsEcsServicePlacementStrategiesDetailsTypeDef,
     AwsEcsServiceServiceRegistriesDetailsTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationAwsVpcConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDependsOnDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsEnvironmentFilesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsExtraHostsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsMountPointsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsPortMappingsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsRepositoryCredentialsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsResourceRequirementsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSecretsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsSystemControlsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsUlimitsDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsVolumesFromDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsFirelensConfigurationDetailsTypeDef,
+    AwsEcsTaskDefinitionContainerDefinitionsHealthCheckDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersCapabilitiesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDevicesDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersTmpfsDetailsTypeDef,
-    AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationSecretOptionsDetailsTypeDef,
-    AwsEcsTaskDefinitionInferenceAcceleratorsDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionPlacementConstraintsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionInferenceAcceleratorsDetailsTypeDef,
     AwsEcsTaskDefinitionPlacementConstraintsDetailsTypeDef,
-    AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationProxyConfigurationPropertiesDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionVolumesHostDetailsOutputTypeDef,
-    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesHostDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsOutputTypeDef,
+    AwsEcsTaskDefinitionVolumesDockerVolumeConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationAuthorizationConfigDetailsTypeDef,
-    AwsEcsTaskVolumeHostDetailsOutputTypeDef,
     AwsEcsTaskVolumeHostDetailsTypeDef,
     AwsEfsAccessPointPosixUserDetailsOutputTypeDef,
     AwsEfsAccessPointPosixUserDetailsTypeDef,
-    AwsEfsAccessPointRootDirectoryCreationInfoDetailsOutputTypeDef,
     AwsEfsAccessPointRootDirectoryCreationInfoDetailsTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsOutputTypeDef,
     AwsEksClusterResourcesVpcConfigDetailsTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingClusterLoggingDetailsTypeDef,
-    AwsElasticBeanstalkEnvironmentEnvironmentLinkOutputTypeDef,
-    AwsElasticBeanstalkEnvironmentOptionSettingOutputTypeDef,
-    AwsElasticBeanstalkEnvironmentTierOutputTypeDef,
     AwsElasticBeanstalkEnvironmentEnvironmentLinkTypeDef,
     AwsElasticBeanstalkEnvironmentOptionSettingTypeDef,
     AwsElasticBeanstalkEnvironmentTierTypeDef,
-    AwsElasticsearchDomainDomainEndpointOptionsOutputTypeDef,
-    AwsElasticsearchDomainEncryptionAtRestOptionsOutputTypeDef,
-    AwsElasticsearchDomainNodeToNodeEncryptionOptionsOutputTypeDef,
-    AwsElasticsearchDomainServiceSoftwareOptionsOutputTypeDef,
-    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainDomainEndpointOptionsTypeDef,
     AwsElasticsearchDomainEncryptionAtRestOptionsTypeDef,
     AwsElasticsearchDomainNodeToNodeEncryptionOptionsTypeDef,
     AwsElasticsearchDomainServiceSoftwareOptionsTypeDef,
+    AwsElasticsearchDomainVPCOptionsOutputTypeDef,
     AwsElasticsearchDomainVPCOptionsTypeDef,
-    AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsOutputTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigZoneAwarenessConfigDetailsTypeDef,
-    AwsElasticsearchDomainLogPublishingOptionsLogConfigOutputTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsLogConfigTypeDef,
-    AwsElbAppCookieStickinessPolicyOutputTypeDef,
     AwsElbAppCookieStickinessPolicyTypeDef,
-    AwsElbLbCookieStickinessPolicyOutputTypeDef,
     AwsElbLbCookieStickinessPolicyTypeDef,
-    AwsElbLoadBalancerAccessLogOutputTypeDef,
     AwsElbLoadBalancerAccessLogTypeDef,
-    AwsElbLoadBalancerAdditionalAttributeOutputTypeDef,
     AwsElbLoadBalancerAdditionalAttributeTypeDef,
-    AwsElbLoadBalancerConnectionDrainingOutputTypeDef,
-    AwsElbLoadBalancerConnectionSettingsOutputTypeDef,
-    AwsElbLoadBalancerCrossZoneLoadBalancingOutputTypeDef,
     AwsElbLoadBalancerConnectionDrainingTypeDef,
     AwsElbLoadBalancerConnectionSettingsTypeDef,
     AwsElbLoadBalancerCrossZoneLoadBalancingTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionOutputTypeDef,
     AwsElbLoadBalancerBackendServerDescriptionTypeDef,
-    AwsElbLoadBalancerHealthCheckOutputTypeDef,
-    AwsElbLoadBalancerInstanceOutputTypeDef,
-    AwsElbLoadBalancerSourceSecurityGroupOutputTypeDef,
     AwsElbLoadBalancerHealthCheckTypeDef,
     AwsElbLoadBalancerInstanceTypeDef,
     AwsElbLoadBalancerSourceSecurityGroupTypeDef,
-    AwsElbLoadBalancerListenerOutputTypeDef,
     AwsElbLoadBalancerListenerTypeDef,
-    AwsElbv2LoadBalancerAttributeOutputTypeDef,
     AwsElbv2LoadBalancerAttributeTypeDef,
-    LoadBalancerStateOutputTypeDef,
     LoadBalancerStateTypeDef,
-    AwsEventSchemasRegistryDetailsOutputTypeDef,
     AwsEventSchemasRegistryDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesCloudTrailDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesCloudTrailDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesDnsLogsDetailsOutputTypeDef,
-    AwsGuardDutyDetectorDataSourcesFlowLogsDetailsOutputTypeDef,
-    AwsGuardDutyDetectorDataSourcesS3LogsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesDnsLogsDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesFlowLogsDetailsTypeDef,
     AwsGuardDutyDetectorDataSourcesS3LogsDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesAuditLogsDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsEbsVolumesDetailsTypeDef,
-    AwsGuardDutyDetectorFeaturesDetailsOutputTypeDef,
     AwsGuardDutyDetectorFeaturesDetailsTypeDef,
-    AwsIamAccessKeySessionContextAttributesOutputTypeDef,
     AwsIamAccessKeySessionContextAttributesTypeDef,
-    AwsIamAccessKeySessionContextSessionIssuerOutputTypeDef,
     AwsIamAccessKeySessionContextSessionIssuerTypeDef,
-    AwsIamAttachedManagedPolicyOutputTypeDef,
     AwsIamAttachedManagedPolicyTypeDef,
-    AwsIamGroupPolicyOutputTypeDef,
     AwsIamGroupPolicyTypeDef,
-    AwsIamInstanceProfileRoleOutputTypeDef,
     AwsIamInstanceProfileRoleTypeDef,
-    AwsIamPermissionsBoundaryOutputTypeDef,
     AwsIamPermissionsBoundaryTypeDef,
-    AwsIamPolicyVersionOutputTypeDef,
     AwsIamPolicyVersionTypeDef,
-    AwsIamRolePolicyOutputTypeDef,
     AwsIamRolePolicyTypeDef,
-    AwsIamUserPolicyOutputTypeDef,
     AwsIamUserPolicyTypeDef,
-    AwsKinesisStreamStreamEncryptionDetailsOutputTypeDef,
     AwsKinesisStreamStreamEncryptionDetailsTypeDef,
-    AwsKmsKeyDetailsOutputTypeDef,
     AwsKmsKeyDetailsTypeDef,
-    AwsLambdaFunctionCodeOutputTypeDef,
     AwsLambdaFunctionCodeTypeDef,
-    AwsLambdaFunctionDeadLetterConfigOutputTypeDef,
     AwsLambdaFunctionDeadLetterConfigTypeDef,
-    AwsLambdaFunctionLayerOutputTypeDef,
-    AwsLambdaFunctionTracingConfigOutputTypeDef,
-    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionLayerTypeDef,
     AwsLambdaFunctionTracingConfigTypeDef,
+    AwsLambdaFunctionVpcConfigOutputTypeDef,
     AwsLambdaFunctionVpcConfigTypeDef,
-    AwsLambdaFunctionEnvironmentErrorOutputTypeDef,
     AwsLambdaFunctionEnvironmentErrorTypeDef,
     AwsLambdaLayerVersionDetailsOutputTypeDef,
     AwsLambdaLayerVersionDetailsTypeDef,
-    AwsNetworkFirewallFirewallSubnetMappingsDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallSubnetMappingsDetailsTypeDef,
-    AwsOpenSearchServiceDomainMasterUserOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainMasterUserOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainClusterConfigZoneAwarenessConfigDetailsTypeDef,
-    AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsOutputTypeDef,
-    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDomainEndpointOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainEncryptionAtRestOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainNodeToNodeEncryptionOptionsDetailsTypeDef,
     AwsOpenSearchServiceDomainServiceSoftwareOptionsDetailsTypeDef,
+    AwsOpenSearchServiceDomainVpcOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainVpcOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainLogPublishingOptionOutputTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionTypeDef,
-    AwsRdsDbClusterAssociatedRoleOutputTypeDef,
     AwsRdsDbClusterAssociatedRoleTypeDef,
-    AwsRdsDbClusterMemberOutputTypeDef,
-    AwsRdsDbClusterOptionGroupMembershipOutputTypeDef,
-    AwsRdsDbDomainMembershipOutputTypeDef,
-    AwsRdsDbInstanceVpcSecurityGroupOutputTypeDef,
     AwsRdsDbClusterMemberTypeDef,
     AwsRdsDbClusterOptionGroupMembershipTypeDef,
     AwsRdsDbDomainMembershipTypeDef,
     AwsRdsDbInstanceVpcSecurityGroupTypeDef,
     AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeOutputTypeDef,
     AwsRdsDbClusterSnapshotDbClusterSnapshotAttributeTypeDef,
-    AwsRdsDbInstanceAssociatedRoleOutputTypeDef,
     AwsRdsDbInstanceAssociatedRoleTypeDef,
-    AwsRdsDbInstanceEndpointOutputTypeDef,
-    AwsRdsDbOptionGroupMembershipOutputTypeDef,
-    AwsRdsDbParameterGroupOutputTypeDef,
-    AwsRdsDbProcessorFeatureOutputTypeDef,
-    AwsRdsDbStatusInfoOutputTypeDef,
     AwsRdsDbInstanceEndpointTypeDef,
     AwsRdsDbOptionGroupMembershipTypeDef,
     AwsRdsDbParameterGroupTypeDef,
     AwsRdsDbProcessorFeatureTypeDef,
     AwsRdsDbStatusInfoTypeDef,
     AwsRdsPendingCloudWatchLogsExportsOutputTypeDef,
     AwsRdsPendingCloudWatchLogsExportsTypeDef,
-    AwsRdsDbSecurityGroupEc2SecurityGroupOutputTypeDef,
-    AwsRdsDbSecurityGroupIpRangeOutputTypeDef,
     AwsRdsDbSecurityGroupEc2SecurityGroupTypeDef,
     AwsRdsDbSecurityGroupIpRangeTypeDef,
-    AwsRdsDbSubnetGroupSubnetAvailabilityZoneOutputTypeDef,
     AwsRdsDbSubnetGroupSubnetAvailabilityZoneTypeDef,
     AwsRdsEventSubscriptionDetailsOutputTypeDef,
     AwsRdsEventSubscriptionDetailsTypeDef,
-    AwsRedshiftClusterClusterNodeOutputTypeDef,
     AwsRedshiftClusterClusterNodeTypeDef,
-    AwsRedshiftClusterClusterParameterStatusOutputTypeDef,
     AwsRedshiftClusterClusterParameterStatusTypeDef,
-    AwsRedshiftClusterClusterSecurityGroupOutputTypeDef,
     AwsRedshiftClusterClusterSecurityGroupTypeDef,
-    AwsRedshiftClusterClusterSnapshotCopyStatusOutputTypeDef,
     AwsRedshiftClusterClusterSnapshotCopyStatusTypeDef,
-    AwsRedshiftClusterDeferredMaintenanceWindowOutputTypeDef,
     AwsRedshiftClusterDeferredMaintenanceWindowTypeDef,
-    AwsRedshiftClusterElasticIpStatusOutputTypeDef,
-    AwsRedshiftClusterEndpointOutputTypeDef,
-    AwsRedshiftClusterHsmStatusOutputTypeDef,
-    AwsRedshiftClusterIamRoleOutputTypeDef,
-    AwsRedshiftClusterLoggingStatusOutputTypeDef,
-    AwsRedshiftClusterPendingModifiedValuesOutputTypeDef,
-    AwsRedshiftClusterResizeInfoOutputTypeDef,
-    AwsRedshiftClusterRestoreStatusOutputTypeDef,
-    AwsRedshiftClusterVpcSecurityGroupOutputTypeDef,
     AwsRedshiftClusterElasticIpStatusTypeDef,
     AwsRedshiftClusterEndpointTypeDef,
     AwsRedshiftClusterHsmStatusTypeDef,
     AwsRedshiftClusterIamRoleTypeDef,
     AwsRedshiftClusterLoggingStatusTypeDef,
     AwsRedshiftClusterPendingModifiedValuesTypeDef,
     AwsRedshiftClusterResizeInfoTypeDef,
     AwsRedshiftClusterRestoreStatusTypeDef,
     AwsRedshiftClusterVpcSecurityGroupTypeDef,
-    AwsS3AccountPublicAccessBlockDetailsOutputTypeDef,
     AwsS3AccountPublicAccessBlockDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesAbortIncompleteMultipartUploadDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsOutputTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesNoncurrentVersionTransitionsDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesTransitionsDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateTagDetailsTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsTagDetailsTypeDef,
-    AwsS3BucketBucketVersioningConfigurationOutputTypeDef,
     AwsS3BucketBucketVersioningConfigurationTypeDef,
-    AwsS3BucketLoggingConfigurationOutputTypeDef,
     AwsS3BucketLoggingConfigurationTypeDef,
-    AwsS3BucketNotificationConfigurationS3KeyFilterRuleOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterRuleTypeDef,
-    AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsOutputTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDefaultRetentionDetailsTypeDef,
-    AwsS3BucketServerSideEncryptionByDefaultOutputTypeDef,
     AwsS3BucketServerSideEncryptionByDefaultTypeDef,
-    AwsS3BucketWebsiteConfigurationRedirectToOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRedirectToTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleConditionOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleConditionTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleRedirectOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleRedirectTypeDef,
-    AwsS3ObjectDetailsOutputTypeDef,
     AwsS3ObjectDetailsTypeDef,
-    AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceMetadataServiceConfigurationDetailsTypeDef,
-    AwsSecretsManagerSecretRotationRulesOutputTypeDef,
     AwsSecretsManagerSecretRotationRulesTypeDef,
-    BooleanFilterOutputTypeDef,
-    IpFilterOutputTypeDef,
-    KeywordFilterOutputTypeDef,
     BooleanFilterTypeDef,
     IpFilterTypeDef,
     KeywordFilterTypeDef,
-    AwsSecurityFindingIdentifierOutputTypeDef,
     AwsSecurityFindingIdentifierTypeDef,
-    MalwareOutputTypeDef,
-    NoteOutputTypeDef,
-    PatchSummaryOutputTypeDef,
-    ProcessDetailsOutputTypeDef,
-    SeverityOutputTypeDef,
-    ThreatIntelIndicatorOutputTypeDef,
-    WorkflowOutputTypeDef,
     MalwareTypeDef,
     NoteTypeDef,
     PatchSummaryTypeDef,
     ProcessDetailsTypeDef,
     SeverityTypeDef,
     ThreatIntelIndicatorTypeDef,
     WorkflowTypeDef,
-    AwsSnsTopicSubscriptionOutputTypeDef,
     AwsSnsTopicSubscriptionTypeDef,
-    AwsSqsQueueDetailsOutputTypeDef,
     AwsSqsQueueDetailsTypeDef,
-    AwsSsmComplianceSummaryOutputTypeDef,
     AwsSsmComplianceSummaryTypeDef,
-    AwsStepFunctionStateMachineTracingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineTracingConfigurationDetailsTypeDef,
-    AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsCloudWatchLogsLogGroupDetailsTypeDef,
-    AwsWafRateBasedRuleMatchPredicateOutputTypeDef,
     AwsWafRateBasedRuleMatchPredicateTypeDef,
-    AwsWafRegionalRateBasedRuleMatchPredicateOutputTypeDef,
     AwsWafRegionalRateBasedRuleMatchPredicateTypeDef,
-    AwsWafRegionalRulePredicateListDetailsOutputTypeDef,
     AwsWafRegionalRulePredicateListDetailsTypeDef,
-    AwsWafRegionalRuleGroupRulesActionDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupRulesActionDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListActionDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListActionDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListOverrideActionDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListOverrideActionDetailsTypeDef,
-    AwsWafRulePredicateListDetailsOutputTypeDef,
     AwsWafRulePredicateListDetailsTypeDef,
-    AwsWafRuleGroupRulesActionDetailsOutputTypeDef,
     AwsWafRuleGroupRulesActionDetailsTypeDef,
-    WafActionOutputTypeDef,
-    WafExcludedRuleOutputTypeDef,
-    WafOverrideActionOutputTypeDef,
     WafActionTypeDef,
     WafExcludedRuleTypeDef,
     WafOverrideActionTypeDef,
-    AwsWafv2CustomHttpHeaderOutputTypeDef,
     AwsWafv2CustomHttpHeaderTypeDef,
-    AwsWafv2VisibilityConfigDetailsOutputTypeDef,
     AwsWafv2VisibilityConfigDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsOutputTypeDef,
     AwsWafv2WebAclCaptchaConfigImmunityTimePropertyDetailsTypeDef,
-    AwsXrayEncryptionConfigDetailsOutputTypeDef,
     AwsXrayEncryptionConfigDetailsTypeDef,
     BatchDeleteAutomationRulesRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     UnprocessedAutomationRuleTypeDef,
     BatchDisableStandardsRequestRequestTypeDef,
     StandardsSubscriptionRequestTypeDef,
     BatchGetAutomationRulesRequestRequestTypeDef,
     BatchGetSecurityControlsRequestRequestTypeDef,
     SecurityControlTypeDef,
     UnprocessedSecurityControlTypeDef,
     StandardsControlAssociationIdTypeDef,
     StandardsControlAssociationDetailTypeDef,
     ImportFindingsErrorTypeDef,
     StandardsControlAssociationUpdateTypeDef,
-    CellOutputTypeDef,
     CellTypeDef,
-    ClassificationStatusOutputTypeDef,
     ClassificationStatusTypeDef,
-    StatusReasonOutputTypeDef,
     StatusReasonTypeDef,
-    VolumeMountOutputTypeDef,
     VolumeMountTypeDef,
     CreateActionTargetRequestRequestTypeDef,
     CreateFindingAggregatorRequestRequestTypeDef,
     ResultTypeDef,
-    DateRangeOutputTypeDef,
     DateRangeTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteActionTargetRequestRequestTypeDef,
     DeleteFindingAggregatorRequestRequestTypeDef,
     DeleteInsightRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
@@ -1107,23 +813,19 @@
     DescribeStandardsRequestRequestTypeDef,
     DisableImportFindingsForProductRequestRequestTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMembersRequestRequestTypeDef,
     EnableImportFindingsForProductRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     EnableSecurityHubRequestRequestTypeDef,
-    FilePathsOutputTypeDef,
     FilePathsTypeDef,
     FindingAggregatorTypeDef,
     FindingHistoryUpdateSourceTypeDef,
     FindingHistoryUpdateTypeDef,
-    FindingProviderSeverityOutputTypeDef,
     FindingProviderSeverityTypeDef,
-    FirewallPolicyStatefulRuleGroupReferencesDetailsOutputTypeDef,
-    FirewallPolicyStatelessRuleGroupReferencesDetailsOutputTypeDef,
     FirewallPolicyStatefulRuleGroupReferencesDetailsTypeDef,
     FirewallPolicyStatelessRuleGroupReferencesDetailsTypeDef,
     InvitationTypeDef,
     GetEnabledStandardsRequestRequestTypeDef,
     GetFindingAggregatorRequestRequestTypeDef,
     SortCriterionTypeDef,
     GetInsightResultsRequestRequestTypeDef,
@@ -1139,91 +841,69 @@
     ListMembersRequestRequestTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListSecurityControlDefinitionsRequestRequestTypeDef,
     SecurityControlDefinitionTypeDef,
     ListStandardsControlAssociationsRequestRequestTypeDef,
     StandardsControlAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PortRangeOutputTypeDef,
     PortRangeTypeDef,
-    RangeOutputTypeDef,
-    RecordOutputTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    RecommendationOutputTypeDef,
     RecommendationTypeDef,
     RuleGroupSourceListDetailsOutputTypeDef,
     RuleGroupSourceListDetailsTypeDef,
-    RuleGroupSourceStatefulRulesHeaderDetailsOutputTypeDef,
-    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesHeaderDetailsTypeDef,
+    RuleGroupSourceStatefulRulesOptionsDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesOptionsDetailsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationPortsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesDestinationsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesDestinationsTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesSourcePortsOutputTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesSourcesOutputTypeDef,
-    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcePortsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesSourcesTypeDef,
+    RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTcpFlagsTypeDef,
     RuleGroupVariablesIpSetsDetailsOutputTypeDef,
     RuleGroupVariablesIpSetsDetailsTypeDef,
     RuleGroupVariablesPortSetsDetailsOutputTypeDef,
     RuleGroupVariablesPortSetsDetailsTypeDef,
-    SoftwarePackageOutputTypeDef,
     SoftwarePackageTypeDef,
     StandardsManagedByTypeDef,
-    StandardsControlAssociationIdOutputTypeDef,
-    StandardsControlAssociationUpdateOutputTypeDef,
     StandardsStatusReasonTypeDef,
-    StatelessCustomPublishMetricActionDimensionOutputTypeDef,
     StatelessCustomPublishMetricActionDimensionTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateActionTargetRequestRequestTypeDef,
     UpdateFindingAggregatorRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateSecurityHubConfigurationRequestRequestTypeDef,
     UpdateStandardsControlRequestRequestTypeDef,
-    VulnerabilityVendorOutputTypeDef,
     VulnerabilityVendorTypeDef,
     CreateMembersRequestRequestTypeDef,
-    ActionRemoteIpDetailsOutputTypeDef,
     ActionRemoteIpDetailsTypeDef,
     CvssOutputTypeDef,
     CvssTypeDef,
-    AssociationSetDetailsOutputTypeDef,
     AssociationSetDetailsTypeDef,
     AutomationRulesFindingFieldsUpdateOutputTypeDef,
     AutomationRulesFindingFieldsUpdateTypeDef,
-    AwsAmazonMqBrokerLogsDetailsOutputTypeDef,
     AwsAmazonMqBrokerLogsDetailsTypeDef,
     AwsApiGatewayRestApiDetailsOutputTypeDef,
     AwsApiGatewayRestApiDetailsTypeDef,
     AwsApiGatewayStageDetailsOutputTypeDef,
     AwsApiGatewayStageDetailsTypeDef,
     AwsApiGatewayV2ApiDetailsOutputTypeDef,
     AwsApiGatewayV2ApiDetailsTypeDef,
     AwsApiGatewayV2StageDetailsOutputTypeDef,
     AwsApiGatewayV2StageDetailsTypeDef,
-    AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiAdditionalAuthenticationProvidersDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationResultConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationResultConfigurationDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyLaunchTemplateDetailsTypeDef,
-    AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationBlockDeviceMappingsDetailsTypeDef,
-    AwsBackupBackupPlanRuleCopyActionsDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleCopyActionsDetailsTypeDef,
     AwsBackupBackupVaultDetailsOutputTypeDef,
     AwsBackupBackupVaultDetailsTypeDef,
-    AwsBackupRecoveryPointDetailsOutputTypeDef,
     AwsBackupRecoveryPointDetailsTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionOutputTypeDef,
     AwsCertificateManagerCertificateDomainValidationOptionTypeDef,
     AwsCloudFormationStackDetailsOutputTypeDef,
     AwsCloudFormationStackDetailsTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsOutputTypeDef,
     AwsCloudFrontDistributionCacheBehaviorsTypeDef,
@@ -1231,35 +911,29 @@
     AwsCloudFrontDistributionOriginCustomOriginConfigTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverOutputTypeDef,
     AwsCloudFrontDistributionOriginGroupFailoverTypeDef,
     AwsCloudWatchAlarmDetailsOutputTypeDef,
     AwsCloudWatchAlarmDetailsTypeDef,
     AwsCodeBuildProjectEnvironmentOutputTypeDef,
     AwsCodeBuildProjectEnvironmentTypeDef,
-    AwsCodeBuildProjectLogsConfigDetailsOutputTypeDef,
     AwsCodeBuildProjectLogsConfigDetailsTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableGlobalSecondaryIndexTypeDef,
     AwsDynamoDbTableLocalSecondaryIndexTypeDef,
-    AwsDynamoDbTableReplicaGlobalSecondaryIndexOutputTypeDef,
     AwsDynamoDbTableReplicaGlobalSecondaryIndexTypeDef,
     AwsEc2InstanceDetailsOutputTypeDef,
     AwsEc2InstanceDetailsTypeDef,
-    AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataBlockDeviceMappingSetDetailsTypeDef,
-    AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataCapacityReservationSpecificationDetailsTypeDef,
-    AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceMarketOptionsDetailsTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataInstanceRequirementsDetailsTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDataNetworkInterfaceSetDetailsTypeDef,
-    AwsEc2NetworkAclEntryOutputTypeDef,
     AwsEc2NetworkAclEntryTypeDef,
     AwsEc2NetworkInterfaceDetailsOutputTypeDef,
     AwsEc2NetworkInterfaceDetailsTypeDef,
     AwsEc2SecurityGroupIpPermissionOutputTypeDef,
     AwsEc2SecurityGroupIpPermissionTypeDef,
     AwsEc2SubnetDetailsOutputTypeDef,
     AwsEc2SubnetDetailsTypeDef,
@@ -1269,136 +943,109 @@
     AwsEc2VpcDetailsTypeDef,
     AwsEc2VpcEndpointServiceDetailsOutputTypeDef,
     AwsEc2VpcEndpointServiceDetailsTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionVpcInfoDetailsTypeDef,
     AwsEc2VpnConnectionOptionsDetailsOutputTypeDef,
     AwsEc2VpnConnectionOptionsDetailsTypeDef,
-    AwsEcrRepositoryDetailsOutputTypeDef,
     AwsEcrRepositoryDetailsTypeDef,
-    AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationExecuteCommandConfigurationDetailsTypeDef,
     AwsEcsContainerDetailsOutputTypeDef,
     AwsEcsContainerDetailsTypeDef,
-    AwsEcsServiceDeploymentConfigurationDetailsOutputTypeDef,
     AwsEcsServiceDeploymentConfigurationDetailsTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsOutputTypeDef,
     AwsEcsServiceNetworkConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLinuxParametersDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsLogConfigurationDetailsTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionProxyConfigurationDetailsTypeDef,
-    AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesEfsVolumeConfigurationDetailsTypeDef,
-    AwsEcsTaskVolumeDetailsOutputTypeDef,
     AwsEcsTaskVolumeDetailsTypeDef,
-    AwsEfsAccessPointRootDirectoryDetailsOutputTypeDef,
     AwsEfsAccessPointRootDirectoryDetailsTypeDef,
     AwsEksClusterLoggingDetailsOutputTypeDef,
     AwsEksClusterLoggingDetailsTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsOutputTypeDef,
     AwsElasticBeanstalkEnvironmentDetailsTypeDef,
-    AwsElasticsearchDomainElasticsearchClusterConfigDetailsOutputTypeDef,
     AwsElasticsearchDomainElasticsearchClusterConfigDetailsTypeDef,
-    AwsElasticsearchDomainLogPublishingOptionsOutputTypeDef,
     AwsElasticsearchDomainLogPublishingOptionsTypeDef,
     AwsElbLoadBalancerPoliciesOutputTypeDef,
     AwsElbLoadBalancerPoliciesTypeDef,
     AwsElbLoadBalancerAttributesOutputTypeDef,
     AwsElbLoadBalancerAttributesTypeDef,
     AwsElbLoadBalancerListenerDescriptionOutputTypeDef,
     AwsElbLoadBalancerListenerDescriptionTypeDef,
     AwsElbv2LoadBalancerDetailsOutputTypeDef,
     AwsElbv2LoadBalancerDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesKubernetesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesKubernetesDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionScanEc2InstanceWithFindingsDetailsTypeDef,
-    AwsIamAccessKeySessionContextOutputTypeDef,
     AwsIamAccessKeySessionContextTypeDef,
     AwsIamGroupDetailsOutputTypeDef,
     AwsIamGroupDetailsTypeDef,
     AwsIamInstanceProfileOutputTypeDef,
     AwsIamInstanceProfileTypeDef,
     AwsIamPolicyDetailsOutputTypeDef,
     AwsIamPolicyDetailsTypeDef,
     AwsIamUserDetailsOutputTypeDef,
     AwsIamUserDetailsTypeDef,
-    AwsKinesisStreamDetailsOutputTypeDef,
     AwsKinesisStreamDetailsTypeDef,
     AwsLambdaFunctionEnvironmentOutputTypeDef,
     AwsLambdaFunctionEnvironmentTypeDef,
     AwsNetworkFirewallFirewallDetailsOutputTypeDef,
     AwsNetworkFirewallFirewallDetailsTypeDef,
-    AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainAdvancedSecurityOptionsDetailsTypeDef,
-    AwsOpenSearchServiceDomainClusterConfigDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainClusterConfigDetailsTypeDef,
-    AwsOpenSearchServiceDomainLogPublishingOptionsDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainLogPublishingOptionsDetailsTypeDef,
     AwsRdsDbClusterDetailsOutputTypeDef,
     AwsRdsDbClusterDetailsTypeDef,
     AwsRdsDbClusterSnapshotDetailsOutputTypeDef,
     AwsRdsDbClusterSnapshotDetailsTypeDef,
     AwsRdsDbSnapshotDetailsOutputTypeDef,
     AwsRdsDbSnapshotDetailsTypeDef,
     AwsRdsDbPendingModifiedValuesOutputTypeDef,
     AwsRdsDbPendingModifiedValuesTypeDef,
     AwsRdsDbSecurityGroupDetailsOutputTypeDef,
     AwsRdsDbSecurityGroupDetailsTypeDef,
-    AwsRdsDbSubnetGroupSubnetOutputTypeDef,
     AwsRdsDbSubnetGroupSubnetTypeDef,
     AwsRedshiftClusterClusterParameterGroupOutputTypeDef,
     AwsRedshiftClusterClusterParameterGroupTypeDef,
-    AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateOperandsDetailsTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationS3KeyFilterTypeDef,
-    AwsS3BucketObjectLockConfigurationRuleDetailsOutputTypeDef,
     AwsS3BucketObjectLockConfigurationRuleDetailsTypeDef,
-    AwsS3BucketServerSideEncryptionRuleOutputTypeDef,
     AwsS3BucketServerSideEncryptionRuleTypeDef,
-    AwsS3BucketWebsiteConfigurationRoutingRuleOutputTypeDef,
     AwsS3BucketWebsiteConfigurationRoutingRuleTypeDef,
     AwsSageMakerNotebookInstanceDetailsOutputTypeDef,
     AwsSageMakerNotebookInstanceDetailsTypeDef,
-    AwsSecretsManagerSecretDetailsOutputTypeDef,
     AwsSecretsManagerSecretDetailsTypeDef,
-    BatchUpdateFindingsUnprocessedFindingTypeDef,
     BatchUpdateFindingsRequestRequestTypeDef,
+    BatchUpdateFindingsUnprocessedFindingTypeDef,
     GetFindingHistoryRequestRequestTypeDef,
     AwsSnsTopicDetailsOutputTypeDef,
     AwsSnsTopicDetailsTypeDef,
-    AwsSsmPatchOutputTypeDef,
     AwsSsmPatchTypeDef,
-    AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDestinationsDetailsTypeDef,
     AwsWafRateBasedRuleDetailsOutputTypeDef,
     AwsWafRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRateBasedRuleDetailsOutputTypeDef,
     AwsWafRegionalRateBasedRuleDetailsTypeDef,
     AwsWafRegionalRuleDetailsOutputTypeDef,
     AwsWafRegionalRuleDetailsTypeDef,
-    AwsWafRegionalRuleGroupRulesDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupRulesDetailsTypeDef,
-    AwsWafRegionalWebAclRulesListDetailsOutputTypeDef,
     AwsWafRegionalWebAclRulesListDetailsTypeDef,
     AwsWafRuleDetailsOutputTypeDef,
     AwsWafRuleDetailsTypeDef,
-    AwsWafRuleGroupRulesDetailsOutputTypeDef,
     AwsWafRuleGroupRulesDetailsTypeDef,
     AwsWafWebAclRuleOutputTypeDef,
     AwsWafWebAclRuleTypeDef,
     AwsWafv2CustomRequestHandlingDetailsOutputTypeDef,
-    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomRequestHandlingDetailsTypeDef,
+    AwsWafv2CustomResponseDetailsOutputTypeDef,
     AwsWafv2CustomResponseDetailsTypeDef,
-    AwsWafv2WebAclCaptchaConfigDetailsOutputTypeDef,
     AwsWafv2WebAclCaptchaConfigDetailsTypeDef,
     CreateActionTargetResponseTypeDef,
     CreateAutomationRuleResponseTypeDef,
     CreateFindingAggregatorResponseTypeDef,
     CreateInsightResponseTypeDef,
     DeleteActionTargetResponseTypeDef,
     DeleteInsightResponseTypeDef,
@@ -1414,26 +1061,27 @@
     ListTagsForResourceResponseTypeDef,
     UpdateFindingAggregatorResponseTypeDef,
     BatchDeleteAutomationRulesResponseTypeDef,
     BatchUpdateAutomationRulesResponseTypeDef,
     BatchEnableStandardsRequestRequestTypeDef,
     BatchGetSecurityControlsResponseTypeDef,
     BatchGetStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationTypeDef,
     BatchImportFindingsResponseTypeDef,
     BatchUpdateStandardsControlAssociationsRequestRequestTypeDef,
+    UnprocessedStandardsControlAssociationUpdateTypeDef,
     ComplianceOutputTypeDef,
     ComplianceTypeDef,
     ContainerDetailsOutputTypeDef,
     ContainerDetailsTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
-    DateFilterOutputTypeDef,
     DateFilterTypeDef,
     DescribeActionTargetsRequestDescribeActionTargetsPaginateTypeDef,
     DescribeProductsRequestDescribeProductsPaginateTypeDef,
     DescribeStandardsControlsRequestDescribeStandardsControlsPaginateTypeDef,
     DescribeStandardsRequestDescribeStandardsPaginateTypeDef,
     GetEnabledStandardsRequestGetEnabledStandardsPaginateTypeDef,
     GetFindingHistoryRequestGetFindingHistoryPaginateTypeDef,
@@ -1457,51 +1105,43 @@
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetMembersResponseTypeDef,
     ListMembersResponseTypeDef,
     InsightResultsTypeDef,
     ListSecurityControlDefinitionsResponseTypeDef,
     ListStandardsControlAssociationsResponseTypeDef,
-    NetworkOutputTypeDef,
     NetworkPathComponentDetailsOutputTypeDef,
     NetworkPathComponentDetailsTypeDef,
     NetworkTypeDef,
-    PageOutputTypeDef,
     PageTypeDef,
-    RemediationOutputTypeDef,
     RemediationTypeDef,
     RuleGroupSourceStatefulRulesDetailsOutputTypeDef,
     RuleGroupSourceStatefulRulesDetailsTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesOutputTypeDef,
     RuleGroupSourceStatelessRuleMatchAttributesTypeDef,
     RuleGroupVariablesOutputTypeDef,
     RuleGroupVariablesTypeDef,
     StandardTypeDef,
-    UnprocessedStandardsControlAssociationTypeDef,
-    UnprocessedStandardsControlAssociationUpdateTypeDef,
     StandardsSubscriptionTypeDef,
     StatelessCustomPublishMetricActionOutputTypeDef,
     StatelessCustomPublishMetricActionTypeDef,
     AwsApiCallActionOutputTypeDef,
-    NetworkConnectionActionOutputTypeDef,
-    PortProbeDetailOutputTypeDef,
     AwsApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     VulnerabilityOutputTypeDef,
     VulnerabilityTypeDef,
     AwsEc2RouteTableDetailsOutputTypeDef,
     AwsEc2RouteTableDetailsTypeDef,
     AutomationRulesActionOutputTypeDef,
     AutomationRulesActionTypeDef,
     AwsAmazonMqBrokerDetailsOutputTypeDef,
     AwsAmazonMqBrokerDetailsTypeDef,
     AwsAppSyncGraphQlApiDetailsOutputTypeDef,
     AwsAppSyncGraphQlApiDetailsTypeDef,
-    AwsAthenaWorkGroupConfigurationDetailsOutputTypeDef,
     AwsAthenaWorkGroupConfigurationDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupMixedInstancesPolicyDetailsTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsOutputTypeDef,
     AwsAutoScalingLaunchConfigurationDetailsTypeDef,
     AwsBackupBackupPlanRuleDetailsOutputTypeDef,
     AwsBackupBackupPlanRuleDetailsTypeDef,
@@ -1521,15 +1161,14 @@
     AwsEc2NetworkAclDetailsTypeDef,
     AwsEc2SecurityGroupDetailsOutputTypeDef,
     AwsEc2SecurityGroupDetailsTypeDef,
     AwsEc2VpcPeeringConnectionDetailsOutputTypeDef,
     AwsEc2VpcPeeringConnectionDetailsTypeDef,
     AwsEc2VpnConnectionDetailsOutputTypeDef,
     AwsEc2VpnConnectionDetailsTypeDef,
-    AwsEcsClusterConfigurationDetailsOutputTypeDef,
     AwsEcsClusterConfigurationDetailsTypeDef,
     AwsEcsServiceDetailsOutputTypeDef,
     AwsEcsServiceDetailsTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsOutputTypeDef,
     AwsEcsTaskDefinitionContainerDefinitionsDetailsTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsOutputTypeDef,
     AwsEcsTaskDefinitionVolumesDetailsTypeDef,
@@ -1539,17 +1178,15 @@
     AwsEfsAccessPointDetailsTypeDef,
     AwsEksClusterDetailsOutputTypeDef,
     AwsEksClusterDetailsTypeDef,
     AwsElasticsearchDomainDetailsOutputTypeDef,
     AwsElasticsearchDomainDetailsTypeDef,
     AwsElbLoadBalancerDetailsOutputTypeDef,
     AwsElbLoadBalancerDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesMalwareProtectionDetailsTypeDef,
-    AwsIamAccessKeyDetailsOutputTypeDef,
     AwsIamAccessKeyDetailsTypeDef,
     AwsIamRoleDetailsOutputTypeDef,
     AwsIamRoleDetailsTypeDef,
     AwsLambdaFunctionDetailsOutputTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     AwsOpenSearchServiceDomainDetailsOutputTypeDef,
     AwsOpenSearchServiceDomainDetailsTypeDef,
@@ -1557,64 +1194,61 @@
     AwsRdsDbSubnetGroupTypeDef,
     AwsRedshiftClusterDetailsOutputTypeDef,
     AwsRedshiftClusterDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterPredicateDetailsTypeDef,
     AwsS3BucketNotificationConfigurationFilterOutputTypeDef,
     AwsS3BucketNotificationConfigurationFilterTypeDef,
-    AwsS3BucketObjectLockConfigurationOutputTypeDef,
     AwsS3BucketObjectLockConfigurationTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationOutputTypeDef,
     AwsS3BucketServerSideEncryptionConfigurationTypeDef,
     AwsS3BucketWebsiteConfigurationOutputTypeDef,
     AwsS3BucketWebsiteConfigurationTypeDef,
     BatchUpdateFindingsResponseTypeDef,
-    AwsSsmPatchComplianceDetailsOutputTypeDef,
     AwsSsmPatchComplianceDetailsTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsOutputTypeDef,
     AwsStepFunctionStateMachineLoggingConfigurationDetailsTypeDef,
     AwsWafRegionalRuleGroupDetailsOutputTypeDef,
     AwsWafRegionalRuleGroupDetailsTypeDef,
     AwsWafRegionalWebAclDetailsOutputTypeDef,
     AwsWafRegionalWebAclDetailsTypeDef,
     AwsWafRuleGroupDetailsOutputTypeDef,
     AwsWafRuleGroupDetailsTypeDef,
     AwsWafWebAclDetailsOutputTypeDef,
     AwsWafWebAclDetailsTypeDef,
     AwsWafv2ActionAllowDetailsOutputTypeDef,
     AwsWafv2RulesActionCaptchaDetailsOutputTypeDef,
     AwsWafv2RulesActionCountDetailsOutputTypeDef,
-    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionAllowDetailsTypeDef,
     AwsWafv2RulesActionCaptchaDetailsTypeDef,
     AwsWafv2RulesActionCountDetailsTypeDef,
+    AwsWafv2ActionBlockDetailsOutputTypeDef,
     AwsWafv2ActionBlockDetailsTypeDef,
+    BatchGetStandardsControlAssociationsResponseTypeDef,
+    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     AutomationRulesFindingFiltersOutputTypeDef,
-    AwsSecurityFindingFiltersOutputTypeDef,
     AutomationRulesFindingFiltersTypeDef,
+    AwsSecurityFindingFiltersOutputTypeDef,
     AwsSecurityFindingFiltersTypeDef,
     GetFindingHistoryResponseTypeDef,
     GetInsightResultsResponseTypeDef,
     NetworkHeaderOutputTypeDef,
     NetworkHeaderTypeDef,
     OccurrencesOutputTypeDef,
     OccurrencesTypeDef,
     RuleGroupSourceStatelessRuleDefinitionOutputTypeDef,
     RuleGroupSourceStatelessRuleDefinitionTypeDef,
     DescribeStandardsResponseTypeDef,
-    BatchGetStandardsControlAssociationsResponseTypeDef,
-    BatchUpdateStandardsControlAssociationsResponseTypeDef,
     BatchDisableStandardsResponseTypeDef,
     BatchEnableStandardsResponseTypeDef,
     GetEnabledStandardsResponseTypeDef,
     StatelessCustomActionDefinitionOutputTypeDef,
     StatelessCustomActionDefinitionTypeDef,
     PortProbeActionOutputTypeDef,
     PortProbeActionTypeDef,
-    AwsAthenaWorkGroupDetailsOutputTypeDef,
     AwsAthenaWorkGroupDetailsTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsOutputTypeDef,
     AwsAutoScalingAutoScalingGroupDetailsTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsOutputTypeDef,
     AwsBackupBackupPlanBackupPlanDetailsTypeDef,
     AwsCertificateManagerCertificateDetailsOutputTypeDef,
     AwsCertificateManagerCertificateDetailsTypeDef,
@@ -1626,32 +1260,31 @@
     AwsDynamoDbTableDetailsTypeDef,
     AwsEc2LaunchTemplateDetailsOutputTypeDef,
     AwsEc2LaunchTemplateDetailsTypeDef,
     AwsEcsClusterDetailsOutputTypeDef,
     AwsEcsClusterDetailsTypeDef,
     AwsEcsTaskDefinitionDetailsOutputTypeDef,
     AwsEcsTaskDefinitionDetailsTypeDef,
-    AwsGuardDutyDetectorDataSourcesDetailsOutputTypeDef,
     AwsGuardDutyDetectorDataSourcesDetailsTypeDef,
     AwsRdsDbInstanceDetailsOutputTypeDef,
     AwsRdsDbInstanceDetailsTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesFilterDetailsTypeDef,
     AwsS3BucketNotificationConfigurationDetailOutputTypeDef,
     AwsS3BucketNotificationConfigurationDetailTypeDef,
     AwsStepFunctionStateMachineDetailsOutputTypeDef,
     AwsStepFunctionStateMachineDetailsTypeDef,
     AwsWafv2RulesActionDetailsOutputTypeDef,
     AwsWafv2WebAclActionDetailsOutputTypeDef,
     AwsWafv2RulesActionDetailsTypeDef,
     AwsWafv2WebAclActionDetailsTypeDef,
     AutomationRulesConfigTypeDef,
-    InsightTypeDef,
     CreateAutomationRuleRequestRequestTypeDef,
     UpdateAutomationRulesRequestItemTypeDef,
+    InsightTypeDef,
     CreateInsightRequestRequestTypeDef,
     GetFindingsRequestGetFindingsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     UpdateFindingsRequestRequestTypeDef,
     UpdateInsightRequestRequestTypeDef,
     NetworkPathComponentOutputTypeDef,
     NetworkPathComponentTypeDef,
@@ -1676,16 +1309,16 @@
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsOutputTypeDef,
     AwsS3BucketBucketLifecycleConfigurationRulesDetailsTypeDef,
     AwsS3BucketNotificationConfigurationOutputTypeDef,
     AwsS3BucketNotificationConfigurationTypeDef,
     AwsWafv2RulesDetailsOutputTypeDef,
     AwsWafv2RulesDetailsTypeDef,
     BatchGetAutomationRulesResponseTypeDef,
-    GetInsightsResponseTypeDef,
     BatchUpdateAutomationRulesRequestRequestTypeDef,
+    GetInsightsResponseTypeDef,
     CustomDataIdentifiersResultOutputTypeDef,
     SensitiveDataResultOutputTypeDef,
     CustomDataIdentifiersResultTypeDef,
     SensitiveDataResultTypeDef,
     FirewallPolicyDetailsOutputTypeDef,
     RuleGroupSourceStatelessRulesAndCustomActionsDetailsOutputTypeDef,
     FirewallPolicyDetailsTypeDef,
```

### Comparing `mypy-boto3-securityhub-1.28.12/mypy_boto3_securityhub.egg-info/SOURCES.txt` & `mypy-boto3-securityhub-1.28.15/mypy_boto3_securityhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-securityhub-1.28.12/setup.py` & `mypy-boto3-securityhub-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-securityhub",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_securityhub"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SecurityHub 1.28.12 service generated with mypy-boto3-builder"
-        " 7.15.2"
+        "Type annotations for boto3.SecurityHub 1.28.15 service generated with mypy-boto3-builder"
+        " 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

