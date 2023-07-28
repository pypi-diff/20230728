# Comparing `tmp/mypy-boto3-iot-1.28.12.tar.gz` & `tmp/mypy-boto3-iot-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-iot-1.28.12.tar", last modified: Thu Jul 27 05:34:48 2023, max compression
+gzip compressed data, was "mypy-boto3-iot-1.28.15.tar", last modified: Fri Jul 28 20:42:59 2023, max compression
```

## Comparing `mypy-boto3-iot-1.28.12.tar` & `mypy-boto3-iot-1.28.15.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.856485 mypy-boto3-iot-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    58207 2023-07-27 05:34:48.852485 mypy-boto3-iot-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    56736 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.848485 mypy-boto3-iot-1.28.12/mypy_boto3_iot/
--rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   181667 2023-07-27 05:23:45.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   181351 2023-07-27 05:23:43.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25037 2023-07-27 05:23:46.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-27 05:23:45.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    69164 2023-07-27 05:23:45.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    69103 2023-07-27 05:23:45.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   293163 2023-07-27 05:23:52.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   292776 2023-07-27 05:23:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:48.848485 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    58207 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:48.000000 mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:48.856485 mypy-boto3-iot-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:23:42.000000 mypy-boto3-iot-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.245254 mypy-boto3-iot-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    55452 2023-07-28 20:42:59.233254 mypy-boto3-iot-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    53981 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.221253 mypy-boto3-iot-1.28.15/mypy_boto3_iot/
+-rw-r--r--   0 runner    (1001) docker     (123)    14116 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181667 2023-07-28 20:27:57.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   181351 2023-07-28 20:27:56.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    25037 2023-07-28 20:27:59.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25035 2023-07-28 20:27:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    68966 2023-07-28 20:27:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68905 2023-07-28 20:27:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   270064 2023-07-28 20:28:09.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   269715 2023-07-28 20:28:04.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:59.233254 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    55452 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-28 20:42:59.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:58.000000 mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:59.245254 mypy-boto3-iot-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:27:54.000000 mypy-boto3-iot-1.28.15/setup.py
```

### Comparing `mypy-boto3-iot-1.28.12/LICENSE` & `mypy-boto3-iot-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.12/PKG-INFO` & `mypy-boto3-iot-1.28.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,29 @@
-Metadata-Version: 2.1
-Name: mypy-boto3-iot
-Version: 1.28.12
-Summary: Type annotations for boto3.IoT 1.28.12 service generated with mypy-boto3-builder 7.15.2
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: boto3 iot type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iot"></a>
 
 # mypy-boto3-iot
 
 [![PyPI - mypy-boto3-iot](https://img.shields.io/pypi/v/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -645,167 +613,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
-    AbortCriteriaOutputTypeDef,
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
-    CloudwatchAlarmActionOutputTypeDef,
-    CloudwatchLogsActionOutputTypeDef,
-    CloudwatchMetricActionOutputTypeDef,
-    DynamoDBActionOutputTypeDef,
-    ElasticsearchActionOutputTypeDef,
-    FirehoseActionOutputTypeDef,
-    IotAnalyticsActionOutputTypeDef,
-    IotEventsActionOutputTypeDef,
-    KafkaActionOutputTypeDef,
-    KinesisActionOutputTypeDef,
-    LambdaActionOutputTypeDef,
-    OpenSearchActionOutputTypeDef,
-    S3ActionOutputTypeDef,
-    SalesforceActionOutputTypeDef,
-    SnsActionOutputTypeDef,
-    SqsActionOutputTypeDef,
-    StepFunctionsActionOutputTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
-    KafkaActionTypeDef,
+    KafkaActionOutputTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
+    KafkaActionTypeDef,
     MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
     AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
     AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
-    AlertTargetOutputTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
-    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
-    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
-    AssociateTargetsWithJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
     AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
-    AuditCheckConfigurationOutputTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
     AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
-    AuditNotificationTargetOutputTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
     AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
-    AuthorizerConfigOutputTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
-    AwsJobRateIncreaseCriteriaOutputTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
-    AwsJobPresignedUrlConfigOutputTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    MachineLearningDetectionConfigOutputTypeDef,
-    StatisticalThresholdOutputTypeDef,
     MachineLearningDetectionConfigTypeDef,
-    MetricValueTypeDef,
     StatisticalThresholdTypeDef,
+    MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
-    BillingGroupPropertiesOutputTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
-    CodeSigningCertificateChainOutputTypeDef,
     CodeSigningCertificateChainTypeDef,
     CodeSigningSignatureOutputTypeDef,
     CodeSigningSignatureTypeDef,
-    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
-    CreateCertificateFromCsrResponseTypeDef,
-    CreateCustomMetricResponseTypeDef,
-    CreateDimensionResponseTypeDef,
     TlsConfigTypeDef,
-    CreateDomainConfigurationResponseTypeDef,
-    CreateDynamicThingGroupResponseTypeDef,
-    CreateFleetMetricResponseTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
-    CreateJobResponseTypeDef,
     MaintenanceWindowTypeDef,
-    CreateJobTemplateResponseTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
-    CreateMitigationActionResponseTypeDef,
-    CreateOTAUpdateResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
-    CreatePackageResponseTypeDef,
     CreatePackageVersionRequestRequestTypeDef,
-    CreatePackageVersionResponseTypeDef,
-    CreatePolicyResponseTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    CreatePolicyVersionResponseTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
-    CreateProvisioningTemplateResponseTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
-    CreateProvisioningTemplateVersionResponseTypeDef,
-    CreateRoleAliasResponseTypeDef,
-    CreateScheduledAuditResponseTypeDef,
-    CreateSecurityProfileResponseTypeDef,
-    CreateStreamResponseTypeDef,
-    CreateThingGroupResponseTypeDef,
-    CreateThingResponseTypeDef,
     ThingTypePropertiesTypeDef,
-    CreateThingTypeResponseTypeDef,
     DeleteAccountAuditConfigurationRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteBillingGroupRequestRequestTypeDef,
     DeleteCACertificateRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteCustomMetricRequestRequestTypeDef,
     DeleteDimensionRequestRequestTypeDef,
@@ -838,371 +749,309 @@
     DescribeAuditMitigationActionsTaskRequestRequestTypeDef,
     TaskStatisticsForAuditCheckTypeDef,
     DescribeAuditTaskRequestRequestTypeDef,
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
-    RegistrationConfigOutputTypeDef,
+    RegistrationConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
-    DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
-    DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
-    TlsConfigOutputTypeDef,
     DescribeEndpointRequestRequestTypeDef,
-    DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
-    MaintenanceWindowOutputTypeDef,
-    PresignedUrlConfigOutputTypeDef,
-    TimeoutConfigOutputTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
-    ProvisioningHookOutputTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
-    DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
-    DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
     DescribeStreamRequestRequestTypeDef,
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
-    DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
-    DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
     ThingTypePropertiesOutputTypeDef,
-    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
     DetectMitigationActionsTaskTargetOutputTypeDef,
     ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
-    PutItemInputOutputTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableIoTLoggingParamsOutputTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
-    RateIncreaseCriteriaOutputTypeDef,
     RateIncreaseCriteriaTypeDef,
-    FieldOutputTypeDef,
     FieldTypeDef,
-    S3LocationOutputTypeDef,
-    StreamOutputTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
-    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
-    GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
-    GetJobDocumentResponseTypeDef,
-    GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
-    VersionUpdateByJobsConfigOutputTypeDef,
+    VersionUpdateByJobsConfigTypeDef,
     GetPackageRequestRequestTypeDef,
-    GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
-    GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
-    GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
-    HttpActionHeaderOutputTypeDef,
     HttpActionHeaderTypeDef,
-    SigV4AuthorizationOutputTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
     IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
-    IssuerCertificateIdentifierOutputTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
-    RetryCriteriaOutputTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
-    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
-    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
-    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
     ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
     ListAuditTasksRequestRequestTypeDef,
-    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
     ListAuthorizersRequestRequestTypeDef,
-    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
-    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
     ListCACertificatesRequestRequestTypeDef,
-    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListCustomMetricsResponseTypeDef,
-    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
     ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
     ListDetectMitigationActionsTasksRequestRequestTypeDef,
-    ListDimensionsRequestListDimensionsPaginateTypeDef,
     ListDimensionsRequestRequestTypeDef,
-    ListDimensionsResponseTypeDef,
-    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
-    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
-    ListIndicesRequestListIndicesPaginateTypeDef,
     ListIndicesRequestRequestTypeDef,
-    ListIndicesResponseTypeDef,
-    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
-    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
     ListMetricValuesRequestRequestTypeDef,
-    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
-    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
-    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     PackageVersionSummaryTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageSummaryTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
     ListPolicyPrincipalsRequestRequestTypeDef,
-    ListPolicyPrincipalsResponseTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     PolicyVersionTypeDef,
-    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
     ListPrincipalPoliciesRequestRequestTypeDef,
-    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
     ListPrincipalThingsRequestRequestTypeDef,
-    ListPrincipalThingsResponseTypeDef,
-    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
     ListProvisioningTemplateVersionsRequestRequestTypeDef,
     ProvisioningTemplateVersionSummaryTypeDef,
-    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
     ListProvisioningTemplatesRequestRequestTypeDef,
     ProvisioningTemplateSummaryTypeDef,
-    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
     ListRelatedResourcesForAuditFindingRequestRequestTypeDef,
-    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
     ListRoleAliasesRequestRequestTypeDef,
-    ListRoleAliasesResponseTypeDef,
-    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
     ListScheduledAuditsRequestRequestTypeDef,
     ScheduledAuditMetadataTypeDef,
-    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
     ListSecurityProfilesForTargetRequestRequestTypeDef,
-    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
-    ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
-    ListTargetsForPolicyResponseTypeDef,
-    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
-    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
     ListThingGroupsForThingRequestRequestTypeDef,
-    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
     ListThingGroupsRequestRequestTypeDef,
-    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
     ListThingPrincipalsRequestRequestTypeDef,
-    ListThingPrincipalsResponseTypeDef,
-    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
     ListThingRegistrationTaskReportsRequestRequestTypeDef,
-    ListThingRegistrationTaskReportsResponseTypeDef,
-    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
     ListThingRegistrationTasksRequestRequestTypeDef,
-    ListThingRegistrationTasksResponseTypeDef,
-    ListThingTypesRequestListThingTypesPaginateTypeDef,
     ListThingTypesRequestRequestTypeDef,
-    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
     ListThingsInBillingGroupRequestRequestTypeDef,
-    ListThingsInBillingGroupResponseTypeDef,
-    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
     ListThingsInThingGroupRequestRequestTypeDef,
-    ListThingsInThingGroupResponseTypeDef,
-    ListThingsRequestListThingsPaginateTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
-    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
-    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
-    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     ListViolationEventsRequestRequestTypeDef,
-    LocationTimestampOutputTypeDef,
     LocationTimestampTypeDef,
-    LogTargetOutputTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
-    PublishFindingToSnsParamsOutputTypeDef,
-    ReplaceDefaultPolicyVersionParamsOutputTypeDef,
-    UpdateCACertificateParamsOutputTypeDef,
-    UpdateDeviceCertificateParamsOutputTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
-    UserPropertyOutputTypeDef,
     UserPropertyTypeDef,
-    PaginatorConfigTypeDef,
-    PolicyVersionIdentifierOutputTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
-    RegistrationConfigTypeDef,
-    RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
-    RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
-    RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
-    RegisterThingResponseTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
     RemoveThingFromThingGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
-    SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
-    SigningProfileParameterOutputTypeDef,
     SigningProfileParameterTypeDef,
-    StartAuditMitigationActionsTaskResponseTypeDef,
     ViolationEventOccurrenceRangeTypeDef,
-    StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
-    StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
-    StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
-    TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
-    TimestreamDimensionOutputTypeDef,
-    TimestreamTimestampOutputTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
-    TransferCertificateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    UpdateBillingGroupResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateCustomMetricRequestRequestTypeDef,
-    UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
-    UpdateDimensionResponseTypeDef,
-    UpdateDomainConfigurationResponseTypeDef,
-    UpdateDynamicThingGroupResponseTypeDef,
-    UpdateMitigationActionResponseTypeDef,
-    VersionUpdateByJobsConfigTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
-    UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
-    UpdateScheduledAuditResponseTypeDef,
-    UpdateStreamResponseTypeDef,
-    UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
     AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
-    DescribeFleetMetricResponseTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
+    AssetPropertyValueTypeDef,
+    AssociateTargetsWithJobResponseTypeDef,
+    CancelJobResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateBillingGroupResponseTypeDef,
+    CreateCertificateFromCsrResponseTypeDef,
+    CreateCustomMetricResponseTypeDef,
+    CreateDimensionResponseTypeDef,
+    CreateDomainConfigurationResponseTypeDef,
+    CreateDynamicThingGroupResponseTypeDef,
+    CreateFleetMetricResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateMitigationActionResponseTypeDef,
+    CreateOTAUpdateResponseTypeDef,
+    CreatePackageResponseTypeDef,
+    CreatePackageVersionResponseTypeDef,
+    CreatePolicyResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    CreateProvisioningTemplateResponseTypeDef,
+    CreateProvisioningTemplateVersionResponseTypeDef,
+    CreateRoleAliasResponseTypeDef,
+    CreateScheduledAuditResponseTypeDef,
+    CreateSecurityProfileResponseTypeDef,
+    CreateStreamResponseTypeDef,
+    CreateThingGroupResponseTypeDef,
+    CreateThingResponseTypeDef,
+    CreateThingTypeResponseTypeDef,
+    DescribeCustomMetricResponseTypeDef,
+    DescribeDimensionResponseTypeDef,
+    DescribeEndpointResponseTypeDef,
+    DescribeFleetMetricResponseTypeDef,
+    DescribeIndexResponseTypeDef,
+    DescribeProvisioningTemplateVersionResponseTypeDef,
+    DescribeScheduledAuditResponseTypeDef,
+    DescribeThingRegistrationTaskResponseTypeDef,
+    DescribeThingResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCardinalityResponseTypeDef,
+    GetJobDocumentResponseTypeDef,
+    GetLoggingOptionsResponseTypeDef,
+    GetPackageResponseTypeDef,
+    GetPackageVersionResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    GetRegistrationCodeResponseTypeDef,
+    GetV2LoggingOptionsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
+    ListCustomMetricsResponseTypeDef,
+    ListDimensionsResponseTypeDef,
+    ListIndicesResponseTypeDef,
     ListPoliciesResponseTypeDef,
+    ListPolicyPrincipalsResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
-    AssetPropertyValueOutputTypeDef,
-    AssetPropertyValueTypeDef,
+    ListPrincipalThingsResponseTypeDef,
+    ListRoleAliasesResponseTypeDef,
+    ListTargetsForPolicyResponseTypeDef,
+    ListThingPrincipalsResponseTypeDef,
+    ListThingRegistrationTaskReportsResponseTypeDef,
+    ListThingRegistrationTasksResponseTypeDef,
+    ListThingsInBillingGroupResponseTypeDef,
+    ListThingsInThingGroupResponseTypeDef,
+    RegisterCACertificateResponseTypeDef,
+    RegisterCertificateResponseTypeDef,
+    RegisterCertificateWithoutCAResponseTypeDef,
+    RegisterThingResponseTypeDef,
+    SetDefaultAuthorizerResponseTypeDef,
+    StartAuditMitigationActionsTaskResponseTypeDef,
+    StartDetectMitigationActionsTaskResponseTypeDef,
+    StartOnDemandAuditTaskResponseTypeDef,
+    StartThingRegistrationTaskResponseTypeDef,
+    TestInvokeAuthorizerResponseTypeDef,
+    TransferCertificateResponseTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateBillingGroupResponseTypeDef,
+    UpdateCustomMetricResponseTypeDef,
+    UpdateDimensionResponseTypeDef,
+    UpdateDomainConfigurationResponseTypeDef,
+    UpdateDynamicThingGroupResponseTypeDef,
+    UpdateMitigationActionResponseTypeDef,
+    UpdateRoleAliasResponseTypeDef,
+    UpdateScheduledAuditResponseTypeDef,
+    UpdateStreamResponseTypeDef,
+    UpdateThingGroupResponseTypeDef,
     ThingGroupPropertiesOutputTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
@@ -1210,20 +1059,18 @@
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
     TestAuthorizationRequestRequestTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
-    AwsJobExponentialRolloutRateOutputTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
     BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
-    MetricToRetainOutputTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
@@ -1238,55 +1085,110 @@
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
+    SchedulingConfigOutputTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
+    DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
+    RegisterCACertificateRequestRequestTypeDef,
+    UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
-    SchedulingConfigOutputTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
-    DescribeProvisioningTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
     ListDomainConfigurationsResponseTypeDef,
-    DynamoDBv2ActionOutputTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
-    ExponentialRolloutRateOutputTypeDef,
     ExponentialRolloutRateTypeDef,
     ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
-    StreamFileOutputTypeDef,
-    FileLocationOutputTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
+    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
+    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
+    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
+    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
+    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
+    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
+    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    ListDimensionsRequestListDimensionsPaginateTypeDef,
+    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
+    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
+    ListIndicesRequestListIndicesPaginateTypeDef,
+    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
+    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
+    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
+    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
+    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
+    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
+    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
+    ListStreamsRequestListStreamsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
+    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
+    ListThingTypesRequestListThingTypesPaginateTypeDef,
+    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    ListThingsRequestListThingsPaginateTypeDef,
+    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
+    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
+    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
+    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     GetPackageConfigurationResponseTypeDef,
+    UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
-    HttpAuthorizationOutputTypeDef,
     HttpAuthorizationTypeDef,
     ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
     JobExecutionsRetryConfigOutputTypeDef,
@@ -1301,64 +1203,55 @@
     ListPackagesResponseTypeDef,
     ListPolicyVersionsResponseTypeDef,
     ListProvisioningTemplateVersionsResponseTypeDef,
     ListProvisioningTemplatesResponseTypeDef,
     ListScheduledAuditsResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListStreamsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetsForSecurityProfileResponseTypeDef,
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
-    LocationActionOutputTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
     MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
-    ResourceIdentifierOutputTypeDef,
     ResourceIdentifierTypeDef,
-    RegisterCACertificateRequestRequestTypeDef,
-    UpdateCACertificateRequestRequestTypeDef,
     StartDetectMitigationActionsTaskRequestRequestTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
-    UpdatePackageConfigurationRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
     PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
-    AwsJobExecutionsRolloutConfigOutputTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     BehaviorOutputTypeDef,
     BehaviorTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     ListThingTypesResponseTypeDef,
-    StartSigningJobParameterOutputTypeDef,
     StartSigningJobParameterTypeDef,
-    JobExecutionsRolloutConfigOutputTypeDef,
     JobExecutionsRolloutConfigTypeDef,
-    StreamInfoTypeDef,
     CreateStreamRequestRequestTypeDef,
+    StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
     HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
@@ -1369,24 +1262,24 @@
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
     RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
-    DescribeAuditSuppressionResponseTypeDef,
-    NonCompliantResourceTypeDef,
-    RelatedResourceTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
+    DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
     ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef,
     ListAuditSuppressionsRequestRequestTypeDef,
+    NonCompliantResourceTypeDef,
+    RelatedResourceTypeDef,
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
@@ -1397,18 +1290,18 @@
     UpdateSecurityProfileResponseTypeDef,
     ViolationEventTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
-    DescribeJobTemplateResponseTypeDef,
-    JobTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
+    DescribeJobTemplateResponseTypeDef,
+    JobTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
@@ -1431,15 +1324,15 @@
     GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
     GetOTAUpdateResponseTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaOutputTypeDef:
+def get_structure() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.12/README.md` & `mypy-boto3-iot-1.28.15/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: mypy-boto3-iot
+Version: 1.28.15
+Summary: Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: boto3 iot type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="mypy-boto3-iot"></a>
 
 # mypy-boto3-iot
 
 [![PyPI - mypy-boto3-iot](https://img.shields.io/pypi/v/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -613,167 +645,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
-    AbortCriteriaOutputTypeDef,
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
-    CloudwatchAlarmActionOutputTypeDef,
-    CloudwatchLogsActionOutputTypeDef,
-    CloudwatchMetricActionOutputTypeDef,
-    DynamoDBActionOutputTypeDef,
-    ElasticsearchActionOutputTypeDef,
-    FirehoseActionOutputTypeDef,
-    IotAnalyticsActionOutputTypeDef,
-    IotEventsActionOutputTypeDef,
-    KafkaActionOutputTypeDef,
-    KinesisActionOutputTypeDef,
-    LambdaActionOutputTypeDef,
-    OpenSearchActionOutputTypeDef,
-    S3ActionOutputTypeDef,
-    SalesforceActionOutputTypeDef,
-    SnsActionOutputTypeDef,
-    SqsActionOutputTypeDef,
-    StepFunctionsActionOutputTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
-    KafkaActionTypeDef,
+    KafkaActionOutputTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
+    KafkaActionTypeDef,
     MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
     AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
     AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
-    AlertTargetOutputTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
-    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
-    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
-    AssociateTargetsWithJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
     AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
-    AuditCheckConfigurationOutputTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
     AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
-    AuditNotificationTargetOutputTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
     AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
-    AuthorizerConfigOutputTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
-    AwsJobRateIncreaseCriteriaOutputTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
-    AwsJobPresignedUrlConfigOutputTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    MachineLearningDetectionConfigOutputTypeDef,
-    StatisticalThresholdOutputTypeDef,
     MachineLearningDetectionConfigTypeDef,
-    MetricValueTypeDef,
     StatisticalThresholdTypeDef,
+    MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
-    BillingGroupPropertiesOutputTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
-    CodeSigningCertificateChainOutputTypeDef,
     CodeSigningCertificateChainTypeDef,
     CodeSigningSignatureOutputTypeDef,
     CodeSigningSignatureTypeDef,
-    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
-    CreateCertificateFromCsrResponseTypeDef,
-    CreateCustomMetricResponseTypeDef,
-    CreateDimensionResponseTypeDef,
     TlsConfigTypeDef,
-    CreateDomainConfigurationResponseTypeDef,
-    CreateDynamicThingGroupResponseTypeDef,
-    CreateFleetMetricResponseTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
-    CreateJobResponseTypeDef,
     MaintenanceWindowTypeDef,
-    CreateJobTemplateResponseTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
-    CreateMitigationActionResponseTypeDef,
-    CreateOTAUpdateResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
-    CreatePackageResponseTypeDef,
     CreatePackageVersionRequestRequestTypeDef,
-    CreatePackageVersionResponseTypeDef,
-    CreatePolicyResponseTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    CreatePolicyVersionResponseTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
-    CreateProvisioningTemplateResponseTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
-    CreateProvisioningTemplateVersionResponseTypeDef,
-    CreateRoleAliasResponseTypeDef,
-    CreateScheduledAuditResponseTypeDef,
-    CreateSecurityProfileResponseTypeDef,
-    CreateStreamResponseTypeDef,
-    CreateThingGroupResponseTypeDef,
-    CreateThingResponseTypeDef,
     ThingTypePropertiesTypeDef,
-    CreateThingTypeResponseTypeDef,
     DeleteAccountAuditConfigurationRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteBillingGroupRequestRequestTypeDef,
     DeleteCACertificateRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteCustomMetricRequestRequestTypeDef,
     DeleteDimensionRequestRequestTypeDef,
@@ -806,371 +781,309 @@
     DescribeAuditMitigationActionsTaskRequestRequestTypeDef,
     TaskStatisticsForAuditCheckTypeDef,
     DescribeAuditTaskRequestRequestTypeDef,
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
-    RegistrationConfigOutputTypeDef,
+    RegistrationConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
-    DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
-    DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
-    TlsConfigOutputTypeDef,
     DescribeEndpointRequestRequestTypeDef,
-    DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
-    MaintenanceWindowOutputTypeDef,
-    PresignedUrlConfigOutputTypeDef,
-    TimeoutConfigOutputTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
-    ProvisioningHookOutputTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
-    DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
-    DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
     DescribeStreamRequestRequestTypeDef,
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
-    DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
-    DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
     ThingTypePropertiesOutputTypeDef,
-    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
     DetectMitigationActionsTaskTargetOutputTypeDef,
     ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
-    PutItemInputOutputTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableIoTLoggingParamsOutputTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
-    RateIncreaseCriteriaOutputTypeDef,
     RateIncreaseCriteriaTypeDef,
-    FieldOutputTypeDef,
     FieldTypeDef,
-    S3LocationOutputTypeDef,
-    StreamOutputTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
-    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
-    GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
-    GetJobDocumentResponseTypeDef,
-    GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
-    VersionUpdateByJobsConfigOutputTypeDef,
+    VersionUpdateByJobsConfigTypeDef,
     GetPackageRequestRequestTypeDef,
-    GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
-    GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
-    GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
-    HttpActionHeaderOutputTypeDef,
     HttpActionHeaderTypeDef,
-    SigV4AuthorizationOutputTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
     IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
-    IssuerCertificateIdentifierOutputTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
-    RetryCriteriaOutputTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
-    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
-    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
-    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
     ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
     ListAuditTasksRequestRequestTypeDef,
-    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
     ListAuthorizersRequestRequestTypeDef,
-    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
-    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
     ListCACertificatesRequestRequestTypeDef,
-    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListCustomMetricsResponseTypeDef,
-    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
     ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
     ListDetectMitigationActionsTasksRequestRequestTypeDef,
-    ListDimensionsRequestListDimensionsPaginateTypeDef,
     ListDimensionsRequestRequestTypeDef,
-    ListDimensionsResponseTypeDef,
-    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
-    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
-    ListIndicesRequestListIndicesPaginateTypeDef,
     ListIndicesRequestRequestTypeDef,
-    ListIndicesResponseTypeDef,
-    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
-    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
     ListMetricValuesRequestRequestTypeDef,
-    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
-    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
-    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     PackageVersionSummaryTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageSummaryTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
     ListPolicyPrincipalsRequestRequestTypeDef,
-    ListPolicyPrincipalsResponseTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     PolicyVersionTypeDef,
-    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
     ListPrincipalPoliciesRequestRequestTypeDef,
-    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
     ListPrincipalThingsRequestRequestTypeDef,
-    ListPrincipalThingsResponseTypeDef,
-    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
     ListProvisioningTemplateVersionsRequestRequestTypeDef,
     ProvisioningTemplateVersionSummaryTypeDef,
-    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
     ListProvisioningTemplatesRequestRequestTypeDef,
     ProvisioningTemplateSummaryTypeDef,
-    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
     ListRelatedResourcesForAuditFindingRequestRequestTypeDef,
-    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
     ListRoleAliasesRequestRequestTypeDef,
-    ListRoleAliasesResponseTypeDef,
-    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
     ListScheduledAuditsRequestRequestTypeDef,
     ScheduledAuditMetadataTypeDef,
-    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
     ListSecurityProfilesForTargetRequestRequestTypeDef,
-    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
-    ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
-    ListTargetsForPolicyResponseTypeDef,
-    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
-    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
     ListThingGroupsForThingRequestRequestTypeDef,
-    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
     ListThingGroupsRequestRequestTypeDef,
-    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
     ListThingPrincipalsRequestRequestTypeDef,
-    ListThingPrincipalsResponseTypeDef,
-    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
     ListThingRegistrationTaskReportsRequestRequestTypeDef,
-    ListThingRegistrationTaskReportsResponseTypeDef,
-    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
     ListThingRegistrationTasksRequestRequestTypeDef,
-    ListThingRegistrationTasksResponseTypeDef,
-    ListThingTypesRequestListThingTypesPaginateTypeDef,
     ListThingTypesRequestRequestTypeDef,
-    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
     ListThingsInBillingGroupRequestRequestTypeDef,
-    ListThingsInBillingGroupResponseTypeDef,
-    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
     ListThingsInThingGroupRequestRequestTypeDef,
-    ListThingsInThingGroupResponseTypeDef,
-    ListThingsRequestListThingsPaginateTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
-    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
-    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
-    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     ListViolationEventsRequestRequestTypeDef,
-    LocationTimestampOutputTypeDef,
     LocationTimestampTypeDef,
-    LogTargetOutputTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
-    PublishFindingToSnsParamsOutputTypeDef,
-    ReplaceDefaultPolicyVersionParamsOutputTypeDef,
-    UpdateCACertificateParamsOutputTypeDef,
-    UpdateDeviceCertificateParamsOutputTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
-    UserPropertyOutputTypeDef,
     UserPropertyTypeDef,
-    PaginatorConfigTypeDef,
-    PolicyVersionIdentifierOutputTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
-    RegistrationConfigTypeDef,
-    RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
-    RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
-    RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
-    RegisterThingResponseTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
     RemoveThingFromThingGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
-    SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
-    SigningProfileParameterOutputTypeDef,
     SigningProfileParameterTypeDef,
-    StartAuditMitigationActionsTaskResponseTypeDef,
     ViolationEventOccurrenceRangeTypeDef,
-    StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
-    StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
-    StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
-    TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
-    TimestreamDimensionOutputTypeDef,
-    TimestreamTimestampOutputTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
-    TransferCertificateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    UpdateBillingGroupResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateCustomMetricRequestRequestTypeDef,
-    UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
-    UpdateDimensionResponseTypeDef,
-    UpdateDomainConfigurationResponseTypeDef,
-    UpdateDynamicThingGroupResponseTypeDef,
-    UpdateMitigationActionResponseTypeDef,
-    VersionUpdateByJobsConfigTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
-    UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
-    UpdateScheduledAuditResponseTypeDef,
-    UpdateStreamResponseTypeDef,
-    UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
     AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
-    DescribeFleetMetricResponseTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
+    AssetPropertyValueTypeDef,
+    AssociateTargetsWithJobResponseTypeDef,
+    CancelJobResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateBillingGroupResponseTypeDef,
+    CreateCertificateFromCsrResponseTypeDef,
+    CreateCustomMetricResponseTypeDef,
+    CreateDimensionResponseTypeDef,
+    CreateDomainConfigurationResponseTypeDef,
+    CreateDynamicThingGroupResponseTypeDef,
+    CreateFleetMetricResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateMitigationActionResponseTypeDef,
+    CreateOTAUpdateResponseTypeDef,
+    CreatePackageResponseTypeDef,
+    CreatePackageVersionResponseTypeDef,
+    CreatePolicyResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    CreateProvisioningTemplateResponseTypeDef,
+    CreateProvisioningTemplateVersionResponseTypeDef,
+    CreateRoleAliasResponseTypeDef,
+    CreateScheduledAuditResponseTypeDef,
+    CreateSecurityProfileResponseTypeDef,
+    CreateStreamResponseTypeDef,
+    CreateThingGroupResponseTypeDef,
+    CreateThingResponseTypeDef,
+    CreateThingTypeResponseTypeDef,
+    DescribeCustomMetricResponseTypeDef,
+    DescribeDimensionResponseTypeDef,
+    DescribeEndpointResponseTypeDef,
+    DescribeFleetMetricResponseTypeDef,
+    DescribeIndexResponseTypeDef,
+    DescribeProvisioningTemplateVersionResponseTypeDef,
+    DescribeScheduledAuditResponseTypeDef,
+    DescribeThingRegistrationTaskResponseTypeDef,
+    DescribeThingResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCardinalityResponseTypeDef,
+    GetJobDocumentResponseTypeDef,
+    GetLoggingOptionsResponseTypeDef,
+    GetPackageResponseTypeDef,
+    GetPackageVersionResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    GetRegistrationCodeResponseTypeDef,
+    GetV2LoggingOptionsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
+    ListCustomMetricsResponseTypeDef,
+    ListDimensionsResponseTypeDef,
+    ListIndicesResponseTypeDef,
     ListPoliciesResponseTypeDef,
+    ListPolicyPrincipalsResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
-    AssetPropertyValueOutputTypeDef,
-    AssetPropertyValueTypeDef,
+    ListPrincipalThingsResponseTypeDef,
+    ListRoleAliasesResponseTypeDef,
+    ListTargetsForPolicyResponseTypeDef,
+    ListThingPrincipalsResponseTypeDef,
+    ListThingRegistrationTaskReportsResponseTypeDef,
+    ListThingRegistrationTasksResponseTypeDef,
+    ListThingsInBillingGroupResponseTypeDef,
+    ListThingsInThingGroupResponseTypeDef,
+    RegisterCACertificateResponseTypeDef,
+    RegisterCertificateResponseTypeDef,
+    RegisterCertificateWithoutCAResponseTypeDef,
+    RegisterThingResponseTypeDef,
+    SetDefaultAuthorizerResponseTypeDef,
+    StartAuditMitigationActionsTaskResponseTypeDef,
+    StartDetectMitigationActionsTaskResponseTypeDef,
+    StartOnDemandAuditTaskResponseTypeDef,
+    StartThingRegistrationTaskResponseTypeDef,
+    TestInvokeAuthorizerResponseTypeDef,
+    TransferCertificateResponseTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateBillingGroupResponseTypeDef,
+    UpdateCustomMetricResponseTypeDef,
+    UpdateDimensionResponseTypeDef,
+    UpdateDomainConfigurationResponseTypeDef,
+    UpdateDynamicThingGroupResponseTypeDef,
+    UpdateMitigationActionResponseTypeDef,
+    UpdateRoleAliasResponseTypeDef,
+    UpdateScheduledAuditResponseTypeDef,
+    UpdateStreamResponseTypeDef,
+    UpdateThingGroupResponseTypeDef,
     ThingGroupPropertiesOutputTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
@@ -1178,20 +1091,18 @@
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
     TestAuthorizationRequestRequestTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
-    AwsJobExponentialRolloutRateOutputTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
     BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
-    MetricToRetainOutputTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
@@ -1206,55 +1117,110 @@
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
+    SchedulingConfigOutputTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
+    DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
+    RegisterCACertificateRequestRequestTypeDef,
+    UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
-    SchedulingConfigOutputTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
-    DescribeProvisioningTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
     ListDomainConfigurationsResponseTypeDef,
-    DynamoDBv2ActionOutputTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
-    ExponentialRolloutRateOutputTypeDef,
     ExponentialRolloutRateTypeDef,
     ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
-    StreamFileOutputTypeDef,
-    FileLocationOutputTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
+    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
+    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
+    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
+    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
+    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
+    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
+    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    ListDimensionsRequestListDimensionsPaginateTypeDef,
+    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
+    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
+    ListIndicesRequestListIndicesPaginateTypeDef,
+    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
+    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
+    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
+    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
+    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
+    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
+    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
+    ListStreamsRequestListStreamsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
+    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
+    ListThingTypesRequestListThingTypesPaginateTypeDef,
+    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    ListThingsRequestListThingsPaginateTypeDef,
+    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
+    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
+    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
+    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     GetPackageConfigurationResponseTypeDef,
+    UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
-    HttpAuthorizationOutputTypeDef,
     HttpAuthorizationTypeDef,
     ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
     JobExecutionsRetryConfigOutputTypeDef,
@@ -1269,64 +1235,55 @@
     ListPackagesResponseTypeDef,
     ListPolicyVersionsResponseTypeDef,
     ListProvisioningTemplateVersionsResponseTypeDef,
     ListProvisioningTemplatesResponseTypeDef,
     ListScheduledAuditsResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListStreamsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetsForSecurityProfileResponseTypeDef,
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
-    LocationActionOutputTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
     MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
-    ResourceIdentifierOutputTypeDef,
     ResourceIdentifierTypeDef,
-    RegisterCACertificateRequestRequestTypeDef,
-    UpdateCACertificateRequestRequestTypeDef,
     StartDetectMitigationActionsTaskRequestRequestTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
-    UpdatePackageConfigurationRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
     PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
-    AwsJobExecutionsRolloutConfigOutputTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     BehaviorOutputTypeDef,
     BehaviorTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     ListThingTypesResponseTypeDef,
-    StartSigningJobParameterOutputTypeDef,
     StartSigningJobParameterTypeDef,
-    JobExecutionsRolloutConfigOutputTypeDef,
     JobExecutionsRolloutConfigTypeDef,
-    StreamInfoTypeDef,
     CreateStreamRequestRequestTypeDef,
+    StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
     HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
@@ -1337,24 +1294,24 @@
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
     RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
-    DescribeAuditSuppressionResponseTypeDef,
-    NonCompliantResourceTypeDef,
-    RelatedResourceTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
+    DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
     ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef,
     ListAuditSuppressionsRequestRequestTypeDef,
+    NonCompliantResourceTypeDef,
+    RelatedResourceTypeDef,
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
@@ -1365,18 +1322,18 @@
     UpdateSecurityProfileResponseTypeDef,
     ViolationEventTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
-    DescribeJobTemplateResponseTypeDef,
-    JobTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
+    DescribeJobTemplateResponseTypeDef,
+    JobTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
@@ -1399,15 +1356,15 @@
     GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
     GetOTAUpdateResponseTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaOutputTypeDef:
+def get_structure() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/__init__.py` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/__init__.pyi` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/__main__.py` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.IoT 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.IoT 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT\nOther"
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

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/client.py` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/client.pyi` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/literals.py` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/literals.pyi` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/paginator.py` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,15 +300,15 @@
 class GetBehaviorModelTrainingSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#getbehaviormodeltrainingsummariespaginator)
     """
 
     def paginate(
-        self, *, securityProfileName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, securityProfileName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBehaviorModelTrainingSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#getbehaviormodeltrainingsummariespaginator)
         """
 
 
@@ -322,34 +322,30 @@
         self,
         *,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActiveViolationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListActiveViolations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listactiveviolationspaginator)
         """
 
 
 class ListAttachedPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listattachedpoliciespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        target: str,
-        recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, target: str, recursive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttachedPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listattachedpoliciespaginator)
         """
 
 
@@ -364,15 +360,15 @@
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         startTime: Union[datetime, str] = ...,
         endTime: Union[datetime, str] = ...,
         listSuppressedFindings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditfindingspaginator)
         """
 
 
@@ -384,15 +380,15 @@
 
     def paginate(
         self,
         *,
         taskId: str,
         findingId: str,
         actionStatus: AuditMitigationActionsExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditmitigationactionsexecutionspaginator)
         """
 
 
@@ -406,15 +402,15 @@
         self,
         *,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditmitigationactionstaskspaginator)
         """
 
 
@@ -426,15 +422,15 @@
 
     def paginate(
         self,
         *,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditSuppressionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditSuppressions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditsuppressionspaginator)
         """
 
 
@@ -447,15 +443,15 @@
     def paginate(
         self,
         *,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listaudittaskspaginator)
         """
 
 
@@ -466,30 +462,30 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         status: AuthorizerStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuthorizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauthorizerspaginator)
         """
 
 
 class ListBillingGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listbillinggroupspaginator)
     """
 
     def paginate(
-        self, *, namePrefixFilter: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, namePrefixFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBillingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listbillinggroupspaginator)
         """
 
 
@@ -500,30 +496,30 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         templateName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCACertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCACertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcacertificatespaginator)
         """
 
 
 class ListCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcertificatespaginator)
         """
 
 
@@ -534,30 +530,30 @@
     """
 
     def paginate(
         self,
         *,
         caCertificateId: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCertificatesByCAResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificatesByCA.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcertificatesbycapaginator)
         """
 
 
 class ListCustomMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcustommetricspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcustommetricspaginator)
         """
 
 
@@ -571,15 +567,15 @@
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
         startTime: Union[datetime, str] = ...,
         endTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionsexecutionspaginator)
         """
 
 
@@ -590,78 +586,75 @@
     """
 
     def paginate(
         self,
         *,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionstaskspaginator)
         """
 
 
 class ListDimensionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdimensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDimensionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdimensionspaginator)
         """
 
 
 class ListDomainConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdomainconfigurationspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        serviceType: ServiceTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serviceType: ServiceTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdomainconfigurationspaginator)
         """
 
 
 class ListFleetMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listfleetmetricspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFleetMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listfleetmetricspaginator)
         """
 
 
 class ListIndicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listindicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listindicespaginator)
         """
 
 
@@ -672,15 +665,15 @@
     """
 
     def paginate(
         self,
         *,
         jobId: str,
         status: JobExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobExecutionsForJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForJob.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobexecutionsforjobpaginator)
         """
 
 
@@ -693,30 +686,30 @@
     def paginate(
         self,
         *,
         thingName: str,
         status: JobExecutionStatusType = ...,
         namespaceId: str = ...,
         jobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobExecutionsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForThing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobexecutionsforthingpaginator)
         """
 
 
 class ListJobTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobtemplatespaginator)
         """
 
 
@@ -730,30 +723,30 @@
         self,
         *,
         status: JobStatusType = ...,
         targetSelection: TargetSelectionType = ...,
         thingGroupName: str = ...,
         thingGroupId: str = ...,
         namespaceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobspaginator)
         """
 
 
 class ListManagedJobTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListManagedJobTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmanagedjobtemplatespaginator)
     """
 
     def paginate(
-        self, *, templateName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListManagedJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmanagedjobtemplatespaginator)
         """
 
 
@@ -768,15 +761,15 @@
         *,
         thingName: str,
         metricName: str,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMetricValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmetricvaluespaginator)
         """
 
 
@@ -786,15 +779,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmitigationactionspaginator)
     """
 
     def paginate(
         self,
         *,
         actionType: MitigationActionTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMitigationActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMitigationActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmitigationactionspaginator)
         """
 
 
@@ -804,30 +797,30 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listotaupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         otaUpdateStatus: OTAUpdateStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOTAUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOTAUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listotaupdatespaginator)
         """
 
 
 class ListOutgoingCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listoutgoingcertificatespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOutgoingCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listoutgoingcertificatespaginator)
         """
 
 
@@ -838,45 +831,45 @@
     """
 
     def paginate(
         self,
         *,
         packageName: str,
         status: PackageVersionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackageVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackageVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpackageversionspaginator)
         """
 
 
 class ListPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpackagespaginator)
         """
 
 
 class ListPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpoliciespaginator)
         """
 
 
@@ -887,15 +880,15 @@
     """
 
     def paginate(
         self,
         *,
         policyName: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicyPrincipals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpolicyprincipalspaginator)
         """
 
 
@@ -906,105 +899,105 @@
     """
 
     def paginate(
         self,
         *,
         principal: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPrincipalPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprincipalpoliciespaginator)
         """
 
 
 class ListPrincipalThingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprincipalthingspaginator)
     """
 
     def paginate(
-        self, *, principal: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, principal: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPrincipalThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprincipalthingspaginator)
         """
 
 
 class ListProvisioningTemplateVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprovisioningtemplateversionspaginator)
     """
 
     def paginate(
-        self, *, templateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisioningTemplateVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprovisioningtemplateversionspaginator)
         """
 
 
 class ListProvisioningTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprovisioningtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisioningTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprovisioningtemplatespaginator)
         """
 
 
 class ListRelatedResourcesForAuditFindingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRelatedResourcesForAuditFinding)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listrelatedresourcesforauditfindingpaginator)
     """
 
     def paginate(
-        self, *, findingId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, findingId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRelatedResourcesForAuditFindingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRelatedResourcesForAuditFinding.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listrelatedresourcesforauditfindingpaginator)
         """
 
 
 class ListRoleAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listrolealiasespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRoleAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listrolealiasespaginator)
         """
 
 
 class ListScheduledAuditsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listscheduledauditspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScheduledAuditsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listscheduledauditspaginator)
         """
 
 
@@ -1015,15 +1008,15 @@
     """
 
     def paginate(
         self,
         *,
         dimensionName: str = ...,
         metricName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listsecurityprofilespaginator)
         """
 
 
@@ -1034,75 +1027,75 @@
     """
 
     def paginate(
         self,
         *,
         securityProfileTargetArn: str,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityProfilesForTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfilesForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listsecurityprofilesfortargetpaginator)
         """
 
 
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#liststreamspaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#liststreamspaginator)
         """
 
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListTargetsForPolicyPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtargetsforpolicypaginator)
     """
 
     def paginate(
-        self, *, policyName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, policyName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtargetsforpolicypaginator)
         """
 
 
 class ListTargetsForSecurityProfilePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtargetsforsecurityprofilepaginator)
     """
 
     def paginate(
-        self, *, securityProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, securityProfileName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsForSecurityProfileResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtargetsforsecurityprofilepaginator)
         """
 
 
@@ -1114,45 +1107,45 @@
 
     def paginate(
         self,
         *,
         parentGroup: str = ...,
         namePrefixFilter: str = ...,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthinggroupspaginator)
         """
 
 
 class ListThingGroupsForThingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthinggroupsforthingpaginator)
     """
 
     def paginate(
-        self, *, thingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingGroupsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthinggroupsforthingpaginator)
         """
 
 
 class ListThingPrincipalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingprincipalspaginator)
     """
 
     def paginate(
-        self, *, thingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingprincipalspaginator)
         """
 
 
@@ -1163,45 +1156,45 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         reportType: ReportTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingRegistrationTaskReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTaskReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingregistrationtaskreportspaginator)
         """
 
 
 class ListThingRegistrationTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingregistrationtaskspaginator)
     """
 
     def paginate(
-        self, *, status: StatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: StatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingRegistrationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingregistrationtaskspaginator)
         """
 
 
 class ListThingTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingtypespaginator)
     """
 
     def paginate(
-        self, *, thingTypeName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingTypeName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingtypespaginator)
         """
 
 
@@ -1214,30 +1207,30 @@
     def paginate(
         self,
         *,
         attributeName: str = ...,
         attributeValue: str = ...,
         thingTypeName: str = ...,
         usePrefixAttributeValue: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingspaginator)
         """
 
 
 class ListThingsInBillingGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingsinbillinggrouppaginator)
     """
 
     def paginate(
-        self, *, billingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, billingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingsInBillingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingsinbillinggrouppaginator)
         """
 
 
@@ -1248,30 +1241,30 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupName: str,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingsInThingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInThingGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingsinthinggrouppaginator)
         """
 
 
 class ListTopicRuleDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtopicruledestinationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTopicRuleDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtopicruledestinationspaginator)
         """
 
 
@@ -1282,33 +1275,30 @@
     """
 
     def paginate(
         self,
         *,
         topic: str = ...,
         ruleDisabled: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTopicRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtopicrulespaginator)
         """
 
 
 class ListV2LoggingLevelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listv2logginglevelspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        targetType: LogTargetTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, targetType: LogTargetTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListV2LoggingLevelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listv2logginglevelspaginator)
         """
 
 
@@ -1324,13 +1314,13 @@
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListViolationEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listviolationeventspaginator)
         """
```

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/paginator.pyi` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -297,15 +297,15 @@
 class GetBehaviorModelTrainingSummariesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#getbehaviormodeltrainingsummariespaginator)
     """
 
     def paginate(
-        self, *, securityProfileName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, securityProfileName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[GetBehaviorModelTrainingSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.GetBehaviorModelTrainingSummaries.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#getbehaviormodeltrainingsummariespaginator)
         """
 
 class ListActiveViolationsPaginator(Paginator):
@@ -318,33 +318,29 @@
         self,
         *,
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListActiveViolationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListActiveViolations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listactiveviolationspaginator)
         """
 
 class ListAttachedPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listattachedpoliciespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        target: str,
-        recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, target: str, recursive: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAttachedPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAttachedPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listattachedpoliciespaginator)
         """
 
 class ListAuditFindingsPaginator(Paginator):
@@ -358,15 +354,15 @@
         *,
         taskId: str = ...,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         startTime: Union[datetime, str] = ...,
         endTime: Union[datetime, str] = ...,
         listSuppressedFindings: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditFindings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditfindingspaginator)
         """
 
 class ListAuditMitigationActionsExecutionsPaginator(Paginator):
@@ -377,15 +373,15 @@
 
     def paginate(
         self,
         *,
         taskId: str,
         findingId: str,
         actionStatus: AuditMitigationActionsExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditmitigationactionsexecutionspaginator)
         """
 
 class ListAuditMitigationActionsTasksPaginator(Paginator):
@@ -398,15 +394,15 @@
         self,
         *,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         auditTaskId: str = ...,
         findingId: str = ...,
         taskStatus: AuditMitigationActionsTaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditMitigationActionsTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditmitigationactionstaskspaginator)
         """
 
 class ListAuditSuppressionsPaginator(Paginator):
@@ -417,15 +413,15 @@
 
     def paginate(
         self,
         *,
         checkName: str = ...,
         resourceIdentifier: ResourceIdentifierTypeDef = ...,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditSuppressionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditSuppressions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauditsuppressionspaginator)
         """
 
 class ListAuditTasksPaginator(Paginator):
@@ -437,15 +433,15 @@
     def paginate(
         self,
         *,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         taskType: AuditTaskTypeType = ...,
         taskStatus: AuditTaskStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuditTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuditTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listaudittaskspaginator)
         """
 
 class ListAuthorizersPaginator(Paginator):
@@ -455,29 +451,29 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         status: AuthorizerStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListAuthorizers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listauthorizerspaginator)
         """
 
 class ListBillingGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listbillinggroupspaginator)
     """
 
     def paginate(
-        self, *, namePrefixFilter: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, namePrefixFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBillingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListBillingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listbillinggroupspaginator)
         """
 
 class ListCACertificatesPaginator(Paginator):
@@ -487,29 +483,29 @@
     """
 
     def paginate(
         self,
         *,
         ascendingOrder: bool = ...,
         templateName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCACertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCACertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcacertificatespaginator)
         """
 
 class ListCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcertificatespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcertificatespaginator)
         """
 
 class ListCertificatesByCAPaginator(Paginator):
@@ -519,29 +515,29 @@
     """
 
     def paginate(
         self,
         *,
         caCertificateId: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCertificatesByCAResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCertificatesByCA.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcertificatesbycapaginator)
         """
 
 class ListCustomMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcustommetricspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListCustomMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListCustomMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listcustommetricspaginator)
         """
 
 class ListDetectMitigationActionsExecutionsPaginator(Paginator):
@@ -554,15 +550,15 @@
         self,
         *,
         taskId: str = ...,
         violationId: str = ...,
         thingName: str = ...,
         startTime: Union[datetime, str] = ...,
         endTime: Union[datetime, str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectMitigationActionsExecutionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionsexecutionspaginator)
         """
 
 class ListDetectMitigationActionsTasksPaginator(Paginator):
@@ -572,74 +568,71 @@
     """
 
     def paginate(
         self,
         *,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDetectMitigationActionsTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDetectMitigationActionsTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdetectmitigationactionstaskspaginator)
         """
 
 class ListDimensionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdimensionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDimensionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDimensions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdimensionspaginator)
         """
 
 class ListDomainConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdomainconfigurationspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        serviceType: ServiceTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serviceType: ServiceTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListDomainConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListDomainConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listdomainconfigurationspaginator)
         """
 
 class ListFleetMetricsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listfleetmetricspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListFleetMetricsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListFleetMetrics.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listfleetmetricspaginator)
         """
 
 class ListIndicesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listindicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIndicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListIndices.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listindicespaginator)
         """
 
 class ListJobExecutionsForJobPaginator(Paginator):
@@ -649,15 +642,15 @@
     """
 
     def paginate(
         self,
         *,
         jobId: str,
         status: JobExecutionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobExecutionsForJobResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForJob.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobexecutionsforjobpaginator)
         """
 
 class ListJobExecutionsForThingPaginator(Paginator):
@@ -669,29 +662,29 @@
     def paginate(
         self,
         *,
         thingName: str,
         status: JobExecutionStatusType = ...,
         namespaceId: str = ...,
         jobId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobExecutionsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobExecutionsForThing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobexecutionsforthingpaginator)
         """
 
 class ListJobTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobtemplatespaginator)
         """
 
 class ListJobsPaginator(Paginator):
@@ -704,29 +697,29 @@
         self,
         *,
         status: JobStatusType = ...,
         targetSelection: TargetSelectionType = ...,
         thingGroupName: str = ...,
         thingGroupId: str = ...,
         namespaceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListJobs.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listjobspaginator)
         """
 
 class ListManagedJobTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListManagedJobTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmanagedjobtemplatespaginator)
     """
 
     def paginate(
-        self, *, templateName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListManagedJobTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListManagedJobTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmanagedjobtemplatespaginator)
         """
 
 class ListMetricValuesPaginator(Paginator):
@@ -740,15 +733,15 @@
         *,
         thingName: str,
         metricName: str,
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         dimensionName: str = ...,
         dimensionValueOperator: DimensionValueOperatorType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMetricValuesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMetricValues.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmetricvaluespaginator)
         """
 
 class ListMitigationActionsPaginator(Paginator):
@@ -757,15 +750,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmitigationactionspaginator)
     """
 
     def paginate(
         self,
         *,
         actionType: MitigationActionTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListMitigationActionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListMitigationActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listmitigationactionspaginator)
         """
 
 class ListOTAUpdatesPaginator(Paginator):
@@ -774,29 +767,29 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listotaupdatespaginator)
     """
 
     def paginate(
         self,
         *,
         otaUpdateStatus: OTAUpdateStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOTAUpdatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOTAUpdates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listotaupdatespaginator)
         """
 
 class ListOutgoingCertificatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listoutgoingcertificatespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListOutgoingCertificatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListOutgoingCertificates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listoutgoingcertificatespaginator)
         """
 
 class ListPackageVersionsPaginator(Paginator):
@@ -806,43 +799,43 @@
     """
 
     def paginate(
         self,
         *,
         packageName: str,
         status: PackageVersionStatusType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackageVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackageVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpackageversionspaginator)
         """
 
 class ListPackagesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackages)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpackagespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPackagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPackages.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpackagespaginator)
         """
 
 class ListPoliciesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpoliciespaginator)
         """
 
 class ListPolicyPrincipalsPaginator(Paginator):
@@ -852,15 +845,15 @@
     """
 
     def paginate(
         self,
         *,
         policyName: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPolicyPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPolicyPrincipals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listpolicyprincipalspaginator)
         """
 
 class ListPrincipalPoliciesPaginator(Paginator):
@@ -870,99 +863,99 @@
     """
 
     def paginate(
         self,
         *,
         principal: str,
         ascendingOrder: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPrincipalPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalPolicies.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprincipalpoliciespaginator)
         """
 
 class ListPrincipalThingsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprincipalthingspaginator)
     """
 
     def paginate(
-        self, *, principal: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, principal: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPrincipalThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListPrincipalThings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprincipalthingspaginator)
         """
 
 class ListProvisioningTemplateVersionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprovisioningtemplateversionspaginator)
     """
 
     def paginate(
-        self, *, templateName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, templateName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisioningTemplateVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplateVersions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprovisioningtemplateversionspaginator)
         """
 
 class ListProvisioningTemplatesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprovisioningtemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListProvisioningTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListProvisioningTemplates.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listprovisioningtemplatespaginator)
         """
 
 class ListRelatedResourcesForAuditFindingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRelatedResourcesForAuditFinding)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listrelatedresourcesforauditfindingpaginator)
     """
 
     def paginate(
-        self, *, findingId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, findingId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRelatedResourcesForAuditFindingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRelatedResourcesForAuditFinding.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listrelatedresourcesforauditfindingpaginator)
         """
 
 class ListRoleAliasesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listrolealiasespaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListRoleAliasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListRoleAliases.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listrolealiasespaginator)
         """
 
 class ListScheduledAuditsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listscheduledauditspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListScheduledAuditsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListScheduledAudits.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listscheduledauditspaginator)
         """
 
 class ListSecurityProfilesPaginator(Paginator):
@@ -972,15 +965,15 @@
     """
 
     def paginate(
         self,
         *,
         dimensionName: str = ...,
         metricName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityProfilesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfiles.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listsecurityprofilespaginator)
         """
 
 class ListSecurityProfilesForTargetPaginator(Paginator):
@@ -990,71 +983,71 @@
     """
 
     def paginate(
         self,
         *,
         securityProfileTargetArn: str,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityProfilesForTargetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListSecurityProfilesForTarget.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listsecurityprofilesfortargetpaginator)
         """
 
 class ListStreamsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#liststreamspaginator)
     """
 
     def paginate(
-        self, *, ascendingOrder: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ascendingOrder: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStreamsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListStreams.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#liststreamspaginator)
         """
 
 class ListTagsForResourcePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTagsForResource.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtagsforresourcepaginator)
         """
 
 class ListTargetsForPolicyPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtargetsforpolicypaginator)
     """
 
     def paginate(
-        self, *, policyName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, policyName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsForPolicyResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForPolicy.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtargetsforpolicypaginator)
         """
 
 class ListTargetsForSecurityProfilePaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtargetsforsecurityprofilepaginator)
     """
 
     def paginate(
-        self, *, securityProfileName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, securityProfileName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTargetsForSecurityProfileResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTargetsForSecurityProfile.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtargetsforsecurityprofilepaginator)
         """
 
 class ListThingGroupsPaginator(Paginator):
@@ -1065,43 +1058,43 @@
 
     def paginate(
         self,
         *,
         parentGroup: str = ...,
         namePrefixFilter: str = ...,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthinggroupspaginator)
         """
 
 class ListThingGroupsForThingPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthinggroupsforthingpaginator)
     """
 
     def paginate(
-        self, *, thingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingGroupsForThingResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingGroupsForThing.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthinggroupsforthingpaginator)
         """
 
 class ListThingPrincipalsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingprincipalspaginator)
     """
 
     def paginate(
-        self, *, thingName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingPrincipalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingPrincipals.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingprincipalspaginator)
         """
 
 class ListThingRegistrationTaskReportsPaginator(Paginator):
@@ -1111,43 +1104,43 @@
     """
 
     def paginate(
         self,
         *,
         taskId: str,
         reportType: ReportTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingRegistrationTaskReportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTaskReports.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingregistrationtaskreportspaginator)
         """
 
 class ListThingRegistrationTasksPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingregistrationtaskspaginator)
     """
 
     def paginate(
-        self, *, status: StatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, status: StatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingRegistrationTasksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingRegistrationTasks.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingregistrationtaskspaginator)
         """
 
 class ListThingTypesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingtypespaginator)
     """
 
     def paginate(
-        self, *, thingTypeName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, thingTypeName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingTypes.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingtypespaginator)
         """
 
 class ListThingsPaginator(Paginator):
@@ -1159,29 +1152,29 @@
     def paginate(
         self,
         *,
         attributeName: str = ...,
         attributeValue: str = ...,
         thingTypeName: str = ...,
         usePrefixAttributeValue: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingspaginator)
         """
 
 class ListThingsInBillingGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingsinbillinggrouppaginator)
     """
 
     def paginate(
-        self, *, billingGroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, billingGroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingsInBillingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInBillingGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingsinbillinggrouppaginator)
         """
 
 class ListThingsInThingGroupPaginator(Paginator):
@@ -1191,29 +1184,29 @@
     """
 
     def paginate(
         self,
         *,
         thingGroupName: str,
         recursive: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListThingsInThingGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListThingsInThingGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listthingsinthinggrouppaginator)
         """
 
 class ListTopicRuleDestinationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtopicruledestinationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTopicRuleDestinationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRuleDestinations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtopicruledestinationspaginator)
         """
 
 class ListTopicRulesPaginator(Paginator):
@@ -1223,32 +1216,29 @@
     """
 
     def paginate(
         self,
         *,
         topic: str = ...,
         ruleDisabled: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListTopicRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListTopicRules.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listtopicrulespaginator)
         """
 
 class ListV2LoggingLevelsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listv2logginglevelspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        targetType: LogTargetTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, targetType: LogTargetTypeType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListV2LoggingLevelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListV2LoggingLevels.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listv2logginglevelspaginator)
         """
 
 class ListViolationEventsPaginator(Paginator):
@@ -1263,13 +1253,13 @@
         startTime: Union[datetime, str],
         endTime: Union[datetime, str],
         thingName: str = ...,
         securityProfileName: str = ...,
         behaviorCriteriaType: BehaviorCriteriaTypeType = ...,
         listSuppressedAlerts: bool = ...,
         verificationState: VerificationStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListViolationEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT.Paginator.ListViolationEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/paginators/#listviolationeventspaginator)
         """
```

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/type_defs.py` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iot service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot.type_defs import AbortCriteriaOutputTypeDef
+    from mypy_boto3_iot.type_defs import AbortCriteriaTypeDef
 
-    data: AbortCriteriaOutputTypeDef = {...}
+    data: AbortCriteriaTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -89,167 +89,110 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AbortCriteriaOutputTypeDef",
     "AbortCriteriaTypeDef",
     "AcceptCertificateTransferRequestRequestTypeDef",
-    "CloudwatchAlarmActionOutputTypeDef",
-    "CloudwatchLogsActionOutputTypeDef",
-    "CloudwatchMetricActionOutputTypeDef",
-    "DynamoDBActionOutputTypeDef",
-    "ElasticsearchActionOutputTypeDef",
-    "FirehoseActionOutputTypeDef",
-    "IotAnalyticsActionOutputTypeDef",
-    "IotEventsActionOutputTypeDef",
-    "KafkaActionOutputTypeDef",
-    "KinesisActionOutputTypeDef",
-    "LambdaActionOutputTypeDef",
-    "OpenSearchActionOutputTypeDef",
-    "S3ActionOutputTypeDef",
-    "SalesforceActionOutputTypeDef",
-    "SnsActionOutputTypeDef",
-    "SqsActionOutputTypeDef",
-    "StepFunctionsActionOutputTypeDef",
     "CloudwatchAlarmActionTypeDef",
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
     "ElasticsearchActionTypeDef",
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
     "IotEventsActionTypeDef",
-    "KafkaActionTypeDef",
+    "KafkaActionOutputTypeDef",
     "KinesisActionTypeDef",
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
+    "KafkaActionTypeDef",
     "MetricValueOutputTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
     "AddThingToBillingGroupRequestRequestTypeDef",
     "AddThingToThingGroupRequestRequestTypeDef",
     "AddThingsToThingGroupParamsOutputTypeDef",
     "AddThingsToThingGroupParamsTypeDef",
     "AggregationTypeOutputTypeDef",
     "AggregationTypeTypeDef",
-    "AlertTargetOutputTypeDef",
     "AlertTargetTypeDef",
     "PolicyTypeDef",
-    "AssetPropertyTimestampOutputTypeDef",
     "AssetPropertyTimestampTypeDef",
-    "AssetPropertyVariantOutputTypeDef",
     "AssetPropertyVariantTypeDef",
     "AssociateTargetsWithJobRequestRequestTypeDef",
-    "AssociateTargetsWithJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachPrincipalPolicyRequestRequestTypeDef",
     "AttachSecurityProfileRequestRequestTypeDef",
     "AttachThingPrincipalRequestRequestTypeDef",
     "AttributePayloadOutputTypeDef",
     "AttributePayloadTypeDef",
-    "AuditCheckConfigurationOutputTypeDef",
     "AuditCheckConfigurationTypeDef",
     "AuditCheckDetailsTypeDef",
     "AuditMitigationActionExecutionMetadataTypeDef",
     "AuditMitigationActionsTaskMetadataTypeDef",
     "AuditMitigationActionsTaskTargetOutputTypeDef",
     "AuditMitigationActionsTaskTargetTypeDef",
-    "AuditNotificationTargetOutputTypeDef",
     "AuditNotificationTargetTypeDef",
     "AuditTaskMetadataTypeDef",
     "AuthInfoOutputTypeDef",
     "AuthInfoTypeDef",
-    "AuthorizerConfigOutputTypeDef",
     "AuthorizerConfigTypeDef",
     "AuthorizerDescriptionTypeDef",
     "AuthorizerSummaryTypeDef",
     "AwsJobAbortCriteriaTypeDef",
-    "AwsJobRateIncreaseCriteriaOutputTypeDef",
     "AwsJobRateIncreaseCriteriaTypeDef",
-    "AwsJobPresignedUrlConfigOutputTypeDef",
     "AwsJobPresignedUrlConfigTypeDef",
     "AwsJobTimeoutConfigTypeDef",
-    "MachineLearningDetectionConfigOutputTypeDef",
-    "StatisticalThresholdOutputTypeDef",
     "MachineLearningDetectionConfigTypeDef",
-    "MetricValueTypeDef",
     "StatisticalThresholdTypeDef",
+    "MetricValueTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
-    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
-    "BillingGroupPropertiesOutputTypeDef",
     "BillingGroupPropertiesTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
     "CertificateValidityTypeDef",
     "CACertificateTypeDef",
     "CancelAuditMitigationActionsTaskRequestRequestTypeDef",
     "CancelAuditTaskRequestRequestTypeDef",
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "CancelJobResponseTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
-    "CodeSigningCertificateChainOutputTypeDef",
     "CodeSigningCertificateChainTypeDef",
     "CodeSigningSignatureOutputTypeDef",
     "CodeSigningSignatureTypeDef",
-    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "CreateBillingGroupResponseTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
-    "CreateCertificateFromCsrResponseTypeDef",
-    "CreateCustomMetricResponseTypeDef",
-    "CreateDimensionResponseTypeDef",
     "TlsConfigTypeDef",
-    "CreateDomainConfigurationResponseTypeDef",
-    "CreateDynamicThingGroupResponseTypeDef",
-    "CreateFleetMetricResponseTypeDef",
     "PresignedUrlConfigTypeDef",
     "TimeoutConfigTypeDef",
-    "CreateJobResponseTypeDef",
     "MaintenanceWindowTypeDef",
-    "CreateJobTemplateResponseTypeDef",
     "CreateKeysAndCertificateRequestRequestTypeDef",
     "KeyPairTypeDef",
-    "CreateMitigationActionResponseTypeDef",
-    "CreateOTAUpdateResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
-    "CreatePackageResponseTypeDef",
     "CreatePackageVersionRequestRequestTypeDef",
-    "CreatePackageVersionResponseTypeDef",
-    "CreatePolicyResponseTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "CreatePolicyVersionResponseTypeDef",
     "CreateProvisioningClaimRequestRequestTypeDef",
     "ProvisioningHookTypeDef",
-    "CreateProvisioningTemplateResponseTypeDef",
     "CreateProvisioningTemplateVersionRequestRequestTypeDef",
-    "CreateProvisioningTemplateVersionResponseTypeDef",
-    "CreateRoleAliasResponseTypeDef",
-    "CreateScheduledAuditResponseTypeDef",
-    "CreateSecurityProfileResponseTypeDef",
-    "CreateStreamResponseTypeDef",
-    "CreateThingGroupResponseTypeDef",
-    "CreateThingResponseTypeDef",
     "ThingTypePropertiesTypeDef",
-    "CreateThingTypeResponseTypeDef",
     "DeleteAccountAuditConfigurationRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteBillingGroupRequestRequestTypeDef",
     "DeleteCACertificateRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteCustomMetricRequestRequestTypeDef",
     "DeleteDimensionRequestRequestTypeDef",
@@ -282,371 +225,309 @@
     "DescribeAuditMitigationActionsTaskRequestRequestTypeDef",
     "TaskStatisticsForAuditCheckTypeDef",
     "DescribeAuditTaskRequestRequestTypeDef",
     "TaskStatisticsTypeDef",
     "DescribeAuthorizerRequestRequestTypeDef",
     "DescribeBillingGroupRequestRequestTypeDef",
     "DescribeCACertificateRequestRequestTypeDef",
-    "RegistrationConfigOutputTypeDef",
+    "RegistrationConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeCustomMetricRequestRequestTypeDef",
-    "DescribeCustomMetricResponseTypeDef",
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     "DescribeDimensionRequestRequestTypeDef",
-    "DescribeDimensionResponseTypeDef",
     "DescribeDomainConfigurationRequestRequestTypeDef",
     "ServerCertificateSummaryTypeDef",
-    "TlsConfigOutputTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
-    "DescribeEndpointResponseTypeDef",
     "DescribeFleetMetricRequestRequestTypeDef",
     "DescribeIndexRequestRequestTypeDef",
-    "DescribeIndexResponseTypeDef",
     "DescribeJobExecutionRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
-    "MaintenanceWindowOutputTypeDef",
-    "PresignedUrlConfigOutputTypeDef",
-    "TimeoutConfigOutputTypeDef",
     "DescribeManagedJobTemplateRequestRequestTypeDef",
     "DocumentParameterTypeDef",
     "DescribeMitigationActionRequestRequestTypeDef",
     "DescribeProvisioningTemplateRequestRequestTypeDef",
-    "ProvisioningHookOutputTypeDef",
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
-    "DescribeProvisioningTemplateVersionResponseTypeDef",
     "DescribeRoleAliasRequestRequestTypeDef",
     "RoleAliasDescriptionTypeDef",
     "DescribeScheduledAuditRequestRequestTypeDef",
-    "DescribeScheduledAuditResponseTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
     "DescribeStreamRequestRequestTypeDef",
     "DescribeThingGroupRequestRequestTypeDef",
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
-    "DescribeThingRegistrationTaskResponseTypeDef",
     "DescribeThingRequestRequestTypeDef",
-    "DescribeThingResponseTypeDef",
     "DescribeThingTypeRequestRequestTypeDef",
     "ThingTypeMetadataTypeDef",
     "ThingTypePropertiesOutputTypeDef",
-    "S3DestinationOutputTypeDef",
     "S3DestinationTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "DetachPrincipalPolicyRequestRequestTypeDef",
     "DetachSecurityProfileRequestRequestTypeDef",
     "DetachThingPrincipalRequestRequestTypeDef",
     "DetectMitigationActionExecutionTypeDef",
     "DetectMitigationActionsTaskStatisticsTypeDef",
     "DetectMitigationActionsTaskTargetOutputTypeDef",
     "ViolationEventOccurrenceRangeOutputTypeDef",
     "DetectMitigationActionsTaskTargetTypeDef",
     "DisableTopicRuleRequestRequestTypeDef",
     "DomainConfigurationSummaryTypeDef",
-    "PutItemInputOutputTypeDef",
     "PutItemInputTypeDef",
     "EffectivePolicyTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EnableIoTLoggingParamsOutputTypeDef",
     "EnableIoTLoggingParamsTypeDef",
     "EnableTopicRuleRequestRequestTypeDef",
     "ErrorInfoTypeDef",
-    "RateIncreaseCriteriaOutputTypeDef",
     "RateIncreaseCriteriaTypeDef",
-    "FieldOutputTypeDef",
     "FieldTypeDef",
-    "S3LocationOutputTypeDef",
-    "StreamOutputTypeDef",
     "S3LocationTypeDef",
     "StreamTypeDef",
     "FleetMetricNameAndArnTypeDef",
-    "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     "GetCardinalityRequestRequestTypeDef",
-    "GetCardinalityResponseTypeDef",
     "GetEffectivePoliciesRequestRequestTypeDef",
     "GetJobDocumentRequestRequestTypeDef",
-    "GetJobDocumentResponseTypeDef",
-    "GetLoggingOptionsResponseTypeDef",
     "GetOTAUpdateRequestRequestTypeDef",
-    "VersionUpdateByJobsConfigOutputTypeDef",
+    "VersionUpdateByJobsConfigTypeDef",
     "GetPackageRequestRequestTypeDef",
-    "GetPackageResponseTypeDef",
     "GetPackageVersionRequestRequestTypeDef",
-    "GetPackageVersionResponseTypeDef",
     "GetPercentilesRequestRequestTypeDef",
     "PercentPairTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
-    "GetPolicyVersionResponseTypeDef",
-    "GetRegistrationCodeResponseTypeDef",
     "GetStatisticsRequestRequestTypeDef",
     "StatisticsTypeDef",
     "GetTopicRuleDestinationRequestRequestTypeDef",
     "GetTopicRuleRequestRequestTypeDef",
-    "GetV2LoggingOptionsResponseTypeDef",
     "GroupNameAndArnTypeDef",
-    "HttpActionHeaderOutputTypeDef",
     "HttpActionHeaderTypeDef",
-    "SigV4AuthorizationOutputTypeDef",
     "SigV4AuthorizationTypeDef",
     "HttpContextTypeDef",
     "HttpUrlDestinationConfigurationTypeDef",
     "HttpUrlDestinationPropertiesTypeDef",
     "HttpUrlDestinationSummaryTypeDef",
     "IndexingFilterOutputTypeDef",
     "IndexingFilterTypeDef",
-    "IssuerCertificateIdentifierOutputTypeDef",
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
-    "RetryCriteriaOutputTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
     "ScheduledJobRolloutTypeDef",
-    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
-    "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
     "ListAttachedPoliciesRequestRequestTypeDef",
-    "ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
     "ListAuditMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
     "ListAuditMitigationActionsTasksRequestRequestTypeDef",
-    "ListAuditTasksRequestListAuditTasksPaginateTypeDef",
     "ListAuditTasksRequestRequestTypeDef",
-    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
     "ListAuthorizersRequestRequestTypeDef",
-    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsRequestRequestTypeDef",
-    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
     "ListCACertificatesRequestRequestTypeDef",
-    "ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
     "ListCertificatesByCARequestRequestTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
-    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
     "ListCustomMetricsRequestRequestTypeDef",
-    "ListCustomMetricsResponseTypeDef",
-    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
     "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
     "ListDetectMitigationActionsTasksRequestRequestTypeDef",
-    "ListDimensionsRequestListDimensionsPaginateTypeDef",
     "ListDimensionsRequestRequestTypeDef",
-    "ListDimensionsResponseTypeDef",
-    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
     "ListDomainConfigurationsRequestRequestTypeDef",
-    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
     "ListFleetMetricsRequestRequestTypeDef",
-    "ListIndicesRequestListIndicesPaginateTypeDef",
     "ListIndicesRequestRequestTypeDef",
-    "ListIndicesResponseTypeDef",
-    "ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
     "ListJobExecutionsForJobRequestRequestTypeDef",
-    "ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
     "ListJobExecutionsForThingRequestRequestTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
     "ListManagedJobTemplatesRequestRequestTypeDef",
     "ManagedJobTemplateSummaryTypeDef",
-    "ListMetricValuesRequestListMetricValuesPaginateTypeDef",
     "ListMetricValuesRequestRequestTypeDef",
-    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
     "ListMitigationActionsRequestRequestTypeDef",
     "MitigationActionIdentifierTypeDef",
-    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
     "ListOTAUpdatesRequestRequestTypeDef",
     "OTAUpdateSummaryTypeDef",
-    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
     "ListOutgoingCertificatesRequestRequestTypeDef",
     "OutgoingCertificateTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "PackageVersionSummaryTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageSummaryTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
-    "ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
     "ListPolicyPrincipalsRequestRequestTypeDef",
-    "ListPolicyPrincipalsResponseTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
     "PolicyVersionTypeDef",
-    "ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
     "ListPrincipalPoliciesRequestRequestTypeDef",
-    "ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
     "ListPrincipalThingsRequestRequestTypeDef",
-    "ListPrincipalThingsResponseTypeDef",
-    "ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
     "ListProvisioningTemplateVersionsRequestRequestTypeDef",
     "ProvisioningTemplateVersionSummaryTypeDef",
-    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
     "ListProvisioningTemplatesRequestRequestTypeDef",
     "ProvisioningTemplateSummaryTypeDef",
-    "ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
     "ListRelatedResourcesForAuditFindingRequestRequestTypeDef",
-    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
     "ListRoleAliasesRequestRequestTypeDef",
-    "ListRoleAliasesResponseTypeDef",
-    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
     "ListScheduledAuditsRequestRequestTypeDef",
     "ScheduledAuditMetadataTypeDef",
-    "ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
     "ListSecurityProfilesForTargetRequestRequestTypeDef",
-    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     "ListSecurityProfilesRequestRequestTypeDef",
     "SecurityProfileIdentifierTypeDef",
-    "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "StreamSummaryTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     "ListTargetsForPolicyRequestRequestTypeDef",
-    "ListTargetsForPolicyResponseTypeDef",
-    "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
     "ListTargetsForSecurityProfileRequestRequestTypeDef",
     "SecurityProfileTargetTypeDef",
-    "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
     "ListThingGroupsForThingRequestRequestTypeDef",
-    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
     "ListThingGroupsRequestRequestTypeDef",
-    "ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
     "ListThingPrincipalsRequestRequestTypeDef",
-    "ListThingPrincipalsResponseTypeDef",
-    "ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
     "ListThingRegistrationTaskReportsRequestRequestTypeDef",
-    "ListThingRegistrationTaskReportsResponseTypeDef",
-    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
     "ListThingRegistrationTasksRequestRequestTypeDef",
-    "ListThingRegistrationTasksResponseTypeDef",
-    "ListThingTypesRequestListThingTypesPaginateTypeDef",
     "ListThingTypesRequestRequestTypeDef",
-    "ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
     "ListThingsInBillingGroupRequestRequestTypeDef",
-    "ListThingsInBillingGroupResponseTypeDef",
-    "ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
     "ListThingsInThingGroupRequestRequestTypeDef",
-    "ListThingsInThingGroupResponseTypeDef",
-    "ListThingsRequestListThingsPaginateTypeDef",
     "ListThingsRequestRequestTypeDef",
     "ThingAttributeTypeDef",
-    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
     "ListTopicRuleDestinationsRequestRequestTypeDef",
-    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
     "ListTopicRulesRequestRequestTypeDef",
     "TopicRuleListItemTypeDef",
-    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
     "ListV2LoggingLevelsRequestRequestTypeDef",
-    "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
     "ListViolationEventsRequestRequestTypeDef",
-    "LocationTimestampOutputTypeDef",
     "LocationTimestampTypeDef",
-    "LogTargetOutputTypeDef",
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
-    "PublishFindingToSnsParamsOutputTypeDef",
-    "ReplaceDefaultPolicyVersionParamsOutputTypeDef",
-    "UpdateCACertificateParamsOutputTypeDef",
-    "UpdateDeviceCertificateParamsOutputTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
     "MqttContextTypeDef",
-    "UserPropertyOutputTypeDef",
     "UserPropertyTypeDef",
-    "PaginatorConfigTypeDef",
-    "PolicyVersionIdentifierOutputTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
-    "RegistrationConfigTypeDef",
-    "RegisterCACertificateResponseTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
-    "RegisterCertificateResponseTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
-    "RegisterCertificateWithoutCAResponseTypeDef",
     "RegisterThingRequestRequestTypeDef",
-    "RegisterThingResponseTypeDef",
     "RejectCertificateTransferRequestRequestTypeDef",
     "RemoveThingFromBillingGroupRequestRequestTypeDef",
     "RemoveThingFromThingGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchIndexRequestRequestTypeDef",
     "ThingGroupDocumentTypeDef",
     "SetDefaultAuthorizerRequestRequestTypeDef",
-    "SetDefaultAuthorizerResponseTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetV2LoggingOptionsRequestRequestTypeDef",
-    "SigningProfileParameterOutputTypeDef",
     "SigningProfileParameterTypeDef",
-    "StartAuditMitigationActionsTaskResponseTypeDef",
     "ViolationEventOccurrenceRangeTypeDef",
-    "StartDetectMitigationActionsTaskResponseTypeDef",
     "StartOnDemandAuditTaskRequestRequestTypeDef",
-    "StartOnDemandAuditTaskResponseTypeDef",
     "StartThingRegistrationTaskRequestRequestTypeDef",
-    "StartThingRegistrationTaskResponseTypeDef",
     "StopThingRegistrationTaskRequestRequestTypeDef",
     "TlsContextTypeDef",
-    "TestInvokeAuthorizerResponseTypeDef",
     "ThingConnectivityTypeDef",
-    "TimestreamDimensionOutputTypeDef",
-    "TimestreamTimestampOutputTypeDef",
     "TimestreamDimensionTypeDef",
     "TimestreamTimestampTypeDef",
     "VpcDestinationConfigurationTypeDef",
     "VpcDestinationSummaryTypeDef",
     "VpcDestinationPropertiesTypeDef",
     "TransferCertificateRequestRequestTypeDef",
-    "TransferCertificateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "UpdateAuthorizerResponseTypeDef",
-    "UpdateBillingGroupResponseTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
     "UpdateCustomMetricRequestRequestTypeDef",
-    "UpdateCustomMetricResponseTypeDef",
     "UpdateDimensionRequestRequestTypeDef",
-    "UpdateDimensionResponseTypeDef",
-    "UpdateDomainConfigurationResponseTypeDef",
-    "UpdateDynamicThingGroupResponseTypeDef",
-    "UpdateMitigationActionResponseTypeDef",
-    "VersionUpdateByJobsConfigTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "UpdatePackageVersionRequestRequestTypeDef",
     "UpdateRoleAliasRequestRequestTypeDef",
-    "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditRequestRequestTypeDef",
-    "UpdateScheduledAuditResponseTypeDef",
-    "UpdateStreamResponseTypeDef",
-    "UpdateThingGroupResponseTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
     "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
-    "DescribeFleetMetricResponseTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
+    "AssetPropertyValueTypeDef",
+    "AssociateTargetsWithJobResponseTypeDef",
+    "CancelJobResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateBillingGroupResponseTypeDef",
+    "CreateCertificateFromCsrResponseTypeDef",
+    "CreateCustomMetricResponseTypeDef",
+    "CreateDimensionResponseTypeDef",
+    "CreateDomainConfigurationResponseTypeDef",
+    "CreateDynamicThingGroupResponseTypeDef",
+    "CreateFleetMetricResponseTypeDef",
+    "CreateJobResponseTypeDef",
+    "CreateJobTemplateResponseTypeDef",
+    "CreateMitigationActionResponseTypeDef",
+    "CreateOTAUpdateResponseTypeDef",
+    "CreatePackageResponseTypeDef",
+    "CreatePackageVersionResponseTypeDef",
+    "CreatePolicyResponseTypeDef",
+    "CreatePolicyVersionResponseTypeDef",
+    "CreateProvisioningTemplateResponseTypeDef",
+    "CreateProvisioningTemplateVersionResponseTypeDef",
+    "CreateRoleAliasResponseTypeDef",
+    "CreateScheduledAuditResponseTypeDef",
+    "CreateSecurityProfileResponseTypeDef",
+    "CreateStreamResponseTypeDef",
+    "CreateThingGroupResponseTypeDef",
+    "CreateThingResponseTypeDef",
+    "CreateThingTypeResponseTypeDef",
+    "DescribeCustomMetricResponseTypeDef",
+    "DescribeDimensionResponseTypeDef",
+    "DescribeEndpointResponseTypeDef",
+    "DescribeFleetMetricResponseTypeDef",
+    "DescribeIndexResponseTypeDef",
+    "DescribeProvisioningTemplateVersionResponseTypeDef",
+    "DescribeScheduledAuditResponseTypeDef",
+    "DescribeThingRegistrationTaskResponseTypeDef",
+    "DescribeThingResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCardinalityResponseTypeDef",
+    "GetJobDocumentResponseTypeDef",
+    "GetLoggingOptionsResponseTypeDef",
+    "GetPackageResponseTypeDef",
+    "GetPackageVersionResponseTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetPolicyVersionResponseTypeDef",
+    "GetRegistrationCodeResponseTypeDef",
+    "GetV2LoggingOptionsResponseTypeDef",
     "ListAttachedPoliciesResponseTypeDef",
+    "ListCustomMetricsResponseTypeDef",
+    "ListDimensionsResponseTypeDef",
+    "ListIndicesResponseTypeDef",
     "ListPoliciesResponseTypeDef",
+    "ListPolicyPrincipalsResponseTypeDef",
     "ListPrincipalPoliciesResponseTypeDef",
-    "AssetPropertyValueOutputTypeDef",
-    "AssetPropertyValueTypeDef",
+    "ListPrincipalThingsResponseTypeDef",
+    "ListRoleAliasesResponseTypeDef",
+    "ListTargetsForPolicyResponseTypeDef",
+    "ListThingPrincipalsResponseTypeDef",
+    "ListThingRegistrationTaskReportsResponseTypeDef",
+    "ListThingRegistrationTasksResponseTypeDef",
+    "ListThingsInBillingGroupResponseTypeDef",
+    "ListThingsInThingGroupResponseTypeDef",
+    "RegisterCACertificateResponseTypeDef",
+    "RegisterCertificateResponseTypeDef",
+    "RegisterCertificateWithoutCAResponseTypeDef",
+    "RegisterThingResponseTypeDef",
+    "SetDefaultAuthorizerResponseTypeDef",
+    "StartAuditMitigationActionsTaskResponseTypeDef",
+    "StartDetectMitigationActionsTaskResponseTypeDef",
+    "StartOnDemandAuditTaskResponseTypeDef",
+    "StartThingRegistrationTaskResponseTypeDef",
+    "TestInvokeAuthorizerResponseTypeDef",
+    "TransferCertificateResponseTypeDef",
+    "UpdateAuthorizerResponseTypeDef",
+    "UpdateBillingGroupResponseTypeDef",
+    "UpdateCustomMetricResponseTypeDef",
+    "UpdateDimensionResponseTypeDef",
+    "UpdateDomainConfigurationResponseTypeDef",
+    "UpdateDynamicThingGroupResponseTypeDef",
+    "UpdateMitigationActionResponseTypeDef",
+    "UpdateRoleAliasResponseTypeDef",
+    "UpdateScheduledAuditResponseTypeDef",
+    "UpdateStreamResponseTypeDef",
+    "UpdateThingGroupResponseTypeDef",
     "ThingGroupPropertiesOutputTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
@@ -654,20 +535,18 @@
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
     "TestAuthorizationRequestRequestTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
-    "AwsJobExponentialRolloutRateOutputTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
     "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
-    "MetricToRetainOutputTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
@@ -682,55 +561,110 @@
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainConfigurationRequestRequestTypeDef",
     "UpdateDomainConfigurationRequestRequestTypeDef",
+    "SchedulingConfigOutputTypeDef",
     "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
+    "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
     "DescribeAuditTaskResponseTypeDef",
+    "RegisterCACertificateRequestRequestTypeDef",
+    "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
-    "SchedulingConfigOutputTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
-    "DescribeProvisioningTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
-    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
-    "DynamoDBv2ActionOutputTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
-    "ExponentialRolloutRateOutputTypeDef",
     "ExponentialRolloutRateTypeDef",
     "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
-    "StreamFileOutputTypeDef",
-    "FileLocationOutputTypeDef",
     "StreamFileTypeDef",
     "FileLocationTypeDef",
     "ListFleetMetricsResponseTypeDef",
+    "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
+    "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    "ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    "ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    "ListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
+    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
+    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
+    "ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
+    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
+    "ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    "ListDimensionsRequestListDimensionsPaginateTypeDef",
+    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
+    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
+    "ListIndicesRequestListIndicesPaginateTypeDef",
+    "ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    "ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
+    "ListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
+    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
+    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    "ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    "ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    "ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
+    "ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
+    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
+    "ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
+    "ListStreamsRequestListStreamsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+    "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
+    "ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    "ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
+    "ListThingTypesRequestListThingTypesPaginateTypeDef",
+    "ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    "ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    "ListThingsRequestListThingsPaginateTypeDef",
+    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
+    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
+    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
+    "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
     "GetPackageConfigurationResponseTypeDef",
+    "UpdatePackageConfigurationRequestRequestTypeDef",
     "GetPercentilesResponseTypeDef",
     "GetStatisticsResponseTypeDef",
     "ListBillingGroupsResponseTypeDef",
     "ListThingGroupsForThingResponseTypeDef",
     "ListThingGroupsResponseTypeDef",
     "ThingGroupMetadataTypeDef",
-    "HttpAuthorizationOutputTypeDef",
     "HttpAuthorizationTypeDef",
     "ThingIndexingConfigurationOutputTypeDef",
     "ThingIndexingConfigurationTypeDef",
     "JobExecutionTypeDef",
     "JobExecutionSummaryForJobTypeDef",
     "JobExecutionSummaryForThingTypeDef",
     "JobExecutionsRetryConfigOutputTypeDef",
@@ -745,64 +679,55 @@
     "ListPackagesResponseTypeDef",
     "ListPolicyVersionsResponseTypeDef",
     "ListProvisioningTemplateVersionsResponseTypeDef",
     "ListProvisioningTemplatesResponseTypeDef",
     "ListScheduledAuditsResponseTypeDef",
     "ListSecurityProfilesResponseTypeDef",
     "ListStreamsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTargetsForSecurityProfileResponseTypeDef",
     "SecurityProfileTargetMappingTypeDef",
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
-    "LocationActionOutputTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
     "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
     "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
-    "ResourceIdentifierOutputTypeDef",
     "ResourceIdentifierTypeDef",
-    "RegisterCACertificateRequestRequestTypeDef",
-    "UpdateCACertificateRequestRequestTypeDef",
     "StartDetectMitigationActionsTaskRequestRequestTypeDef",
     "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
     "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
-    "UpdatePackageConfigurationRequestRequestTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
     "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
-    "AwsJobExecutionsRolloutConfigOutputTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
     "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
     "ListThingTypesResponseTypeDef",
-    "StartSigningJobParameterOutputTypeDef",
     "StartSigningJobParameterTypeDef",
-    "JobExecutionsRolloutConfigOutputTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
-    "StreamInfoTypeDef",
     "CreateStreamRequestRequestTypeDef",
+    "StreamInfoTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
     "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
@@ -813,24 +738,24 @@
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
     "CreateMitigationActionRequestRequestTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
     "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
-    "DescribeAuditSuppressionResponseTypeDef",
-    "NonCompliantResourceTypeDef",
-    "RelatedResourceTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
+    "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     "ListAuditFindingsRequestRequestTypeDef",
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
     "ListAuditSuppressionsRequestRequestTypeDef",
+    "NonCompliantResourceTypeDef",
+    "RelatedResourceTypeDef",
     "UpdateAuditSuppressionRequestRequestTypeDef",
     "SearchIndexResponseTypeDef",
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     "ListTopicRuleDestinationsResponseTypeDef",
     "CreateTopicRuleDestinationResponseTypeDef",
     "GetTopicRuleDestinationResponseTypeDef",
     "AuthResultTypeDef",
@@ -841,18 +766,18 @@
     "UpdateSecurityProfileResponseTypeDef",
     "ViolationEventTypeDef",
     "CreateSecurityProfileRequestRequestTypeDef",
     "UpdateSecurityProfileRequestRequestTypeDef",
     "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
-    "DescribeJobTemplateResponseTypeDef",
-    "JobTypeDef",
     "CreateJobRequestRequestTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
+    "DescribeJobTemplateResponseTypeDef",
+    "JobTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "DescribeStreamResponseTypeDef",
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     "DetectMitigationActionsTaskSummaryTypeDef",
     "ListAuditSuppressionsResponseTypeDef",
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
@@ -874,24 +799,14 @@
     "CreateOTAUpdateRequestRequestTypeDef",
     "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
     "GetOTAUpdateResponseTypeDef",
 )
 
-AbortCriteriaOutputTypeDef = TypedDict(
-    "AbortCriteriaOutputTypeDef",
-    {
-        "failureType": JobExecutionFailureTypeType,
-        "action": Literal["CANCEL"],
-        "thresholdPercentage": float,
-        "minNumberOfExecutedThings": int,
-    },
-)
-
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
@@ -916,323 +831,14 @@
 class AcceptCertificateTransferRequestRequestTypeDef(
     _RequiredAcceptCertificateTransferRequestRequestTypeDef,
     _OptionalAcceptCertificateTransferRequestRequestTypeDef,
 ):
     pass
 
 
-CloudwatchAlarmActionOutputTypeDef = TypedDict(
-    "CloudwatchAlarmActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "alarmName": str,
-        "stateReason": str,
-        "stateValue": str,
-    },
-)
-
-_RequiredCloudwatchLogsActionOutputTypeDef = TypedDict(
-    "_RequiredCloudwatchLogsActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "logGroupName": str,
-    },
-)
-_OptionalCloudwatchLogsActionOutputTypeDef = TypedDict(
-    "_OptionalCloudwatchLogsActionOutputTypeDef",
-    {
-        "batchMode": bool,
-    },
-    total=False,
-)
-
-
-class CloudwatchLogsActionOutputTypeDef(
-    _RequiredCloudwatchLogsActionOutputTypeDef, _OptionalCloudwatchLogsActionOutputTypeDef
-):
-    pass
-
-
-_RequiredCloudwatchMetricActionOutputTypeDef = TypedDict(
-    "_RequiredCloudwatchMetricActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "metricNamespace": str,
-        "metricName": str,
-        "metricValue": str,
-        "metricUnit": str,
-    },
-)
-_OptionalCloudwatchMetricActionOutputTypeDef = TypedDict(
-    "_OptionalCloudwatchMetricActionOutputTypeDef",
-    {
-        "metricTimestamp": str,
-    },
-    total=False,
-)
-
-
-class CloudwatchMetricActionOutputTypeDef(
-    _RequiredCloudwatchMetricActionOutputTypeDef, _OptionalCloudwatchMetricActionOutputTypeDef
-):
-    pass
-
-
-_RequiredDynamoDBActionOutputTypeDef = TypedDict(
-    "_RequiredDynamoDBActionOutputTypeDef",
-    {
-        "tableName": str,
-        "roleArn": str,
-        "hashKeyField": str,
-        "hashKeyValue": str,
-    },
-)
-_OptionalDynamoDBActionOutputTypeDef = TypedDict(
-    "_OptionalDynamoDBActionOutputTypeDef",
-    {
-        "operation": str,
-        "hashKeyType": DynamoKeyTypeType,
-        "rangeKeyField": str,
-        "rangeKeyValue": str,
-        "rangeKeyType": DynamoKeyTypeType,
-        "payloadField": str,
-    },
-    total=False,
-)
-
-
-class DynamoDBActionOutputTypeDef(
-    _RequiredDynamoDBActionOutputTypeDef, _OptionalDynamoDBActionOutputTypeDef
-):
-    pass
-
-
-ElasticsearchActionOutputTypeDef = TypedDict(
-    "ElasticsearchActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "endpoint": str,
-        "index": str,
-        "type": str,
-        "id": str,
-    },
-)
-
-_RequiredFirehoseActionOutputTypeDef = TypedDict(
-    "_RequiredFirehoseActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "deliveryStreamName": str,
-    },
-)
-_OptionalFirehoseActionOutputTypeDef = TypedDict(
-    "_OptionalFirehoseActionOutputTypeDef",
-    {
-        "separator": str,
-        "batchMode": bool,
-    },
-    total=False,
-)
-
-
-class FirehoseActionOutputTypeDef(
-    _RequiredFirehoseActionOutputTypeDef, _OptionalFirehoseActionOutputTypeDef
-):
-    pass
-
-
-IotAnalyticsActionOutputTypeDef = TypedDict(
-    "IotAnalyticsActionOutputTypeDef",
-    {
-        "channelArn": str,
-        "channelName": str,
-        "batchMode": bool,
-        "roleArn": str,
-    },
-    total=False,
-)
-
-_RequiredIotEventsActionOutputTypeDef = TypedDict(
-    "_RequiredIotEventsActionOutputTypeDef",
-    {
-        "inputName": str,
-        "roleArn": str,
-    },
-)
-_OptionalIotEventsActionOutputTypeDef = TypedDict(
-    "_OptionalIotEventsActionOutputTypeDef",
-    {
-        "messageId": str,
-        "batchMode": bool,
-    },
-    total=False,
-)
-
-
-class IotEventsActionOutputTypeDef(
-    _RequiredIotEventsActionOutputTypeDef, _OptionalIotEventsActionOutputTypeDef
-):
-    pass
-
-
-_RequiredKafkaActionOutputTypeDef = TypedDict(
-    "_RequiredKafkaActionOutputTypeDef",
-    {
-        "destinationArn": str,
-        "topic": str,
-        "clientProperties": Dict[str, str],
-    },
-)
-_OptionalKafkaActionOutputTypeDef = TypedDict(
-    "_OptionalKafkaActionOutputTypeDef",
-    {
-        "key": str,
-        "partition": str,
-    },
-    total=False,
-)
-
-
-class KafkaActionOutputTypeDef(
-    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
-):
-    pass
-
-
-_RequiredKinesisActionOutputTypeDef = TypedDict(
-    "_RequiredKinesisActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "streamName": str,
-    },
-)
-_OptionalKinesisActionOutputTypeDef = TypedDict(
-    "_OptionalKinesisActionOutputTypeDef",
-    {
-        "partitionKey": str,
-    },
-    total=False,
-)
-
-
-class KinesisActionOutputTypeDef(
-    _RequiredKinesisActionOutputTypeDef, _OptionalKinesisActionOutputTypeDef
-):
-    pass
-
-
-LambdaActionOutputTypeDef = TypedDict(
-    "LambdaActionOutputTypeDef",
-    {
-        "functionArn": str,
-    },
-)
-
-OpenSearchActionOutputTypeDef = TypedDict(
-    "OpenSearchActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "endpoint": str,
-        "index": str,
-        "type": str,
-        "id": str,
-    },
-)
-
-_RequiredS3ActionOutputTypeDef = TypedDict(
-    "_RequiredS3ActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "bucketName": str,
-        "key": str,
-    },
-)
-_OptionalS3ActionOutputTypeDef = TypedDict(
-    "_OptionalS3ActionOutputTypeDef",
-    {
-        "cannedAcl": CannedAccessControlListType,
-    },
-    total=False,
-)
-
-
-class S3ActionOutputTypeDef(_RequiredS3ActionOutputTypeDef, _OptionalS3ActionOutputTypeDef):
-    pass
-
-
-SalesforceActionOutputTypeDef = TypedDict(
-    "SalesforceActionOutputTypeDef",
-    {
-        "token": str,
-        "url": str,
-    },
-)
-
-_RequiredSnsActionOutputTypeDef = TypedDict(
-    "_RequiredSnsActionOutputTypeDef",
-    {
-        "targetArn": str,
-        "roleArn": str,
-    },
-)
-_OptionalSnsActionOutputTypeDef = TypedDict(
-    "_OptionalSnsActionOutputTypeDef",
-    {
-        "messageFormat": MessageFormatType,
-    },
-    total=False,
-)
-
-
-class SnsActionOutputTypeDef(_RequiredSnsActionOutputTypeDef, _OptionalSnsActionOutputTypeDef):
-    pass
-
-
-_RequiredSqsActionOutputTypeDef = TypedDict(
-    "_RequiredSqsActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "queueUrl": str,
-    },
-)
-_OptionalSqsActionOutputTypeDef = TypedDict(
-    "_OptionalSqsActionOutputTypeDef",
-    {
-        "useBase64": bool,
-    },
-    total=False,
-)
-
-
-class SqsActionOutputTypeDef(_RequiredSqsActionOutputTypeDef, _OptionalSqsActionOutputTypeDef):
-    pass
-
-
-_RequiredStepFunctionsActionOutputTypeDef = TypedDict(
-    "_RequiredStepFunctionsActionOutputTypeDef",
-    {
-        "stateMachineName": str,
-        "roleArn": str,
-    },
-)
-_OptionalStepFunctionsActionOutputTypeDef = TypedDict(
-    "_OptionalStepFunctionsActionOutputTypeDef",
-    {
-        "executionNamePrefix": str,
-    },
-    total=False,
-)
-
-
-class StepFunctionsActionOutputTypeDef(
-    _RequiredStepFunctionsActionOutputTypeDef, _OptionalStepFunctionsActionOutputTypeDef
-):
-    pass
-
-
 CloudwatchAlarmActionTypeDef = TypedDict(
     "CloudwatchAlarmActionTypeDef",
     {
         "roleArn": str,
         "alarmName": str,
         "stateReason": str,
         "stateValue": str,
@@ -1373,33 +979,35 @@
 )
 
 
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
 
-_RequiredKafkaActionTypeDef = TypedDict(
-    "_RequiredKafkaActionTypeDef",
+_RequiredKafkaActionOutputTypeDef = TypedDict(
+    "_RequiredKafkaActionOutputTypeDef",
     {
         "destinationArn": str,
         "topic": str,
-        "clientProperties": Mapping[str, str],
+        "clientProperties": Dict[str, str],
     },
 )
-_OptionalKafkaActionTypeDef = TypedDict(
-    "_OptionalKafkaActionTypeDef",
+_OptionalKafkaActionOutputTypeDef = TypedDict(
+    "_OptionalKafkaActionOutputTypeDef",
     {
         "key": str,
         "partition": str,
     },
     total=False,
 )
 
 
-class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
+class KafkaActionOutputTypeDef(
+    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
+):
     pass
 
 
 _RequiredKinesisActionTypeDef = TypedDict(
     "_RequiredKinesisActionTypeDef",
     {
         "roleArn": str,
@@ -1524,14 +1132,36 @@
 
 class StepFunctionsActionTypeDef(
     _RequiredStepFunctionsActionTypeDef, _OptionalStepFunctionsActionTypeDef
 ):
     pass
 
 
+_RequiredKafkaActionTypeDef = TypedDict(
+    "_RequiredKafkaActionTypeDef",
+    {
+        "destinationArn": str,
+        "topic": str,
+        "clientProperties": Mapping[str, str],
+    },
+)
+_OptionalKafkaActionTypeDef = TypedDict(
+    "_OptionalKafkaActionTypeDef",
+    {
+        "key": str,
+        "partition": str,
+    },
+    total=False,
+)
+
+
+class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
+    pass
+
+
 MetricValueOutputTypeDef = TypedDict(
     "MetricValueOutputTypeDef",
     {
         "count": int,
         "cidrs": List[str],
         "ports": List[int],
         "number": float,
@@ -1651,22 +1281,14 @@
 )
 
 
 class AggregationTypeTypeDef(_RequiredAggregationTypeTypeDef, _OptionalAggregationTypeTypeDef):
     pass
 
 
-AlertTargetOutputTypeDef = TypedDict(
-    "AlertTargetOutputTypeDef",
-    {
-        "alertTargetArn": str,
-        "roleArn": str,
-    },
-)
-
 AlertTargetTypeDef = TypedDict(
     "AlertTargetTypeDef",
     {
         "alertTargetArn": str,
         "roleArn": str,
     },
 )
@@ -1676,35 +1298,14 @@
     {
         "policyName": str,
         "policyArn": str,
     },
     total=False,
 )
 
-_RequiredAssetPropertyTimestampOutputTypeDef = TypedDict(
-    "_RequiredAssetPropertyTimestampOutputTypeDef",
-    {
-        "timeInSeconds": str,
-    },
-)
-_OptionalAssetPropertyTimestampOutputTypeDef = TypedDict(
-    "_OptionalAssetPropertyTimestampOutputTypeDef",
-    {
-        "offsetInNanos": str,
-    },
-    total=False,
-)
-
-
-class AssetPropertyTimestampOutputTypeDef(
-    _RequiredAssetPropertyTimestampOutputTypeDef, _OptionalAssetPropertyTimestampOutputTypeDef
-):
-    pass
-
-
 _RequiredAssetPropertyTimestampTypeDef = TypedDict(
     "_RequiredAssetPropertyTimestampTypeDef",
     {
         "timeInSeconds": str,
     },
 )
 _OptionalAssetPropertyTimestampTypeDef = TypedDict(
@@ -1718,25 +1319,14 @@
 
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
 
-AssetPropertyVariantOutputTypeDef = TypedDict(
-    "AssetPropertyVariantOutputTypeDef",
-    {
-        "stringValue": str,
-        "integerValue": str,
-        "doubleValue": str,
-        "booleanValue": str,
-    },
-    total=False,
-)
-
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
@@ -1764,21 +1354,22 @@
 class AssociateTargetsWithJobRequestRequestTypeDef(
     _RequiredAssociateTargetsWithJobRequestRequestTypeDef,
     _OptionalAssociateTargetsWithJobRequestRequestTypeDef,
 ):
     pass
 
 
-AssociateTargetsWithJobResponseTypeDef = TypedDict(
-    "AssociateTargetsWithJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AttachPolicyRequestRequestTypeDef = TypedDict(
     "AttachPolicyRequestRequestTypeDef",
     {
         "policyName": str,
@@ -1824,22 +1415,14 @@
     {
         "attributes": Mapping[str, str],
         "merge": bool,
     },
     total=False,
 )
 
-AuditCheckConfigurationOutputTypeDef = TypedDict(
-    "AuditCheckConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-    total=False,
-)
-
 AuditCheckConfigurationTypeDef = TypedDict(
     "AuditCheckConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
@@ -1900,24 +1483,14 @@
         "auditTaskId": str,
         "findingIds": Sequence[str],
         "auditCheckToReasonCodeFilter": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-AuditNotificationTargetOutputTypeDef = TypedDict(
-    "AuditNotificationTargetOutputTypeDef",
-    {
-        "targetArn": str,
-        "roleArn": str,
-        "enabled": bool,
-    },
-    total=False,
-)
-
 AuditNotificationTargetTypeDef = TypedDict(
     "AuditNotificationTargetTypeDef",
     {
         "targetArn": str,
         "roleArn": str,
         "enabled": bool,
     },
@@ -1968,23 +1541,14 @@
 )
 
 
 class AuthInfoTypeDef(_RequiredAuthInfoTypeDef, _OptionalAuthInfoTypeDef):
     pass
 
 
-AuthorizerConfigOutputTypeDef = TypedDict(
-    "AuthorizerConfigOutputTypeDef",
-    {
-        "defaultAuthorizerName": str,
-        "allowAuthorizerOverride": bool,
-    },
-    total=False,
-)
-
 AuthorizerConfigTypeDef = TypedDict(
     "AuthorizerConfigTypeDef",
     {
         "defaultAuthorizerName": str,
         "allowAuthorizerOverride": bool,
     },
     total=False,
@@ -2022,40 +1586,23 @@
         "failureType": AwsJobAbortCriteriaFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
     },
 )
 
-AwsJobRateIncreaseCriteriaOutputTypeDef = TypedDict(
-    "AwsJobRateIncreaseCriteriaOutputTypeDef",
-    {
-        "numberOfNotifiedThings": int,
-        "numberOfSucceededThings": int,
-    },
-    total=False,
-)
-
 AwsJobRateIncreaseCriteriaTypeDef = TypedDict(
     "AwsJobRateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
 )
 
-AwsJobPresignedUrlConfigOutputTypeDef = TypedDict(
-    "AwsJobPresignedUrlConfigOutputTypeDef",
-    {
-        "expiresInSec": int,
-    },
-    total=False,
-)
-
 AwsJobPresignedUrlConfigTypeDef = TypedDict(
     "AwsJobPresignedUrlConfigTypeDef",
     {
         "expiresInSec": int,
     },
     total=False,
 )
@@ -2064,91 +1611,55 @@
     "AwsJobTimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
-MachineLearningDetectionConfigOutputTypeDef = TypedDict(
-    "MachineLearningDetectionConfigOutputTypeDef",
+MachineLearningDetectionConfigTypeDef = TypedDict(
+    "MachineLearningDetectionConfigTypeDef",
     {
         "confidenceLevel": ConfidenceLevelType,
     },
 )
 
-StatisticalThresholdOutputTypeDef = TypedDict(
-    "StatisticalThresholdOutputTypeDef",
+StatisticalThresholdTypeDef = TypedDict(
+    "StatisticalThresholdTypeDef",
     {
         "statistic": str,
     },
     total=False,
 )
 
-MachineLearningDetectionConfigTypeDef = TypedDict(
-    "MachineLearningDetectionConfigTypeDef",
-    {
-        "confidenceLevel": ConfidenceLevelType,
-    },
-)
-
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "count": int,
         "cidrs": Sequence[str],
         "ports": Sequence[int],
         "number": float,
         "numbers": Sequence[float],
         "strings": Sequence[str],
     },
     total=False,
 )
 
-StatisticalThresholdTypeDef = TypedDict(
-    "StatisticalThresholdTypeDef",
-    {
-        "statistic": str,
-    },
-    total=False,
-)
-
 BehaviorModelTrainingSummaryTypeDef = TypedDict(
     "BehaviorModelTrainingSummaryTypeDef",
     {
         "securityProfileName": str,
         "behaviorName": str,
         "trainingDataCollectionStartDate": datetime,
         "modelStatus": ModelStatusType,
         "datapointsCollectionPercentage": float,
         "lastModelRefreshDate": datetime,
     },
     total=False,
 )
 
-_RequiredMetricDimensionOutputTypeDef = TypedDict(
-    "_RequiredMetricDimensionOutputTypeDef",
-    {
-        "dimensionName": str,
-    },
-)
-_OptionalMetricDimensionOutputTypeDef = TypedDict(
-    "_OptionalMetricDimensionOutputTypeDef",
-    {
-        "operator": DimensionValueOperatorType,
-    },
-    total=False,
-)
-
-
-class MetricDimensionOutputTypeDef(
-    _RequiredMetricDimensionOutputTypeDef, _OptionalMetricDimensionOutputTypeDef
-):
-    pass
-
-
 _RequiredMetricDimensionTypeDef = TypedDict(
     "_RequiredMetricDimensionTypeDef",
     {
         "dimensionName": str,
     },
 )
 _OptionalMetricDimensionTypeDef = TypedDict(
@@ -2168,22 +1679,14 @@
     "BillingGroupMetadataTypeDef",
     {
         "creationDate": datetime,
     },
     total=False,
 )
 
-BillingGroupPropertiesOutputTypeDef = TypedDict(
-    "BillingGroupPropertiesOutputTypeDef",
-    {
-        "billingGroupDescription": str,
-    },
-    total=False,
-)
-
 BillingGroupPropertiesTypeDef = TypedDict(
     "BillingGroupPropertiesTypeDef",
     {
         "billingGroupDescription": str,
     },
     total=False,
 )
@@ -2297,24 +1800,14 @@
 
 class CancelJobRequestRequestTypeDef(
     _RequiredCancelJobRequestRequestTypeDef, _OptionalCancelJobRequestRequestTypeDef
 ):
     pass
 
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TransferDataTypeDef = TypedDict(
     "TransferDataTypeDef",
     {
         "transferMessage": str,
         "rejectReason": str,
         "transferDate": datetime,
         "acceptDate": datetime,
@@ -2331,23 +1824,14 @@
         "status": CertificateStatusType,
         "certificateMode": CertificateModeType,
         "creationDate": datetime,
     },
     total=False,
 )
 
-CodeSigningCertificateChainOutputTypeDef = TypedDict(
-    "CodeSigningCertificateChainOutputTypeDef",
-    {
-        "certificateName": str,
-        "inlineDocument": str,
-    },
-    total=False,
-)
-
 CodeSigningCertificateChainTypeDef = TypedDict(
     "CodeSigningCertificateChainTypeDef",
     {
         "certificateName": str,
         "inlineDocument": str,
     },
     total=False,
@@ -2365,22 +1849,14 @@
     "CodeSigningSignatureTypeDef",
     {
         "inlineDocument": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-ConfigurationOutputTypeDef = TypedDict(
-    "ConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -2407,33 +1883,14 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateBillingGroupResponseTypeDef = TypedDict(
-    "CreateBillingGroupResponseTypeDef",
-    {
-        "billingGroupName": str,
-        "billingGroupArn": str,
-        "billingGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCertificateFromCsrRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateFromCsrRequestRequestTypeDef",
     {
         "certificateSigningRequest": str,
     },
 )
 _OptionalCreateCertificateFromCsrRequestRequestTypeDef = TypedDict(
@@ -2448,81 +1905,22 @@
 class CreateCertificateFromCsrRequestRequestTypeDef(
     _RequiredCreateCertificateFromCsrRequestRequestTypeDef,
     _OptionalCreateCertificateFromCsrRequestRequestTypeDef,
 ):
     pass
 
 
-CreateCertificateFromCsrResponseTypeDef = TypedDict(
-    "CreateCertificateFromCsrResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "certificatePem": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomMetricResponseTypeDef = TypedDict(
-    "CreateCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDimensionResponseTypeDef = TypedDict(
-    "CreateDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "securityPolicy": str,
     },
     total=False,
 )
 
-CreateDomainConfigurationResponseTypeDef = TypedDict(
-    "CreateDomainConfigurationResponseTypeDef",
-    {
-        "domainConfigurationName": str,
-        "domainConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDynamicThingGroupResponseTypeDef = TypedDict(
-    "CreateDynamicThingGroupResponseTypeDef",
-    {
-        "thingGroupName": str,
-        "thingGroupArn": str,
-        "thingGroupId": str,
-        "indexName": str,
-        "queryString": str,
-        "queryVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFleetMetricResponseTypeDef = TypedDict(
-    "CreateFleetMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PresignedUrlConfigTypeDef = TypedDict(
     "PresignedUrlConfigTypeDef",
     {
         "roleArn": str,
         "expiresInSec": int,
     },
     total=False,
@@ -2532,41 +1930,22 @@
     "TimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MaintenanceWindowTypeDef = TypedDict(
     "MaintenanceWindowTypeDef",
     {
         "startTime": str,
         "durationInMinutes": int,
     },
 )
 
-CreateJobTemplateResponseTypeDef = TypedDict(
-    "CreateJobTemplateResponseTypeDef",
-    {
-        "jobTemplateArn": str,
-        "jobTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateKeysAndCertificateRequestRequestTypeDef = TypedDict(
     "CreateKeysAndCertificateRequestRequestTypeDef",
     {
         "setAsActive": bool,
     },
     total=False,
 )
@@ -2576,35 +1955,14 @@
     {
         "PublicKey": str,
         "PrivateKey": str,
     },
     total=False,
 )
 
-CreateMitigationActionResponseTypeDef = TypedDict(
-    "CreateMitigationActionResponseTypeDef",
-    {
-        "actionArn": str,
-        "actionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateOTAUpdateResponseTypeDef = TypedDict(
-    "CreateOTAUpdateResponseTypeDef",
-    {
-        "otaUpdateId": str,
-        "awsIotJobId": str,
-        "otaUpdateArn": str,
-        "awsIotJobArn": str,
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -2620,24 +1978,14 @@
 
 class CreatePackageRequestRequestTypeDef(
     _RequiredCreatePackageRequestRequestTypeDef, _OptionalCreatePackageRequestRequestTypeDef
 ):
     pass
 
 
-CreatePackageResponseTypeDef = TypedDict(
-    "CreatePackageResponseTypeDef",
-    {
-        "packageName": str,
-        "packageArn": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageVersionRequestRequestTypeDef",
     {
         "packageName": str,
         "versionName": str,
     },
 )
@@ -2656,39 +2004,14 @@
 class CreatePackageVersionRequestRequestTypeDef(
     _RequiredCreatePackageVersionRequestRequestTypeDef,
     _OptionalCreatePackageVersionRequestRequestTypeDef,
 ):
     pass
 
 
-CreatePackageVersionResponseTypeDef = TypedDict(
-    "CreatePackageVersionResponseTypeDef",
-    {
-        "packageVersionArn": str,
-        "packageName": str,
-        "versionName": str,
-        "description": str,
-        "attributes": Dict[str, str],
-        "status": PackageVersionStatusType,
-        "errorReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePolicyResponseTypeDef = TypedDict(
-    "CreatePolicyResponseTypeDef",
-    {
-        "policyName": str,
-        "policyArn": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePolicyVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
     },
 )
@@ -2704,25 +2027,14 @@
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
 
-CreatePolicyVersionResponseTypeDef = TypedDict(
-    "CreatePolicyVersionResponseTypeDef",
-    {
-        "policyArn": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProvisioningClaimRequestRequestTypeDef = TypedDict(
     "CreateProvisioningClaimRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 
@@ -2741,24 +2053,14 @@
 )
 
 
 class ProvisioningHookTypeDef(_RequiredProvisioningHookTypeDef, _OptionalProvisioningHookTypeDef):
     pass
 
 
-CreateProvisioningTemplateResponseTypeDef = TypedDict(
-    "CreateProvisioningTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "defaultVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "templateBody": str,
     },
 )
@@ -2774,101 +2076,23 @@
 class CreateProvisioningTemplateVersionRequestRequestTypeDef(
     _RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef,
     _OptionalCreateProvisioningTemplateVersionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateProvisioningTemplateVersionResponseTypeDef = TypedDict(
-    "CreateProvisioningTemplateVersionResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "versionId": int,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRoleAliasResponseTypeDef = TypedDict(
-    "CreateRoleAliasResponseTypeDef",
-    {
-        "roleAlias": str,
-        "roleAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateScheduledAuditResponseTypeDef = TypedDict(
-    "CreateScheduledAuditResponseTypeDef",
-    {
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSecurityProfileResponseTypeDef = TypedDict(
-    "CreateSecurityProfileResponseTypeDef",
-    {
-        "securityProfileName": str,
-        "securityProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStreamResponseTypeDef = TypedDict(
-    "CreateStreamResponseTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "description": str,
-        "streamVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThingGroupResponseTypeDef = TypedDict(
-    "CreateThingGroupResponseTypeDef",
-    {
-        "thingGroupName": str,
-        "thingGroupArn": str,
-        "thingGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThingResponseTypeDef = TypedDict(
-    "CreateThingResponseTypeDef",
-    {
-        "thingName": str,
-        "thingArn": str,
-        "thingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ThingTypePropertiesTypeDef = TypedDict(
     "ThingTypePropertiesTypeDef",
     {
         "thingTypeDescription": str,
         "searchableAttributes": Sequence[str],
     },
     total=False,
 )
 
-CreateThingTypeResponseTypeDef = TypedDict(
-    "CreateThingTypeResponseTypeDef",
-    {
-        "thingTypeName": str,
-        "thingTypeArn": str,
-        "thingTypeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAccountAuditConfigurationRequestRequestTypeDef",
     {
         "deleteScheduledAudits": bool,
     },
     total=False,
 )
@@ -3351,16 +2575,16 @@
 DescribeCACertificateRequestRequestTypeDef = TypedDict(
     "DescribeCACertificateRequestRequestTypeDef",
     {
         "certificateId": str,
     },
 )
 
-RegistrationConfigOutputTypeDef = TypedDict(
-    "RegistrationConfigOutputTypeDef",
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
     {
         "templateBody": str,
         "roleArn": str,
         "templateName": str,
     },
     total=False,
 )
@@ -3375,54 +2599,28 @@
 DescribeCustomMetricRequestRequestTypeDef = TypedDict(
     "DescribeCustomMetricRequestRequestTypeDef",
     {
         "metricName": str,
     },
 )
 
-DescribeCustomMetricResponseTypeDef = TypedDict(
-    "DescribeCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "metricType": CustomMetricTypeType,
-        "displayName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
 DescribeDimensionRequestRequestTypeDef = TypedDict(
     "DescribeDimensionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DescribeDimensionResponseTypeDef = TypedDict(
-    "DescribeDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "type": Literal["TOPIC_FILTER"],
-        "stringValues": List[str],
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDomainConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDomainConfigurationRequestRequestTypeDef",
     {
         "domainConfigurationName": str,
     },
 )
 
@@ -3432,62 +2630,36 @@
         "serverCertificateArn": str,
         "serverCertificateStatus": ServerCertificateStatusType,
         "serverCertificateStatusDetail": str,
     },
     total=False,
 )
 
-TlsConfigOutputTypeDef = TypedDict(
-    "TlsConfigOutputTypeDef",
-    {
-        "securityPolicy": str,
-    },
-    total=False,
-)
-
 DescribeEndpointRequestRequestTypeDef = TypedDict(
     "DescribeEndpointRequestRequestTypeDef",
     {
         "endpointType": str,
     },
     total=False,
 )
 
-DescribeEndpointResponseTypeDef = TypedDict(
-    "DescribeEndpointResponseTypeDef",
-    {
-        "endpointAddress": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetMetricRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
     },
 )
 
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "indexName": str,
     },
 )
 
-DescribeIndexResponseTypeDef = TypedDict(
-    "DescribeIndexResponseTypeDef",
-    {
-        "indexName": str,
-        "indexStatus": IndexStatusType,
-        "schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobExecutionRequestRequestTypeDef",
     {
         "jobId": str,
         "thingName": str,
     },
 )
@@ -3517,39 +2689,14 @@
 DescribeJobTemplateRequestRequestTypeDef = TypedDict(
     "DescribeJobTemplateRequestRequestTypeDef",
     {
         "jobTemplateId": str,
     },
 )
 
-MaintenanceWindowOutputTypeDef = TypedDict(
-    "MaintenanceWindowOutputTypeDef",
-    {
-        "startTime": str,
-        "durationInMinutes": int,
-    },
-)
-
-PresignedUrlConfigOutputTypeDef = TypedDict(
-    "PresignedUrlConfigOutputTypeDef",
-    {
-        "roleArn": str,
-        "expiresInSec": int,
-    },
-    total=False,
-)
-
-TimeoutConfigOutputTypeDef = TypedDict(
-    "TimeoutConfigOutputTypeDef",
-    {
-        "inProgressTimeoutInMinutes": int,
-    },
-    total=False,
-)
-
 _RequiredDescribeManagedJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeManagedJobTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalDescribeManagedJobTemplateRequestRequestTypeDef = TypedDict(
@@ -3590,54 +2737,22 @@
 DescribeProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "DescribeProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 
-_RequiredProvisioningHookOutputTypeDef = TypedDict(
-    "_RequiredProvisioningHookOutputTypeDef",
-    {
-        "targetArn": str,
-    },
-)
-_OptionalProvisioningHookOutputTypeDef = TypedDict(
-    "_OptionalProvisioningHookOutputTypeDef",
-    {
-        "payloadVersion": str,
-    },
-    total=False,
-)
-
-
-class ProvisioningHookOutputTypeDef(
-    _RequiredProvisioningHookOutputTypeDef, _OptionalProvisioningHookOutputTypeDef
-):
-    pass
-
-
 DescribeProvisioningTemplateVersionRequestRequestTypeDef = TypedDict(
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "versionId": int,
     },
 )
 
-DescribeProvisioningTemplateVersionResponseTypeDef = TypedDict(
-    "DescribeProvisioningTemplateVersionResponseTypeDef",
-    {
-        "versionId": int,
-        "creationDate": datetime,
-        "templateBody": str,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRoleAliasRequestRequestTypeDef = TypedDict(
     "DescribeRoleAliasRequestRequestTypeDef",
     {
         "roleAlias": str,
     },
 )
 
@@ -3658,27 +2773,14 @@
 DescribeScheduledAuditRequestRequestTypeDef = TypedDict(
     "DescribeScheduledAuditRequestRequestTypeDef",
     {
         "scheduledAuditName": str,
     },
 )
 
-DescribeScheduledAuditResponseTypeDef = TypedDict(
-    "DescribeScheduledAuditResponseTypeDef",
-    {
-        "frequency": AuditFrequencyType,
-        "dayOfMonth": str,
-        "dayOfWeek": DayOfWeekType,
-        "targetCheckNames": List[str],
-        "scheduledAuditName": str,
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSecurityProfileRequestRequestTypeDef = TypedDict(
     "DescribeSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 
@@ -3699,55 +2801,21 @@
 DescribeThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-DescribeThingRegistrationTaskResponseTypeDef = TypedDict(
-    "DescribeThingRegistrationTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "templateBody": str,
-        "inputFileBucket": str,
-        "inputFileKey": str,
-        "roleArn": str,
-        "status": StatusType,
-        "message": str,
-        "successCount": int,
-        "failureCount": int,
-        "percentageProgress": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeThingRequestRequestTypeDef = TypedDict(
     "DescribeThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
-DescribeThingResponseTypeDef = TypedDict(
-    "DescribeThingResponseTypeDef",
-    {
-        "defaultClientId": str,
-        "thingName": str,
-        "thingId": str,
-        "thingArn": str,
-        "thingTypeName": str,
-        "attributes": Dict[str, str],
-        "version": int,
-        "billingGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeThingTypeRequestRequestTypeDef = TypedDict(
     "DescribeThingTypeRequestRequestTypeDef",
     {
         "thingTypeName": str,
     },
 )
 
@@ -3766,23 +2834,14 @@
     {
         "thingTypeDescription": str,
         "searchableAttributes": List[str],
     },
     total=False,
 )
 
-S3DestinationOutputTypeDef = TypedDict(
-    "S3DestinationOutputTypeDef",
-    {
-        "bucket": str,
-        "prefix": str,
-    },
-    total=False,
-)
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -3887,21 +2946,14 @@
         "domainConfigurationName": str,
         "domainConfigurationArn": str,
         "serviceType": ServiceTypeType,
     },
     total=False,
 )
 
-PutItemInputOutputTypeDef = TypedDict(
-    "PutItemInputOutputTypeDef",
-    {
-        "tableName": str,
-    },
-)
-
 PutItemInputTypeDef = TypedDict(
     "PutItemInputTypeDef",
     {
         "tableName": str,
     },
 )
 
@@ -3911,29 +2963,14 @@
         "policyName": str,
         "policyArn": str,
         "policyDocument": str,
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
-EnableIoTLoggingParamsOutputTypeDef = TypedDict(
-    "EnableIoTLoggingParamsOutputTypeDef",
-    {
-        "roleArnForLogging": str,
-        "logLevel": LogLevelType,
-    },
-)
-
 EnableIoTLoggingParamsTypeDef = TypedDict(
     "EnableIoTLoggingParamsTypeDef",
     {
         "roleArnForLogging": str,
         "logLevel": LogLevelType,
     },
 )
@@ -3950,69 +2987,32 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-RateIncreaseCriteriaOutputTypeDef = TypedDict(
-    "RateIncreaseCriteriaOutputTypeDef",
-    {
-        "numberOfNotifiedThings": int,
-        "numberOfSucceededThings": int,
-    },
-    total=False,
-)
-
 RateIncreaseCriteriaTypeDef = TypedDict(
     "RateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
 )
 
-FieldOutputTypeDef = TypedDict(
-    "FieldOutputTypeDef",
-    {
-        "name": str,
-        "type": FieldTypeType,
-    },
-    total=False,
-)
-
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "name": str,
         "type": FieldTypeType,
     },
     total=False,
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-        "version": str,
-    },
-    total=False,
-)
-
-StreamOutputTypeDef = TypedDict(
-    "StreamOutputTypeDef",
-    {
-        "streamId": str,
-        "fileId": int,
-    },
-    total=False,
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "version": str,
     },
@@ -4033,23 +3033,22 @@
     {
         "metricName": str,
         "metricArn": str,
     },
     total=False,
 )
 
-GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = (
-    TypedDict(
-        "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
-        {
-            "securityProfileName": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
 )
 
 GetBehaviorModelTrainingSummariesRequestRequestTypeDef = TypedDict(
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     {
         "securityProfileName": str,
         "maxResults": int,
@@ -4077,22 +3076,14 @@
 
 class GetCardinalityRequestRequestTypeDef(
     _RequiredGetCardinalityRequestRequestTypeDef, _OptionalGetCardinalityRequestRequestTypeDef
 ):
     pass
 
 
-GetCardinalityResponseTypeDef = TypedDict(
-    "GetCardinalityResponseTypeDef",
-    {
-        "cardinality": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEffectivePoliciesRequestRequestTypeDef = TypedDict(
     "GetEffectivePoliciesRequestRequestTypeDef",
     {
         "principal": str,
         "cognitoIdentityPoolId": str,
         "thingName": str,
     },
@@ -4102,91 +3093,45 @@
 GetJobDocumentRequestRequestTypeDef = TypedDict(
     "GetJobDocumentRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
-GetJobDocumentResponseTypeDef = TypedDict(
-    "GetJobDocumentResponseTypeDef",
-    {
-        "document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLoggingOptionsResponseTypeDef = TypedDict(
-    "GetLoggingOptionsResponseTypeDef",
-    {
-        "roleArn": str,
-        "logLevel": LogLevelType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOTAUpdateRequestRequestTypeDef = TypedDict(
     "GetOTAUpdateRequestRequestTypeDef",
     {
         "otaUpdateId": str,
     },
 )
 
-VersionUpdateByJobsConfigOutputTypeDef = TypedDict(
-    "VersionUpdateByJobsConfigOutputTypeDef",
+VersionUpdateByJobsConfigTypeDef = TypedDict(
+    "VersionUpdateByJobsConfigTypeDef",
     {
         "enabled": bool,
         "roleArn": str,
     },
     total=False,
 )
 
 GetPackageRequestRequestTypeDef = TypedDict(
     "GetPackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 
-GetPackageResponseTypeDef = TypedDict(
-    "GetPackageResponseTypeDef",
-    {
-        "packageName": str,
-        "packageArn": str,
-        "description": str,
-        "defaultVersionName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPackageVersionRequestRequestTypeDef = TypedDict(
     "GetPackageVersionRequestRequestTypeDef",
     {
         "packageName": str,
         "versionName": str,
     },
 )
 
-GetPackageVersionResponseTypeDef = TypedDict(
-    "GetPackageVersionResponseTypeDef",
-    {
-        "packageVersionArn": str,
-        "packageName": str,
-        "versionName": str,
-        "description": str,
-        "attributes": Dict[str, str],
-        "status": PackageVersionStatusType,
-        "errorReason": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPercentilesRequestRequestTypeDef = TypedDict(
     "_RequiredGetPercentilesRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalGetPercentilesRequestRequestTypeDef = TypedDict(
@@ -4219,59 +3164,22 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policyName": str,
-        "policyArn": str,
-        "policyDocument": str,
-        "defaultVersionId": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "generationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPolicyVersionRequestRequestTypeDef = TypedDict(
     "GetPolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
 )
 
-GetPolicyVersionResponseTypeDef = TypedDict(
-    "GetPolicyVersionResponseTypeDef",
-    {
-        "policyArn": str,
-        "policyName": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "isDefaultVersion": bool,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "generationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRegistrationCodeResponseTypeDef = TypedDict(
-    "GetRegistrationCodeResponseTypeDef",
-    {
-        "registrationCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatisticsRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalGetStatisticsRequestRequestTypeDef = TypedDict(
@@ -4316,58 +3224,31 @@
 GetTopicRuleRequestRequestTypeDef = TypedDict(
     "GetTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
-GetV2LoggingOptionsResponseTypeDef = TypedDict(
-    "GetV2LoggingOptionsResponseTypeDef",
-    {
-        "roleArn": str,
-        "defaultLogLevel": LogLevelType,
-        "disableAllLogs": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupNameAndArnTypeDef = TypedDict(
     "GroupNameAndArnTypeDef",
     {
         "groupName": str,
         "groupArn": str,
     },
     total=False,
 )
 
-HttpActionHeaderOutputTypeDef = TypedDict(
-    "HttpActionHeaderOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 HttpActionHeaderTypeDef = TypedDict(
     "HttpActionHeaderTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-SigV4AuthorizationOutputTypeDef = TypedDict(
-    "SigV4AuthorizationOutputTypeDef",
-    {
-        "signingRegion": str,
-        "serviceName": str,
-        "roleArn": str,
-    },
-)
-
 SigV4AuthorizationTypeDef = TypedDict(
     "SigV4AuthorizationTypeDef",
     {
         "signingRegion": str,
         "serviceName": str,
         "roleArn": str,
     },
@@ -4417,24 +3298,14 @@
     "IndexingFilterTypeDef",
     {
         "namedShadowNames": Sequence[str],
     },
     total=False,
 )
 
-IssuerCertificateIdentifierOutputTypeDef = TypedDict(
-    "IssuerCertificateIdentifierOutputTypeDef",
-    {
-        "issuerCertificateSubject": str,
-        "issuerId": str,
-        "issuerCertificateSerialNumber": str,
-    },
-    total=False,
-)
-
 IssuerCertificateIdentifierTypeDef = TypedDict(
     "IssuerCertificateIdentifierTypeDef",
     {
         "issuerCertificateSubject": str,
         "issuerId": str,
         "issuerCertificateSerialNumber": str,
     },
@@ -4458,22 +3329,14 @@
         "lastUpdatedAt": datetime,
         "executionNumber": int,
         "retryAttempt": int,
     },
     total=False,
 )
 
-RetryCriteriaOutputTypeDef = TypedDict(
-    "RetryCriteriaOutputTypeDef",
-    {
-        "failureType": RetryableFailureTypeType,
-        "numberOfRetries": int,
-    },
-)
-
 RetryCriteriaTypeDef = TypedDict(
     "RetryCriteriaTypeDef",
     {
         "failureType": RetryableFailureTypeType,
         "numberOfRetries": int,
     },
 )
@@ -4525,64 +3388,28 @@
     "ScheduledJobRolloutTypeDef",
     {
         "startTime": str,
     },
     total=False,
 )
 
-ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = TypedDict(
-    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActiveViolationsRequestRequestTypeDef = TypedDict(
     "ListActiveViolationsRequestRequestTypeDef",
     {
         "thingName": str,
         "securityProfileName": str,
         "behaviorCriteriaType": BehaviorCriteriaTypeType,
         "listSuppressedAlerts": bool,
         "verificationState": VerificationStateType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
-    {
-        "target": str,
-    },
-)
-_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
-    {
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef(
-    _RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
-    _OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttachedPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedPoliciesRequestRequestTypeDef",
     {
         "target": str,
     },
 )
 _OptionalListAttachedPoliciesRequestRequestTypeDef = TypedDict(
@@ -4599,38 +3426,14 @@
 class ListAttachedPoliciesRequestRequestTypeDef(
     _RequiredListAttachedPoliciesRequestRequestTypeDef,
     _OptionalListAttachedPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-        "findingId": str,
-    },
-)
-_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "actionStatus": AuditMitigationActionsExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef(
-    _RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
-    _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef",
     {
         "taskId": str,
         "findingId": str,
     },
 )
@@ -4648,40 +3451,14 @@
 class ListAuditMitigationActionsExecutionsRequestRequestTypeDef(
     _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     _OptionalListAuditMitigationActionsExecutionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    {
-        "auditTaskId": str,
-        "findingId": str,
-        "taskStatus": AuditMitigationActionsTaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef(
-    _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-    _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
@@ -4701,39 +3478,14 @@
 class ListAuditMitigationActionsTasksRequestRequestTypeDef(
     _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
     _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
-    "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
-    "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    {
-        "taskType": AuditTaskTypeType,
-        "taskStatus": AuditTaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAuditTasksRequestListAuditTasksPaginateTypeDef(
-    _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef,
-    _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListAuditTasksRequestRequestTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
@@ -4751,98 +3503,46 @@
 
 class ListAuditTasksRequestRequestTypeDef(
     _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
 ):
     pass
 
 
-ListAuthorizersRequestListAuthorizersPaginateTypeDef = TypedDict(
-    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "status": AuthorizerStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAuthorizersRequestRequestTypeDef = TypedDict(
     "ListAuthorizersRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "status": AuthorizerStatusType,
     },
     total=False,
 )
 
-ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = TypedDict(
-    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
-    {
-        "namePrefixFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBillingGroupsRequestRequestTypeDef = TypedDict(
     "ListBillingGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "namePrefixFilter": str,
     },
     total=False,
 )
 
-ListCACertificatesRequestListCACertificatesPaginateTypeDef = TypedDict(
-    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "templateName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCACertificatesRequestRequestTypeDef = TypedDict(
     "ListCACertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "templateName": str,
     },
     total=False,
 )
 
-_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
-    "_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
-    {
-        "caCertificateId": str,
-    },
-)
-_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
-    "_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef(
-    _RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
-    _OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCertificatesByCARequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesByCARequestRequestTypeDef",
     {
         "caCertificateId": str,
     },
 )
 _OptionalListCertificatesByCARequestRequestTypeDef = TypedDict(
@@ -4859,109 +3559,47 @@
 class ListCertificatesByCARequestRequestTypeDef(
     _RequiredListCertificatesByCARequestRequestTypeDef,
     _OptionalListCertificatesByCARequestRequestTypeDef,
 ):
     pass
 
 
-ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = TypedDict(
-    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomMetricsRequestRequestTypeDef = TypedDict(
     "ListCustomMetricsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListCustomMetricsResponseTypeDef = TypedDict(
-    "ListCustomMetricsResponseTypeDef",
-    {
-        "metricNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-        "violationId": str,
-        "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
     "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
     {
         "taskId": str,
         "violationId": str,
         "thingName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef(
-    _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-    _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
@@ -4978,125 +3616,51 @@
 class ListDetectMitigationActionsTasksRequestRequestTypeDef(
     _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
     _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
 ):
     pass
 
 
-ListDimensionsRequestListDimensionsPaginateTypeDef = TypedDict(
-    "ListDimensionsRequestListDimensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDimensionsRequestRequestTypeDef = TypedDict(
     "ListDimensionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDimensionsResponseTypeDef = TypedDict(
-    "ListDimensionsResponseTypeDef",
-    {
-        "dimensionNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = TypedDict(
-    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
-    {
-        "serviceType": ServiceTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDomainConfigurationsRequestRequestTypeDef = TypedDict(
     "ListDomainConfigurationsRequestRequestTypeDef",
     {
         "marker": str,
         "pageSize": int,
         "serviceType": ServiceTypeType,
     },
     total=False,
 )
 
-ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = TypedDict(
-    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFleetMetricsRequestRequestTypeDef = TypedDict(
     "ListFleetMetricsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListIndicesRequestListIndicesPaginateTypeDef = TypedDict(
-    "ListIndicesRequestListIndicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListIndicesResponseTypeDef = TypedDict(
-    "ListIndicesResponseTypeDef",
-    {
-        "indexNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
-    "_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
-    {
-        "jobId": str,
-    },
-)
-_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
-    "_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
-    {
-        "status": JobExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef(
-    _RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
-    _OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobExecutionsForJobRequestRequestTypeDef = TypedDict(
     "_RequiredListJobExecutionsForJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalListJobExecutionsForJobRequestRequestTypeDef = TypedDict(
@@ -5113,39 +3677,14 @@
 class ListJobExecutionsForJobRequestRequestTypeDef(
     _RequiredListJobExecutionsForJobRequestRequestTypeDef,
     _OptionalListJobExecutionsForJobRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
-    "_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
-    "_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
-    {
-        "status": JobExecutionStatusType,
-        "namespaceId": str,
-        "jobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef(
-    _RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
-    _OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobExecutionsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListJobExecutionsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListJobExecutionsForThingRequestRequestTypeDef = TypedDict(
@@ -5164,67 +3703,37 @@
 class ListJobExecutionsForThingRequestRequestTypeDef(
     _RequiredListJobExecutionsForThingRequestRequestTypeDef,
     _OptionalListJobExecutionsForThingRequestRequestTypeDef,
 ):
     pass
 
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "status": JobStatusType,
-        "targetSelection": TargetSelectionType,
-        "thingGroupName": str,
-        "thingGroupId": str,
-        "namespaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "status": JobStatusType,
         "targetSelection": TargetSelectionType,
         "maxResults": int,
         "nextToken": str,
         "thingGroupName": str,
         "thingGroupId": str,
         "namespaceId": str,
     },
     total=False,
 )
 
-ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef = TypedDict(
-    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
-    {
-        "templateName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListManagedJobTemplatesRequestRequestTypeDef",
     {
         "templateName": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -5239,41 +3748,14 @@
         "description": str,
         "environments": List[str],
         "templateVersion": str,
     },
     total=False,
 )
 
-_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
-    "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    {
-        "thingName": str,
-        "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
-    "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    {
-        "dimensionName": str,
-        "dimensionValueOperator": DimensionValueOperatorType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMetricValuesRequestListMetricValuesPaginateTypeDef(
-    _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef,
-    _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
     "_RequiredListMetricValuesRequestRequestTypeDef",
     {
         "thingName": str,
         "metricName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
@@ -5293,23 +3775,14 @@
 
 class ListMetricValuesRequestRequestTypeDef(
     _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
 ):
     pass
 
 
-ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = TypedDict(
-    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
-    {
-        "actionType": MitigationActionTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMitigationActionsRequestRequestTypeDef = TypedDict(
     "ListMitigationActionsRequestRequestTypeDef",
     {
         "actionType": MitigationActionTypeType,
         "maxResults": int,
         "nextToken": str,
     },
@@ -5322,23 +3795,14 @@
         "actionName": str,
         "actionArn": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = TypedDict(
-    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
-    {
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOTAUpdatesRequestRequestTypeDef = TypedDict(
     "ListOTAUpdatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "otaUpdateStatus": OTAUpdateStatusType,
     },
@@ -5351,23 +3815,14 @@
         "otaUpdateId": str,
         "otaUpdateArn": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = TypedDict(
-    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOutgoingCertificatesRequestRequestTypeDef = TypedDict(
     "ListOutgoingCertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
@@ -5383,37 +3838,14 @@
         "transferDate": datetime,
         "transferMessage": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "packageName": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "status": PackageVersionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalListPackageVersionsRequestRequestTypeDef = TypedDict(
@@ -5442,22 +3874,14 @@
         "status": PackageVersionStatusType,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
     },
     total=False,
 )
 
-ListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "ListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPackagesRequestRequestTypeDef = TypedDict(
     "ListPackagesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -5470,56 +3894,24 @@
         "defaultVersionName": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
     },
     total=False,
 )
 
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "marker": str,
         "pageSize": int,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
-    {
-        "policyName": str,
-    },
-)
-_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef(
-    _RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
-    _OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPolicyPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyPrincipalsRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListPolicyPrincipalsRequestRequestTypeDef = TypedDict(
@@ -5536,23 +3928,14 @@
 class ListPolicyPrincipalsRequestRequestTypeDef(
     _RequiredListPolicyPrincipalsRequestRequestTypeDef,
     _OptionalListPolicyPrincipalsRequestRequestTypeDef,
 ):
     pass
 
 
-ListPolicyPrincipalsResponseTypeDef = TypedDict(
-    "ListPolicyPrincipalsResponseTypeDef",
-    {
-        "principals": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPolicyVersionsRequestRequestTypeDef = TypedDict(
     "ListPolicyVersionsRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 
@@ -5562,37 +3945,14 @@
         "versionId": str,
         "isDefaultVersion": bool,
         "createDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
-    {
-        "principal": str,
-    },
-)
-_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef(
-    _RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
-    _OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPrincipalPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalPoliciesRequestRequestTypeDef",
     {
         "principal": str,
     },
 )
 _OptionalListPrincipalPoliciesRequestRequestTypeDef = TypedDict(
@@ -5609,36 +3969,14 @@
 class ListPrincipalPoliciesRequestRequestTypeDef(
     _RequiredListPrincipalPoliciesRequestRequestTypeDef,
     _OptionalListPrincipalPoliciesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
-    {
-        "principal": str,
-    },
-)
-_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef(
-    _RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
-    _OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListPrincipalThingsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalThingsRequestRequestTypeDef",
     {
         "principal": str,
     },
 )
 _OptionalListPrincipalThingsRequestRequestTypeDef = TypedDict(
@@ -5654,45 +3992,14 @@
 class ListPrincipalThingsRequestRequestTypeDef(
     _RequiredListPrincipalThingsRequestRequestTypeDef,
     _OptionalListPrincipalThingsRequestRequestTypeDef,
 ):
     pass
 
 
-ListPrincipalThingsResponseTypeDef = TypedDict(
-    "ListPrincipalThingsResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
-    {
-        "templateName": str,
-    },
-)
-_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef(
-    _RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
-    _OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListProvisioningTemplateVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListProvisioningTemplateVersionsRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalListProvisioningTemplateVersionsRequestRequestTypeDef = TypedDict(
@@ -5718,22 +4025,14 @@
         "versionId": int,
         "creationDate": datetime,
         "isDefaultVersion": bool,
     },
     total=False,
 )
 
-ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = TypedDict(
-    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProvisioningTemplatesRequestRequestTypeDef = TypedDict(
     "ListProvisioningTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -5749,36 +4048,14 @@
         "lastModifiedDate": datetime,
         "enabled": bool,
         "type": TemplateTypeType,
     },
     total=False,
 )
 
-_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
-    "_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
-    {
-        "findingId": str,
-    },
-)
-_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
-    "_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef(
-    _RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
-    _OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef = TypedDict(
     "_RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef",
     {
         "findingId": str,
     },
 )
 _OptionalListRelatedResourcesForAuditFindingRequestRequestTypeDef = TypedDict(
@@ -5794,50 +4071,24 @@
 class ListRelatedResourcesForAuditFindingRequestRequestTypeDef(
     _RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef,
     _OptionalListRelatedResourcesForAuditFindingRequestRequestTypeDef,
 ):
     pass
 
 
-ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = TypedDict(
-    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRoleAliasesRequestRequestTypeDef = TypedDict(
     "ListRoleAliasesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-ListRoleAliasesResponseTypeDef = TypedDict(
-    "ListRoleAliasesResponseTypeDef",
-    {
-        "roleAliases": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = TypedDict(
-    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListScheduledAuditsRequestRequestTypeDef = TypedDict(
     "ListScheduledAuditsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -5851,41 +4102,14 @@
         "frequency": AuditFrequencyType,
         "dayOfMonth": str,
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
-_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
-        {
-            "securityProfileTargetArn": str,
-        },
-    )
-)
-_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
-        {
-            "recursive": bool,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef(
-    _RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
-    _OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSecurityProfilesForTargetRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilesForTargetRequestRequestTypeDef",
     {
         "securityProfileTargetArn": str,
     },
 )
 _OptionalListSecurityProfilesForTargetRequestRequestTypeDef = TypedDict(
@@ -5902,24 +4126,14 @@
 class ListSecurityProfilesForTargetRequestRequestTypeDef(
     _RequiredListSecurityProfilesForTargetRequestRequestTypeDef,
     _OptionalListSecurityProfilesForTargetRequestRequestTypeDef,
 ):
     pass
 
 
-ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
-    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
-    {
-        "dimensionName": str,
-        "metricName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityProfilesRequestRequestTypeDef = TypedDict(
     "ListSecurityProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "dimensionName": str,
         "metricName": str,
@@ -5931,23 +4145,14 @@
     "SecurityProfileIdentifierTypeDef",
     {
         "name": str,
         "arn": str,
     },
 )
 
-ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
-    "ListStreamsRequestListStreamsPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "ascendingOrder": bool,
     },
@@ -5961,36 +4166,14 @@
         "streamArn": str,
         "streamVersion": int,
         "description": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -6005,55 +4188,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-
-_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
-    {
-        "policyName": str,
-    },
-)
-_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(
-    _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
-    _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTargetsForPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForPolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListTargetsForPolicyRequestRequestTypeDef = TypedDict(
@@ -6069,49 +4211,14 @@
 class ListTargetsForPolicyRequestRequestTypeDef(
     _RequiredListTargetsForPolicyRequestRequestTypeDef,
     _OptionalListTargetsForPolicyRequestRequestTypeDef,
 ):
     pass
 
 
-ListTargetsForPolicyResponseTypeDef = TypedDict(
-    "ListTargetsForPolicyResponseTypeDef",
-    {
-        "targets": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
-    TypedDict(
-        "_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
-        {
-            "securityProfileName": str,
-        },
-    )
-)
-_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
-    TypedDict(
-        "_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef(
-    _RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
-    _OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTargetsForSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 _OptionalListTargetsForSecurityProfileRequestRequestTypeDef = TypedDict(
@@ -6134,36 +4241,14 @@
 SecurityProfileTargetTypeDef = TypedDict(
     "SecurityProfileTargetTypeDef",
     {
         "arn": str,
     },
 )
 
-_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
-    "_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
-    "_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef(
-    _RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
-    _OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingGroupsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListThingGroupsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListThingGroupsForThingRequestRequestTypeDef = TypedDict(
@@ -6179,59 +4264,26 @@
 class ListThingGroupsForThingRequestRequestTypeDef(
     _RequiredListThingGroupsForThingRequestRequestTypeDef,
     _OptionalListThingGroupsForThingRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingGroupsRequestListThingGroupsPaginateTypeDef = TypedDict(
-    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
-    {
-        "parentGroup": str,
-        "namePrefixFilter": str,
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingGroupsRequestRequestTypeDef = TypedDict(
     "ListThingGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "parentGroup": str,
         "namePrefixFilter": str,
         "recursive": bool,
     },
     total=False,
 )
 
-_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef(
-    _RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
-    _OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListThingPrincipalsRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListThingPrincipalsRequestRequestTypeDef = TypedDict(
@@ -6247,46 +4299,14 @@
 class ListThingPrincipalsRequestRequestTypeDef(
     _RequiredListThingPrincipalsRequestRequestTypeDef,
     _OptionalListThingPrincipalsRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingPrincipalsResponseTypeDef = TypedDict(
-    "ListThingPrincipalsResponseTypeDef",
-    {
-        "principals": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
-    "_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
-    {
-        "taskId": str,
-        "reportType": ReportTypeType,
-    },
-)
-_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
-    "_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef(
-    _RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
-    _OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingRegistrationTaskReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListThingRegistrationTaskReportsRequestRequestTypeDef",
     {
         "taskId": str,
         "reportType": ReportTypeType,
     },
 )
@@ -6303,93 +4323,34 @@
 class ListThingRegistrationTaskReportsRequestRequestTypeDef(
     _RequiredListThingRegistrationTaskReportsRequestRequestTypeDef,
     _OptionalListThingRegistrationTaskReportsRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingRegistrationTaskReportsResponseTypeDef = TypedDict(
-    "ListThingRegistrationTaskReportsResponseTypeDef",
-    {
-        "resourceLinks": List[str],
-        "reportType": ReportTypeType,
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = TypedDict(
-    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
-    {
-        "status": StatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingRegistrationTasksRequestRequestTypeDef = TypedDict(
     "ListThingRegistrationTasksRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": StatusType,
     },
     total=False,
 )
 
-ListThingRegistrationTasksResponseTypeDef = TypedDict(
-    "ListThingRegistrationTasksResponseTypeDef",
-    {
-        "taskIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingTypesRequestListThingTypesPaginateTypeDef = TypedDict(
-    "ListThingTypesRequestListThingTypesPaginateTypeDef",
-    {
-        "thingTypeName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingTypesRequestRequestTypeDef = TypedDict(
     "ListThingTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "thingTypeName": str,
     },
     total=False,
 )
 
-_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
-    "_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
-    {
-        "billingGroupName": str,
-    },
-)
-_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
-    "_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef(
-    _RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
-    _OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingsInBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListThingsInBillingGroupRequestRequestTypeDef",
     {
         "billingGroupName": str,
     },
 )
 _OptionalListThingsInBillingGroupRequestRequestTypeDef = TypedDict(
@@ -6405,46 +4366,14 @@
 class ListThingsInBillingGroupRequestRequestTypeDef(
     _RequiredListThingsInBillingGroupRequestRequestTypeDef,
     _OptionalListThingsInBillingGroupRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingsInBillingGroupResponseTypeDef = TypedDict(
-    "ListThingsInBillingGroupResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
-    "_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
-    {
-        "thingGroupName": str,
-    },
-)
-_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
-    "_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
-    {
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef(
-    _RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
-    _OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThingsInThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListThingsInThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
     },
 )
 _OptionalListThingsInThingGroupRequestRequestTypeDef = TypedDict(
@@ -6461,35 +4390,14 @@
 class ListThingsInThingGroupRequestRequestTypeDef(
     _RequiredListThingsInThingGroupRequestRequestTypeDef,
     _OptionalListThingsInThingGroupRequestRequestTypeDef,
 ):
     pass
 
 
-ListThingsInThingGroupResponseTypeDef = TypedDict(
-    "ListThingsInThingGroupResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingsRequestListThingsPaginateTypeDef = TypedDict(
-    "ListThingsRequestListThingsPaginateTypeDef",
-    {
-        "attributeName": str,
-        "attributeValue": str,
-        "thingTypeName": str,
-        "usePrefixAttributeValue": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingsRequestRequestTypeDef = TypedDict(
     "ListThingsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "attributeName": str,
         "attributeValue": str,
@@ -6507,41 +4415,23 @@
         "thingArn": str,
         "attributes": Dict[str, str],
         "version": int,
     },
     total=False,
 )
 
-ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = TypedDict(
-    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTopicRuleDestinationsRequestRequestTypeDef = TypedDict(
     "ListTopicRuleDestinationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListTopicRulesRequestListTopicRulesPaginateTypeDef = TypedDict(
-    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
-    {
-        "topic": str,
-        "ruleDisabled": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTopicRulesRequestRequestTypeDef = TypedDict(
     "ListTopicRulesRequestRequestTypeDef",
     {
         "topic": str,
         "maxResults": int,
         "nextToken": str,
         "ruleDisabled": bool,
@@ -6557,61 +4447,24 @@
         "topicPattern": str,
         "createdAt": datetime,
         "ruleDisabled": bool,
     },
     total=False,
 )
 
-ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = TypedDict(
-    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
-    {
-        "targetType": LogTargetTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListV2LoggingLevelsRequestRequestTypeDef = TypedDict(
     "ListV2LoggingLevelsRequestRequestTypeDef",
     {
         "targetType": LogTargetTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
-    "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
-    "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListViolationEventsRequestListViolationEventsPaginateTypeDef(
-    _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef,
-    _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListViolationEventsRequestRequestTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
@@ -6633,35 +4486,14 @@
 class ListViolationEventsRequestRequestTypeDef(
     _RequiredListViolationEventsRequestRequestTypeDef,
     _OptionalListViolationEventsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredLocationTimestampOutputTypeDef = TypedDict(
-    "_RequiredLocationTimestampOutputTypeDef",
-    {
-        "value": str,
-    },
-)
-_OptionalLocationTimestampOutputTypeDef = TypedDict(
-    "_OptionalLocationTimestampOutputTypeDef",
-    {
-        "unit": str,
-    },
-    total=False,
-)
-
-
-class LocationTimestampOutputTypeDef(
-    _RequiredLocationTimestampOutputTypeDef, _OptionalLocationTimestampOutputTypeDef
-):
-    pass
-
-
 _RequiredLocationTimestampTypeDef = TypedDict(
     "_RequiredLocationTimestampTypeDef",
     {
         "value": str,
     },
 )
 _OptionalLocationTimestampTypeDef = TypedDict(
@@ -6675,33 +4507,14 @@
 
 class LocationTimestampTypeDef(
     _RequiredLocationTimestampTypeDef, _OptionalLocationTimestampTypeDef
 ):
     pass
 
 
-_RequiredLogTargetOutputTypeDef = TypedDict(
-    "_RequiredLogTargetOutputTypeDef",
-    {
-        "targetType": LogTargetTypeType,
-    },
-)
-_OptionalLogTargetOutputTypeDef = TypedDict(
-    "_OptionalLogTargetOutputTypeDef",
-    {
-        "targetName": str,
-    },
-    total=False,
-)
-
-
-class LogTargetOutputTypeDef(_RequiredLogTargetOutputTypeDef, _OptionalLogTargetOutputTypeDef):
-    pass
-
-
 _RequiredLogTargetTypeDef = TypedDict(
     "_RequiredLogTargetTypeDef",
     {
         "targetType": LogTargetTypeType,
     },
 )
 _OptionalLogTargetTypeDef = TypedDict(
@@ -6734,42 +4547,14 @@
 
 class LoggingOptionsPayloadTypeDef(
     _RequiredLoggingOptionsPayloadTypeDef, _OptionalLoggingOptionsPayloadTypeDef
 ):
     pass
 
 
-PublishFindingToSnsParamsOutputTypeDef = TypedDict(
-    "PublishFindingToSnsParamsOutputTypeDef",
-    {
-        "topicArn": str,
-    },
-)
-
-ReplaceDefaultPolicyVersionParamsOutputTypeDef = TypedDict(
-    "ReplaceDefaultPolicyVersionParamsOutputTypeDef",
-    {
-        "templateName": Literal["BLANK_POLICY"],
-    },
-)
-
-UpdateCACertificateParamsOutputTypeDef = TypedDict(
-    "UpdateCACertificateParamsOutputTypeDef",
-    {
-        "action": Literal["DEACTIVATE"],
-    },
-)
-
-UpdateDeviceCertificateParamsOutputTypeDef = TypedDict(
-    "UpdateDeviceCertificateParamsOutputTypeDef",
-    {
-        "action": Literal["DEACTIVATE"],
-    },
-)
-
 PublishFindingToSnsParamsTypeDef = TypedDict(
     "PublishFindingToSnsParamsTypeDef",
     {
         "topicArn": str,
     },
 )
 
@@ -6800,49 +4585,22 @@
         "username": str,
         "password": Union[str, bytes, IO[Any], StreamingBody],
         "clientId": str,
     },
     total=False,
 )
 
-UserPropertyOutputTypeDef = TypedDict(
-    "UserPropertyOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 UserPropertyTypeDef = TypedDict(
     "UserPropertyTypeDef",
     {
         "key": str,
         "value": str,
     },
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
-PolicyVersionIdentifierOutputTypeDef = TypedDict(
-    "PolicyVersionIdentifierOutputTypeDef",
-    {
-        "policyName": str,
-        "policyVersionId": str,
-    },
-    total=False,
-)
-
 PolicyVersionIdentifierTypeDef = TypedDict(
     "PolicyVersionIdentifierTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
     total=False,
@@ -6867,33 +4625,14 @@
 class PutVerificationStateOnViolationRequestRequestTypeDef(
     _RequiredPutVerificationStateOnViolationRequestRequestTypeDef,
     _OptionalPutVerificationStateOnViolationRequestRequestTypeDef,
 ):
     pass
 
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
-    {
-        "templateBody": str,
-        "roleArn": str,
-        "templateName": str,
-    },
-    total=False,
-)
-
-RegisterCACertificateResponseTypeDef = TypedDict(
-    "RegisterCACertificateResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateRequestRequestTypeDef",
     {
         "certificatePem": str,
     },
 )
 _OptionalRegisterCertificateRequestRequestTypeDef = TypedDict(
@@ -6910,23 +4649,14 @@
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
 
-RegisterCertificateResponseTypeDef = TypedDict(
-    "RegisterCertificateResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateWithoutCARequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateWithoutCARequestRequestTypeDef",
     {
         "certificatePem": str,
     },
 )
 _OptionalRegisterCertificateWithoutCARequestRequestTypeDef = TypedDict(
@@ -6941,23 +4671,14 @@
 class RegisterCertificateWithoutCARequestRequestTypeDef(
     _RequiredRegisterCertificateWithoutCARequestRequestTypeDef,
     _OptionalRegisterCertificateWithoutCARequestRequestTypeDef,
 ):
     pass
 
 
-RegisterCertificateWithoutCAResponseTypeDef = TypedDict(
-    "RegisterCertificateWithoutCAResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterThingRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterThingRequestRequestTypeDef",
     {
         "templateBody": str,
     },
 )
 _OptionalRegisterThingRequestRequestTypeDef = TypedDict(
@@ -6971,23 +4692,14 @@
 
 class RegisterThingRequestRequestTypeDef(
     _RequiredRegisterThingRequestRequestTypeDef, _OptionalRegisterThingRequestRequestTypeDef
 ):
     pass
 
 
-RegisterThingResponseTypeDef = TypedDict(
-    "RegisterThingResponseTypeDef",
-    {
-        "certificatePem": str,
-        "resourceArns": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRejectCertificateTransferRequestRequestTypeDef = TypedDict(
     "_RequiredRejectCertificateTransferRequestRequestTypeDef",
     {
         "certificateId": str,
     },
 )
 _OptionalRejectCertificateTransferRequestRequestTypeDef = TypedDict(
@@ -7024,25 +4736,14 @@
         "thingGroupArn": str,
         "thingName": str,
         "thingArn": str,
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
 _RequiredSearchIndexRequestRequestTypeDef = TypedDict(
     "_RequiredSearchIndexRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalSearchIndexRequestRequestTypeDef = TypedDict(
@@ -7078,23 +4779,14 @@
 SetDefaultAuthorizerRequestRequestTypeDef = TypedDict(
     "SetDefaultAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
     },
 )
 
-SetDefaultAuthorizerResponseTypeDef = TypedDict(
-    "SetDefaultAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetDefaultPolicyVersionRequestRequestTypeDef = TypedDict(
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
 )
@@ -7105,91 +4797,49 @@
         "roleArn": str,
         "defaultLogLevel": LogLevelType,
         "disableAllLogs": bool,
     },
     total=False,
 )
 
-SigningProfileParameterOutputTypeDef = TypedDict(
-    "SigningProfileParameterOutputTypeDef",
-    {
-        "certificateArn": str,
-        "platform": str,
-        "certificatePathOnDevice": str,
-    },
-    total=False,
-)
-
 SigningProfileParameterTypeDef = TypedDict(
     "SigningProfileParameterTypeDef",
     {
         "certificateArn": str,
         "platform": str,
         "certificatePathOnDevice": str,
     },
     total=False,
 )
 
-StartAuditMitigationActionsTaskResponseTypeDef = TypedDict(
-    "StartAuditMitigationActionsTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ViolationEventOccurrenceRangeTypeDef = TypedDict(
     "ViolationEventOccurrenceRangeTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
 
-StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
-    "StartDetectMitigationActionsTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartOnDemandAuditTaskRequestRequestTypeDef = TypedDict(
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     {
         "targetCheckNames": Sequence[str],
     },
 )
 
-StartOnDemandAuditTaskResponseTypeDef = TypedDict(
-    "StartOnDemandAuditTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "StartThingRegistrationTaskRequestRequestTypeDef",
     {
         "templateBody": str,
         "inputFileBucket": str,
         "inputFileKey": str,
         "roleArn": str,
     },
 )
 
-StartThingRegistrationTaskResponseTypeDef = TypedDict(
-    "StartThingRegistrationTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "StopThingRegistrationTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
@@ -7197,52 +4847,24 @@
     "TlsContextTypeDef",
     {
         "serverName": str,
     },
     total=False,
 )
 
-TestInvokeAuthorizerResponseTypeDef = TypedDict(
-    "TestInvokeAuthorizerResponseTypeDef",
-    {
-        "isAuthenticated": bool,
-        "principalId": str,
-        "policyDocuments": List[str],
-        "refreshAfterInSeconds": int,
-        "disconnectAfterInSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ThingConnectivityTypeDef = TypedDict(
     "ThingConnectivityTypeDef",
     {
         "connected": bool,
         "timestamp": int,
         "disconnectReason": str,
     },
     total=False,
 )
 
-TimestreamDimensionOutputTypeDef = TypedDict(
-    "TimestreamDimensionOutputTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-)
-
-TimestreamTimestampOutputTypeDef = TypedDict(
-    "TimestreamTimestampOutputTypeDef",
-    {
-        "value": str,
-        "unit": str,
-    },
-)
-
 TimestreamDimensionTypeDef = TypedDict(
     "TimestreamDimensionTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
@@ -7319,22 +4941,14 @@
 class TransferCertificateRequestRequestTypeDef(
     _RequiredTransferCertificateRequestRequestTypeDef,
     _OptionalTransferCertificateRequestRequestTypeDef,
 ):
     pass
 
 
-TransferCertificateResponseTypeDef = TypedDict(
-    "TransferCertificateResponseTypeDef",
-    {
-        "transferredCertificateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -7360,31 +4974,14 @@
 
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBillingGroupResponseTypeDef = TypedDict(
-    "UpdateBillingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCertificateRequestRequestTypeDef = TypedDict(
     "UpdateCertificateRequestRequestTypeDef",
     {
         "certificateId": str,
         "newStatus": CertificateStatusType,
     },
 )
@@ -7393,83 +4990,22 @@
     "UpdateCustomMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "displayName": str,
     },
 )
 
-UpdateCustomMetricResponseTypeDef = TypedDict(
-    "UpdateCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "metricType": CustomMetricTypeType,
-        "displayName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDimensionRequestRequestTypeDef = TypedDict(
     "UpdateDimensionRequestRequestTypeDef",
     {
         "name": str,
         "stringValues": Sequence[str],
     },
 )
 
-UpdateDimensionResponseTypeDef = TypedDict(
-    "UpdateDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "type": Literal["TOPIC_FILTER"],
-        "stringValues": List[str],
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDomainConfigurationResponseTypeDef = TypedDict(
-    "UpdateDomainConfigurationResponseTypeDef",
-    {
-        "domainConfigurationName": str,
-        "domainConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDynamicThingGroupResponseTypeDef = TypedDict(
-    "UpdateDynamicThingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMitigationActionResponseTypeDef = TypedDict(
-    "UpdateMitigationActionResponseTypeDef",
-    {
-        "actionArn": str,
-        "actionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VersionUpdateByJobsConfigTypeDef = TypedDict(
-    "VersionUpdateByJobsConfigTypeDef",
-    {
-        "enabled": bool,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalUpdatePackageRequestRequestTypeDef = TypedDict(
@@ -7534,23 +5070,14 @@
 
 class UpdateRoleAliasRequestRequestTypeDef(
     _RequiredUpdateRoleAliasRequestRequestTypeDef, _OptionalUpdateRoleAliasRequestRequestTypeDef
 ):
     pass
 
 
-UpdateRoleAliasResponseTypeDef = TypedDict(
-    "UpdateRoleAliasResponseTypeDef",
-    {
-        "roleAlias": str,
-        "roleAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateScheduledAuditRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduledAuditRequestRequestTypeDef",
     {
         "scheduledAuditName": str,
     },
 )
 _OptionalUpdateScheduledAuditRequestRequestTypeDef = TypedDict(
@@ -7568,41 +5095,14 @@
 class UpdateScheduledAuditRequestRequestTypeDef(
     _RequiredUpdateScheduledAuditRequestRequestTypeDef,
     _OptionalUpdateScheduledAuditRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateScheduledAuditResponseTypeDef = TypedDict(
-    "UpdateScheduledAuditResponseTypeDef",
-    {
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStreamResponseTypeDef = TypedDict(
-    "UpdateStreamResponseTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "description": str,
-        "streamVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateThingGroupResponseTypeDef = TypedDict(
-    "UpdateThingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateThingGroupsForThingRequestRequestTypeDef = TypedDict(
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     {
         "thingName": str,
         "thingGroupsToAdd": Sequence[str],
         "thingGroupsToRemove": Sequence[str],
         "overrideDynamicGroups": bool,
@@ -7625,15 +5125,15 @@
     },
     total=False,
 )
 
 AbortConfigOutputTypeDef = TypedDict(
     "AbortConfigOutputTypeDef",
     {
-        "criteriaList": List[AbortCriteriaOutputTypeDef],
+        "criteriaList": List[AbortCriteriaTypeDef],
     },
 )
 
 AbortConfigTypeDef = TypedDict(
     "AbortConfigTypeDef",
     {
         "criteriaList": Sequence[AbortCriteriaTypeDef],
@@ -7645,34 +5145,14 @@
     {
         "timestamp": datetime,
         "value": MetricValueOutputTypeDef,
     },
     total=False,
 )
 
-DescribeFleetMetricResponseTypeDef = TypedDict(
-    "DescribeFleetMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "queryString": str,
-        "aggregationType": AggregationTypeOutputTypeDef,
-        "period": int,
-        "aggregationField": str,
-        "description": str,
-        "queryVersion": str,
-        "indexName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "unit": FleetMetricUnitType,
-        "version": int,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFleetMetricRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "indexName": str,
     },
 )
@@ -7718,84 +5198,875 @@
     "ImplicitDenyTypeDef",
     {
         "policies": List[PolicyTypeDef],
     },
     total=False,
 )
 
+_RequiredAssetPropertyValueTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueTypeDef",
+    {
+        "value": AssetPropertyVariantTypeDef,
+        "timestamp": AssetPropertyTimestampTypeDef,
+    },
+)
+_OptionalAssetPropertyValueTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueTypeDef",
+    {
+        "quality": str,
+    },
+    total=False,
+)
+
+
+class AssetPropertyValueTypeDef(
+    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
+):
+    pass
+
+
+AssociateTargetsWithJobResponseTypeDef = TypedDict(
+    "AssociateTargetsWithJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBillingGroupResponseTypeDef = TypedDict(
+    "CreateBillingGroupResponseTypeDef",
+    {
+        "billingGroupName": str,
+        "billingGroupArn": str,
+        "billingGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCertificateFromCsrResponseTypeDef = TypedDict(
+    "CreateCertificateFromCsrResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "certificatePem": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomMetricResponseTypeDef = TypedDict(
+    "CreateCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDimensionResponseTypeDef = TypedDict(
+    "CreateDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainConfigurationResponseTypeDef = TypedDict(
+    "CreateDomainConfigurationResponseTypeDef",
+    {
+        "domainConfigurationName": str,
+        "domainConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDynamicThingGroupResponseTypeDef = TypedDict(
+    "CreateDynamicThingGroupResponseTypeDef",
+    {
+        "thingGroupName": str,
+        "thingGroupArn": str,
+        "thingGroupId": str,
+        "indexName": str,
+        "queryString": str,
+        "queryVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetMetricResponseTypeDef = TypedDict(
+    "CreateFleetMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobTemplateResponseTypeDef = TypedDict(
+    "CreateJobTemplateResponseTypeDef",
+    {
+        "jobTemplateArn": str,
+        "jobTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMitigationActionResponseTypeDef = TypedDict(
+    "CreateMitigationActionResponseTypeDef",
+    {
+        "actionArn": str,
+        "actionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOTAUpdateResponseTypeDef = TypedDict(
+    "CreateOTAUpdateResponseTypeDef",
+    {
+        "otaUpdateId": str,
+        "awsIotJobId": str,
+        "otaUpdateArn": str,
+        "awsIotJobArn": str,
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageResponseTypeDef = TypedDict(
+    "CreatePackageResponseTypeDef",
+    {
+        "packageName": str,
+        "packageArn": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageVersionResponseTypeDef = TypedDict(
+    "CreatePackageVersionResponseTypeDef",
+    {
+        "packageVersionArn": str,
+        "packageName": str,
+        "versionName": str,
+        "description": str,
+        "attributes": Dict[str, str],
+        "status": PackageVersionStatusType,
+        "errorReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyResponseTypeDef = TypedDict(
+    "CreatePolicyResponseTypeDef",
+    {
+        "policyName": str,
+        "policyArn": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyVersionResponseTypeDef = TypedDict(
+    "CreatePolicyVersionResponseTypeDef",
+    {
+        "policyArn": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisioningTemplateResponseTypeDef = TypedDict(
+    "CreateProvisioningTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "defaultVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisioningTemplateVersionResponseTypeDef = TypedDict(
+    "CreateProvisioningTemplateVersionResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "versionId": int,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRoleAliasResponseTypeDef = TypedDict(
+    "CreateRoleAliasResponseTypeDef",
+    {
+        "roleAlias": str,
+        "roleAliasArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduledAuditResponseTypeDef = TypedDict(
+    "CreateScheduledAuditResponseTypeDef",
+    {
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSecurityProfileResponseTypeDef = TypedDict(
+    "CreateSecurityProfileResponseTypeDef",
+    {
+        "securityProfileName": str,
+        "securityProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamResponseTypeDef = TypedDict(
+    "CreateStreamResponseTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "description": str,
+        "streamVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingGroupResponseTypeDef = TypedDict(
+    "CreateThingGroupResponseTypeDef",
+    {
+        "thingGroupName": str,
+        "thingGroupArn": str,
+        "thingGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingResponseTypeDef = TypedDict(
+    "CreateThingResponseTypeDef",
+    {
+        "thingName": str,
+        "thingArn": str,
+        "thingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingTypeResponseTypeDef = TypedDict(
+    "CreateThingTypeResponseTypeDef",
+    {
+        "thingTypeName": str,
+        "thingTypeArn": str,
+        "thingTypeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomMetricResponseTypeDef = TypedDict(
+    "DescribeCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "metricType": CustomMetricTypeType,
+        "displayName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDimensionResponseTypeDef = TypedDict(
+    "DescribeDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "type": Literal["TOPIC_FILTER"],
+        "stringValues": List[str],
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEndpointResponseTypeDef = TypedDict(
+    "DescribeEndpointResponseTypeDef",
+    {
+        "endpointAddress": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetMetricResponseTypeDef = TypedDict(
+    "DescribeFleetMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "queryString": str,
+        "aggregationType": AggregationTypeOutputTypeDef,
+        "period": int,
+        "aggregationField": str,
+        "description": str,
+        "queryVersion": str,
+        "indexName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "unit": FleetMetricUnitType,
+        "version": int,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeIndexResponseTypeDef = TypedDict(
+    "DescribeIndexResponseTypeDef",
+    {
+        "indexName": str,
+        "indexStatus": IndexStatusType,
+        "schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProvisioningTemplateVersionResponseTypeDef = TypedDict(
+    "DescribeProvisioningTemplateVersionResponseTypeDef",
+    {
+        "versionId": int,
+        "creationDate": datetime,
+        "templateBody": str,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScheduledAuditResponseTypeDef = TypedDict(
+    "DescribeScheduledAuditResponseTypeDef",
+    {
+        "frequency": AuditFrequencyType,
+        "dayOfMonth": str,
+        "dayOfWeek": DayOfWeekType,
+        "targetCheckNames": List[str],
+        "scheduledAuditName": str,
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThingRegistrationTaskResponseTypeDef = TypedDict(
+    "DescribeThingRegistrationTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "templateBody": str,
+        "inputFileBucket": str,
+        "inputFileKey": str,
+        "roleArn": str,
+        "status": StatusType,
+        "message": str,
+        "successCount": int,
+        "failureCount": int,
+        "percentageProgress": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThingResponseTypeDef = TypedDict(
+    "DescribeThingResponseTypeDef",
+    {
+        "defaultClientId": str,
+        "thingName": str,
+        "thingId": str,
+        "thingArn": str,
+        "thingTypeName": str,
+        "attributes": Dict[str, str],
+        "version": int,
+        "billingGroupName": str,
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
+GetCardinalityResponseTypeDef = TypedDict(
+    "GetCardinalityResponseTypeDef",
+    {
+        "cardinality": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobDocumentResponseTypeDef = TypedDict(
+    "GetJobDocumentResponseTypeDef",
+    {
+        "document": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLoggingOptionsResponseTypeDef = TypedDict(
+    "GetLoggingOptionsResponseTypeDef",
+    {
+        "roleArn": str,
+        "logLevel": LogLevelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageResponseTypeDef = TypedDict(
+    "GetPackageResponseTypeDef",
+    {
+        "packageName": str,
+        "packageArn": str,
+        "description": str,
+        "defaultVersionName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionResponseTypeDef = TypedDict(
+    "GetPackageVersionResponseTypeDef",
+    {
+        "packageVersionArn": str,
+        "packageName": str,
+        "versionName": str,
+        "description": str,
+        "attributes": Dict[str, str],
+        "status": PackageVersionStatusType,
+        "errorReason": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "policyName": str,
+        "policyArn": str,
+        "policyDocument": str,
+        "defaultVersionId": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "generationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyVersionResponseTypeDef = TypedDict(
+    "GetPolicyVersionResponseTypeDef",
+    {
+        "policyArn": str,
+        "policyName": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "isDefaultVersion": bool,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "generationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegistrationCodeResponseTypeDef = TypedDict(
+    "GetRegistrationCodeResponseTypeDef",
+    {
+        "registrationCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetV2LoggingOptionsResponseTypeDef = TypedDict(
+    "GetV2LoggingOptionsResponseTypeDef",
+    {
+        "roleArn": str,
+        "defaultLogLevel": LogLevelType,
+        "disableAllLogs": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAttachedPoliciesResponseTypeDef = TypedDict(
     "ListAttachedPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomMetricsResponseTypeDef = TypedDict(
+    "ListCustomMetricsResponseTypeDef",
+    {
+        "metricNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDimensionsResponseTypeDef = TypedDict(
+    "ListDimensionsResponseTypeDef",
+    {
+        "dimensionNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndicesResponseTypeDef = TypedDict(
+    "ListIndicesResponseTypeDef",
+    {
+        "indexNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyPrincipalsResponseTypeDef = TypedDict(
+    "ListPolicyPrincipalsResponseTypeDef",
+    {
+        "principals": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPrincipalPoliciesResponseTypeDef = TypedDict(
     "ListPrincipalPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssetPropertyValueOutputTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueOutputTypeDef",
+ListPrincipalThingsResponseTypeDef = TypedDict(
+    "ListPrincipalThingsResponseTypeDef",
     {
-        "value": AssetPropertyVariantOutputTypeDef,
-        "timestamp": AssetPropertyTimestampOutputTypeDef,
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssetPropertyValueOutputTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueOutputTypeDef",
+
+ListRoleAliasesResponseTypeDef = TypedDict(
+    "ListRoleAliasesResponseTypeDef",
     {
-        "quality": str,
+        "roleAliases": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListTargetsForPolicyResponseTypeDef = TypedDict(
+    "ListTargetsForPolicyResponseTypeDef",
+    {
+        "targets": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AssetPropertyValueOutputTypeDef(
-    _RequiredAssetPropertyValueOutputTypeDef, _OptionalAssetPropertyValueOutputTypeDef
-):
-    pass
+ListThingPrincipalsResponseTypeDef = TypedDict(
+    "ListThingPrincipalsResponseTypeDef",
+    {
+        "principals": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListThingRegistrationTaskReportsResponseTypeDef = TypedDict(
+    "ListThingRegistrationTaskReportsResponseTypeDef",
+    {
+        "resourceLinks": List[str],
+        "reportType": ReportTypeType,
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredAssetPropertyValueTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueTypeDef",
+ListThingRegistrationTasksResponseTypeDef = TypedDict(
+    "ListThingRegistrationTasksResponseTypeDef",
     {
-        "value": AssetPropertyVariantTypeDef,
-        "timestamp": AssetPropertyTimestampTypeDef,
+        "taskIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssetPropertyValueTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueTypeDef",
+
+ListThingsInBillingGroupResponseTypeDef = TypedDict(
+    "ListThingsInBillingGroupResponseTypeDef",
     {
-        "quality": str,
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListThingsInThingGroupResponseTypeDef = TypedDict(
+    "ListThingsInThingGroupResponseTypeDef",
+    {
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AssetPropertyValueTypeDef(
-    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
-):
-    pass
+RegisterCACertificateResponseTypeDef = TypedDict(
+    "RegisterCACertificateResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateResponseTypeDef = TypedDict(
+    "RegisterCertificateResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateWithoutCAResponseTypeDef = TypedDict(
+    "RegisterCertificateWithoutCAResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterThingResponseTypeDef = TypedDict(
+    "RegisterThingResponseTypeDef",
+    {
+        "certificatePem": str,
+        "resourceArns": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultAuthorizerResponseTypeDef = TypedDict(
+    "SetDefaultAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StartAuditMitigationActionsTaskResponseTypeDef = TypedDict(
+    "StartAuditMitigationActionsTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
+    "StartDetectMitigationActionsTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartOnDemandAuditTaskResponseTypeDef = TypedDict(
+    "StartOnDemandAuditTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartThingRegistrationTaskResponseTypeDef = TypedDict(
+    "StartThingRegistrationTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestInvokeAuthorizerResponseTypeDef = TypedDict(
+    "TestInvokeAuthorizerResponseTypeDef",
+    {
+        "isAuthenticated": bool,
+        "principalId": str,
+        "policyDocuments": List[str],
+        "refreshAfterInSeconds": int,
+        "disconnectAfterInSeconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferCertificateResponseTypeDef = TypedDict(
+    "TransferCertificateResponseTypeDef",
+    {
+        "transferredCertificateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBillingGroupResponseTypeDef = TypedDict(
+    "UpdateBillingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCustomMetricResponseTypeDef = TypedDict(
+    "UpdateCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "metricType": CustomMetricTypeType,
+        "displayName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDimensionResponseTypeDef = TypedDict(
+    "UpdateDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "type": Literal["TOPIC_FILTER"],
+        "stringValues": List[str],
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainConfigurationResponseTypeDef = TypedDict(
+    "UpdateDomainConfigurationResponseTypeDef",
+    {
+        "domainConfigurationName": str,
+        "domainConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDynamicThingGroupResponseTypeDef = TypedDict(
+    "UpdateDynamicThingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMitigationActionResponseTypeDef = TypedDict(
+    "UpdateMitigationActionResponseTypeDef",
+    {
+        "actionArn": str,
+        "actionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRoleAliasResponseTypeDef = TypedDict(
+    "UpdateRoleAliasResponseTypeDef",
+    {
+        "roleAlias": str,
+        "roleAliasArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduledAuditResponseTypeDef = TypedDict(
+    "UpdateScheduledAuditResponseTypeDef",
+    {
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStreamResponseTypeDef = TypedDict(
+    "UpdateStreamResponseTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "description": str,
+        "streamVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateThingGroupResponseTypeDef = TypedDict(
+    "UpdateThingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ThingGroupPropertiesOutputTypeDef = TypedDict(
     "ThingGroupPropertiesOutputTypeDef",
     {
         "thingGroupDescription": str,
         "attributePayload": AttributePayloadOutputTypeDef,
     },
@@ -7859,24 +6130,24 @@
 
 
 ListAuditMitigationActionsExecutionsResponseTypeDef = TypedDict(
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     {
         "actionsExecutions": List[AuditMitigationActionExecutionMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditMitigationActionsTasksResponseTypeDef = TypedDict(
     "ListAuditMitigationActionsTasksResponseTypeDef",
     {
         "tasks": List[AuditMitigationActionsTaskMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartAuditMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
@@ -7887,18 +6158,18 @@
 )
 
 DescribeAccountAuditConfigurationResponseTypeDef = TypedDict(
     "DescribeAccountAuditConfigurationResponseTypeDef",
     {
         "roleArn": str,
         "auditNotificationTargetConfigurations": Dict[
-            Literal["SNS"], AuditNotificationTargetOutputTypeDef
+            Literal["SNS"], AuditNotificationTargetTypeDef
         ],
-        "auditCheckConfigurations": Dict[str, AuditCheckConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "auditCheckConfigurations": Dict[str, AuditCheckConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     {
         "roleArn": str,
@@ -7911,15 +6182,15 @@
 )
 
 ListAuditTasksResponseTypeDef = TypedDict(
     "ListAuditTasksResponseTypeDef",
     {
         "tasks": List[AuditTaskMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredTestAuthorizationRequestRequestTypeDef",
     {
         "authInfos": Sequence[AuthInfoTypeDef],
@@ -7944,51 +6215,42 @@
     pass
 
 
 DescribeAuthorizerResponseTypeDef = TypedDict(
     "DescribeAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDefaultAuthorizerResponseTypeDef = TypedDict(
     "DescribeDefaultAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuthorizersResponseTypeDef = TypedDict(
     "ListAuthorizersResponseTypeDef",
     {
         "authorizers": List[AuthorizerSummaryTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AwsJobAbortConfigTypeDef = TypedDict(
     "AwsJobAbortConfigTypeDef",
     {
         "abortCriteriaList": Sequence[AwsJobAbortCriteriaTypeDef],
     },
 )
 
-AwsJobExponentialRolloutRateOutputTypeDef = TypedDict(
-    "AwsJobExponentialRolloutRateOutputTypeDef",
-    {
-        "baseRatePerMinute": int,
-        "incrementFactor": float,
-        "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaOutputTypeDef,
-    },
-)
-
 AwsJobExponentialRolloutRateTypeDef = TypedDict(
     "AwsJobExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaTypeDef,
     },
@@ -7998,16 +6260,16 @@
     "BehaviorCriteriaOutputTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
         "value": MetricValueOutputTypeDef,
         "durationSeconds": int,
         "consecutiveDatapointsToAlarm": int,
         "consecutiveDatapointsToClear": int,
-        "statisticalThreshold": StatisticalThresholdOutputTypeDef,
-        "mlDetectionConfig": MachineLearningDetectionConfigOutputTypeDef,
+        "statisticalThreshold": StatisticalThresholdTypeDef,
+        "mlDetectionConfig": MachineLearningDetectionConfigTypeDef,
     },
     total=False,
 )
 
 BehaviorCriteriaTypeDef = TypedDict(
     "BehaviorCriteriaTypeDef",
     {
@@ -8023,39 +6285,18 @@
 )
 
 GetBehaviorModelTrainingSummariesResponseTypeDef = TypedDict(
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     {
         "summaries": List[BehaviorModelTrainingSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredMetricToRetainOutputTypeDef = TypedDict(
-    "_RequiredMetricToRetainOutputTypeDef",
-    {
-        "metric": str,
-    },
-)
-_OptionalMetricToRetainOutputTypeDef = TypedDict(
-    "_OptionalMetricToRetainOutputTypeDef",
-    {
-        "metricDimension": MetricDimensionOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class MetricToRetainOutputTypeDef(
-    _RequiredMetricToRetainOutputTypeDef, _OptionalMetricToRetainOutputTypeDef
-):
-    pass
-
-
 _RequiredMetricToRetainTypeDef = TypedDict(
     "_RequiredMetricToRetainTypeDef",
     {
         "metric": str,
     },
 )
 _OptionalMetricToRetainTypeDef = TypedDict(
@@ -8074,17 +6315,17 @@
 DescribeBillingGroupResponseTypeDef = TypedDict(
     "DescribeBillingGroupResponseTypeDef",
     {
         "billingGroupName": str,
         "billingGroupId": str,
         "billingGroupArn": str,
         "version": int,
-        "billingGroupProperties": BillingGroupPropertiesOutputTypeDef,
+        "billingGroupProperties": BillingGroupPropertiesTypeDef,
         "billingGroupMetadata": BillingGroupMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBillingGroupRequestRequestTypeDef",
     {
         "billingGroupName": str,
@@ -8108,15 +6349,15 @@
 
 
 GetBucketsAggregationResponseTypeDef = TypedDict(
     "GetBucketsAggregationResponseTypeDef",
     {
         "totalCount": int,
         "buckets": List[BucketTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketsAggregationTypeTypeDef = TypedDict(
     "BucketsAggregationTypeTypeDef",
     {
         "termsAggregation": TermsAggregationTypeDef,
@@ -8144,15 +6385,15 @@
 )
 
 ListCACertificatesResponseTypeDef = TypedDict(
     "ListCACertificatesResponseTypeDef",
     {
         "certificates": List[CACertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateDescriptionTypeDef = TypedDict(
     "CertificateDescriptionTypeDef",
     {
         "certificateArn": str,
@@ -8174,32 +6415,32 @@
 )
 
 ListCertificatesByCAResponseTypeDef = TypedDict(
     "ListCertificatesByCAResponseTypeDef",
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomCodeSigningOutputTypeDef = TypedDict(
     "CustomCodeSigningOutputTypeDef",
     {
         "signature": CodeSigningSignatureOutputTypeDef,
-        "certificateChain": CodeSigningCertificateChainOutputTypeDef,
+        "certificateChain": CodeSigningCertificateChainTypeDef,
         "hashAlgorithm": str,
         "signatureAlgorithm": str,
     },
     total=False,
 )
 
 CustomCodeSigningTypeDef = TypedDict(
@@ -8212,18 +6453,18 @@
     },
     total=False,
 )
 
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
-        "eventConfigurations": Dict[EventTypeType, ConfigurationOutputTypeDef],
+        "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventConfigurationsRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationsRequestRequestTypeDef",
     {
         "eventConfigurations": Mapping[EventTypeType, ConfigurationTypeDef],
@@ -8426,14 +6667,23 @@
 class CreateScheduledAuditRequestRequestTypeDef(
     _RequiredCreateScheduledAuditRequestRequestTypeDef,
     _OptionalCreateScheduledAuditRequestRequestTypeDef,
 ):
     pass
 
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -8487,14 +6737,25 @@
 class UpdateDomainConfigurationRequestRequestTypeDef(
     _RequiredUpdateDomainConfigurationRequestRequestTypeDef,
     _OptionalUpdateDomainConfigurationRequestRequestTypeDef,
 ):
     pass
 
 
+SchedulingConfigOutputTypeDef = TypedDict(
+    "SchedulingConfigOutputTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+        "endBehavior": JobEndBehaviorType,
+        "maintenanceWindows": List[MaintenanceWindowTypeDef],
+    },
+    total=False,
+)
+
 SchedulingConfigTypeDef = TypedDict(
     "SchedulingConfigTypeDef",
     {
         "startTime": str,
         "endTime": str,
         "endBehavior": JobEndBehaviorType,
         "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
@@ -8505,26 +6766,26 @@
 CreateKeysAndCertificateResponseTypeDef = TypedDict(
     "CreateKeysAndCertificateResponseTypeDef",
     {
         "certificateArn": str,
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProvisioningClaimResponseTypeDef = TypedDict(
     "CreateProvisioningClaimResponseTypeDef",
     {
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
         "expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
@@ -8548,14 +6809,32 @@
 class CreateProvisioningTemplateRequestRequestTypeDef(
     _RequiredCreateProvisioningTemplateRequestRequestTypeDef,
     _OptionalCreateProvisioningTemplateRequestRequestTypeDef,
 ):
     pass
 
 
+DescribeProvisioningTemplateResponseTypeDef = TypedDict(
+    "DescribeProvisioningTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "description": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "defaultVersionId": int,
+        "templateBody": str,
+        "enabled": bool,
+        "provisioningRoleArn": str,
+        "preProvisioningHook": ProvisioningHookTypeDef,
+        "type": TemplateTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
@@ -8606,148 +6885,155 @@
     {
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
         "taskStartTime": datetime,
         "taskStatistics": TaskStatisticsTypeDef,
         "scheduledAuditName": str,
         "auditDetails": Dict[str, AuditCheckDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterCACertificateRequestRequestTypeDef",
+    {
+        "caCertificate": str,
+    },
+)
+_OptionalRegisterCACertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterCACertificateRequestRequestTypeDef",
+    {
+        "verificationCertificate": str,
+        "setAsActive": bool,
+        "allowAutoRegistration": bool,
+        "registrationConfig": RegistrationConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "certificateMode": CertificateModeType,
+    },
+    total=False,
+)
+
+
+class RegisterCACertificateRequestRequestTypeDef(
+    _RequiredRegisterCACertificateRequestRequestTypeDef,
+    _OptionalRegisterCACertificateRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateCACertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCACertificateRequestRequestTypeDef",
+    {
+        "certificateId": str,
+    },
+)
+_OptionalUpdateCACertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCACertificateRequestRequestTypeDef",
+    {
+        "newStatus": CACertificateStatusType,
+        "newAutoRegistrationStatus": AutoRegistrationStatusType,
+        "registrationConfig": RegistrationConfigTypeDef,
+        "removeAutoRegistration": bool,
+    },
+    total=False,
+)
+
+
+class UpdateCACertificateRequestRequestTypeDef(
+    _RequiredUpdateCACertificateRequestRequestTypeDef,
+    _OptionalUpdateCACertificateRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeDomainConfigurationResponseTypeDef = TypedDict(
     "DescribeDomainConfigurationResponseTypeDef",
     {
         "domainConfigurationName": str,
         "domainConfigurationArn": str,
         "domainName": str,
         "serverCertificates": List[ServerCertificateSummaryTypeDef],
-        "authorizerConfig": AuthorizerConfigOutputTypeDef,
+        "authorizerConfig": AuthorizerConfigTypeDef,
         "domainConfigurationStatus": DomainConfigurationStatusType,
         "serviceType": ServiceTypeType,
         "domainType": DomainTypeType,
         "lastStatusChangeDate": datetime,
-        "tlsConfig": TlsConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SchedulingConfigOutputTypeDef = TypedDict(
-    "SchedulingConfigOutputTypeDef",
-    {
-        "startTime": str,
-        "endTime": str,
-        "endBehavior": JobEndBehaviorType,
-        "maintenanceWindows": List[MaintenanceWindowOutputTypeDef],
+        "tlsConfig": TlsConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeManagedJobTemplateResponseTypeDef = TypedDict(
     "DescribeManagedJobTemplateResponseTypeDef",
     {
         "templateName": str,
         "templateArn": str,
         "description": str,
         "templateVersion": str,
         "environments": List[str],
         "documentParameters": List[DocumentParameterTypeDef],
         "document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeProvisioningTemplateResponseTypeDef = TypedDict(
-    "DescribeProvisioningTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "description": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "defaultVersionId": int,
-        "templateBody": str,
-        "enabled": bool,
-        "provisioningRoleArn": str,
-        "preProvisioningHook": ProvisioningHookOutputTypeDef,
-        "type": TemplateTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRoleAliasResponseTypeDef = TypedDict(
     "DescribeRoleAliasResponseTypeDef",
     {
         "roleAliasDescription": RoleAliasDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeThingTypeResponseTypeDef = TypedDict(
     "DescribeThingTypeResponseTypeDef",
     {
         "thingTypeName": str,
         "thingTypeId": str,
         "thingTypeArn": str,
         "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingTypeDefinitionTypeDef = TypedDict(
     "ThingTypeDefinitionTypeDef",
     {
         "thingTypeName": str,
         "thingTypeArn": str,
         "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
-DestinationOutputTypeDef = TypedDict(
-    "DestinationOutputTypeDef",
-    {
-        "s3Destination": S3DestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
 
 ListDetectMitigationActionsExecutionsResponseTypeDef = TypedDict(
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DynamoDBv2ActionOutputTypeDef = TypedDict(
-    "DynamoDBv2ActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "putItem": PutItemInputOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DynamoDBv2ActionTypeDef = TypedDict(
     "DynamoDBv2ActionTypeDef",
     {
         "roleArn": str,
@@ -8755,24 +7041,15 @@
     },
 )
 
 GetEffectivePoliciesResponseTypeDef = TypedDict(
     "GetEffectivePoliciesResponseTypeDef",
     {
         "effectivePolicies": List[EffectivePolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExponentialRolloutRateOutputTypeDef = TypedDict(
-    "ExponentialRolloutRateOutputTypeDef",
-    {
-        "baseRatePerMinute": int,
-        "incrementFactor": float,
-        "rateIncreaseCriteria": RateIncreaseCriteriaOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExponentialRolloutRateTypeDef = TypedDict(
     "ExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
@@ -8786,16 +7063,16 @@
     {
         "thingGroupIndexingMode": ThingGroupIndexingModeType,
     },
 )
 _OptionalThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
     "_OptionalThingGroupIndexingConfigurationOutputTypeDef",
     {
-        "managedFields": List[FieldOutputTypeDef],
-        "customFields": List[FieldOutputTypeDef],
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
     },
     total=False,
 )
 
 
 class ThingGroupIndexingConfigurationOutputTypeDef(
     _RequiredThingGroupIndexingConfigurationOutputTypeDef,
@@ -8822,32 +7099,14 @@
 
 class ThingGroupIndexingConfigurationTypeDef(
     _RequiredThingGroupIndexingConfigurationTypeDef, _OptionalThingGroupIndexingConfigurationTypeDef
 ):
     pass
 
 
-StreamFileOutputTypeDef = TypedDict(
-    "StreamFileOutputTypeDef",
-    {
-        "fileId": int,
-        "s3Location": S3LocationOutputTypeDef,
-    },
-    total=False,
-)
-
-FileLocationOutputTypeDef = TypedDict(
-    "FileLocationOutputTypeDef",
-    {
-        "stream": StreamOutputTypeDef,
-        "s3Location": S3LocationOutputTypeDef,
-    },
-    total=False,
-)
-
 StreamFileTypeDef = TypedDict(
     "StreamFileTypeDef",
     {
         "fileId": int,
         "s3Location": S3LocationTypeDef,
     },
     total=False,
@@ -8863,87 +7122,981 @@
 )
 
 ListFleetMetricsResponseTypeDef = TypedDict(
     "ListFleetMetricsResponseTypeDef",
     {
         "fleetMetrics": List[FleetMetricNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = (
+    TypedDict(
+        "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+        {
+            "securityProfileName": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = TypedDict(
+    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    {
+        "target": str,
+    },
+)
+_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    {
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef(
+    _RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    _OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+        "findingId": str,
+    },
+)
+_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "actionStatus": AuditMitigationActionsExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef(
+    _RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    {
+        "auditTaskId": str,
+        "findingId": str,
+        "taskStatus": AuditMitigationActionsTaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef(
+    _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
+    "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
+    "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    {
+        "taskType": AuditTaskTypeType,
+        "taskStatus": AuditTaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAuditTasksRequestListAuditTasksPaginateTypeDef(
+    _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef,
+):
+    pass
+
+
+ListAuthorizersRequestListAuthorizersPaginateTypeDef = TypedDict(
+    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "status": AuthorizerStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = TypedDict(
+    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
+    {
+        "namePrefixFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCACertificatesRequestListCACertificatesPaginateTypeDef = TypedDict(
+    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "templateName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
+    "_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    {
+        "caCertificateId": str,
+    },
+)
+_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
+    "_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef(
+    _RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    _OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+):
+    pass
+
+
+ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = TypedDict(
+    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+        "violationId": str,
+        "thingName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef(
+    _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+):
+    pass
+
+
+ListDimensionsRequestListDimensionsPaginateTypeDef = TypedDict(
+    "ListDimensionsRequestListDimensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = TypedDict(
+    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
+    {
+        "serviceType": ServiceTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = TypedDict(
+    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIndicesRequestListIndicesPaginateTypeDef = TypedDict(
+    "ListIndicesRequestListIndicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
+    "_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    {
+        "jobId": str,
+    },
+)
+_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
+    "_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    {
+        "status": JobExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef(
+    _RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    _OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
+    "_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
+    "_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    {
+        "status": JobExecutionStatusType,
+        "namespaceId": str,
+        "jobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef(
+    _RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    _OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+):
+    pass
+
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "status": JobStatusType,
+        "targetSelection": TargetSelectionType,
+        "thingGroupName": str,
+        "thingGroupId": str,
+        "namespaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef = TypedDict(
+    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
+    {
+        "templateName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
+    "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    {
+        "thingName": str,
+        "metricName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
+    "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    {
+        "dimensionName": str,
+        "dimensionValueOperator": DimensionValueOperatorType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMetricValuesRequestListMetricValuesPaginateTypeDef(
+    _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef,
+):
+    pass
+
+
+ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = TypedDict(
+    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
+    {
+        "actionType": MitigationActionTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = TypedDict(
+    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
+    {
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = TypedDict(
+    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "packageName": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "status": PackageVersionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    {
+        "policyName": str,
+    },
+)
+_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef(
+    _RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    _OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    {
+        "principal": str,
+    },
+)
+_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef(
+    _RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    _OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    {
+        "principal": str,
+    },
+)
+_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef(
+    _RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    _OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    {
+        "templateName": str,
+    },
+)
+_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef(
+    _RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    _OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = TypedDict(
+    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
+    "_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    {
+        "findingId": str,
+    },
+)
+_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
+    "_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef(
+    _RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    _OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+):
+    pass
+
+
+ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = TypedDict(
+    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = TypedDict(
+    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+        {
+            "securityProfileTargetArn": str,
+        },
+    )
+)
+_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+        {
+            "recursive": bool,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef(
+    _RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    _OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+):
+    pass
+
+
+ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
+    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
+    {
+        "dimensionName": str,
+        "metricName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
+    "ListStreamsRequestListStreamsPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    {
+        "policyName": str,
+    },
+)
+_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(
+    _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
+    TypedDict(
+        "_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+        {
+            "securityProfileName": str,
+        },
+    )
+)
+_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
+    TypedDict(
+        "_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef(
+    _RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    _OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
+    "_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
+    "_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef(
+    _RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    _OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+):
+    pass
+
+
+ListThingGroupsRequestListThingGroupsPaginateTypeDef = TypedDict(
+    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
+    {
+        "parentGroup": str,
+        "namePrefixFilter": str,
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef(
+    _RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    _OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
+    "_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    {
+        "taskId": str,
+        "reportType": ReportTypeType,
+    },
+)
+_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
+    "_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef(
+    _RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    _OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+):
+    pass
+
+
+ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = TypedDict(
+    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListThingTypesRequestListThingTypesPaginateTypeDef = TypedDict(
+    "ListThingTypesRequestListThingTypesPaginateTypeDef",
+    {
+        "thingTypeName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
+    "_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    {
+        "billingGroupName": str,
+    },
+)
+_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
+    "_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef(
+    _RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    _OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
+    "_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    {
+        "thingGroupName": str,
+    },
+)
+_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
+    "_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    {
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef(
+    _RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    _OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+):
+    pass
+
+
+ListThingsRequestListThingsPaginateTypeDef = TypedDict(
+    "ListThingsRequestListThingsPaginateTypeDef",
+    {
+        "attributeName": str,
+        "attributeValue": str,
+        "thingTypeName": str,
+        "usePrefixAttributeValue": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = TypedDict(
+    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicRulesRequestListTopicRulesPaginateTypeDef = TypedDict(
+    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
+    {
+        "topic": str,
+        "ruleDisabled": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = TypedDict(
+    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
+    {
+        "targetType": LogTargetTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
+    "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
+    "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListViolationEventsRequestListViolationEventsPaginateTypeDef(
+    _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef,
+    _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef,
+):
+    pass
+
+
 GetPackageConfigurationResponseTypeDef = TypedDict(
     "GetPackageConfigurationResponseTypeDef",
     {
-        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdatePackageConfigurationRequestRequestTypeDef",
+    {
+        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
+        "clientToken": str,
     },
+    total=False,
 )
 
 GetPercentilesResponseTypeDef = TypedDict(
     "GetPercentilesResponseTypeDef",
     {
         "percentiles": List[PercentPairTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStatisticsResponseTypeDef = TypedDict(
     "GetStatisticsResponseTypeDef",
     {
         "statistics": StatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBillingGroupsResponseTypeDef = TypedDict(
     "ListBillingGroupsResponseTypeDef",
     {
         "billingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingGroupsForThingResponseTypeDef = TypedDict(
     "ListThingGroupsForThingResponseTypeDef",
     {
         "thingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingGroupsResponseTypeDef = TypedDict(
     "ListThingGroupsResponseTypeDef",
     {
         "thingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingGroupMetadataTypeDef = TypedDict(
     "ThingGroupMetadataTypeDef",
     {
         "parentGroupName": str,
         "rootToParentThingGroups": List[GroupNameAndArnTypeDef],
         "creationDate": datetime,
     },
     total=False,
 )
 
-HttpAuthorizationOutputTypeDef = TypedDict(
-    "HttpAuthorizationOutputTypeDef",
-    {
-        "sigv4": SigV4AuthorizationOutputTypeDef,
-    },
-    total=False,
-)
-
 HttpAuthorizationTypeDef = TypedDict(
     "HttpAuthorizationTypeDef",
     {
         "sigv4": SigV4AuthorizationTypeDef,
     },
     total=False,
 )
@@ -8956,16 +8109,16 @@
 )
 _OptionalThingIndexingConfigurationOutputTypeDef = TypedDict(
     "_OptionalThingIndexingConfigurationOutputTypeDef",
     {
         "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
         "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
         "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": List[FieldOutputTypeDef],
-        "customFields": List[FieldOutputTypeDef],
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
         "filter": IndexingFilterOutputTypeDef,
     },
     total=False,
 )
 
 
 class ThingIndexingConfigurationOutputTypeDef(
@@ -9036,15 +8189,15 @@
     },
     total=False,
 )
 
 JobExecutionsRetryConfigOutputTypeDef = TypedDict(
     "JobExecutionsRetryConfigOutputTypeDef",
     {
-        "criteriaList": List[RetryCriteriaOutputTypeDef],
+        "criteriaList": List[RetryCriteriaTypeDef],
     },
 )
 
 JobExecutionsRetryConfigTypeDef = TypedDict(
     "JobExecutionsRetryConfigTypeDef",
     {
         "criteriaList": Sequence[RetryCriteriaTypeDef],
@@ -9052,149 +8205,140 @@
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "jobTemplates": List[JobTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedJobTemplatesResponseTypeDef = TypedDict(
     "ListManagedJobTemplatesResponseTypeDef",
     {
         "managedJobTemplates": List[ManagedJobTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMitigationActionsResponseTypeDef = TypedDict(
     "ListMitigationActionsResponseTypeDef",
     {
         "actionIdentifiers": List[MitigationActionIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOTAUpdatesResponseTypeDef = TypedDict(
     "ListOTAUpdatesResponseTypeDef",
     {
         "otaUpdates": List[OTAUpdateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutgoingCertificatesResponseTypeDef = TypedDict(
     "ListOutgoingCertificatesResponseTypeDef",
     {
         "outgoingCertificates": List[OutgoingCertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageVersionsResponseTypeDef = TypedDict(
     "ListPackageVersionsResponseTypeDef",
     {
         "packageVersionSummaries": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "packageSummaries": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyVersionsResponseTypeDef = TypedDict(
     "ListPolicyVersionsResponseTypeDef",
     {
         "policyVersions": List[PolicyVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningTemplateVersionsResponseTypeDef = TypedDict(
     "ListProvisioningTemplateVersionsResponseTypeDef",
     {
         "versions": List[ProvisioningTemplateVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningTemplatesResponseTypeDef = TypedDict(
     "ListProvisioningTemplatesResponseTypeDef",
     {
         "templates": List[ProvisioningTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScheduledAuditsResponseTypeDef = TypedDict(
     "ListScheduledAuditsResponseTypeDef",
     {
         "scheduledAudits": List[ScheduledAuditMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityProfilesResponseTypeDef = TypedDict(
     "ListSecurityProfilesResponseTypeDef",
     {
         "securityProfileIdentifiers": List[SecurityProfileIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "streams": List[StreamSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsForSecurityProfileResponseTypeDef = TypedDict(
     "ListTargetsForSecurityProfileResponseTypeDef",
     {
         "securityProfileTargets": List[SecurityProfileTargetTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SecurityProfileTargetMappingTypeDef = TypedDict(
     "SecurityProfileTargetMappingTypeDef",
     {
         "securityProfileIdentifier": SecurityProfileIdentifierTypeDef,
@@ -9204,51 +8348,26 @@
 )
 
 ListThingsResponseTypeDef = TypedDict(
     "ListThingsResponseTypeDef",
     {
         "things": List[ThingAttributeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTopicRulesResponseTypeDef = TypedDict(
     "ListTopicRulesResponseTypeDef",
     {
         "rules": List[TopicRuleListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredLocationActionOutputTypeDef = TypedDict(
-    "_RequiredLocationActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "trackerName": str,
-        "deviceId": str,
-        "latitude": str,
-        "longitude": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalLocationActionOutputTypeDef = TypedDict(
-    "_OptionalLocationActionOutputTypeDef",
-    {
-        "timestamp": LocationTimestampOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class LocationActionOutputTypeDef(
-    _RequiredLocationActionOutputTypeDef, _OptionalLocationActionOutputTypeDef
-):
-    pass
-
 
 _RequiredLocationActionTypeDef = TypedDict(
     "_RequiredLocationActionTypeDef",
     {
         "roleArn": str,
         "trackerName": str,
         "deviceId": str,
@@ -9268,15 +8387,15 @@
 class LocationActionTypeDef(_RequiredLocationActionTypeDef, _OptionalLocationActionTypeDef):
     pass
 
 
 LogTargetConfigurationTypeDef = TypedDict(
     "LogTargetConfigurationTypeDef",
     {
-        "logTarget": LogTargetOutputTypeDef,
+        "logTarget": LogTargetTypeDef,
         "logLevel": LogLevelType,
     },
     total=False,
 )
 
 SetV2LoggingLevelRequestRequestTypeDef = TypedDict(
     "SetV2LoggingLevelRequestRequestTypeDef",
@@ -9292,20 +8411,20 @@
         "loggingOptionsPayload": LoggingOptionsPayloadTypeDef,
     },
 )
 
 MitigationActionParamsOutputTypeDef = TypedDict(
     "MitigationActionParamsOutputTypeDef",
     {
-        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsOutputTypeDef,
-        "updateCACertificateParams": UpdateCACertificateParamsOutputTypeDef,
+        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
+        "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
         "addThingsToThingGroupParams": AddThingsToThingGroupParamsOutputTypeDef,
-        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsOutputTypeDef,
-        "enableIoTLoggingParams": EnableIoTLoggingParamsOutputTypeDef,
-        "publishFindingToSnsParams": PublishFindingToSnsParamsOutputTypeDef,
+        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
+        "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
+        "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
 MitigationActionParamsTypeDef = TypedDict(
     "MitigationActionParamsTypeDef",
     {
@@ -9323,15 +8442,15 @@
     "MqttHeadersOutputTypeDef",
     {
         "payloadFormatIndicator": str,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
         "messageExpiry": str,
-        "userProperties": List[UserPropertyOutputTypeDef],
+        "userProperties": List[UserPropertyTypeDef],
     },
     total=False,
 )
 
 MqttHeadersTypeDef = TypedDict(
     "MqttHeadersTypeDef",
     {
@@ -9341,31 +8460,14 @@
         "correlationData": str,
         "messageExpiry": str,
         "userProperties": Sequence[UserPropertyTypeDef],
     },
     total=False,
 )
 
-ResourceIdentifierOutputTypeDef = TypedDict(
-    "ResourceIdentifierOutputTypeDef",
-    {
-        "deviceCertificateId": str,
-        "caCertificateId": str,
-        "cognitoIdentityPoolId": str,
-        "clientId": str,
-        "policyVersionIdentifier": PolicyVersionIdentifierOutputTypeDef,
-        "account": str,
-        "iamRoleArn": str,
-        "roleAliasArn": str,
-        "issuerCertificateIdentifier": IssuerCertificateIdentifierOutputTypeDef,
-        "deviceCertificateArn": str,
-    },
-    total=False,
-)
-
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "deviceCertificateId": str,
         "caCertificateId": str,
         "cognitoIdentityPoolId": str,
         "clientId": str,
@@ -9375,66 +8477,14 @@
         "roleAliasArn": str,
         "issuerCertificateIdentifier": IssuerCertificateIdentifierTypeDef,
         "deviceCertificateArn": str,
     },
     total=False,
 )
 
-_RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterCACertificateRequestRequestTypeDef",
-    {
-        "caCertificate": str,
-    },
-)
-_OptionalRegisterCACertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterCACertificateRequestRequestTypeDef",
-    {
-        "verificationCertificate": str,
-        "setAsActive": bool,
-        "allowAutoRegistration": bool,
-        "registrationConfig": RegistrationConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "certificateMode": CertificateModeType,
-    },
-    total=False,
-)
-
-
-class RegisterCACertificateRequestRequestTypeDef(
-    _RequiredRegisterCACertificateRequestRequestTypeDef,
-    _OptionalRegisterCACertificateRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateCACertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCACertificateRequestRequestTypeDef",
-    {
-        "certificateId": str,
-    },
-)
-_OptionalUpdateCACertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCACertificateRequestRequestTypeDef",
-    {
-        "newStatus": CACertificateStatusType,
-        "newAutoRegistrationStatus": AutoRegistrationStatusType,
-        "registrationConfig": RegistrationConfigTypeDef,
-        "removeAutoRegistration": bool,
-    },
-    total=False,
-)
-
-
-class UpdateCACertificateRequestRequestTypeDef(
-    _RequiredUpdateCACertificateRequestRequestTypeDef,
-    _OptionalUpdateCACertificateRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
         "target": DetectMitigationActionsTaskTargetTypeDef,
         "actions": Sequence[str],
         "clientRequestToken": str,
@@ -9501,21 +8551,21 @@
 
 _RequiredTimestreamActionOutputTypeDef = TypedDict(
     "_RequiredTimestreamActionOutputTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tableName": str,
-        "dimensions": List[TimestreamDimensionOutputTypeDef],
+        "dimensions": List[TimestreamDimensionTypeDef],
     },
 )
 _OptionalTimestreamActionOutputTypeDef = TypedDict(
     "_OptionalTimestreamActionOutputTypeDef",
     {
-        "timestamp": TimestreamTimestampOutputTypeDef,
+        "timestamp": TimestreamTimestampTypeDef,
     },
     total=False,
 )
 
 
 class TimestreamActionOutputTypeDef(
     _RequiredTimestreamActionOutputTypeDef, _OptionalTimestreamActionOutputTypeDef
@@ -9578,38 +8628,29 @@
         "statusReason": str,
         "httpUrlProperties": HttpUrlDestinationPropertiesTypeDef,
         "vpcProperties": VpcDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
-UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdatePackageConfigurationRequestRequestTypeDef",
-    {
-        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
-        "clientToken": str,
-    },
-    total=False,
-)
-
 ValidateSecurityProfileBehaviorsResponseTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricValuesResponseTypeDef = TypedDict(
     "ListMetricValuesResponseTypeDef",
     {
         "metricDatumList": List[MetricDatumTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeniedTypeDef = TypedDict(
     "DeniedTypeDef",
     {
         "implicitDeny": ImplicitDenyTypeDef,
@@ -9617,15 +8658,15 @@
     },
     total=False,
 )
 
 _RequiredPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryOutputTypeDef",
     {
-        "propertyValues": List[AssetPropertyValueOutputTypeDef],
+        "propertyValues": List[AssetPropertyValueTypeDef],
     },
 )
 _OptionalPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
     "_OptionalPutAssetPropertyValueEntryOutputTypeDef",
     {
         "entryId": str,
         "assetId": str,
@@ -9760,23 +8801,14 @@
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
 
-AwsJobExecutionsRolloutConfigOutputTypeDef = TypedDict(
-    "AwsJobExecutionsRolloutConfigOutputTypeDef",
-    {
-        "maximumPerMinute": int,
-        "exponentialRate": AwsJobExponentialRolloutRateOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
@@ -9788,15 +8820,15 @@
         "name": str,
     },
 )
 _OptionalBehaviorOutputTypeDef = TypedDict(
     "_OptionalBehaviorOutputTypeDef",
     {
         "metric": str,
-        "metricDimension": MetricDimensionOutputTypeDef,
+        "metricDimension": MetricDimensionTypeDef,
         "criteria": BehaviorCriteriaOutputTypeDef,
         "suppressAlerts": bool,
     },
     total=False,
 )
 
 
@@ -9851,89 +8883,55 @@
     pass
 
 
 DescribeCACertificateResponseTypeDef = TypedDict(
     "DescribeCACertificateResponseTypeDef",
     {
         "certificateDescription": CACertificateDescriptionTypeDef,
-        "registrationConfig": RegistrationConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registrationConfig": RegistrationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
         "certificateDescription": CertificateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingTypesResponseTypeDef = TypedDict(
     "ListThingTypesResponseTypeDef",
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartSigningJobParameterOutputTypeDef = TypedDict(
-    "StartSigningJobParameterOutputTypeDef",
-    {
-        "signingProfileParameter": SigningProfileParameterOutputTypeDef,
-        "signingProfileName": str,
-        "destination": DestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 StartSigningJobParameterTypeDef = TypedDict(
     "StartSigningJobParameterTypeDef",
     {
         "signingProfileParameter": SigningProfileParameterTypeDef,
         "signingProfileName": str,
         "destination": DestinationTypeDef,
     },
     total=False,
 )
 
-JobExecutionsRolloutConfigOutputTypeDef = TypedDict(
-    "JobExecutionsRolloutConfigOutputTypeDef",
-    {
-        "maximumPerMinute": int,
-        "exponentialRate": ExponentialRolloutRateOutputTypeDef,
-    },
-    total=False,
-)
-
 JobExecutionsRolloutConfigTypeDef = TypedDict(
     "JobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
-StreamInfoTypeDef = TypedDict(
-    "StreamInfoTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "streamVersion": int,
-        "description": str,
-        "files": List[StreamFileOutputTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -9950,14 +8948,29 @@
 
 class CreateStreamRequestRequestTypeDef(
     _RequiredCreateStreamRequestRequestTypeDef, _OptionalCreateStreamRequestRequestTypeDef
 ):
     pass
 
 
+StreamInfoTypeDef = TypedDict(
+    "StreamInfoTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "streamVersion": int,
+        "description": str,
+        "files": List[StreamFileTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamRequestRequestTypeDef",
     {
         "streamId": str,
     },
 )
 _OptionalUpdateStreamRequestRequestTypeDef = TypedDict(
@@ -9986,30 +8999,30 @@
         "version": int,
         "thingGroupProperties": ThingGroupPropertiesOutputTypeDef,
         "thingGroupMetadata": ThingGroupMetadataTypeDef,
         "indexName": str,
         "queryString": str,
         "queryVersion": str,
         "status": DynamicGroupStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHttpActionOutputTypeDef = TypedDict(
     "_RequiredHttpActionOutputTypeDef",
     {
         "url": str,
     },
 )
 _OptionalHttpActionOutputTypeDef = TypedDict(
     "_OptionalHttpActionOutputTypeDef",
     {
         "confirmationUrl": str,
-        "headers": List[HttpActionHeaderOutputTypeDef],
-        "auth": HttpAuthorizationOutputTypeDef,
+        "headers": List[HttpActionHeaderTypeDef],
+        "auth": HttpAuthorizationTypeDef,
     },
     total=False,
 )
 
 
 class HttpActionOutputTypeDef(_RequiredHttpActionOutputTypeDef, _OptionalHttpActionOutputTypeDef):
     pass
@@ -10037,15 +9050,15 @@
 
 
 GetIndexingConfigurationResponseTypeDef = TypedDict(
     "GetIndexingConfigurationResponseTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
@@ -10054,66 +9067,66 @@
     total=False,
 )
 
 DescribeJobExecutionResponseTypeDef = TypedDict(
     "DescribeJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobExecutionsForJobResponseTypeDef = TypedDict(
     "ListJobExecutionsForJobResponseTypeDef",
     {
         "executionSummaries": List[JobExecutionSummaryForJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobExecutionsForThingResponseTypeDef = TypedDict(
     "ListJobExecutionsForThingResponseTypeDef",
     {
         "executionSummaries": List[JobExecutionSummaryForThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityProfilesForTargetResponseTypeDef = TypedDict(
     "ListSecurityProfilesForTargetResponseTypeDef",
     {
         "securityProfileTargetMappings": List[SecurityProfileTargetMappingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListV2LoggingLevelsResponseTypeDef = TypedDict(
     "ListV2LoggingLevelsResponseTypeDef",
     {
         "logTargetConfigurations": List[LogTargetConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMitigationActionResponseTypeDef = TypedDict(
     "DescribeMitigationActionResponseTypeDef",
     {
         "actionName": str,
         "actionType": MitigationActionTypeType,
         "actionArn": str,
         "actionId": str,
         "roleArn": str,
         "actionParams": MitigationActionParamsOutputTypeDef,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MitigationActionTypeDef = TypedDict(
     "MitigationActionTypeDef",
     {
         "name": str,
@@ -10215,15 +9228,15 @@
     pass
 
 
 _RequiredAuditSuppressionTypeDef = TypedDict(
     "_RequiredAuditSuppressionTypeDef",
     {
         "checkName": str,
-        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
+        "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 _OptionalAuditSuppressionTypeDef = TypedDict(
     "_OptionalAuditSuppressionTypeDef",
     {
         "expirationDate": datetime,
         "suppressIndefinitely": bool,
@@ -10233,46 +9246,14 @@
 )
 
 
 class AuditSuppressionTypeDef(_RequiredAuditSuppressionTypeDef, _OptionalAuditSuppressionTypeDef):
     pass
 
 
-DescribeAuditSuppressionResponseTypeDef = TypedDict(
-    "DescribeAuditSuppressionResponseTypeDef",
-    {
-        "checkName": str,
-        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
-        "expirationDate": datetime,
-        "suppressIndefinitely": bool,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-NonCompliantResourceTypeDef = TypedDict(
-    "NonCompliantResourceTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
-        "additionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
-RelatedResourceTypeDef = TypedDict(
-    "RelatedResourceTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
-        "additionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "clientRequestToken": str,
     },
@@ -10307,24 +9288,36 @@
     "DescribeAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 
+DescribeAuditSuppressionResponseTypeDef = TypedDict(
+    "DescribeAuditSuppressionResponseTypeDef",
+    {
+        "checkName": str,
+        "resourceIdentifier": ResourceIdentifierTypeDef,
+        "expirationDate": datetime,
+        "suppressIndefinitely": bool,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = TypedDict(
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "listSuppressedFindings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditFindingsRequestRequestTypeDef = TypedDict(
     "ListAuditFindingsRequestRequestTypeDef",
     {
@@ -10342,15 +9335,15 @@
 
 ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef = TypedDict(
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditSuppressionsRequestRequestTypeDef = TypedDict(
     "ListAuditSuppressionsRequestRequestTypeDef",
     {
@@ -10359,14 +9352,34 @@
         "ascendingOrder": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+NonCompliantResourceTypeDef = TypedDict(
+    "NonCompliantResourceTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceIdentifier": ResourceIdentifierTypeDef,
+        "additionalInfo": Dict[str, str],
+    },
+    total=False,
+)
+
+RelatedResourceTypeDef = TypedDict(
+    "RelatedResourceTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceIdentifier": ResourceIdentifierTypeDef,
+        "additionalInfo": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredUpdateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
@@ -10390,15 +9403,15 @@
 
 SearchIndexResponseTypeDef = TypedDict(
     "SearchIndexResponseTypeDef",
     {
         "nextToken": str,
         "things": List[ThingDocumentTypeDef],
         "thingGroups": List[ThingGroupDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTopicRuleDestinationRequestRequestTypeDef = TypedDict(
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     {
         "destinationConfiguration": TopicRuleDestinationConfigurationTypeDef,
@@ -10406,31 +9419,31 @@
 )
 
 ListTopicRuleDestinationsResponseTypeDef = TypedDict(
     "ListTopicRuleDestinationsResponseTypeDef",
     {
         "destinationSummaries": List[TopicRuleDestinationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTopicRuleDestinationResponseTypeDef = TypedDict(
     "CreateTopicRuleDestinationResponseTypeDef",
     {
         "topicRuleDestination": TopicRuleDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTopicRuleDestinationResponseTypeDef = TypedDict(
     "GetTopicRuleDestinationResponseTypeDef",
     {
         "topicRuleDestination": TopicRuleDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthResultTypeDef = TypedDict(
     "AuthResultTypeDef",
     {
         "authInfo": AuthInfoOutputTypeDef,
@@ -10478,38 +9491,38 @@
 DescribeSecurityProfileResponseTypeDef = TypedDict(
     "DescribeSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
         "behaviors": List[BehaviorOutputTypeDef],
-        "alertTargets": Dict[Literal["SNS"], AlertTargetOutputTypeDef],
+        "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
-        "additionalMetricsToRetainV2": List[MetricToRetainOutputTypeDef],
+        "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSecurityProfileResponseTypeDef = TypedDict(
     "UpdateSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
         "behaviors": List[BehaviorOutputTypeDef],
-        "alertTargets": Dict[Literal["SNS"], AlertTargetOutputTypeDef],
+        "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
-        "additionalMetricsToRetainV2": List[MetricToRetainOutputTypeDef],
+        "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ViolationEventTypeDef = TypedDict(
     "ViolationEventTypeDef",
     {
         "violationId": str,
@@ -10590,15 +9603,15 @@
     },
 )
 
 CodeSigningOutputTypeDef = TypedDict(
     "CodeSigningOutputTypeDef",
     {
         "awsSignerJobId": str,
-        "startSigningJobParameter": StartSigningJobParameterOutputTypeDef,
+        "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningOutputTypeDef,
     },
     total=False,
 )
 
 CodeSigningTypeDef = TypedDict(
     "CodeSigningTypeDef",
@@ -10606,66 +9619,14 @@
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningTypeDef,
     },
     total=False,
 )
 
-DescribeJobTemplateResponseTypeDef = TypedDict(
-    "DescribeJobTemplateResponseTypeDef",
-    {
-        "jobTemplateArn": str,
-        "jobTemplateId": str,
-        "description": str,
-        "documentSource": str,
-        "document": str,
-        "createdAt": datetime,
-        "presignedUrlConfig": PresignedUrlConfigOutputTypeDef,
-        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigOutputTypeDef,
-        "abortConfig": AbortConfigOutputTypeDef,
-        "timeoutConfig": TimeoutConfigOutputTypeDef,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
-        "maintenanceWindows": List[MaintenanceWindowOutputTypeDef],
-        "destinationPackageVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-JobTypeDef = TypedDict(
-    "JobTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "targetSelection": TargetSelectionType,
-        "status": JobStatusType,
-        "forceCanceled": bool,
-        "reasonCode": str,
-        "comment": str,
-        "targets": List[str],
-        "description": str,
-        "presignedUrlConfig": PresignedUrlConfigOutputTypeDef,
-        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigOutputTypeDef,
-        "abortConfig": AbortConfigOutputTypeDef,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "completedAt": datetime,
-        "jobProcessDetails": JobProcessDetailsTypeDef,
-        "timeoutConfig": TimeoutConfigOutputTypeDef,
-        "namespaceId": str,
-        "jobTemplateArn": str,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
-        "documentParameters": Dict[str, str],
-        "isConcurrent": bool,
-        "schedulingConfig": SchedulingConfigOutputTypeDef,
-        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
-        "destinationPackageVersions": List[str],
-    },
-    total=False,
-)
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "jobId": str,
         "targets": Sequence[str],
     },
 )
@@ -10726,14 +9687,66 @@
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
 
+DescribeJobTemplateResponseTypeDef = TypedDict(
+    "DescribeJobTemplateResponseTypeDef",
+    {
+        "jobTemplateArn": str,
+        "jobTemplateId": str,
+        "description": str,
+        "documentSource": str,
+        "document": str,
+        "createdAt": datetime,
+        "presignedUrlConfig": PresignedUrlConfigTypeDef,
+        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
+        "timeoutConfig": TimeoutConfigTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "maintenanceWindows": List[MaintenanceWindowTypeDef],
+        "destinationPackageVersions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JobTypeDef = TypedDict(
+    "JobTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "targetSelection": TargetSelectionType,
+        "status": JobStatusType,
+        "forceCanceled": bool,
+        "reasonCode": str,
+        "comment": str,
+        "targets": List[str],
+        "description": str,
+        "presignedUrlConfig": PresignedUrlConfigTypeDef,
+        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "completedAt": datetime,
+        "jobProcessDetails": JobProcessDetailsTypeDef,
+        "timeoutConfig": TimeoutConfigTypeDef,
+        "namespaceId": str,
+        "jobTemplateArn": str,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "documentParameters": Dict[str, str],
+        "isConcurrent": bool,
+        "schedulingConfig": SchedulingConfigOutputTypeDef,
+        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
+        "destinationPackageVersions": List[str],
+    },
+    total=False,
+)
+
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalUpdateJobRequestRequestTypeDef = TypedDict(
@@ -10757,29 +9770,29 @@
     pass
 
 
 DescribeStreamResponseTypeDef = TypedDict(
     "DescribeStreamResponseTypeDef",
     {
         "streamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAuditMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskStatus": AuditMitigationActionsTaskStatusType,
         "startTime": datetime,
         "endTime": datetime,
         "taskStatistics": Dict[str, TaskStatisticsForAuditCheckTypeDef],
         "target": AuditMitigationActionsTaskTargetOutputTypeDef,
         "auditCheckToActionsMapping": Dict[str, List[str]],
         "actionsDefinition": List[MitigationActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectMitigationActionsTaskSummaryTypeDef = TypedDict(
     "DetectMitigationActionsTaskSummaryTypeDef",
     {
         "taskId": str,
@@ -10797,15 +9810,15 @@
 )
 
 ListAuditSuppressionsResponseTypeDef = TypedDict(
     "ListAuditSuppressionsResponseTypeDef",
     {
         "suppressions": List[AuditSuppressionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuditFindingTypeDef = TypedDict(
     "AuditFindingTypeDef",
     {
         "findingId": str,
@@ -10824,52 +9837,52 @@
 )
 
 ListRelatedResourcesForAuditFindingResponseTypeDef = TypedDict(
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     {
         "relatedResources": List[RelatedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestAuthorizationResponseTypeDef = TypedDict(
     "TestAuthorizationResponseTypeDef",
     {
         "authResults": List[AuthResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
-        "dynamoDB": DynamoDBActionOutputTypeDef,
-        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
-        "lambda": LambdaActionOutputTypeDef,
-        "sns": SnsActionOutputTypeDef,
-        "sqs": SqsActionOutputTypeDef,
-        "kinesis": KinesisActionOutputTypeDef,
+        "dynamoDB": DynamoDBActionTypeDef,
+        "dynamoDBv2": DynamoDBv2ActionTypeDef,
+        "lambda": LambdaActionTypeDef,
+        "sns": SnsActionTypeDef,
+        "sqs": SqsActionTypeDef,
+        "kinesis": KinesisActionTypeDef,
         "republish": RepublishActionOutputTypeDef,
-        "s3": S3ActionOutputTypeDef,
-        "firehose": FirehoseActionOutputTypeDef,
-        "cloudwatchMetric": CloudwatchMetricActionOutputTypeDef,
-        "cloudwatchAlarm": CloudwatchAlarmActionOutputTypeDef,
-        "cloudwatchLogs": CloudwatchLogsActionOutputTypeDef,
-        "elasticsearch": ElasticsearchActionOutputTypeDef,
-        "salesforce": SalesforceActionOutputTypeDef,
-        "iotAnalytics": IotAnalyticsActionOutputTypeDef,
-        "iotEvents": IotEventsActionOutputTypeDef,
+        "s3": S3ActionTypeDef,
+        "firehose": FirehoseActionTypeDef,
+        "cloudwatchMetric": CloudwatchMetricActionTypeDef,
+        "cloudwatchAlarm": CloudwatchAlarmActionTypeDef,
+        "cloudwatchLogs": CloudwatchLogsActionTypeDef,
+        "elasticsearch": ElasticsearchActionTypeDef,
+        "salesforce": SalesforceActionTypeDef,
+        "iotAnalytics": IotAnalyticsActionTypeDef,
+        "iotEvents": IotEventsActionTypeDef,
         "iotSiteWise": IotSiteWiseActionOutputTypeDef,
-        "stepFunctions": StepFunctionsActionOutputTypeDef,
+        "stepFunctions": StepFunctionsActionTypeDef,
         "timestream": TimestreamActionOutputTypeDef,
         "http": HttpActionOutputTypeDef,
         "kafka": KafkaActionOutputTypeDef,
-        "openSearch": OpenSearchActionOutputTypeDef,
-        "location": LocationActionOutputTypeDef,
+        "openSearch": OpenSearchActionTypeDef,
+        "location": LocationActionTypeDef,
     },
     total=False,
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
@@ -10901,34 +9914,34 @@
 )
 
 ListActiveViolationsResponseTypeDef = TypedDict(
     "ListActiveViolationsResponseTypeDef",
     {
         "activeViolations": List[ActiveViolationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListViolationEventsResponseTypeDef = TypedDict(
     "ListViolationEventsResponseTypeDef",
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OTAUpdateFileOutputTypeDef = TypedDict(
     "OTAUpdateFileOutputTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
-        "fileLocation": FileLocationOutputTypeDef,
+        "fileLocation": FileLocationTypeDef,
         "codeSigning": CodeSigningOutputTypeDef,
         "attributes": Dict[str, str],
     },
     total=False,
 )
 
 OTAUpdateFileTypeDef = TypedDict(
@@ -10945,49 +9958,49 @@
 )
 
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "documentSource": str,
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDetectMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     {
         "taskSummary": DetectMitigationActionsTaskSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDetectMitigationActionsTasksResponseTypeDef = TypedDict(
     "ListDetectMitigationActionsTasksResponseTypeDef",
     {
         "tasks": List[DetectMitigationActionsTaskSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAuditFindingResponseTypeDef = TypedDict(
     "DescribeAuditFindingResponseTypeDef",
     {
         "finding": AuditFindingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditFindingsResponseTypeDef = TypedDict(
     "ListAuditFindingsResponseTypeDef",
     {
         "findings": List[AuditFindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TopicRuleTypeDef = TypedDict(
     "TopicRuleTypeDef",
     {
         "ruleName": str,
@@ -11031,16 +10044,16 @@
         "otaUpdateId": str,
         "otaUpdateArn": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "description": str,
         "targets": List[str],
         "protocols": List[ProtocolType],
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigOutputTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigOutputTypeDef,
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
         "targetSelection": TargetSelectionType,
         "otaUpdateFiles": List[OTAUpdateFileOutputTypeDef],
         "otaUpdateStatus": OTAUpdateStatusType,
         "awsIotJobId": str,
         "awsIotJobArn": str,
         "errorInfo": ErrorInfoTypeDef,
         "additionalParameters": Dict[str, str],
@@ -11081,15 +10094,15 @@
 
 
 GetTopicRuleResponseTypeDef = TypedDict(
     "GetTopicRuleResponseTypeDef",
     {
         "ruleArn": str,
         "rule": TopicRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateTopicRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
@@ -11119,10 +10132,10 @@
     },
 )
 
 GetOTAUpdateResponseTypeDef = TypedDict(
     "GetOTAUpdateResponseTypeDef",
     {
         "otaUpdateInfo": OTAUpdateInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot/type_defs.pyi` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for iot service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_iot.type_defs import AbortCriteriaOutputTypeDef
+    from mypy_boto3_iot.type_defs import AbortCriteriaTypeDef
 
-    data: AbortCriteriaOutputTypeDef = {...}
+    data: AbortCriteriaTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from botocore.response import StreamingBody
@@ -88,167 +88,110 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AbortCriteriaOutputTypeDef",
     "AbortCriteriaTypeDef",
     "AcceptCertificateTransferRequestRequestTypeDef",
-    "CloudwatchAlarmActionOutputTypeDef",
-    "CloudwatchLogsActionOutputTypeDef",
-    "CloudwatchMetricActionOutputTypeDef",
-    "DynamoDBActionOutputTypeDef",
-    "ElasticsearchActionOutputTypeDef",
-    "FirehoseActionOutputTypeDef",
-    "IotAnalyticsActionOutputTypeDef",
-    "IotEventsActionOutputTypeDef",
-    "KafkaActionOutputTypeDef",
-    "KinesisActionOutputTypeDef",
-    "LambdaActionOutputTypeDef",
-    "OpenSearchActionOutputTypeDef",
-    "S3ActionOutputTypeDef",
-    "SalesforceActionOutputTypeDef",
-    "SnsActionOutputTypeDef",
-    "SqsActionOutputTypeDef",
-    "StepFunctionsActionOutputTypeDef",
     "CloudwatchAlarmActionTypeDef",
     "CloudwatchLogsActionTypeDef",
     "CloudwatchMetricActionTypeDef",
     "DynamoDBActionTypeDef",
     "ElasticsearchActionTypeDef",
     "FirehoseActionTypeDef",
     "IotAnalyticsActionTypeDef",
     "IotEventsActionTypeDef",
-    "KafkaActionTypeDef",
+    "KafkaActionOutputTypeDef",
     "KinesisActionTypeDef",
     "LambdaActionTypeDef",
     "OpenSearchActionTypeDef",
     "S3ActionTypeDef",
     "SalesforceActionTypeDef",
     "SnsActionTypeDef",
     "SqsActionTypeDef",
     "StepFunctionsActionTypeDef",
+    "KafkaActionTypeDef",
     "MetricValueOutputTypeDef",
     "ViolationEventAdditionalInfoTypeDef",
     "AddThingToBillingGroupRequestRequestTypeDef",
     "AddThingToThingGroupRequestRequestTypeDef",
     "AddThingsToThingGroupParamsOutputTypeDef",
     "AddThingsToThingGroupParamsTypeDef",
     "AggregationTypeOutputTypeDef",
     "AggregationTypeTypeDef",
-    "AlertTargetOutputTypeDef",
     "AlertTargetTypeDef",
     "PolicyTypeDef",
-    "AssetPropertyTimestampOutputTypeDef",
     "AssetPropertyTimestampTypeDef",
-    "AssetPropertyVariantOutputTypeDef",
     "AssetPropertyVariantTypeDef",
     "AssociateTargetsWithJobRequestRequestTypeDef",
-    "AssociateTargetsWithJobResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AttachPolicyRequestRequestTypeDef",
     "AttachPrincipalPolicyRequestRequestTypeDef",
     "AttachSecurityProfileRequestRequestTypeDef",
     "AttachThingPrincipalRequestRequestTypeDef",
     "AttributePayloadOutputTypeDef",
     "AttributePayloadTypeDef",
-    "AuditCheckConfigurationOutputTypeDef",
     "AuditCheckConfigurationTypeDef",
     "AuditCheckDetailsTypeDef",
     "AuditMitigationActionExecutionMetadataTypeDef",
     "AuditMitigationActionsTaskMetadataTypeDef",
     "AuditMitigationActionsTaskTargetOutputTypeDef",
     "AuditMitigationActionsTaskTargetTypeDef",
-    "AuditNotificationTargetOutputTypeDef",
     "AuditNotificationTargetTypeDef",
     "AuditTaskMetadataTypeDef",
     "AuthInfoOutputTypeDef",
     "AuthInfoTypeDef",
-    "AuthorizerConfigOutputTypeDef",
     "AuthorizerConfigTypeDef",
     "AuthorizerDescriptionTypeDef",
     "AuthorizerSummaryTypeDef",
     "AwsJobAbortCriteriaTypeDef",
-    "AwsJobRateIncreaseCriteriaOutputTypeDef",
     "AwsJobRateIncreaseCriteriaTypeDef",
-    "AwsJobPresignedUrlConfigOutputTypeDef",
     "AwsJobPresignedUrlConfigTypeDef",
     "AwsJobTimeoutConfigTypeDef",
-    "MachineLearningDetectionConfigOutputTypeDef",
-    "StatisticalThresholdOutputTypeDef",
     "MachineLearningDetectionConfigTypeDef",
-    "MetricValueTypeDef",
     "StatisticalThresholdTypeDef",
+    "MetricValueTypeDef",
     "BehaviorModelTrainingSummaryTypeDef",
-    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "BillingGroupMetadataTypeDef",
-    "BillingGroupPropertiesOutputTypeDef",
     "BillingGroupPropertiesTypeDef",
     "BucketTypeDef",
     "TermsAggregationTypeDef",
     "CertificateValidityTypeDef",
     "CACertificateTypeDef",
     "CancelAuditMitigationActionsTaskRequestRequestTypeDef",
     "CancelAuditTaskRequestRequestTypeDef",
     "CancelCertificateTransferRequestRequestTypeDef",
     "CancelDetectMitigationActionsTaskRequestRequestTypeDef",
     "CancelJobExecutionRequestRequestTypeDef",
     "CancelJobRequestRequestTypeDef",
-    "CancelJobResponseTypeDef",
     "TransferDataTypeDef",
     "CertificateTypeDef",
-    "CodeSigningCertificateChainOutputTypeDef",
     "CodeSigningCertificateChainTypeDef",
     "CodeSigningSignatureOutputTypeDef",
     "CodeSigningSignatureTypeDef",
-    "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "ConfirmTopicRuleDestinationRequestRequestTypeDef",
     "TagTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "CreateBillingGroupResponseTypeDef",
     "CreateCertificateFromCsrRequestRequestTypeDef",
-    "CreateCertificateFromCsrResponseTypeDef",
-    "CreateCustomMetricResponseTypeDef",
-    "CreateDimensionResponseTypeDef",
     "TlsConfigTypeDef",
-    "CreateDomainConfigurationResponseTypeDef",
-    "CreateDynamicThingGroupResponseTypeDef",
-    "CreateFleetMetricResponseTypeDef",
     "PresignedUrlConfigTypeDef",
     "TimeoutConfigTypeDef",
-    "CreateJobResponseTypeDef",
     "MaintenanceWindowTypeDef",
-    "CreateJobTemplateResponseTypeDef",
     "CreateKeysAndCertificateRequestRequestTypeDef",
     "KeyPairTypeDef",
-    "CreateMitigationActionResponseTypeDef",
-    "CreateOTAUpdateResponseTypeDef",
     "CreatePackageRequestRequestTypeDef",
-    "CreatePackageResponseTypeDef",
     "CreatePackageVersionRequestRequestTypeDef",
-    "CreatePackageVersionResponseTypeDef",
-    "CreatePolicyResponseTypeDef",
     "CreatePolicyVersionRequestRequestTypeDef",
-    "CreatePolicyVersionResponseTypeDef",
     "CreateProvisioningClaimRequestRequestTypeDef",
     "ProvisioningHookTypeDef",
-    "CreateProvisioningTemplateResponseTypeDef",
     "CreateProvisioningTemplateVersionRequestRequestTypeDef",
-    "CreateProvisioningTemplateVersionResponseTypeDef",
-    "CreateRoleAliasResponseTypeDef",
-    "CreateScheduledAuditResponseTypeDef",
-    "CreateSecurityProfileResponseTypeDef",
-    "CreateStreamResponseTypeDef",
-    "CreateThingGroupResponseTypeDef",
-    "CreateThingResponseTypeDef",
     "ThingTypePropertiesTypeDef",
-    "CreateThingTypeResponseTypeDef",
     "DeleteAccountAuditConfigurationRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteBillingGroupRequestRequestTypeDef",
     "DeleteCACertificateRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
     "DeleteCustomMetricRequestRequestTypeDef",
     "DeleteDimensionRequestRequestTypeDef",
@@ -281,371 +224,309 @@
     "DescribeAuditMitigationActionsTaskRequestRequestTypeDef",
     "TaskStatisticsForAuditCheckTypeDef",
     "DescribeAuditTaskRequestRequestTypeDef",
     "TaskStatisticsTypeDef",
     "DescribeAuthorizerRequestRequestTypeDef",
     "DescribeBillingGroupRequestRequestTypeDef",
     "DescribeCACertificateRequestRequestTypeDef",
-    "RegistrationConfigOutputTypeDef",
+    "RegistrationConfigTypeDef",
     "DescribeCertificateRequestRequestTypeDef",
     "DescribeCustomMetricRequestRequestTypeDef",
-    "DescribeCustomMetricResponseTypeDef",
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     "DescribeDimensionRequestRequestTypeDef",
-    "DescribeDimensionResponseTypeDef",
     "DescribeDomainConfigurationRequestRequestTypeDef",
     "ServerCertificateSummaryTypeDef",
-    "TlsConfigOutputTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
-    "DescribeEndpointResponseTypeDef",
     "DescribeFleetMetricRequestRequestTypeDef",
     "DescribeIndexRequestRequestTypeDef",
-    "DescribeIndexResponseTypeDef",
     "DescribeJobExecutionRequestRequestTypeDef",
     "DescribeJobRequestRequestTypeDef",
     "DescribeJobTemplateRequestRequestTypeDef",
-    "MaintenanceWindowOutputTypeDef",
-    "PresignedUrlConfigOutputTypeDef",
-    "TimeoutConfigOutputTypeDef",
     "DescribeManagedJobTemplateRequestRequestTypeDef",
     "DocumentParameterTypeDef",
     "DescribeMitigationActionRequestRequestTypeDef",
     "DescribeProvisioningTemplateRequestRequestTypeDef",
-    "ProvisioningHookOutputTypeDef",
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
-    "DescribeProvisioningTemplateVersionResponseTypeDef",
     "DescribeRoleAliasRequestRequestTypeDef",
     "RoleAliasDescriptionTypeDef",
     "DescribeScheduledAuditRequestRequestTypeDef",
-    "DescribeScheduledAuditResponseTypeDef",
     "DescribeSecurityProfileRequestRequestTypeDef",
     "DescribeStreamRequestRequestTypeDef",
     "DescribeThingGroupRequestRequestTypeDef",
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
-    "DescribeThingRegistrationTaskResponseTypeDef",
     "DescribeThingRequestRequestTypeDef",
-    "DescribeThingResponseTypeDef",
     "DescribeThingTypeRequestRequestTypeDef",
     "ThingTypeMetadataTypeDef",
     "ThingTypePropertiesOutputTypeDef",
-    "S3DestinationOutputTypeDef",
     "S3DestinationTypeDef",
     "DetachPolicyRequestRequestTypeDef",
     "DetachPrincipalPolicyRequestRequestTypeDef",
     "DetachSecurityProfileRequestRequestTypeDef",
     "DetachThingPrincipalRequestRequestTypeDef",
     "DetectMitigationActionExecutionTypeDef",
     "DetectMitigationActionsTaskStatisticsTypeDef",
     "DetectMitigationActionsTaskTargetOutputTypeDef",
     "ViolationEventOccurrenceRangeOutputTypeDef",
     "DetectMitigationActionsTaskTargetTypeDef",
     "DisableTopicRuleRequestRequestTypeDef",
     "DomainConfigurationSummaryTypeDef",
-    "PutItemInputOutputTypeDef",
     "PutItemInputTypeDef",
     "EffectivePolicyTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "EnableIoTLoggingParamsOutputTypeDef",
     "EnableIoTLoggingParamsTypeDef",
     "EnableTopicRuleRequestRequestTypeDef",
     "ErrorInfoTypeDef",
-    "RateIncreaseCriteriaOutputTypeDef",
     "RateIncreaseCriteriaTypeDef",
-    "FieldOutputTypeDef",
     "FieldTypeDef",
-    "S3LocationOutputTypeDef",
-    "StreamOutputTypeDef",
     "S3LocationTypeDef",
     "StreamTypeDef",
     "FleetMetricNameAndArnTypeDef",
-    "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     "GetCardinalityRequestRequestTypeDef",
-    "GetCardinalityResponseTypeDef",
     "GetEffectivePoliciesRequestRequestTypeDef",
     "GetJobDocumentRequestRequestTypeDef",
-    "GetJobDocumentResponseTypeDef",
-    "GetLoggingOptionsResponseTypeDef",
     "GetOTAUpdateRequestRequestTypeDef",
-    "VersionUpdateByJobsConfigOutputTypeDef",
+    "VersionUpdateByJobsConfigTypeDef",
     "GetPackageRequestRequestTypeDef",
-    "GetPackageResponseTypeDef",
     "GetPackageVersionRequestRequestTypeDef",
-    "GetPackageVersionResponseTypeDef",
     "GetPercentilesRequestRequestTypeDef",
     "PercentPairTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetPolicyResponseTypeDef",
     "GetPolicyVersionRequestRequestTypeDef",
-    "GetPolicyVersionResponseTypeDef",
-    "GetRegistrationCodeResponseTypeDef",
     "GetStatisticsRequestRequestTypeDef",
     "StatisticsTypeDef",
     "GetTopicRuleDestinationRequestRequestTypeDef",
     "GetTopicRuleRequestRequestTypeDef",
-    "GetV2LoggingOptionsResponseTypeDef",
     "GroupNameAndArnTypeDef",
-    "HttpActionHeaderOutputTypeDef",
     "HttpActionHeaderTypeDef",
-    "SigV4AuthorizationOutputTypeDef",
     "SigV4AuthorizationTypeDef",
     "HttpContextTypeDef",
     "HttpUrlDestinationConfigurationTypeDef",
     "HttpUrlDestinationPropertiesTypeDef",
     "HttpUrlDestinationSummaryTypeDef",
     "IndexingFilterOutputTypeDef",
     "IndexingFilterTypeDef",
-    "IssuerCertificateIdentifierOutputTypeDef",
     "IssuerCertificateIdentifierTypeDef",
     "JobExecutionStatusDetailsTypeDef",
     "JobExecutionSummaryTypeDef",
-    "RetryCriteriaOutputTypeDef",
     "RetryCriteriaTypeDef",
     "JobProcessDetailsTypeDef",
     "JobSummaryTypeDef",
     "JobTemplateSummaryTypeDef",
     "ScheduledJobRolloutTypeDef",
-    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
     "ListActiveViolationsRequestRequestTypeDef",
-    "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
     "ListAttachedPoliciesRequestRequestTypeDef",
-    "ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
     "ListAuditMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
     "ListAuditMitigationActionsTasksRequestRequestTypeDef",
-    "ListAuditTasksRequestListAuditTasksPaginateTypeDef",
     "ListAuditTasksRequestRequestTypeDef",
-    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
     "ListAuthorizersRequestRequestTypeDef",
-    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
     "ListBillingGroupsRequestRequestTypeDef",
-    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
     "ListCACertificatesRequestRequestTypeDef",
-    "ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
     "ListCertificatesByCARequestRequestTypeDef",
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
     "ListCertificatesRequestRequestTypeDef",
-    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
     "ListCustomMetricsRequestRequestTypeDef",
-    "ListCustomMetricsResponseTypeDef",
-    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
     "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
-    "ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
     "ListDetectMitigationActionsTasksRequestRequestTypeDef",
-    "ListDimensionsRequestListDimensionsPaginateTypeDef",
     "ListDimensionsRequestRequestTypeDef",
-    "ListDimensionsResponseTypeDef",
-    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
     "ListDomainConfigurationsRequestRequestTypeDef",
-    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
     "ListFleetMetricsRequestRequestTypeDef",
-    "ListIndicesRequestListIndicesPaginateTypeDef",
     "ListIndicesRequestRequestTypeDef",
-    "ListIndicesResponseTypeDef",
-    "ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
     "ListJobExecutionsForJobRequestRequestTypeDef",
-    "ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
     "ListJobExecutionsForThingRequestRequestTypeDef",
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobTemplatesRequestRequestTypeDef",
-    "ListJobsRequestListJobsPaginateTypeDef",
     "ListJobsRequestRequestTypeDef",
-    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
     "ListManagedJobTemplatesRequestRequestTypeDef",
     "ManagedJobTemplateSummaryTypeDef",
-    "ListMetricValuesRequestListMetricValuesPaginateTypeDef",
     "ListMetricValuesRequestRequestTypeDef",
-    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
     "ListMitigationActionsRequestRequestTypeDef",
     "MitigationActionIdentifierTypeDef",
-    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
     "ListOTAUpdatesRequestRequestTypeDef",
     "OTAUpdateSummaryTypeDef",
-    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
     "ListOutgoingCertificatesRequestRequestTypeDef",
     "OutgoingCertificateTypeDef",
-    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
     "ListPackageVersionsRequestRequestTypeDef",
     "PackageVersionSummaryTypeDef",
-    "ListPackagesRequestListPackagesPaginateTypeDef",
     "ListPackagesRequestRequestTypeDef",
     "PackageSummaryTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
-    "ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
     "ListPolicyPrincipalsRequestRequestTypeDef",
-    "ListPolicyPrincipalsResponseTypeDef",
     "ListPolicyVersionsRequestRequestTypeDef",
     "PolicyVersionTypeDef",
-    "ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
     "ListPrincipalPoliciesRequestRequestTypeDef",
-    "ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
     "ListPrincipalThingsRequestRequestTypeDef",
-    "ListPrincipalThingsResponseTypeDef",
-    "ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
     "ListProvisioningTemplateVersionsRequestRequestTypeDef",
     "ProvisioningTemplateVersionSummaryTypeDef",
-    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
     "ListProvisioningTemplatesRequestRequestTypeDef",
     "ProvisioningTemplateSummaryTypeDef",
-    "ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
     "ListRelatedResourcesForAuditFindingRequestRequestTypeDef",
-    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
     "ListRoleAliasesRequestRequestTypeDef",
-    "ListRoleAliasesResponseTypeDef",
-    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
     "ListScheduledAuditsRequestRequestTypeDef",
     "ScheduledAuditMetadataTypeDef",
-    "ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
     "ListSecurityProfilesForTargetRequestRequestTypeDef",
-    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
     "ListSecurityProfilesRequestRequestTypeDef",
     "SecurityProfileIdentifierTypeDef",
-    "ListStreamsRequestListStreamsPaginateTypeDef",
     "ListStreamsRequestRequestTypeDef",
     "StreamSummaryTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "TagOutputTypeDef",
-    "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
     "ListTargetsForPolicyRequestRequestTypeDef",
-    "ListTargetsForPolicyResponseTypeDef",
-    "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
     "ListTargetsForSecurityProfileRequestRequestTypeDef",
     "SecurityProfileTargetTypeDef",
-    "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
     "ListThingGroupsForThingRequestRequestTypeDef",
-    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
     "ListThingGroupsRequestRequestTypeDef",
-    "ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
     "ListThingPrincipalsRequestRequestTypeDef",
-    "ListThingPrincipalsResponseTypeDef",
-    "ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
     "ListThingRegistrationTaskReportsRequestRequestTypeDef",
-    "ListThingRegistrationTaskReportsResponseTypeDef",
-    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
     "ListThingRegistrationTasksRequestRequestTypeDef",
-    "ListThingRegistrationTasksResponseTypeDef",
-    "ListThingTypesRequestListThingTypesPaginateTypeDef",
     "ListThingTypesRequestRequestTypeDef",
-    "ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
     "ListThingsInBillingGroupRequestRequestTypeDef",
-    "ListThingsInBillingGroupResponseTypeDef",
-    "ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
     "ListThingsInThingGroupRequestRequestTypeDef",
-    "ListThingsInThingGroupResponseTypeDef",
-    "ListThingsRequestListThingsPaginateTypeDef",
     "ListThingsRequestRequestTypeDef",
     "ThingAttributeTypeDef",
-    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
     "ListTopicRuleDestinationsRequestRequestTypeDef",
-    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
     "ListTopicRulesRequestRequestTypeDef",
     "TopicRuleListItemTypeDef",
-    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
     "ListV2LoggingLevelsRequestRequestTypeDef",
-    "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
     "ListViolationEventsRequestRequestTypeDef",
-    "LocationTimestampOutputTypeDef",
     "LocationTimestampTypeDef",
-    "LogTargetOutputTypeDef",
     "LogTargetTypeDef",
     "LoggingOptionsPayloadTypeDef",
-    "PublishFindingToSnsParamsOutputTypeDef",
-    "ReplaceDefaultPolicyVersionParamsOutputTypeDef",
-    "UpdateCACertificateParamsOutputTypeDef",
-    "UpdateDeviceCertificateParamsOutputTypeDef",
     "PublishFindingToSnsParamsTypeDef",
     "ReplaceDefaultPolicyVersionParamsTypeDef",
     "UpdateCACertificateParamsTypeDef",
     "UpdateDeviceCertificateParamsTypeDef",
     "MqttContextTypeDef",
-    "UserPropertyOutputTypeDef",
     "UserPropertyTypeDef",
-    "PaginatorConfigTypeDef",
-    "PolicyVersionIdentifierOutputTypeDef",
     "PolicyVersionIdentifierTypeDef",
     "PutVerificationStateOnViolationRequestRequestTypeDef",
-    "RegistrationConfigTypeDef",
-    "RegisterCACertificateResponseTypeDef",
     "RegisterCertificateRequestRequestTypeDef",
-    "RegisterCertificateResponseTypeDef",
     "RegisterCertificateWithoutCARequestRequestTypeDef",
-    "RegisterCertificateWithoutCAResponseTypeDef",
     "RegisterThingRequestRequestTypeDef",
-    "RegisterThingResponseTypeDef",
     "RejectCertificateTransferRequestRequestTypeDef",
     "RemoveThingFromBillingGroupRequestRequestTypeDef",
     "RemoveThingFromThingGroupRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchIndexRequestRequestTypeDef",
     "ThingGroupDocumentTypeDef",
     "SetDefaultAuthorizerRequestRequestTypeDef",
-    "SetDefaultAuthorizerResponseTypeDef",
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     "SetV2LoggingOptionsRequestRequestTypeDef",
-    "SigningProfileParameterOutputTypeDef",
     "SigningProfileParameterTypeDef",
-    "StartAuditMitigationActionsTaskResponseTypeDef",
     "ViolationEventOccurrenceRangeTypeDef",
-    "StartDetectMitigationActionsTaskResponseTypeDef",
     "StartOnDemandAuditTaskRequestRequestTypeDef",
-    "StartOnDemandAuditTaskResponseTypeDef",
     "StartThingRegistrationTaskRequestRequestTypeDef",
-    "StartThingRegistrationTaskResponseTypeDef",
     "StopThingRegistrationTaskRequestRequestTypeDef",
     "TlsContextTypeDef",
-    "TestInvokeAuthorizerResponseTypeDef",
     "ThingConnectivityTypeDef",
-    "TimestreamDimensionOutputTypeDef",
-    "TimestreamTimestampOutputTypeDef",
     "TimestreamDimensionTypeDef",
     "TimestreamTimestampTypeDef",
     "VpcDestinationConfigurationTypeDef",
     "VpcDestinationSummaryTypeDef",
     "VpcDestinationPropertiesTypeDef",
     "TransferCertificateRequestRequestTypeDef",
-    "TransferCertificateResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "UpdateAuthorizerResponseTypeDef",
-    "UpdateBillingGroupResponseTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
     "UpdateCustomMetricRequestRequestTypeDef",
-    "UpdateCustomMetricResponseTypeDef",
     "UpdateDimensionRequestRequestTypeDef",
-    "UpdateDimensionResponseTypeDef",
-    "UpdateDomainConfigurationResponseTypeDef",
-    "UpdateDynamicThingGroupResponseTypeDef",
-    "UpdateMitigationActionResponseTypeDef",
-    "VersionUpdateByJobsConfigTypeDef",
     "UpdatePackageRequestRequestTypeDef",
     "UpdatePackageVersionRequestRequestTypeDef",
     "UpdateRoleAliasRequestRequestTypeDef",
-    "UpdateRoleAliasResponseTypeDef",
     "UpdateScheduledAuditRequestRequestTypeDef",
-    "UpdateScheduledAuditResponseTypeDef",
-    "UpdateStreamResponseTypeDef",
-    "UpdateThingGroupResponseTypeDef",
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     "UpdateTopicRuleDestinationRequestRequestTypeDef",
     "ValidationErrorTypeDef",
     "AbortConfigOutputTypeDef",
     "AbortConfigTypeDef",
     "MetricDatumTypeDef",
-    "DescribeFleetMetricResponseTypeDef",
     "UpdateFleetMetricRequestRequestTypeDef",
     "AllowedTypeDef",
     "ExplicitDenyTypeDef",
     "ImplicitDenyTypeDef",
+    "AssetPropertyValueTypeDef",
+    "AssociateTargetsWithJobResponseTypeDef",
+    "CancelJobResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateBillingGroupResponseTypeDef",
+    "CreateCertificateFromCsrResponseTypeDef",
+    "CreateCustomMetricResponseTypeDef",
+    "CreateDimensionResponseTypeDef",
+    "CreateDomainConfigurationResponseTypeDef",
+    "CreateDynamicThingGroupResponseTypeDef",
+    "CreateFleetMetricResponseTypeDef",
+    "CreateJobResponseTypeDef",
+    "CreateJobTemplateResponseTypeDef",
+    "CreateMitigationActionResponseTypeDef",
+    "CreateOTAUpdateResponseTypeDef",
+    "CreatePackageResponseTypeDef",
+    "CreatePackageVersionResponseTypeDef",
+    "CreatePolicyResponseTypeDef",
+    "CreatePolicyVersionResponseTypeDef",
+    "CreateProvisioningTemplateResponseTypeDef",
+    "CreateProvisioningTemplateVersionResponseTypeDef",
+    "CreateRoleAliasResponseTypeDef",
+    "CreateScheduledAuditResponseTypeDef",
+    "CreateSecurityProfileResponseTypeDef",
+    "CreateStreamResponseTypeDef",
+    "CreateThingGroupResponseTypeDef",
+    "CreateThingResponseTypeDef",
+    "CreateThingTypeResponseTypeDef",
+    "DescribeCustomMetricResponseTypeDef",
+    "DescribeDimensionResponseTypeDef",
+    "DescribeEndpointResponseTypeDef",
+    "DescribeFleetMetricResponseTypeDef",
+    "DescribeIndexResponseTypeDef",
+    "DescribeProvisioningTemplateVersionResponseTypeDef",
+    "DescribeScheduledAuditResponseTypeDef",
+    "DescribeThingRegistrationTaskResponseTypeDef",
+    "DescribeThingResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCardinalityResponseTypeDef",
+    "GetJobDocumentResponseTypeDef",
+    "GetLoggingOptionsResponseTypeDef",
+    "GetPackageResponseTypeDef",
+    "GetPackageVersionResponseTypeDef",
+    "GetPolicyResponseTypeDef",
+    "GetPolicyVersionResponseTypeDef",
+    "GetRegistrationCodeResponseTypeDef",
+    "GetV2LoggingOptionsResponseTypeDef",
     "ListAttachedPoliciesResponseTypeDef",
+    "ListCustomMetricsResponseTypeDef",
+    "ListDimensionsResponseTypeDef",
+    "ListIndicesResponseTypeDef",
     "ListPoliciesResponseTypeDef",
+    "ListPolicyPrincipalsResponseTypeDef",
     "ListPrincipalPoliciesResponseTypeDef",
-    "AssetPropertyValueOutputTypeDef",
-    "AssetPropertyValueTypeDef",
+    "ListPrincipalThingsResponseTypeDef",
+    "ListRoleAliasesResponseTypeDef",
+    "ListTargetsForPolicyResponseTypeDef",
+    "ListThingPrincipalsResponseTypeDef",
+    "ListThingRegistrationTaskReportsResponseTypeDef",
+    "ListThingRegistrationTasksResponseTypeDef",
+    "ListThingsInBillingGroupResponseTypeDef",
+    "ListThingsInThingGroupResponseTypeDef",
+    "RegisterCACertificateResponseTypeDef",
+    "RegisterCertificateResponseTypeDef",
+    "RegisterCertificateWithoutCAResponseTypeDef",
+    "RegisterThingResponseTypeDef",
+    "SetDefaultAuthorizerResponseTypeDef",
+    "StartAuditMitigationActionsTaskResponseTypeDef",
+    "StartDetectMitigationActionsTaskResponseTypeDef",
+    "StartOnDemandAuditTaskResponseTypeDef",
+    "StartThingRegistrationTaskResponseTypeDef",
+    "TestInvokeAuthorizerResponseTypeDef",
+    "TransferCertificateResponseTypeDef",
+    "UpdateAuthorizerResponseTypeDef",
+    "UpdateBillingGroupResponseTypeDef",
+    "UpdateCustomMetricResponseTypeDef",
+    "UpdateDimensionResponseTypeDef",
+    "UpdateDomainConfigurationResponseTypeDef",
+    "UpdateDynamicThingGroupResponseTypeDef",
+    "UpdateMitigationActionResponseTypeDef",
+    "UpdateRoleAliasResponseTypeDef",
+    "UpdateScheduledAuditResponseTypeDef",
+    "UpdateStreamResponseTypeDef",
+    "UpdateThingGroupResponseTypeDef",
     "ThingGroupPropertiesOutputTypeDef",
     "CreateThingRequestRequestTypeDef",
     "ThingGroupPropertiesTypeDef",
     "UpdateThingRequestRequestTypeDef",
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     "ListAuditMitigationActionsTasksResponseTypeDef",
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
@@ -653,20 +534,18 @@
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     "ListAuditTasksResponseTypeDef",
     "TestAuthorizationRequestRequestTypeDef",
     "DescribeAuthorizerResponseTypeDef",
     "DescribeDefaultAuthorizerResponseTypeDef",
     "ListAuthorizersResponseTypeDef",
     "AwsJobAbortConfigTypeDef",
-    "AwsJobExponentialRolloutRateOutputTypeDef",
     "AwsJobExponentialRolloutRateTypeDef",
     "BehaviorCriteriaOutputTypeDef",
     "BehaviorCriteriaTypeDef",
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
-    "MetricToRetainOutputTypeDef",
     "MetricToRetainTypeDef",
     "DescribeBillingGroupResponseTypeDef",
     "UpdateBillingGroupRequestRequestTypeDef",
     "GetBucketsAggregationResponseTypeDef",
     "BucketsAggregationTypeTypeDef",
     "CACertificateDescriptionTypeDef",
     "ListCACertificatesResponseTypeDef",
@@ -681,55 +560,110 @@
     "CreateBillingGroupRequestRequestTypeDef",
     "CreateCustomMetricRequestRequestTypeDef",
     "CreateDimensionRequestRequestTypeDef",
     "CreateFleetMetricRequestRequestTypeDef",
     "CreatePolicyRequestRequestTypeDef",
     "CreateRoleAliasRequestRequestTypeDef",
     "CreateScheduledAuditRequestRequestTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDomainConfigurationRequestRequestTypeDef",
     "UpdateDomainConfigurationRequestRequestTypeDef",
+    "SchedulingConfigOutputTypeDef",
     "SchedulingConfigTypeDef",
     "CreateKeysAndCertificateResponseTypeDef",
     "CreateProvisioningClaimResponseTypeDef",
     "CreateProvisioningTemplateRequestRequestTypeDef",
+    "DescribeProvisioningTemplateResponseTypeDef",
     "UpdateProvisioningTemplateRequestRequestTypeDef",
     "CreateThingTypeRequestRequestTypeDef",
     "DescribeAuditTaskResponseTypeDef",
+    "RegisterCACertificateRequestRequestTypeDef",
+    "UpdateCACertificateRequestRequestTypeDef",
     "DescribeDomainConfigurationResponseTypeDef",
-    "SchedulingConfigOutputTypeDef",
     "DescribeManagedJobTemplateResponseTypeDef",
-    "DescribeProvisioningTemplateResponseTypeDef",
     "DescribeRoleAliasResponseTypeDef",
     "DescribeThingTypeResponseTypeDef",
     "ThingTypeDefinitionTypeDef",
-    "DestinationOutputTypeDef",
     "DestinationTypeDef",
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
     "ListDomainConfigurationsResponseTypeDef",
-    "DynamoDBv2ActionOutputTypeDef",
     "DynamoDBv2ActionTypeDef",
     "GetEffectivePoliciesResponseTypeDef",
-    "ExponentialRolloutRateOutputTypeDef",
     "ExponentialRolloutRateTypeDef",
     "ThingGroupIndexingConfigurationOutputTypeDef",
     "ThingGroupIndexingConfigurationTypeDef",
-    "StreamFileOutputTypeDef",
-    "FileLocationOutputTypeDef",
     "StreamFileTypeDef",
     "FileLocationTypeDef",
     "ListFleetMetricsResponseTypeDef",
+    "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
+    "ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    "ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    "ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    "ListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
+    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
+    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
+    "ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
+    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
+    "ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    "ListDimensionsRequestListDimensionsPaginateTypeDef",
+    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
+    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
+    "ListIndicesRequestListIndicesPaginateTypeDef",
+    "ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    "ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    "ListJobsRequestListJobsPaginateTypeDef",
+    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
+    "ListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
+    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
+    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
+    "ListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    "ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    "ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    "ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
+    "ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
+    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
+    "ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
+    "ListStreamsRequestListStreamsPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    "ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+    "ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
+    "ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    "ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
+    "ListThingTypesRequestListThingTypesPaginateTypeDef",
+    "ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    "ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    "ListThingsRequestListThingsPaginateTypeDef",
+    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
+    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
+    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
+    "ListViolationEventsRequestListViolationEventsPaginateTypeDef",
     "GetPackageConfigurationResponseTypeDef",
+    "UpdatePackageConfigurationRequestRequestTypeDef",
     "GetPercentilesResponseTypeDef",
     "GetStatisticsResponseTypeDef",
     "ListBillingGroupsResponseTypeDef",
     "ListThingGroupsForThingResponseTypeDef",
     "ListThingGroupsResponseTypeDef",
     "ThingGroupMetadataTypeDef",
-    "HttpAuthorizationOutputTypeDef",
     "HttpAuthorizationTypeDef",
     "ThingIndexingConfigurationOutputTypeDef",
     "ThingIndexingConfigurationTypeDef",
     "JobExecutionTypeDef",
     "JobExecutionSummaryForJobTypeDef",
     "JobExecutionSummaryForThingTypeDef",
     "JobExecutionsRetryConfigOutputTypeDef",
@@ -744,64 +678,55 @@
     "ListPackagesResponseTypeDef",
     "ListPolicyVersionsResponseTypeDef",
     "ListProvisioningTemplateVersionsResponseTypeDef",
     "ListProvisioningTemplatesResponseTypeDef",
     "ListScheduledAuditsResponseTypeDef",
     "ListSecurityProfilesResponseTypeDef",
     "ListStreamsResponseTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTargetsForSecurityProfileResponseTypeDef",
     "SecurityProfileTargetMappingTypeDef",
     "ListThingsResponseTypeDef",
     "ListTopicRulesResponseTypeDef",
-    "LocationActionOutputTypeDef",
     "LocationActionTypeDef",
     "LogTargetConfigurationTypeDef",
     "SetV2LoggingLevelRequestRequestTypeDef",
     "SetLoggingOptionsRequestRequestTypeDef",
     "MitigationActionParamsOutputTypeDef",
     "MitigationActionParamsTypeDef",
     "MqttHeadersOutputTypeDef",
     "MqttHeadersTypeDef",
-    "ResourceIdentifierOutputTypeDef",
     "ResourceIdentifierTypeDef",
-    "RegisterCACertificateRequestRequestTypeDef",
-    "UpdateCACertificateRequestRequestTypeDef",
     "StartDetectMitigationActionsTaskRequestRequestTypeDef",
     "TestInvokeAuthorizerRequestRequestTypeDef",
     "ThingDocumentTypeDef",
     "TimestreamActionOutputTypeDef",
     "TimestreamActionTypeDef",
     "TopicRuleDestinationConfigurationTypeDef",
     "TopicRuleDestinationSummaryTypeDef",
     "TopicRuleDestinationTypeDef",
-    "UpdatePackageConfigurationRequestRequestTypeDef",
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     "ListMetricValuesResponseTypeDef",
     "DeniedTypeDef",
     "PutAssetPropertyValueEntryOutputTypeDef",
     "PutAssetPropertyValueEntryTypeDef",
     "CreateDynamicThingGroupRequestRequestTypeDef",
     "CreateThingGroupRequestRequestTypeDef",
     "UpdateDynamicThingGroupRequestRequestTypeDef",
     "UpdateThingGroupRequestRequestTypeDef",
-    "AwsJobExecutionsRolloutConfigOutputTypeDef",
     "AwsJobExecutionsRolloutConfigTypeDef",
     "BehaviorOutputTypeDef",
     "BehaviorTypeDef",
     "GetBucketsAggregationRequestRequestTypeDef",
     "DescribeCACertificateResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
     "ListThingTypesResponseTypeDef",
-    "StartSigningJobParameterOutputTypeDef",
     "StartSigningJobParameterTypeDef",
-    "JobExecutionsRolloutConfigOutputTypeDef",
     "JobExecutionsRolloutConfigTypeDef",
-    "StreamInfoTypeDef",
     "CreateStreamRequestRequestTypeDef",
+    "StreamInfoTypeDef",
     "UpdateStreamRequestRequestTypeDef",
     "DescribeThingGroupResponseTypeDef",
     "HttpActionOutputTypeDef",
     "HttpActionTypeDef",
     "GetIndexingConfigurationResponseTypeDef",
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     "DescribeJobExecutionResponseTypeDef",
@@ -812,24 +737,24 @@
     "DescribeMitigationActionResponseTypeDef",
     "MitigationActionTypeDef",
     "CreateMitigationActionRequestRequestTypeDef",
     "UpdateMitigationActionRequestRequestTypeDef",
     "RepublishActionOutputTypeDef",
     "RepublishActionTypeDef",
     "AuditSuppressionTypeDef",
-    "DescribeAuditSuppressionResponseTypeDef",
-    "NonCompliantResourceTypeDef",
-    "RelatedResourceTypeDef",
     "CreateAuditSuppressionRequestRequestTypeDef",
     "DeleteAuditSuppressionRequestRequestTypeDef",
     "DescribeAuditSuppressionRequestRequestTypeDef",
+    "DescribeAuditSuppressionResponseTypeDef",
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     "ListAuditFindingsRequestRequestTypeDef",
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
     "ListAuditSuppressionsRequestRequestTypeDef",
+    "NonCompliantResourceTypeDef",
+    "RelatedResourceTypeDef",
     "UpdateAuditSuppressionRequestRequestTypeDef",
     "SearchIndexResponseTypeDef",
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     "ListTopicRuleDestinationsResponseTypeDef",
     "CreateTopicRuleDestinationResponseTypeDef",
     "GetTopicRuleDestinationResponseTypeDef",
     "AuthResultTypeDef",
@@ -840,18 +765,18 @@
     "UpdateSecurityProfileResponseTypeDef",
     "ViolationEventTypeDef",
     "CreateSecurityProfileRequestRequestTypeDef",
     "UpdateSecurityProfileRequestRequestTypeDef",
     "ValidateSecurityProfileBehaviorsRequestRequestTypeDef",
     "CodeSigningOutputTypeDef",
     "CodeSigningTypeDef",
-    "DescribeJobTemplateResponseTypeDef",
-    "JobTypeDef",
     "CreateJobRequestRequestTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
+    "DescribeJobTemplateResponseTypeDef",
+    "JobTypeDef",
     "UpdateJobRequestRequestTypeDef",
     "DescribeStreamResponseTypeDef",
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     "DetectMitigationActionsTaskSummaryTypeDef",
     "ListAuditSuppressionsResponseTypeDef",
     "AuditFindingTypeDef",
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
@@ -873,24 +798,14 @@
     "CreateOTAUpdateRequestRequestTypeDef",
     "GetTopicRuleResponseTypeDef",
     "CreateTopicRuleRequestRequestTypeDef",
     "ReplaceTopicRuleRequestRequestTypeDef",
     "GetOTAUpdateResponseTypeDef",
 )
 
-AbortCriteriaOutputTypeDef = TypedDict(
-    "AbortCriteriaOutputTypeDef",
-    {
-        "failureType": JobExecutionFailureTypeType,
-        "action": Literal["CANCEL"],
-        "thresholdPercentage": float,
-        "minNumberOfExecutedThings": int,
-    },
-)
-
 AbortCriteriaTypeDef = TypedDict(
     "AbortCriteriaTypeDef",
     {
         "failureType": JobExecutionFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
@@ -913,301 +828,14 @@
 
 class AcceptCertificateTransferRequestRequestTypeDef(
     _RequiredAcceptCertificateTransferRequestRequestTypeDef,
     _OptionalAcceptCertificateTransferRequestRequestTypeDef,
 ):
     pass
 
-CloudwatchAlarmActionOutputTypeDef = TypedDict(
-    "CloudwatchAlarmActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "alarmName": str,
-        "stateReason": str,
-        "stateValue": str,
-    },
-)
-
-_RequiredCloudwatchLogsActionOutputTypeDef = TypedDict(
-    "_RequiredCloudwatchLogsActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "logGroupName": str,
-    },
-)
-_OptionalCloudwatchLogsActionOutputTypeDef = TypedDict(
-    "_OptionalCloudwatchLogsActionOutputTypeDef",
-    {
-        "batchMode": bool,
-    },
-    total=False,
-)
-
-class CloudwatchLogsActionOutputTypeDef(
-    _RequiredCloudwatchLogsActionOutputTypeDef, _OptionalCloudwatchLogsActionOutputTypeDef
-):
-    pass
-
-_RequiredCloudwatchMetricActionOutputTypeDef = TypedDict(
-    "_RequiredCloudwatchMetricActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "metricNamespace": str,
-        "metricName": str,
-        "metricValue": str,
-        "metricUnit": str,
-    },
-)
-_OptionalCloudwatchMetricActionOutputTypeDef = TypedDict(
-    "_OptionalCloudwatchMetricActionOutputTypeDef",
-    {
-        "metricTimestamp": str,
-    },
-    total=False,
-)
-
-class CloudwatchMetricActionOutputTypeDef(
-    _RequiredCloudwatchMetricActionOutputTypeDef, _OptionalCloudwatchMetricActionOutputTypeDef
-):
-    pass
-
-_RequiredDynamoDBActionOutputTypeDef = TypedDict(
-    "_RequiredDynamoDBActionOutputTypeDef",
-    {
-        "tableName": str,
-        "roleArn": str,
-        "hashKeyField": str,
-        "hashKeyValue": str,
-    },
-)
-_OptionalDynamoDBActionOutputTypeDef = TypedDict(
-    "_OptionalDynamoDBActionOutputTypeDef",
-    {
-        "operation": str,
-        "hashKeyType": DynamoKeyTypeType,
-        "rangeKeyField": str,
-        "rangeKeyValue": str,
-        "rangeKeyType": DynamoKeyTypeType,
-        "payloadField": str,
-    },
-    total=False,
-)
-
-class DynamoDBActionOutputTypeDef(
-    _RequiredDynamoDBActionOutputTypeDef, _OptionalDynamoDBActionOutputTypeDef
-):
-    pass
-
-ElasticsearchActionOutputTypeDef = TypedDict(
-    "ElasticsearchActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "endpoint": str,
-        "index": str,
-        "type": str,
-        "id": str,
-    },
-)
-
-_RequiredFirehoseActionOutputTypeDef = TypedDict(
-    "_RequiredFirehoseActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "deliveryStreamName": str,
-    },
-)
-_OptionalFirehoseActionOutputTypeDef = TypedDict(
-    "_OptionalFirehoseActionOutputTypeDef",
-    {
-        "separator": str,
-        "batchMode": bool,
-    },
-    total=False,
-)
-
-class FirehoseActionOutputTypeDef(
-    _RequiredFirehoseActionOutputTypeDef, _OptionalFirehoseActionOutputTypeDef
-):
-    pass
-
-IotAnalyticsActionOutputTypeDef = TypedDict(
-    "IotAnalyticsActionOutputTypeDef",
-    {
-        "channelArn": str,
-        "channelName": str,
-        "batchMode": bool,
-        "roleArn": str,
-    },
-    total=False,
-)
-
-_RequiredIotEventsActionOutputTypeDef = TypedDict(
-    "_RequiredIotEventsActionOutputTypeDef",
-    {
-        "inputName": str,
-        "roleArn": str,
-    },
-)
-_OptionalIotEventsActionOutputTypeDef = TypedDict(
-    "_OptionalIotEventsActionOutputTypeDef",
-    {
-        "messageId": str,
-        "batchMode": bool,
-    },
-    total=False,
-)
-
-class IotEventsActionOutputTypeDef(
-    _RequiredIotEventsActionOutputTypeDef, _OptionalIotEventsActionOutputTypeDef
-):
-    pass
-
-_RequiredKafkaActionOutputTypeDef = TypedDict(
-    "_RequiredKafkaActionOutputTypeDef",
-    {
-        "destinationArn": str,
-        "topic": str,
-        "clientProperties": Dict[str, str],
-    },
-)
-_OptionalKafkaActionOutputTypeDef = TypedDict(
-    "_OptionalKafkaActionOutputTypeDef",
-    {
-        "key": str,
-        "partition": str,
-    },
-    total=False,
-)
-
-class KafkaActionOutputTypeDef(
-    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
-):
-    pass
-
-_RequiredKinesisActionOutputTypeDef = TypedDict(
-    "_RequiredKinesisActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "streamName": str,
-    },
-)
-_OptionalKinesisActionOutputTypeDef = TypedDict(
-    "_OptionalKinesisActionOutputTypeDef",
-    {
-        "partitionKey": str,
-    },
-    total=False,
-)
-
-class KinesisActionOutputTypeDef(
-    _RequiredKinesisActionOutputTypeDef, _OptionalKinesisActionOutputTypeDef
-):
-    pass
-
-LambdaActionOutputTypeDef = TypedDict(
-    "LambdaActionOutputTypeDef",
-    {
-        "functionArn": str,
-    },
-)
-
-OpenSearchActionOutputTypeDef = TypedDict(
-    "OpenSearchActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "endpoint": str,
-        "index": str,
-        "type": str,
-        "id": str,
-    },
-)
-
-_RequiredS3ActionOutputTypeDef = TypedDict(
-    "_RequiredS3ActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "bucketName": str,
-        "key": str,
-    },
-)
-_OptionalS3ActionOutputTypeDef = TypedDict(
-    "_OptionalS3ActionOutputTypeDef",
-    {
-        "cannedAcl": CannedAccessControlListType,
-    },
-    total=False,
-)
-
-class S3ActionOutputTypeDef(_RequiredS3ActionOutputTypeDef, _OptionalS3ActionOutputTypeDef):
-    pass
-
-SalesforceActionOutputTypeDef = TypedDict(
-    "SalesforceActionOutputTypeDef",
-    {
-        "token": str,
-        "url": str,
-    },
-)
-
-_RequiredSnsActionOutputTypeDef = TypedDict(
-    "_RequiredSnsActionOutputTypeDef",
-    {
-        "targetArn": str,
-        "roleArn": str,
-    },
-)
-_OptionalSnsActionOutputTypeDef = TypedDict(
-    "_OptionalSnsActionOutputTypeDef",
-    {
-        "messageFormat": MessageFormatType,
-    },
-    total=False,
-)
-
-class SnsActionOutputTypeDef(_RequiredSnsActionOutputTypeDef, _OptionalSnsActionOutputTypeDef):
-    pass
-
-_RequiredSqsActionOutputTypeDef = TypedDict(
-    "_RequiredSqsActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "queueUrl": str,
-    },
-)
-_OptionalSqsActionOutputTypeDef = TypedDict(
-    "_OptionalSqsActionOutputTypeDef",
-    {
-        "useBase64": bool,
-    },
-    total=False,
-)
-
-class SqsActionOutputTypeDef(_RequiredSqsActionOutputTypeDef, _OptionalSqsActionOutputTypeDef):
-    pass
-
-_RequiredStepFunctionsActionOutputTypeDef = TypedDict(
-    "_RequiredStepFunctionsActionOutputTypeDef",
-    {
-        "stateMachineName": str,
-        "roleArn": str,
-    },
-)
-_OptionalStepFunctionsActionOutputTypeDef = TypedDict(
-    "_OptionalStepFunctionsActionOutputTypeDef",
-    {
-        "executionNamePrefix": str,
-    },
-    total=False,
-)
-
-class StepFunctionsActionOutputTypeDef(
-    _RequiredStepFunctionsActionOutputTypeDef, _OptionalStepFunctionsActionOutputTypeDef
-):
-    pass
-
 CloudwatchAlarmActionTypeDef = TypedDict(
     "CloudwatchAlarmActionTypeDef",
     {
         "roleArn": str,
         "alarmName": str,
         "stateReason": str,
         "stateValue": str,
@@ -1338,32 +966,34 @@
     },
     total=False,
 )
 
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
-_RequiredKafkaActionTypeDef = TypedDict(
-    "_RequiredKafkaActionTypeDef",
+_RequiredKafkaActionOutputTypeDef = TypedDict(
+    "_RequiredKafkaActionOutputTypeDef",
     {
         "destinationArn": str,
         "topic": str,
-        "clientProperties": Mapping[str, str],
+        "clientProperties": Dict[str, str],
     },
 )
-_OptionalKafkaActionTypeDef = TypedDict(
-    "_OptionalKafkaActionTypeDef",
+_OptionalKafkaActionOutputTypeDef = TypedDict(
+    "_OptionalKafkaActionOutputTypeDef",
     {
         "key": str,
         "partition": str,
     },
     total=False,
 )
 
-class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
+class KafkaActionOutputTypeDef(
+    _RequiredKafkaActionOutputTypeDef, _OptionalKafkaActionOutputTypeDef
+):
     pass
 
 _RequiredKinesisActionTypeDef = TypedDict(
     "_RequiredKinesisActionTypeDef",
     {
         "roleArn": str,
         "streamName": str,
@@ -1477,14 +1107,34 @@
 )
 
 class StepFunctionsActionTypeDef(
     _RequiredStepFunctionsActionTypeDef, _OptionalStepFunctionsActionTypeDef
 ):
     pass
 
+_RequiredKafkaActionTypeDef = TypedDict(
+    "_RequiredKafkaActionTypeDef",
+    {
+        "destinationArn": str,
+        "topic": str,
+        "clientProperties": Mapping[str, str],
+    },
+)
+_OptionalKafkaActionTypeDef = TypedDict(
+    "_OptionalKafkaActionTypeDef",
+    {
+        "key": str,
+        "partition": str,
+    },
+    total=False,
+)
+
+class KafkaActionTypeDef(_RequiredKafkaActionTypeDef, _OptionalKafkaActionTypeDef):
+    pass
+
 MetricValueOutputTypeDef = TypedDict(
     "MetricValueOutputTypeDef",
     {
         "count": int,
         "cidrs": List[str],
         "ports": List[int],
         "number": float,
@@ -1596,22 +1246,14 @@
     },
     total=False,
 )
 
 class AggregationTypeTypeDef(_RequiredAggregationTypeTypeDef, _OptionalAggregationTypeTypeDef):
     pass
 
-AlertTargetOutputTypeDef = TypedDict(
-    "AlertTargetOutputTypeDef",
-    {
-        "alertTargetArn": str,
-        "roleArn": str,
-    },
-)
-
 AlertTargetTypeDef = TypedDict(
     "AlertTargetTypeDef",
     {
         "alertTargetArn": str,
         "roleArn": str,
     },
 )
@@ -1621,33 +1263,14 @@
     {
         "policyName": str,
         "policyArn": str,
     },
     total=False,
 )
 
-_RequiredAssetPropertyTimestampOutputTypeDef = TypedDict(
-    "_RequiredAssetPropertyTimestampOutputTypeDef",
-    {
-        "timeInSeconds": str,
-    },
-)
-_OptionalAssetPropertyTimestampOutputTypeDef = TypedDict(
-    "_OptionalAssetPropertyTimestampOutputTypeDef",
-    {
-        "offsetInNanos": str,
-    },
-    total=False,
-)
-
-class AssetPropertyTimestampOutputTypeDef(
-    _RequiredAssetPropertyTimestampOutputTypeDef, _OptionalAssetPropertyTimestampOutputTypeDef
-):
-    pass
-
 _RequiredAssetPropertyTimestampTypeDef = TypedDict(
     "_RequiredAssetPropertyTimestampTypeDef",
     {
         "timeInSeconds": str,
     },
 )
 _OptionalAssetPropertyTimestampTypeDef = TypedDict(
@@ -1659,25 +1282,14 @@
 )
 
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
-AssetPropertyVariantOutputTypeDef = TypedDict(
-    "AssetPropertyVariantOutputTypeDef",
-    {
-        "stringValue": str,
-        "integerValue": str,
-        "doubleValue": str,
-        "booleanValue": str,
-    },
-    total=False,
-)
-
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
@@ -1703,21 +1315,22 @@
 
 class AssociateTargetsWithJobRequestRequestTypeDef(
     _RequiredAssociateTargetsWithJobRequestRequestTypeDef,
     _OptionalAssociateTargetsWithJobRequestRequestTypeDef,
 ):
     pass
 
-AssociateTargetsWithJobResponseTypeDef = TypedDict(
-    "AssociateTargetsWithJobResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AttachPolicyRequestRequestTypeDef = TypedDict(
     "AttachPolicyRequestRequestTypeDef",
     {
         "policyName": str,
@@ -1763,22 +1376,14 @@
     {
         "attributes": Mapping[str, str],
         "merge": bool,
     },
     total=False,
 )
 
-AuditCheckConfigurationOutputTypeDef = TypedDict(
-    "AuditCheckConfigurationOutputTypeDef",
-    {
-        "enabled": bool,
-    },
-    total=False,
-)
-
 AuditCheckConfigurationTypeDef = TypedDict(
     "AuditCheckConfigurationTypeDef",
     {
         "enabled": bool,
     },
     total=False,
 )
@@ -1839,24 +1444,14 @@
         "auditTaskId": str,
         "findingIds": Sequence[str],
         "auditCheckToReasonCodeFilter": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-AuditNotificationTargetOutputTypeDef = TypedDict(
-    "AuditNotificationTargetOutputTypeDef",
-    {
-        "targetArn": str,
-        "roleArn": str,
-        "enabled": bool,
-    },
-    total=False,
-)
-
 AuditNotificationTargetTypeDef = TypedDict(
     "AuditNotificationTargetTypeDef",
     {
         "targetArn": str,
         "roleArn": str,
         "enabled": bool,
     },
@@ -1903,23 +1498,14 @@
     },
     total=False,
 )
 
 class AuthInfoTypeDef(_RequiredAuthInfoTypeDef, _OptionalAuthInfoTypeDef):
     pass
 
-AuthorizerConfigOutputTypeDef = TypedDict(
-    "AuthorizerConfigOutputTypeDef",
-    {
-        "defaultAuthorizerName": str,
-        "allowAuthorizerOverride": bool,
-    },
-    total=False,
-)
-
 AuthorizerConfigTypeDef = TypedDict(
     "AuthorizerConfigTypeDef",
     {
         "defaultAuthorizerName": str,
         "allowAuthorizerOverride": bool,
     },
     total=False,
@@ -1957,40 +1543,23 @@
         "failureType": AwsJobAbortCriteriaFailureTypeType,
         "action": Literal["CANCEL"],
         "thresholdPercentage": float,
         "minNumberOfExecutedThings": int,
     },
 )
 
-AwsJobRateIncreaseCriteriaOutputTypeDef = TypedDict(
-    "AwsJobRateIncreaseCriteriaOutputTypeDef",
-    {
-        "numberOfNotifiedThings": int,
-        "numberOfSucceededThings": int,
-    },
-    total=False,
-)
-
 AwsJobRateIncreaseCriteriaTypeDef = TypedDict(
     "AwsJobRateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
 )
 
-AwsJobPresignedUrlConfigOutputTypeDef = TypedDict(
-    "AwsJobPresignedUrlConfigOutputTypeDef",
-    {
-        "expiresInSec": int,
-    },
-    total=False,
-)
-
 AwsJobPresignedUrlConfigTypeDef = TypedDict(
     "AwsJobPresignedUrlConfigTypeDef",
     {
         "expiresInSec": int,
     },
     total=False,
 )
@@ -1999,89 +1568,55 @@
     "AwsJobTimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
-MachineLearningDetectionConfigOutputTypeDef = TypedDict(
-    "MachineLearningDetectionConfigOutputTypeDef",
+MachineLearningDetectionConfigTypeDef = TypedDict(
+    "MachineLearningDetectionConfigTypeDef",
     {
         "confidenceLevel": ConfidenceLevelType,
     },
 )
 
-StatisticalThresholdOutputTypeDef = TypedDict(
-    "StatisticalThresholdOutputTypeDef",
+StatisticalThresholdTypeDef = TypedDict(
+    "StatisticalThresholdTypeDef",
     {
         "statistic": str,
     },
     total=False,
 )
 
-MachineLearningDetectionConfigTypeDef = TypedDict(
-    "MachineLearningDetectionConfigTypeDef",
-    {
-        "confidenceLevel": ConfidenceLevelType,
-    },
-)
-
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "count": int,
         "cidrs": Sequence[str],
         "ports": Sequence[int],
         "number": float,
         "numbers": Sequence[float],
         "strings": Sequence[str],
     },
     total=False,
 )
 
-StatisticalThresholdTypeDef = TypedDict(
-    "StatisticalThresholdTypeDef",
-    {
-        "statistic": str,
-    },
-    total=False,
-)
-
 BehaviorModelTrainingSummaryTypeDef = TypedDict(
     "BehaviorModelTrainingSummaryTypeDef",
     {
         "securityProfileName": str,
         "behaviorName": str,
         "trainingDataCollectionStartDate": datetime,
         "modelStatus": ModelStatusType,
         "datapointsCollectionPercentage": float,
         "lastModelRefreshDate": datetime,
     },
     total=False,
 )
 
-_RequiredMetricDimensionOutputTypeDef = TypedDict(
-    "_RequiredMetricDimensionOutputTypeDef",
-    {
-        "dimensionName": str,
-    },
-)
-_OptionalMetricDimensionOutputTypeDef = TypedDict(
-    "_OptionalMetricDimensionOutputTypeDef",
-    {
-        "operator": DimensionValueOperatorType,
-    },
-    total=False,
-)
-
-class MetricDimensionOutputTypeDef(
-    _RequiredMetricDimensionOutputTypeDef, _OptionalMetricDimensionOutputTypeDef
-):
-    pass
-
 _RequiredMetricDimensionTypeDef = TypedDict(
     "_RequiredMetricDimensionTypeDef",
     {
         "dimensionName": str,
     },
 )
 _OptionalMetricDimensionTypeDef = TypedDict(
@@ -2099,22 +1634,14 @@
     "BillingGroupMetadataTypeDef",
     {
         "creationDate": datetime,
     },
     total=False,
 )
 
-BillingGroupPropertiesOutputTypeDef = TypedDict(
-    "BillingGroupPropertiesOutputTypeDef",
-    {
-        "billingGroupDescription": str,
-    },
-    total=False,
-)
-
 BillingGroupPropertiesTypeDef = TypedDict(
     "BillingGroupPropertiesTypeDef",
     {
         "billingGroupDescription": str,
     },
     total=False,
 )
@@ -2224,24 +1751,14 @@
 )
 
 class CancelJobRequestRequestTypeDef(
     _RequiredCancelJobRequestRequestTypeDef, _OptionalCancelJobRequestRequestTypeDef
 ):
     pass
 
-CancelJobResponseTypeDef = TypedDict(
-    "CancelJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TransferDataTypeDef = TypedDict(
     "TransferDataTypeDef",
     {
         "transferMessage": str,
         "rejectReason": str,
         "transferDate": datetime,
         "acceptDate": datetime,
@@ -2258,23 +1775,14 @@
         "status": CertificateStatusType,
         "certificateMode": CertificateModeType,
         "creationDate": datetime,
     },
     total=False,
 )
 
-CodeSigningCertificateChainOutputTypeDef = TypedDict(
-    "CodeSigningCertificateChainOutputTypeDef",
-    {
-        "certificateName": str,
-        "inlineDocument": str,
-    },
-    total=False,
-)
-
 CodeSigningCertificateChainTypeDef = TypedDict(
     "CodeSigningCertificateChainTypeDef",
     {
         "certificateName": str,
         "inlineDocument": str,
     },
     total=False,
@@ -2292,22 +1800,14 @@
     "CodeSigningSignatureTypeDef",
     {
         "inlineDocument": Union[str, bytes, IO[Any], StreamingBody],
     },
     total=False,
 )
 
-ConfigurationOutputTypeDef = TypedDict(
-    "ConfigurationOutputTypeDef",
-    {
-        "Enabled": bool,
-    },
-    total=False,
-)
-
 ConfigurationTypeDef = TypedDict(
     "ConfigurationTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
@@ -2332,33 +1832,14 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateBillingGroupResponseTypeDef = TypedDict(
-    "CreateBillingGroupResponseTypeDef",
-    {
-        "billingGroupName": str,
-        "billingGroupArn": str,
-        "billingGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateCertificateFromCsrRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateFromCsrRequestRequestTypeDef",
     {
         "certificateSigningRequest": str,
     },
 )
 _OptionalCreateCertificateFromCsrRequestRequestTypeDef = TypedDict(
@@ -2371,81 +1852,22 @@
 
 class CreateCertificateFromCsrRequestRequestTypeDef(
     _RequiredCreateCertificateFromCsrRequestRequestTypeDef,
     _OptionalCreateCertificateFromCsrRequestRequestTypeDef,
 ):
     pass
 
-CreateCertificateFromCsrResponseTypeDef = TypedDict(
-    "CreateCertificateFromCsrResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "certificatePem": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCustomMetricResponseTypeDef = TypedDict(
-    "CreateCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDimensionResponseTypeDef = TypedDict(
-    "CreateDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "securityPolicy": str,
     },
     total=False,
 )
 
-CreateDomainConfigurationResponseTypeDef = TypedDict(
-    "CreateDomainConfigurationResponseTypeDef",
-    {
-        "domainConfigurationName": str,
-        "domainConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDynamicThingGroupResponseTypeDef = TypedDict(
-    "CreateDynamicThingGroupResponseTypeDef",
-    {
-        "thingGroupName": str,
-        "thingGroupArn": str,
-        "thingGroupId": str,
-        "indexName": str,
-        "queryString": str,
-        "queryVersion": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFleetMetricResponseTypeDef = TypedDict(
-    "CreateFleetMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PresignedUrlConfigTypeDef = TypedDict(
     "PresignedUrlConfigTypeDef",
     {
         "roleArn": str,
         "expiresInSec": int,
     },
     total=False,
@@ -2455,41 +1877,22 @@
     "TimeoutConfigTypeDef",
     {
         "inProgressTimeoutInMinutes": int,
     },
     total=False,
 )
 
-CreateJobResponseTypeDef = TypedDict(
-    "CreateJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MaintenanceWindowTypeDef = TypedDict(
     "MaintenanceWindowTypeDef",
     {
         "startTime": str,
         "durationInMinutes": int,
     },
 )
 
-CreateJobTemplateResponseTypeDef = TypedDict(
-    "CreateJobTemplateResponseTypeDef",
-    {
-        "jobTemplateArn": str,
-        "jobTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateKeysAndCertificateRequestRequestTypeDef = TypedDict(
     "CreateKeysAndCertificateRequestRequestTypeDef",
     {
         "setAsActive": bool,
     },
     total=False,
 )
@@ -2499,35 +1902,14 @@
     {
         "PublicKey": str,
         "PrivateKey": str,
     },
     total=False,
 )
 
-CreateMitigationActionResponseTypeDef = TypedDict(
-    "CreateMitigationActionResponseTypeDef",
-    {
-        "actionArn": str,
-        "actionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateOTAUpdateResponseTypeDef = TypedDict(
-    "CreateOTAUpdateResponseTypeDef",
-    {
-        "otaUpdateId": str,
-        "awsIotJobId": str,
-        "otaUpdateArn": str,
-        "awsIotJobArn": str,
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalCreatePackageRequestRequestTypeDef = TypedDict(
@@ -2541,24 +1923,14 @@
 )
 
 class CreatePackageRequestRequestTypeDef(
     _RequiredCreatePackageRequestRequestTypeDef, _OptionalCreatePackageRequestRequestTypeDef
 ):
     pass
 
-CreatePackageResponseTypeDef = TypedDict(
-    "CreatePackageResponseTypeDef",
-    {
-        "packageName": str,
-        "packageArn": str,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePackageVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePackageVersionRequestRequestTypeDef",
     {
         "packageName": str,
         "versionName": str,
     },
 )
@@ -2575,39 +1947,14 @@
 
 class CreatePackageVersionRequestRequestTypeDef(
     _RequiredCreatePackageVersionRequestRequestTypeDef,
     _OptionalCreatePackageVersionRequestRequestTypeDef,
 ):
     pass
 
-CreatePackageVersionResponseTypeDef = TypedDict(
-    "CreatePackageVersionResponseTypeDef",
-    {
-        "packageVersionArn": str,
-        "packageName": str,
-        "versionName": str,
-        "description": str,
-        "attributes": Dict[str, str],
-        "status": PackageVersionStatusType,
-        "errorReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePolicyResponseTypeDef = TypedDict(
-    "CreatePolicyResponseTypeDef",
-    {
-        "policyName": str,
-        "policyArn": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePolicyVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyDocument": str,
     },
 )
@@ -2621,25 +1968,14 @@
 
 class CreatePolicyVersionRequestRequestTypeDef(
     _RequiredCreatePolicyVersionRequestRequestTypeDef,
     _OptionalCreatePolicyVersionRequestRequestTypeDef,
 ):
     pass
 
-CreatePolicyVersionResponseTypeDef = TypedDict(
-    "CreatePolicyVersionResponseTypeDef",
-    {
-        "policyArn": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateProvisioningClaimRequestRequestTypeDef = TypedDict(
     "CreateProvisioningClaimRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 
@@ -2656,24 +1992,14 @@
     },
     total=False,
 )
 
 class ProvisioningHookTypeDef(_RequiredProvisioningHookTypeDef, _OptionalProvisioningHookTypeDef):
     pass
 
-CreateProvisioningTemplateResponseTypeDef = TypedDict(
-    "CreateProvisioningTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "defaultVersionId": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "templateBody": str,
     },
 )
@@ -2687,101 +2013,23 @@
 
 class CreateProvisioningTemplateVersionRequestRequestTypeDef(
     _RequiredCreateProvisioningTemplateVersionRequestRequestTypeDef,
     _OptionalCreateProvisioningTemplateVersionRequestRequestTypeDef,
 ):
     pass
 
-CreateProvisioningTemplateVersionResponseTypeDef = TypedDict(
-    "CreateProvisioningTemplateVersionResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "versionId": int,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRoleAliasResponseTypeDef = TypedDict(
-    "CreateRoleAliasResponseTypeDef",
-    {
-        "roleAlias": str,
-        "roleAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateScheduledAuditResponseTypeDef = TypedDict(
-    "CreateScheduledAuditResponseTypeDef",
-    {
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSecurityProfileResponseTypeDef = TypedDict(
-    "CreateSecurityProfileResponseTypeDef",
-    {
-        "securityProfileName": str,
-        "securityProfileArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStreamResponseTypeDef = TypedDict(
-    "CreateStreamResponseTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "description": str,
-        "streamVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThingGroupResponseTypeDef = TypedDict(
-    "CreateThingGroupResponseTypeDef",
-    {
-        "thingGroupName": str,
-        "thingGroupArn": str,
-        "thingGroupId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateThingResponseTypeDef = TypedDict(
-    "CreateThingResponseTypeDef",
-    {
-        "thingName": str,
-        "thingArn": str,
-        "thingId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ThingTypePropertiesTypeDef = TypedDict(
     "ThingTypePropertiesTypeDef",
     {
         "thingTypeDescription": str,
         "searchableAttributes": Sequence[str],
     },
     total=False,
 )
 
-CreateThingTypeResponseTypeDef = TypedDict(
-    "CreateThingTypeResponseTypeDef",
-    {
-        "thingTypeName": str,
-        "thingTypeArn": str,
-        "thingTypeId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteAccountAuditConfigurationRequestRequestTypeDef",
     {
         "deleteScheduledAudits": bool,
     },
     total=False,
 )
@@ -3238,16 +2486,16 @@
 DescribeCACertificateRequestRequestTypeDef = TypedDict(
     "DescribeCACertificateRequestRequestTypeDef",
     {
         "certificateId": str,
     },
 )
 
-RegistrationConfigOutputTypeDef = TypedDict(
-    "RegistrationConfigOutputTypeDef",
+RegistrationConfigTypeDef = TypedDict(
+    "RegistrationConfigTypeDef",
     {
         "templateBody": str,
         "roleArn": str,
         "templateName": str,
     },
     total=False,
 )
@@ -3262,54 +2510,28 @@
 DescribeCustomMetricRequestRequestTypeDef = TypedDict(
     "DescribeCustomMetricRequestRequestTypeDef",
     {
         "metricName": str,
     },
 )
 
-DescribeCustomMetricResponseTypeDef = TypedDict(
-    "DescribeCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "metricType": CustomMetricTypeType,
-        "displayName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "DescribeDetectMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
 DescribeDimensionRequestRequestTypeDef = TypedDict(
     "DescribeDimensionRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-DescribeDimensionResponseTypeDef = TypedDict(
-    "DescribeDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "type": Literal["TOPIC_FILTER"],
-        "stringValues": List[str],
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDomainConfigurationRequestRequestTypeDef = TypedDict(
     "DescribeDomainConfigurationRequestRequestTypeDef",
     {
         "domainConfigurationName": str,
     },
 )
 
@@ -3319,62 +2541,36 @@
         "serverCertificateArn": str,
         "serverCertificateStatus": ServerCertificateStatusType,
         "serverCertificateStatusDetail": str,
     },
     total=False,
 )
 
-TlsConfigOutputTypeDef = TypedDict(
-    "TlsConfigOutputTypeDef",
-    {
-        "securityPolicy": str,
-    },
-    total=False,
-)
-
 DescribeEndpointRequestRequestTypeDef = TypedDict(
     "DescribeEndpointRequestRequestTypeDef",
     {
         "endpointType": str,
     },
     total=False,
 )
 
-DescribeEndpointResponseTypeDef = TypedDict(
-    "DescribeEndpointResponseTypeDef",
-    {
-        "endpointAddress": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeFleetMetricRequestRequestTypeDef = TypedDict(
     "DescribeFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
     },
 )
 
 DescribeIndexRequestRequestTypeDef = TypedDict(
     "DescribeIndexRequestRequestTypeDef",
     {
         "indexName": str,
     },
 )
 
-DescribeIndexResponseTypeDef = TypedDict(
-    "DescribeIndexResponseTypeDef",
-    {
-        "indexName": str,
-        "indexStatus": IndexStatusType,
-        "schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeJobExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeJobExecutionRequestRequestTypeDef",
     {
         "jobId": str,
         "thingName": str,
     },
 )
@@ -3402,39 +2598,14 @@
 DescribeJobTemplateRequestRequestTypeDef = TypedDict(
     "DescribeJobTemplateRequestRequestTypeDef",
     {
         "jobTemplateId": str,
     },
 )
 
-MaintenanceWindowOutputTypeDef = TypedDict(
-    "MaintenanceWindowOutputTypeDef",
-    {
-        "startTime": str,
-        "durationInMinutes": int,
-    },
-)
-
-PresignedUrlConfigOutputTypeDef = TypedDict(
-    "PresignedUrlConfigOutputTypeDef",
-    {
-        "roleArn": str,
-        "expiresInSec": int,
-    },
-    total=False,
-)
-
-TimeoutConfigOutputTypeDef = TypedDict(
-    "TimeoutConfigOutputTypeDef",
-    {
-        "inProgressTimeoutInMinutes": int,
-    },
-    total=False,
-)
-
 _RequiredDescribeManagedJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeManagedJobTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalDescribeManagedJobTemplateRequestRequestTypeDef = TypedDict(
@@ -3473,52 +2644,22 @@
 DescribeProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "DescribeProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 
-_RequiredProvisioningHookOutputTypeDef = TypedDict(
-    "_RequiredProvisioningHookOutputTypeDef",
-    {
-        "targetArn": str,
-    },
-)
-_OptionalProvisioningHookOutputTypeDef = TypedDict(
-    "_OptionalProvisioningHookOutputTypeDef",
-    {
-        "payloadVersion": str,
-    },
-    total=False,
-)
-
-class ProvisioningHookOutputTypeDef(
-    _RequiredProvisioningHookOutputTypeDef, _OptionalProvisioningHookOutputTypeDef
-):
-    pass
-
 DescribeProvisioningTemplateVersionRequestRequestTypeDef = TypedDict(
     "DescribeProvisioningTemplateVersionRequestRequestTypeDef",
     {
         "templateName": str,
         "versionId": int,
     },
 )
 
-DescribeProvisioningTemplateVersionResponseTypeDef = TypedDict(
-    "DescribeProvisioningTemplateVersionResponseTypeDef",
-    {
-        "versionId": int,
-        "creationDate": datetime,
-        "templateBody": str,
-        "isDefaultVersion": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRoleAliasRequestRequestTypeDef = TypedDict(
     "DescribeRoleAliasRequestRequestTypeDef",
     {
         "roleAlias": str,
     },
 )
 
@@ -3539,27 +2680,14 @@
 DescribeScheduledAuditRequestRequestTypeDef = TypedDict(
     "DescribeScheduledAuditRequestRequestTypeDef",
     {
         "scheduledAuditName": str,
     },
 )
 
-DescribeScheduledAuditResponseTypeDef = TypedDict(
-    "DescribeScheduledAuditResponseTypeDef",
-    {
-        "frequency": AuditFrequencyType,
-        "dayOfMonth": str,
-        "dayOfWeek": DayOfWeekType,
-        "targetCheckNames": List[str],
-        "scheduledAuditName": str,
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSecurityProfileRequestRequestTypeDef = TypedDict(
     "DescribeSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 
@@ -3580,55 +2708,21 @@
 DescribeThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "DescribeThingRegistrationTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
-DescribeThingRegistrationTaskResponseTypeDef = TypedDict(
-    "DescribeThingRegistrationTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "templateBody": str,
-        "inputFileBucket": str,
-        "inputFileKey": str,
-        "roleArn": str,
-        "status": StatusType,
-        "message": str,
-        "successCount": int,
-        "failureCount": int,
-        "percentageProgress": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeThingRequestRequestTypeDef = TypedDict(
     "DescribeThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 
-DescribeThingResponseTypeDef = TypedDict(
-    "DescribeThingResponseTypeDef",
-    {
-        "defaultClientId": str,
-        "thingName": str,
-        "thingId": str,
-        "thingArn": str,
-        "thingTypeName": str,
-        "attributes": Dict[str, str],
-        "version": int,
-        "billingGroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeThingTypeRequestRequestTypeDef = TypedDict(
     "DescribeThingTypeRequestRequestTypeDef",
     {
         "thingTypeName": str,
     },
 )
 
@@ -3647,23 +2741,14 @@
     {
         "thingTypeDescription": str,
         "searchableAttributes": List[str],
     },
     total=False,
 )
 
-S3DestinationOutputTypeDef = TypedDict(
-    "S3DestinationOutputTypeDef",
-    {
-        "bucket": str,
-        "prefix": str,
-    },
-    total=False,
-)
-
 S3DestinationTypeDef = TypedDict(
     "S3DestinationTypeDef",
     {
         "bucket": str,
         "prefix": str,
     },
     total=False,
@@ -3768,21 +2853,14 @@
         "domainConfigurationName": str,
         "domainConfigurationArn": str,
         "serviceType": ServiceTypeType,
     },
     total=False,
 )
 
-PutItemInputOutputTypeDef = TypedDict(
-    "PutItemInputOutputTypeDef",
-    {
-        "tableName": str,
-    },
-)
-
 PutItemInputTypeDef = TypedDict(
     "PutItemInputTypeDef",
     {
         "tableName": str,
     },
 )
 
@@ -3792,29 +2870,14 @@
         "policyName": str,
         "policyArn": str,
         "policyDocument": str,
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
-EnableIoTLoggingParamsOutputTypeDef = TypedDict(
-    "EnableIoTLoggingParamsOutputTypeDef",
-    {
-        "roleArnForLogging": str,
-        "logLevel": LogLevelType,
-    },
-)
-
 EnableIoTLoggingParamsTypeDef = TypedDict(
     "EnableIoTLoggingParamsTypeDef",
     {
         "roleArnForLogging": str,
         "logLevel": LogLevelType,
     },
 )
@@ -3831,69 +2894,32 @@
     {
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-RateIncreaseCriteriaOutputTypeDef = TypedDict(
-    "RateIncreaseCriteriaOutputTypeDef",
-    {
-        "numberOfNotifiedThings": int,
-        "numberOfSucceededThings": int,
-    },
-    total=False,
-)
-
 RateIncreaseCriteriaTypeDef = TypedDict(
     "RateIncreaseCriteriaTypeDef",
     {
         "numberOfNotifiedThings": int,
         "numberOfSucceededThings": int,
     },
     total=False,
 )
 
-FieldOutputTypeDef = TypedDict(
-    "FieldOutputTypeDef",
-    {
-        "name": str,
-        "type": FieldTypeType,
-    },
-    total=False,
-)
-
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "name": str,
         "type": FieldTypeType,
     },
     total=False,
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
-    {
-        "bucket": str,
-        "key": str,
-        "version": str,
-    },
-    total=False,
-)
-
-StreamOutputTypeDef = TypedDict(
-    "StreamOutputTypeDef",
-    {
-        "streamId": str,
-        "fileId": int,
-    },
-    total=False,
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "key": str,
         "version": str,
     },
@@ -3914,23 +2940,22 @@
     {
         "metricName": str,
         "metricArn": str,
     },
     total=False,
 )
 
-GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = (
-    TypedDict(
-        "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
-        {
-            "securityProfileName": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
 )
 
 GetBehaviorModelTrainingSummariesRequestRequestTypeDef = TypedDict(
     "GetBehaviorModelTrainingSummariesRequestRequestTypeDef",
     {
         "securityProfileName": str,
         "maxResults": int,
@@ -3956,22 +2981,14 @@
 )
 
 class GetCardinalityRequestRequestTypeDef(
     _RequiredGetCardinalityRequestRequestTypeDef, _OptionalGetCardinalityRequestRequestTypeDef
 ):
     pass
 
-GetCardinalityResponseTypeDef = TypedDict(
-    "GetCardinalityResponseTypeDef",
-    {
-        "cardinality": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEffectivePoliciesRequestRequestTypeDef = TypedDict(
     "GetEffectivePoliciesRequestRequestTypeDef",
     {
         "principal": str,
         "cognitoIdentityPoolId": str,
         "thingName": str,
     },
@@ -3981,91 +2998,45 @@
 GetJobDocumentRequestRequestTypeDef = TypedDict(
     "GetJobDocumentRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
-GetJobDocumentResponseTypeDef = TypedDict(
-    "GetJobDocumentResponseTypeDef",
-    {
-        "document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetLoggingOptionsResponseTypeDef = TypedDict(
-    "GetLoggingOptionsResponseTypeDef",
-    {
-        "roleArn": str,
-        "logLevel": LogLevelType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetOTAUpdateRequestRequestTypeDef = TypedDict(
     "GetOTAUpdateRequestRequestTypeDef",
     {
         "otaUpdateId": str,
     },
 )
 
-VersionUpdateByJobsConfigOutputTypeDef = TypedDict(
-    "VersionUpdateByJobsConfigOutputTypeDef",
+VersionUpdateByJobsConfigTypeDef = TypedDict(
+    "VersionUpdateByJobsConfigTypeDef",
     {
         "enabled": bool,
         "roleArn": str,
     },
     total=False,
 )
 
 GetPackageRequestRequestTypeDef = TypedDict(
     "GetPackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 
-GetPackageResponseTypeDef = TypedDict(
-    "GetPackageResponseTypeDef",
-    {
-        "packageName": str,
-        "packageArn": str,
-        "description": str,
-        "defaultVersionName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPackageVersionRequestRequestTypeDef = TypedDict(
     "GetPackageVersionRequestRequestTypeDef",
     {
         "packageName": str,
         "versionName": str,
     },
 )
 
-GetPackageVersionResponseTypeDef = TypedDict(
-    "GetPackageVersionResponseTypeDef",
-    {
-        "packageVersionArn": str,
-        "packageName": str,
-        "versionName": str,
-        "description": str,
-        "attributes": Dict[str, str],
-        "status": PackageVersionStatusType,
-        "errorReason": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetPercentilesRequestRequestTypeDef = TypedDict(
     "_RequiredGetPercentilesRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalGetPercentilesRequestRequestTypeDef = TypedDict(
@@ -4096,59 +3067,22 @@
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 
-GetPolicyResponseTypeDef = TypedDict(
-    "GetPolicyResponseTypeDef",
-    {
-        "policyName": str,
-        "policyArn": str,
-        "policyDocument": str,
-        "defaultVersionId": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "generationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPolicyVersionRequestRequestTypeDef = TypedDict(
     "GetPolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
 )
 
-GetPolicyVersionResponseTypeDef = TypedDict(
-    "GetPolicyVersionResponseTypeDef",
-    {
-        "policyArn": str,
-        "policyName": str,
-        "policyDocument": str,
-        "policyVersionId": str,
-        "isDefaultVersion": bool,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "generationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRegistrationCodeResponseTypeDef = TypedDict(
-    "GetRegistrationCodeResponseTypeDef",
-    {
-        "registrationCode": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatisticsRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalGetStatisticsRequestRequestTypeDef = TypedDict(
@@ -4191,58 +3125,31 @@
 GetTopicRuleRequestRequestTypeDef = TypedDict(
     "GetTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
     },
 )
 
-GetV2LoggingOptionsResponseTypeDef = TypedDict(
-    "GetV2LoggingOptionsResponseTypeDef",
-    {
-        "roleArn": str,
-        "defaultLogLevel": LogLevelType,
-        "disableAllLogs": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GroupNameAndArnTypeDef = TypedDict(
     "GroupNameAndArnTypeDef",
     {
         "groupName": str,
         "groupArn": str,
     },
     total=False,
 )
 
-HttpActionHeaderOutputTypeDef = TypedDict(
-    "HttpActionHeaderOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 HttpActionHeaderTypeDef = TypedDict(
     "HttpActionHeaderTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-SigV4AuthorizationOutputTypeDef = TypedDict(
-    "SigV4AuthorizationOutputTypeDef",
-    {
-        "signingRegion": str,
-        "serviceName": str,
-        "roleArn": str,
-    },
-)
-
 SigV4AuthorizationTypeDef = TypedDict(
     "SigV4AuthorizationTypeDef",
     {
         "signingRegion": str,
         "serviceName": str,
         "roleArn": str,
     },
@@ -4292,24 +3199,14 @@
     "IndexingFilterTypeDef",
     {
         "namedShadowNames": Sequence[str],
     },
     total=False,
 )
 
-IssuerCertificateIdentifierOutputTypeDef = TypedDict(
-    "IssuerCertificateIdentifierOutputTypeDef",
-    {
-        "issuerCertificateSubject": str,
-        "issuerId": str,
-        "issuerCertificateSerialNumber": str,
-    },
-    total=False,
-)
-
 IssuerCertificateIdentifierTypeDef = TypedDict(
     "IssuerCertificateIdentifierTypeDef",
     {
         "issuerCertificateSubject": str,
         "issuerId": str,
         "issuerCertificateSerialNumber": str,
     },
@@ -4333,22 +3230,14 @@
         "lastUpdatedAt": datetime,
         "executionNumber": int,
         "retryAttempt": int,
     },
     total=False,
 )
 
-RetryCriteriaOutputTypeDef = TypedDict(
-    "RetryCriteriaOutputTypeDef",
-    {
-        "failureType": RetryableFailureTypeType,
-        "numberOfRetries": int,
-    },
-)
-
 RetryCriteriaTypeDef = TypedDict(
     "RetryCriteriaTypeDef",
     {
         "failureType": RetryableFailureTypeType,
         "numberOfRetries": int,
     },
 )
@@ -4400,62 +3289,28 @@
     "ScheduledJobRolloutTypeDef",
     {
         "startTime": str,
     },
     total=False,
 )
 
-ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = TypedDict(
-    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListActiveViolationsRequestRequestTypeDef = TypedDict(
     "ListActiveViolationsRequestRequestTypeDef",
     {
         "thingName": str,
         "securityProfileName": str,
         "behaviorCriteriaType": BehaviorCriteriaTypeType,
         "listSuppressedAlerts": bool,
         "verificationState": VerificationStateType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
-    {
-        "target": str,
-    },
-)
-_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
-    {
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef(
-    _RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
-    _OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttachedPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListAttachedPoliciesRequestRequestTypeDef",
     {
         "target": str,
     },
 )
 _OptionalListAttachedPoliciesRequestRequestTypeDef = TypedDict(
@@ -4470,36 +3325,14 @@
 
 class ListAttachedPoliciesRequestRequestTypeDef(
     _RequiredListAttachedPoliciesRequestRequestTypeDef,
     _OptionalListAttachedPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-        "findingId": str,
-    },
-)
-_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "actionStatus": AuditMitigationActionsExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef(
-    _RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
-    _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef",
     {
         "taskId": str,
         "findingId": str,
     },
 )
@@ -4515,38 +3348,14 @@
 
 class ListAuditMitigationActionsExecutionsRequestRequestTypeDef(
     _RequiredListAuditMitigationActionsExecutionsRequestRequestTypeDef,
     _OptionalListAuditMitigationActionsExecutionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
-    {
-        "auditTaskId": str,
-        "findingId": str,
-        "taskStatus": AuditMitigationActionsTaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef(
-    _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-    _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
-):
-    pass
-
 _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListAuditMitigationActionsTasksRequestRequestTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
@@ -4564,37 +3373,14 @@
 
 class ListAuditMitigationActionsTasksRequestRequestTypeDef(
     _RequiredListAuditMitigationActionsTasksRequestRequestTypeDef,
     _OptionalListAuditMitigationActionsTasksRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
-    "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
-    "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
-    {
-        "taskType": AuditTaskTypeType,
-        "taskStatus": AuditTaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAuditTasksRequestListAuditTasksPaginateTypeDef(
-    _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef,
-    _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef,
-):
-    pass
-
 _RequiredListAuditTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListAuditTasksRequestRequestTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
@@ -4610,96 +3396,46 @@
 )
 
 class ListAuditTasksRequestRequestTypeDef(
     _RequiredListAuditTasksRequestRequestTypeDef, _OptionalListAuditTasksRequestRequestTypeDef
 ):
     pass
 
-ListAuthorizersRequestListAuthorizersPaginateTypeDef = TypedDict(
-    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "status": AuthorizerStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAuthorizersRequestRequestTypeDef = TypedDict(
     "ListAuthorizersRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "status": AuthorizerStatusType,
     },
     total=False,
 )
 
-ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = TypedDict(
-    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
-    {
-        "namePrefixFilter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListBillingGroupsRequestRequestTypeDef = TypedDict(
     "ListBillingGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "namePrefixFilter": str,
     },
     total=False,
 )
 
-ListCACertificatesRequestListCACertificatesPaginateTypeDef = TypedDict(
-    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "templateName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCACertificatesRequestRequestTypeDef = TypedDict(
     "ListCACertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
         "templateName": str,
     },
     total=False,
 )
 
-_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
-    "_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
-    {
-        "caCertificateId": str,
-    },
-)
-_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
-    "_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef(
-    _RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
-    _OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
-):
-    pass
-
 _RequiredListCertificatesByCARequestRequestTypeDef = TypedDict(
     "_RequiredListCertificatesByCARequestRequestTypeDef",
     {
         "caCertificateId": str,
     },
 )
 _OptionalListCertificatesByCARequestRequestTypeDef = TypedDict(
@@ -4714,107 +3450,47 @@
 
 class ListCertificatesByCARequestRequestTypeDef(
     _RequiredListCertificatesByCARequestRequestTypeDef,
     _OptionalListCertificatesByCARequestRequestTypeDef,
 ):
     pass
 
-ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
-    "ListCertificatesRequestListCertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCertificatesRequestRequestTypeDef = TypedDict(
     "ListCertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = TypedDict(
-    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomMetricsRequestRequestTypeDef = TypedDict(
     "ListCustomMetricsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListCustomMetricsResponseTypeDef = TypedDict(
-    "ListCustomMetricsResponseTypeDef",
-    {
-        "metricNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
-    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
-    {
-        "taskId": str,
-        "violationId": str,
-        "thingName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDetectMitigationActionsExecutionsRequestRequestTypeDef = TypedDict(
     "ListDetectMitigationActionsExecutionsRequestRequestTypeDef",
     {
         "taskId": str,
         "violationId": str,
         "thingName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
-    "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef(
-    _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-    _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
-):
-    pass
-
 _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef = TypedDict(
     "_RequiredListDetectMitigationActionsTasksRequestRequestTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
@@ -4829,123 +3505,51 @@
 
 class ListDetectMitigationActionsTasksRequestRequestTypeDef(
     _RequiredListDetectMitigationActionsTasksRequestRequestTypeDef,
     _OptionalListDetectMitigationActionsTasksRequestRequestTypeDef,
 ):
     pass
 
-ListDimensionsRequestListDimensionsPaginateTypeDef = TypedDict(
-    "ListDimensionsRequestListDimensionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDimensionsRequestRequestTypeDef = TypedDict(
     "ListDimensionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListDimensionsResponseTypeDef = TypedDict(
-    "ListDimensionsResponseTypeDef",
-    {
-        "dimensionNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = TypedDict(
-    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
-    {
-        "serviceType": ServiceTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDomainConfigurationsRequestRequestTypeDef = TypedDict(
     "ListDomainConfigurationsRequestRequestTypeDef",
     {
         "marker": str,
         "pageSize": int,
         "serviceType": ServiceTypeType,
     },
     total=False,
 )
 
-ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = TypedDict(
-    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFleetMetricsRequestRequestTypeDef = TypedDict(
     "ListFleetMetricsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListIndicesRequestListIndicesPaginateTypeDef = TypedDict(
-    "ListIndicesRequestListIndicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListIndicesRequestRequestTypeDef = TypedDict(
     "ListIndicesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListIndicesResponseTypeDef = TypedDict(
-    "ListIndicesResponseTypeDef",
-    {
-        "indexNames": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
-    "_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
-    {
-        "jobId": str,
-    },
-)
-_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
-    "_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
-    {
-        "status": JobExecutionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef(
-    _RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
-    _OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobExecutionsForJobRequestRequestTypeDef = TypedDict(
     "_RequiredListJobExecutionsForJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalListJobExecutionsForJobRequestRequestTypeDef = TypedDict(
@@ -4960,37 +3564,14 @@
 
 class ListJobExecutionsForJobRequestRequestTypeDef(
     _RequiredListJobExecutionsForJobRequestRequestTypeDef,
     _OptionalListJobExecutionsForJobRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
-    "_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
-    "_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
-    {
-        "status": JobExecutionStatusType,
-        "namespaceId": str,
-        "jobId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef(
-    _RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
-    _OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobExecutionsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListJobExecutionsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListJobExecutionsForThingRequestRequestTypeDef = TypedDict(
@@ -5007,67 +3588,37 @@
 
 class ListJobExecutionsForThingRequestRequestTypeDef(
     _RequiredListJobExecutionsForThingRequestRequestTypeDef,
     _OptionalListJobExecutionsForThingRequestRequestTypeDef,
 ):
     pass
 
-ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
-    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListJobTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListJobsRequestListJobsPaginateTypeDef = TypedDict(
-    "ListJobsRequestListJobsPaginateTypeDef",
-    {
-        "status": JobStatusType,
-        "targetSelection": TargetSelectionType,
-        "thingGroupName": str,
-        "thingGroupId": str,
-        "namespaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListJobsRequestRequestTypeDef = TypedDict(
     "ListJobsRequestRequestTypeDef",
     {
         "status": JobStatusType,
         "targetSelection": TargetSelectionType,
         "maxResults": int,
         "nextToken": str,
         "thingGroupName": str,
         "thingGroupId": str,
         "namespaceId": str,
     },
     total=False,
 )
 
-ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef = TypedDict(
-    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
-    {
-        "templateName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedJobTemplatesRequestRequestTypeDef = TypedDict(
     "ListManagedJobTemplatesRequestRequestTypeDef",
     {
         "templateName": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -5082,39 +3633,14 @@
         "description": str,
         "environments": List[str],
         "templateVersion": str,
     },
     total=False,
 )
 
-_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
-    "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    {
-        "thingName": str,
-        "metricName": str,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
-    "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
-    {
-        "dimensionName": str,
-        "dimensionValueOperator": DimensionValueOperatorType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMetricValuesRequestListMetricValuesPaginateTypeDef(
-    _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef,
-    _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef,
-):
-    pass
-
 _RequiredListMetricValuesRequestRequestTypeDef = TypedDict(
     "_RequiredListMetricValuesRequestRequestTypeDef",
     {
         "thingName": str,
         "metricName": str,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
@@ -5132,23 +3658,14 @@
 )
 
 class ListMetricValuesRequestRequestTypeDef(
     _RequiredListMetricValuesRequestRequestTypeDef, _OptionalListMetricValuesRequestRequestTypeDef
 ):
     pass
 
-ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = TypedDict(
-    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
-    {
-        "actionType": MitigationActionTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMitigationActionsRequestRequestTypeDef = TypedDict(
     "ListMitigationActionsRequestRequestTypeDef",
     {
         "actionType": MitigationActionTypeType,
         "maxResults": int,
         "nextToken": str,
     },
@@ -5161,23 +3678,14 @@
         "actionName": str,
         "actionArn": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = TypedDict(
-    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
-    {
-        "otaUpdateStatus": OTAUpdateStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOTAUpdatesRequestRequestTypeDef = TypedDict(
     "ListOTAUpdatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "otaUpdateStatus": OTAUpdateStatusType,
     },
@@ -5190,23 +3698,14 @@
         "otaUpdateId": str,
         "otaUpdateArn": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = TypedDict(
-    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOutgoingCertificatesRequestRequestTypeDef = TypedDict(
     "ListOutgoingCertificatesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
@@ -5222,35 +3721,14 @@
         "transferDate": datetime,
         "transferMessage": str,
         "creationDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "packageName": str,
-    },
-)
-_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
-    {
-        "status": PackageVersionStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
-    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPackageVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListPackageVersionsRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalListPackageVersionsRequestRequestTypeDef = TypedDict(
@@ -5277,22 +3755,14 @@
         "status": PackageVersionStatusType,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
     },
     total=False,
 )
 
-ListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
-    "ListPackagesRequestListPackagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPackagesRequestRequestTypeDef = TypedDict(
     "ListPackagesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -5305,54 +3775,24 @@
         "defaultVersionName": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
     },
     total=False,
 )
 
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "marker": str,
         "pageSize": int,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
-    {
-        "policyName": str,
-    },
-)
-_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef(
-    _RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
-    _OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPolicyPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListPolicyPrincipalsRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListPolicyPrincipalsRequestRequestTypeDef = TypedDict(
@@ -5367,23 +3807,14 @@
 
 class ListPolicyPrincipalsRequestRequestTypeDef(
     _RequiredListPolicyPrincipalsRequestRequestTypeDef,
     _OptionalListPolicyPrincipalsRequestRequestTypeDef,
 ):
     pass
 
-ListPolicyPrincipalsResponseTypeDef = TypedDict(
-    "ListPolicyPrincipalsResponseTypeDef",
-    {
-        "principals": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListPolicyVersionsRequestRequestTypeDef = TypedDict(
     "ListPolicyVersionsRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 
@@ -5393,35 +3824,14 @@
         "versionId": str,
         "isDefaultVersion": bool,
         "createDate": datetime,
     },
     total=False,
 )
 
-_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
-    {
-        "principal": str,
-    },
-)
-_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef(
-    _RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
-    _OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListPrincipalPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalPoliciesRequestRequestTypeDef",
     {
         "principal": str,
     },
 )
 _OptionalListPrincipalPoliciesRequestRequestTypeDef = TypedDict(
@@ -5436,34 +3846,14 @@
 
 class ListPrincipalPoliciesRequestRequestTypeDef(
     _RequiredListPrincipalPoliciesRequestRequestTypeDef,
     _OptionalListPrincipalPoliciesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
-    "_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
-    {
-        "principal": str,
-    },
-)
-_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
-    "_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef(
-    _RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
-    _OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
-):
-    pass
-
 _RequiredListPrincipalThingsRequestRequestTypeDef = TypedDict(
     "_RequiredListPrincipalThingsRequestRequestTypeDef",
     {
         "principal": str,
     },
 )
 _OptionalListPrincipalThingsRequestRequestTypeDef = TypedDict(
@@ -5477,43 +3867,14 @@
 
 class ListPrincipalThingsRequestRequestTypeDef(
     _RequiredListPrincipalThingsRequestRequestTypeDef,
     _OptionalListPrincipalThingsRequestRequestTypeDef,
 ):
     pass
 
-ListPrincipalThingsResponseTypeDef = TypedDict(
-    "ListPrincipalThingsResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
-    {
-        "templateName": str,
-    },
-)
-_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef(
-    _RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
-    _OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListProvisioningTemplateVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListProvisioningTemplateVersionsRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalListProvisioningTemplateVersionsRequestRequestTypeDef = TypedDict(
@@ -5537,22 +3898,14 @@
         "versionId": int,
         "creationDate": datetime,
         "isDefaultVersion": bool,
     },
     total=False,
 )
 
-ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = TypedDict(
-    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListProvisioningTemplatesRequestRequestTypeDef = TypedDict(
     "ListProvisioningTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -5568,34 +3921,14 @@
         "lastModifiedDate": datetime,
         "enabled": bool,
         "type": TemplateTypeType,
     },
     total=False,
 )
 
-_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
-    "_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
-    {
-        "findingId": str,
-    },
-)
-_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
-    "_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef(
-    _RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
-    _OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
-):
-    pass
-
 _RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef = TypedDict(
     "_RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef",
     {
         "findingId": str,
     },
 )
 _OptionalListRelatedResourcesForAuditFindingRequestRequestTypeDef = TypedDict(
@@ -5609,50 +3942,24 @@
 
 class ListRelatedResourcesForAuditFindingRequestRequestTypeDef(
     _RequiredListRelatedResourcesForAuditFindingRequestRequestTypeDef,
     _OptionalListRelatedResourcesForAuditFindingRequestRequestTypeDef,
 ):
     pass
 
-ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = TypedDict(
-    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRoleAliasesRequestRequestTypeDef = TypedDict(
     "ListRoleAliasesRequestRequestTypeDef",
     {
         "pageSize": int,
         "marker": str,
         "ascendingOrder": bool,
     },
     total=False,
 )
 
-ListRoleAliasesResponseTypeDef = TypedDict(
-    "ListRoleAliasesResponseTypeDef",
-    {
-        "roleAliases": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = TypedDict(
-    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListScheduledAuditsRequestRequestTypeDef = TypedDict(
     "ListScheduledAuditsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -5666,39 +3973,14 @@
         "frequency": AuditFrequencyType,
         "dayOfMonth": str,
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
-_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
-        {
-            "securityProfileTargetArn": str,
-        },
-    )
-)
-_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
-        {
-            "recursive": bool,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef(
-    _RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
-    _OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
-):
-    pass
-
 _RequiredListSecurityProfilesForTargetRequestRequestTypeDef = TypedDict(
     "_RequiredListSecurityProfilesForTargetRequestRequestTypeDef",
     {
         "securityProfileTargetArn": str,
     },
 )
 _OptionalListSecurityProfilesForTargetRequestRequestTypeDef = TypedDict(
@@ -5713,24 +3995,14 @@
 
 class ListSecurityProfilesForTargetRequestRequestTypeDef(
     _RequiredListSecurityProfilesForTargetRequestRequestTypeDef,
     _OptionalListSecurityProfilesForTargetRequestRequestTypeDef,
 ):
     pass
 
-ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
-    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
-    {
-        "dimensionName": str,
-        "metricName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityProfilesRequestRequestTypeDef = TypedDict(
     "ListSecurityProfilesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "dimensionName": str,
         "metricName": str,
@@ -5742,23 +4014,14 @@
     "SecurityProfileIdentifierTypeDef",
     {
         "name": str,
         "arn": str,
     },
 )
 
-ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
-    "ListStreamsRequestListStreamsPaginateTypeDef",
-    {
-        "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStreamsRequestRequestTypeDef = TypedDict(
     "ListStreamsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "ascendingOrder": bool,
     },
@@ -5772,34 +4035,14 @@
         "streamArn": str,
         "streamVersion": int,
         "description": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -5812,51 +4055,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-_RequiredTagOutputTypeDef = TypedDict(
-    "_RequiredTagOutputTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalTagOutputTypeDef = TypedDict(
-    "_OptionalTagOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
-class TagOutputTypeDef(_RequiredTagOutputTypeDef, _OptionalTagOutputTypeDef):
-    pass
-
-_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
-    {
-        "policyName": str,
-    },
-)
-_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(
-    _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
-    _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
-):
-    pass
-
 _RequiredListTargetsForPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForPolicyRequestRequestTypeDef",
     {
         "policyName": str,
     },
 )
 _OptionalListTargetsForPolicyRequestRequestTypeDef = TypedDict(
@@ -5870,47 +4076,14 @@
 
 class ListTargetsForPolicyRequestRequestTypeDef(
     _RequiredListTargetsForPolicyRequestRequestTypeDef,
     _OptionalListTargetsForPolicyRequestRequestTypeDef,
 ):
     pass
 
-ListTargetsForPolicyResponseTypeDef = TypedDict(
-    "ListTargetsForPolicyResponseTypeDef",
-    {
-        "targets": List[str],
-        "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
-    TypedDict(
-        "_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
-        {
-            "securityProfileName": str,
-        },
-    )
-)
-_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
-    TypedDict(
-        "_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef(
-    _RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
-    _OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
-):
-    pass
-
 _RequiredListTargetsForSecurityProfileRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsForSecurityProfileRequestRequestTypeDef",
     {
         "securityProfileName": str,
     },
 )
 _OptionalListTargetsForSecurityProfileRequestRequestTypeDef = TypedDict(
@@ -5931,34 +4104,14 @@
 SecurityProfileTargetTypeDef = TypedDict(
     "SecurityProfileTargetTypeDef",
     {
         "arn": str,
     },
 )
 
-_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
-    "_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
-    "_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef(
-    _RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
-    _OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingGroupsForThingRequestRequestTypeDef = TypedDict(
     "_RequiredListThingGroupsForThingRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListThingGroupsForThingRequestRequestTypeDef = TypedDict(
@@ -5972,57 +4125,26 @@
 
 class ListThingGroupsForThingRequestRequestTypeDef(
     _RequiredListThingGroupsForThingRequestRequestTypeDef,
     _OptionalListThingGroupsForThingRequestRequestTypeDef,
 ):
     pass
 
-ListThingGroupsRequestListThingGroupsPaginateTypeDef = TypedDict(
-    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
-    {
-        "parentGroup": str,
-        "namePrefixFilter": str,
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingGroupsRequestRequestTypeDef = TypedDict(
     "ListThingGroupsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "parentGroup": str,
         "namePrefixFilter": str,
         "recursive": bool,
     },
     total=False,
 )
 
-_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
-    "_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
-    {
-        "thingName": str,
-    },
-)
-_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
-    "_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef(
-    _RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
-    _OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingPrincipalsRequestRequestTypeDef = TypedDict(
     "_RequiredListThingPrincipalsRequestRequestTypeDef",
     {
         "thingName": str,
     },
 )
 _OptionalListThingPrincipalsRequestRequestTypeDef = TypedDict(
@@ -6036,44 +4158,14 @@
 
 class ListThingPrincipalsRequestRequestTypeDef(
     _RequiredListThingPrincipalsRequestRequestTypeDef,
     _OptionalListThingPrincipalsRequestRequestTypeDef,
 ):
     pass
 
-ListThingPrincipalsResponseTypeDef = TypedDict(
-    "ListThingPrincipalsResponseTypeDef",
-    {
-        "principals": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
-    "_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
-    {
-        "taskId": str,
-        "reportType": ReportTypeType,
-    },
-)
-_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
-    "_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef(
-    _RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
-    _OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingRegistrationTaskReportsRequestRequestTypeDef = TypedDict(
     "_RequiredListThingRegistrationTaskReportsRequestRequestTypeDef",
     {
         "taskId": str,
         "reportType": ReportTypeType,
     },
 )
@@ -6088,91 +4180,34 @@
 
 class ListThingRegistrationTaskReportsRequestRequestTypeDef(
     _RequiredListThingRegistrationTaskReportsRequestRequestTypeDef,
     _OptionalListThingRegistrationTaskReportsRequestRequestTypeDef,
 ):
     pass
 
-ListThingRegistrationTaskReportsResponseTypeDef = TypedDict(
-    "ListThingRegistrationTaskReportsResponseTypeDef",
-    {
-        "resourceLinks": List[str],
-        "reportType": ReportTypeType,
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = TypedDict(
-    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
-    {
-        "status": StatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingRegistrationTasksRequestRequestTypeDef = TypedDict(
     "ListThingRegistrationTasksRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "status": StatusType,
     },
     total=False,
 )
 
-ListThingRegistrationTasksResponseTypeDef = TypedDict(
-    "ListThingRegistrationTasksResponseTypeDef",
-    {
-        "taskIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingTypesRequestListThingTypesPaginateTypeDef = TypedDict(
-    "ListThingTypesRequestListThingTypesPaginateTypeDef",
-    {
-        "thingTypeName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingTypesRequestRequestTypeDef = TypedDict(
     "ListThingTypesRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "thingTypeName": str,
     },
     total=False,
 )
 
-_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
-    "_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
-    {
-        "billingGroupName": str,
-    },
-)
-_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
-    "_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef(
-    _RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
-    _OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingsInBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListThingsInBillingGroupRequestRequestTypeDef",
     {
         "billingGroupName": str,
     },
 )
 _OptionalListThingsInBillingGroupRequestRequestTypeDef = TypedDict(
@@ -6186,44 +4221,14 @@
 
 class ListThingsInBillingGroupRequestRequestTypeDef(
     _RequiredListThingsInBillingGroupRequestRequestTypeDef,
     _OptionalListThingsInBillingGroupRequestRequestTypeDef,
 ):
     pass
 
-ListThingsInBillingGroupResponseTypeDef = TypedDict(
-    "ListThingsInBillingGroupResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
-    "_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
-    {
-        "thingGroupName": str,
-    },
-)
-_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
-    "_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
-    {
-        "recursive": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef(
-    _RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
-    _OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
-):
-    pass
-
 _RequiredListThingsInThingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListThingsInThingGroupRequestRequestTypeDef",
     {
         "thingGroupName": str,
     },
 )
 _OptionalListThingsInThingGroupRequestRequestTypeDef = TypedDict(
@@ -6238,35 +4243,14 @@
 
 class ListThingsInThingGroupRequestRequestTypeDef(
     _RequiredListThingsInThingGroupRequestRequestTypeDef,
     _OptionalListThingsInThingGroupRequestRequestTypeDef,
 ):
     pass
 
-ListThingsInThingGroupResponseTypeDef = TypedDict(
-    "ListThingsInThingGroupResponseTypeDef",
-    {
-        "things": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListThingsRequestListThingsPaginateTypeDef = TypedDict(
-    "ListThingsRequestListThingsPaginateTypeDef",
-    {
-        "attributeName": str,
-        "attributeValue": str,
-        "thingTypeName": str,
-        "usePrefixAttributeValue": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListThingsRequestRequestTypeDef = TypedDict(
     "ListThingsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "attributeName": str,
         "attributeValue": str,
@@ -6284,41 +4268,23 @@
         "thingArn": str,
         "attributes": Dict[str, str],
         "version": int,
     },
     total=False,
 )
 
-ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = TypedDict(
-    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTopicRuleDestinationsRequestRequestTypeDef = TypedDict(
     "ListTopicRuleDestinationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListTopicRulesRequestListTopicRulesPaginateTypeDef = TypedDict(
-    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
-    {
-        "topic": str,
-        "ruleDisabled": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTopicRulesRequestRequestTypeDef = TypedDict(
     "ListTopicRulesRequestRequestTypeDef",
     {
         "topic": str,
         "maxResults": int,
         "nextToken": str,
         "ruleDisabled": bool,
@@ -6334,59 +4300,24 @@
         "topicPattern": str,
         "createdAt": datetime,
         "ruleDisabled": bool,
     },
     total=False,
 )
 
-ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = TypedDict(
-    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
-    {
-        "targetType": LogTargetTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListV2LoggingLevelsRequestRequestTypeDef = TypedDict(
     "ListV2LoggingLevelsRequestRequestTypeDef",
     {
         "targetType": LogTargetTypeType,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
-    "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    {
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
-    "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
-    {
-        "thingName": str,
-        "securityProfileName": str,
-        "behaviorCriteriaType": BehaviorCriteriaTypeType,
-        "listSuppressedAlerts": bool,
-        "verificationState": VerificationStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListViolationEventsRequestListViolationEventsPaginateTypeDef(
-    _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef,
-    _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredListViolationEventsRequestRequestTypeDef = TypedDict(
     "_RequiredListViolationEventsRequestRequestTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
@@ -6406,33 +4337,14 @@
 
 class ListViolationEventsRequestRequestTypeDef(
     _RequiredListViolationEventsRequestRequestTypeDef,
     _OptionalListViolationEventsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredLocationTimestampOutputTypeDef = TypedDict(
-    "_RequiredLocationTimestampOutputTypeDef",
-    {
-        "value": str,
-    },
-)
-_OptionalLocationTimestampOutputTypeDef = TypedDict(
-    "_OptionalLocationTimestampOutputTypeDef",
-    {
-        "unit": str,
-    },
-    total=False,
-)
-
-class LocationTimestampOutputTypeDef(
-    _RequiredLocationTimestampOutputTypeDef, _OptionalLocationTimestampOutputTypeDef
-):
-    pass
-
 _RequiredLocationTimestampTypeDef = TypedDict(
     "_RequiredLocationTimestampTypeDef",
     {
         "value": str,
     },
 )
 _OptionalLocationTimestampTypeDef = TypedDict(
@@ -6444,31 +4356,14 @@
 )
 
 class LocationTimestampTypeDef(
     _RequiredLocationTimestampTypeDef, _OptionalLocationTimestampTypeDef
 ):
     pass
 
-_RequiredLogTargetOutputTypeDef = TypedDict(
-    "_RequiredLogTargetOutputTypeDef",
-    {
-        "targetType": LogTargetTypeType,
-    },
-)
-_OptionalLogTargetOutputTypeDef = TypedDict(
-    "_OptionalLogTargetOutputTypeDef",
-    {
-        "targetName": str,
-    },
-    total=False,
-)
-
-class LogTargetOutputTypeDef(_RequiredLogTargetOutputTypeDef, _OptionalLogTargetOutputTypeDef):
-    pass
-
 _RequiredLogTargetTypeDef = TypedDict(
     "_RequiredLogTargetTypeDef",
     {
         "targetType": LogTargetTypeType,
     },
 )
 _OptionalLogTargetTypeDef = TypedDict(
@@ -6497,42 +4392,14 @@
 )
 
 class LoggingOptionsPayloadTypeDef(
     _RequiredLoggingOptionsPayloadTypeDef, _OptionalLoggingOptionsPayloadTypeDef
 ):
     pass
 
-PublishFindingToSnsParamsOutputTypeDef = TypedDict(
-    "PublishFindingToSnsParamsOutputTypeDef",
-    {
-        "topicArn": str,
-    },
-)
-
-ReplaceDefaultPolicyVersionParamsOutputTypeDef = TypedDict(
-    "ReplaceDefaultPolicyVersionParamsOutputTypeDef",
-    {
-        "templateName": Literal["BLANK_POLICY"],
-    },
-)
-
-UpdateCACertificateParamsOutputTypeDef = TypedDict(
-    "UpdateCACertificateParamsOutputTypeDef",
-    {
-        "action": Literal["DEACTIVATE"],
-    },
-)
-
-UpdateDeviceCertificateParamsOutputTypeDef = TypedDict(
-    "UpdateDeviceCertificateParamsOutputTypeDef",
-    {
-        "action": Literal["DEACTIVATE"],
-    },
-)
-
 PublishFindingToSnsParamsTypeDef = TypedDict(
     "PublishFindingToSnsParamsTypeDef",
     {
         "topicArn": str,
     },
 )
 
@@ -6563,49 +4430,22 @@
         "username": str,
         "password": Union[str, bytes, IO[Any], StreamingBody],
         "clientId": str,
     },
     total=False,
 )
 
-UserPropertyOutputTypeDef = TypedDict(
-    "UserPropertyOutputTypeDef",
-    {
-        "key": str,
-        "value": str,
-    },
-)
-
 UserPropertyTypeDef = TypedDict(
     "UserPropertyTypeDef",
     {
         "key": str,
         "value": str,
     },
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
-PolicyVersionIdentifierOutputTypeDef = TypedDict(
-    "PolicyVersionIdentifierOutputTypeDef",
-    {
-        "policyName": str,
-        "policyVersionId": str,
-    },
-    total=False,
-)
-
 PolicyVersionIdentifierTypeDef = TypedDict(
     "PolicyVersionIdentifierTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
     total=False,
@@ -6628,33 +4468,14 @@
 
 class PutVerificationStateOnViolationRequestRequestTypeDef(
     _RequiredPutVerificationStateOnViolationRequestRequestTypeDef,
     _OptionalPutVerificationStateOnViolationRequestRequestTypeDef,
 ):
     pass
 
-RegistrationConfigTypeDef = TypedDict(
-    "RegistrationConfigTypeDef",
-    {
-        "templateBody": str,
-        "roleArn": str,
-        "templateName": str,
-    },
-    total=False,
-)
-
-RegisterCACertificateResponseTypeDef = TypedDict(
-    "RegisterCACertificateResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateRequestRequestTypeDef",
     {
         "certificatePem": str,
     },
 )
 _OptionalRegisterCertificateRequestRequestTypeDef = TypedDict(
@@ -6669,23 +4490,14 @@
 
 class RegisterCertificateRequestRequestTypeDef(
     _RequiredRegisterCertificateRequestRequestTypeDef,
     _OptionalRegisterCertificateRequestRequestTypeDef,
 ):
     pass
 
-RegisterCertificateResponseTypeDef = TypedDict(
-    "RegisterCertificateResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterCertificateWithoutCARequestRequestTypeDef = TypedDict(
     "_RequiredRegisterCertificateWithoutCARequestRequestTypeDef",
     {
         "certificatePem": str,
     },
 )
 _OptionalRegisterCertificateWithoutCARequestRequestTypeDef = TypedDict(
@@ -6698,23 +4510,14 @@
 
 class RegisterCertificateWithoutCARequestRequestTypeDef(
     _RequiredRegisterCertificateWithoutCARequestRequestTypeDef,
     _OptionalRegisterCertificateWithoutCARequestRequestTypeDef,
 ):
     pass
 
-RegisterCertificateWithoutCAResponseTypeDef = TypedDict(
-    "RegisterCertificateWithoutCAResponseTypeDef",
-    {
-        "certificateArn": str,
-        "certificateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRegisterThingRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterThingRequestRequestTypeDef",
     {
         "templateBody": str,
     },
 )
 _OptionalRegisterThingRequestRequestTypeDef = TypedDict(
@@ -6726,23 +4529,14 @@
 )
 
 class RegisterThingRequestRequestTypeDef(
     _RequiredRegisterThingRequestRequestTypeDef, _OptionalRegisterThingRequestRequestTypeDef
 ):
     pass
 
-RegisterThingResponseTypeDef = TypedDict(
-    "RegisterThingResponseTypeDef",
-    {
-        "certificatePem": str,
-        "resourceArns": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRejectCertificateTransferRequestRequestTypeDef = TypedDict(
     "_RequiredRejectCertificateTransferRequestRequestTypeDef",
     {
         "certificateId": str,
     },
 )
 _OptionalRejectCertificateTransferRequestRequestTypeDef = TypedDict(
@@ -6777,25 +4571,14 @@
         "thingGroupArn": str,
         "thingName": str,
         "thingArn": str,
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
 _RequiredSearchIndexRequestRequestTypeDef = TypedDict(
     "_RequiredSearchIndexRequestRequestTypeDef",
     {
         "queryString": str,
     },
 )
 _OptionalSearchIndexRequestRequestTypeDef = TypedDict(
@@ -6829,23 +4612,14 @@
 SetDefaultAuthorizerRequestRequestTypeDef = TypedDict(
     "SetDefaultAuthorizerRequestRequestTypeDef",
     {
         "authorizerName": str,
     },
 )
 
-SetDefaultAuthorizerResponseTypeDef = TypedDict(
-    "SetDefaultAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SetDefaultPolicyVersionRequestRequestTypeDef = TypedDict(
     "SetDefaultPolicyVersionRequestRequestTypeDef",
     {
         "policyName": str,
         "policyVersionId": str,
     },
 )
@@ -6856,91 +4630,49 @@
         "roleArn": str,
         "defaultLogLevel": LogLevelType,
         "disableAllLogs": bool,
     },
     total=False,
 )
 
-SigningProfileParameterOutputTypeDef = TypedDict(
-    "SigningProfileParameterOutputTypeDef",
-    {
-        "certificateArn": str,
-        "platform": str,
-        "certificatePathOnDevice": str,
-    },
-    total=False,
-)
-
 SigningProfileParameterTypeDef = TypedDict(
     "SigningProfileParameterTypeDef",
     {
         "certificateArn": str,
         "platform": str,
         "certificatePathOnDevice": str,
     },
     total=False,
 )
 
-StartAuditMitigationActionsTaskResponseTypeDef = TypedDict(
-    "StartAuditMitigationActionsTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ViolationEventOccurrenceRangeTypeDef = TypedDict(
     "ViolationEventOccurrenceRangeTypeDef",
     {
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
     },
 )
 
-StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
-    "StartDetectMitigationActionsTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartOnDemandAuditTaskRequestRequestTypeDef = TypedDict(
     "StartOnDemandAuditTaskRequestRequestTypeDef",
     {
         "targetCheckNames": Sequence[str],
     },
 )
 
-StartOnDemandAuditTaskResponseTypeDef = TypedDict(
-    "StartOnDemandAuditTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "StartThingRegistrationTaskRequestRequestTypeDef",
     {
         "templateBody": str,
         "inputFileBucket": str,
         "inputFileKey": str,
         "roleArn": str,
     },
 )
 
-StartThingRegistrationTaskResponseTypeDef = TypedDict(
-    "StartThingRegistrationTaskResponseTypeDef",
-    {
-        "taskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopThingRegistrationTaskRequestRequestTypeDef = TypedDict(
     "StopThingRegistrationTaskRequestRequestTypeDef",
     {
         "taskId": str,
     },
 )
 
@@ -6948,52 +4680,24 @@
     "TlsContextTypeDef",
     {
         "serverName": str,
     },
     total=False,
 )
 
-TestInvokeAuthorizerResponseTypeDef = TypedDict(
-    "TestInvokeAuthorizerResponseTypeDef",
-    {
-        "isAuthenticated": bool,
-        "principalId": str,
-        "policyDocuments": List[str],
-        "refreshAfterInSeconds": int,
-        "disconnectAfterInSeconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ThingConnectivityTypeDef = TypedDict(
     "ThingConnectivityTypeDef",
     {
         "connected": bool,
         "timestamp": int,
         "disconnectReason": str,
     },
     total=False,
 )
 
-TimestreamDimensionOutputTypeDef = TypedDict(
-    "TimestreamDimensionOutputTypeDef",
-    {
-        "name": str,
-        "value": str,
-    },
-)
-
-TimestreamTimestampOutputTypeDef = TypedDict(
-    "TimestreamTimestampOutputTypeDef",
-    {
-        "value": str,
-        "unit": str,
-    },
-)
-
 TimestreamDimensionTypeDef = TypedDict(
     "TimestreamDimensionTypeDef",
     {
         "name": str,
         "value": str,
     },
 )
@@ -7066,22 +4770,14 @@
 
 class TransferCertificateRequestRequestTypeDef(
     _RequiredTransferCertificateRequestRequestTypeDef,
     _OptionalTransferCertificateRequestRequestTypeDef,
 ):
     pass
 
-TransferCertificateResponseTypeDef = TypedDict(
-    "TransferCertificateResponseTypeDef",
-    {
-        "transferredCertificateArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -7105,31 +4801,14 @@
 )
 
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
-    {
-        "authorizerName": str,
-        "authorizerArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateBillingGroupResponseTypeDef = TypedDict(
-    "UpdateBillingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCertificateRequestRequestTypeDef = TypedDict(
     "UpdateCertificateRequestRequestTypeDef",
     {
         "certificateId": str,
         "newStatus": CertificateStatusType,
     },
 )
@@ -7138,83 +4817,22 @@
     "UpdateCustomMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "displayName": str,
     },
 )
 
-UpdateCustomMetricResponseTypeDef = TypedDict(
-    "UpdateCustomMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "metricArn": str,
-        "metricType": CustomMetricTypeType,
-        "displayName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDimensionRequestRequestTypeDef = TypedDict(
     "UpdateDimensionRequestRequestTypeDef",
     {
         "name": str,
         "stringValues": Sequence[str],
     },
 )
 
-UpdateDimensionResponseTypeDef = TypedDict(
-    "UpdateDimensionResponseTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "type": Literal["TOPIC_FILTER"],
-        "stringValues": List[str],
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDomainConfigurationResponseTypeDef = TypedDict(
-    "UpdateDomainConfigurationResponseTypeDef",
-    {
-        "domainConfigurationName": str,
-        "domainConfigurationArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateDynamicThingGroupResponseTypeDef = TypedDict(
-    "UpdateDynamicThingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMitigationActionResponseTypeDef = TypedDict(
-    "UpdateMitigationActionResponseTypeDef",
-    {
-        "actionArn": str,
-        "actionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-VersionUpdateByJobsConfigTypeDef = TypedDict(
-    "VersionUpdateByJobsConfigTypeDef",
-    {
-        "enabled": bool,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 _RequiredUpdatePackageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePackageRequestRequestTypeDef",
     {
         "packageName": str,
     },
 )
 _OptionalUpdatePackageRequestRequestTypeDef = TypedDict(
@@ -7273,23 +4891,14 @@
 )
 
 class UpdateRoleAliasRequestRequestTypeDef(
     _RequiredUpdateRoleAliasRequestRequestTypeDef, _OptionalUpdateRoleAliasRequestRequestTypeDef
 ):
     pass
 
-UpdateRoleAliasResponseTypeDef = TypedDict(
-    "UpdateRoleAliasResponseTypeDef",
-    {
-        "roleAlias": str,
-        "roleAliasArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateScheduledAuditRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateScheduledAuditRequestRequestTypeDef",
     {
         "scheduledAuditName": str,
     },
 )
 _OptionalUpdateScheduledAuditRequestRequestTypeDef = TypedDict(
@@ -7305,41 +4914,14 @@
 
 class UpdateScheduledAuditRequestRequestTypeDef(
     _RequiredUpdateScheduledAuditRequestRequestTypeDef,
     _OptionalUpdateScheduledAuditRequestRequestTypeDef,
 ):
     pass
 
-UpdateScheduledAuditResponseTypeDef = TypedDict(
-    "UpdateScheduledAuditResponseTypeDef",
-    {
-        "scheduledAuditArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateStreamResponseTypeDef = TypedDict(
-    "UpdateStreamResponseTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "description": str,
-        "streamVersion": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateThingGroupResponseTypeDef = TypedDict(
-    "UpdateThingGroupResponseTypeDef",
-    {
-        "version": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateThingGroupsForThingRequestRequestTypeDef = TypedDict(
     "UpdateThingGroupsForThingRequestRequestTypeDef",
     {
         "thingName": str,
         "thingGroupsToAdd": Sequence[str],
         "thingGroupsToRemove": Sequence[str],
         "overrideDynamicGroups": bool,
@@ -7362,15 +4944,15 @@
     },
     total=False,
 )
 
 AbortConfigOutputTypeDef = TypedDict(
     "AbortConfigOutputTypeDef",
     {
-        "criteriaList": List[AbortCriteriaOutputTypeDef],
+        "criteriaList": List[AbortCriteriaTypeDef],
     },
 )
 
 AbortConfigTypeDef = TypedDict(
     "AbortConfigTypeDef",
     {
         "criteriaList": Sequence[AbortCriteriaTypeDef],
@@ -7382,34 +4964,14 @@
     {
         "timestamp": datetime,
         "value": MetricValueOutputTypeDef,
     },
     total=False,
 )
 
-DescribeFleetMetricResponseTypeDef = TypedDict(
-    "DescribeFleetMetricResponseTypeDef",
-    {
-        "metricName": str,
-        "queryString": str,
-        "aggregationType": AggregationTypeOutputTypeDef,
-        "period": int,
-        "aggregationField": str,
-        "description": str,
-        "queryVersion": str,
-        "indexName": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "unit": FleetMetricUnitType,
-        "version": int,
-        "metricArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFleetMetricRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFleetMetricRequestRequestTypeDef",
     {
         "metricName": str,
         "indexName": str,
     },
 )
@@ -7453,80 +5015,873 @@
     "ImplicitDenyTypeDef",
     {
         "policies": List[PolicyTypeDef],
     },
     total=False,
 )
 
+_RequiredAssetPropertyValueTypeDef = TypedDict(
+    "_RequiredAssetPropertyValueTypeDef",
+    {
+        "value": AssetPropertyVariantTypeDef,
+        "timestamp": AssetPropertyTimestampTypeDef,
+    },
+)
+_OptionalAssetPropertyValueTypeDef = TypedDict(
+    "_OptionalAssetPropertyValueTypeDef",
+    {
+        "quality": str,
+    },
+    total=False,
+)
+
+class AssetPropertyValueTypeDef(
+    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
+):
+    pass
+
+AssociateTargetsWithJobResponseTypeDef = TypedDict(
+    "AssociateTargetsWithJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelJobResponseTypeDef = TypedDict(
+    "CancelJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBillingGroupResponseTypeDef = TypedDict(
+    "CreateBillingGroupResponseTypeDef",
+    {
+        "billingGroupName": str,
+        "billingGroupArn": str,
+        "billingGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCertificateFromCsrResponseTypeDef = TypedDict(
+    "CreateCertificateFromCsrResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "certificatePem": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomMetricResponseTypeDef = TypedDict(
+    "CreateCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDimensionResponseTypeDef = TypedDict(
+    "CreateDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainConfigurationResponseTypeDef = TypedDict(
+    "CreateDomainConfigurationResponseTypeDef",
+    {
+        "domainConfigurationName": str,
+        "domainConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDynamicThingGroupResponseTypeDef = TypedDict(
+    "CreateDynamicThingGroupResponseTypeDef",
+    {
+        "thingGroupName": str,
+        "thingGroupArn": str,
+        "thingGroupId": str,
+        "indexName": str,
+        "queryString": str,
+        "queryVersion": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFleetMetricResponseTypeDef = TypedDict(
+    "CreateFleetMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobResponseTypeDef = TypedDict(
+    "CreateJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateJobTemplateResponseTypeDef = TypedDict(
+    "CreateJobTemplateResponseTypeDef",
+    {
+        "jobTemplateArn": str,
+        "jobTemplateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMitigationActionResponseTypeDef = TypedDict(
+    "CreateMitigationActionResponseTypeDef",
+    {
+        "actionArn": str,
+        "actionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateOTAUpdateResponseTypeDef = TypedDict(
+    "CreateOTAUpdateResponseTypeDef",
+    {
+        "otaUpdateId": str,
+        "awsIotJobId": str,
+        "otaUpdateArn": str,
+        "awsIotJobArn": str,
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageResponseTypeDef = TypedDict(
+    "CreatePackageResponseTypeDef",
+    {
+        "packageName": str,
+        "packageArn": str,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePackageVersionResponseTypeDef = TypedDict(
+    "CreatePackageVersionResponseTypeDef",
+    {
+        "packageVersionArn": str,
+        "packageName": str,
+        "versionName": str,
+        "description": str,
+        "attributes": Dict[str, str],
+        "status": PackageVersionStatusType,
+        "errorReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyResponseTypeDef = TypedDict(
+    "CreatePolicyResponseTypeDef",
+    {
+        "policyName": str,
+        "policyArn": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePolicyVersionResponseTypeDef = TypedDict(
+    "CreatePolicyVersionResponseTypeDef",
+    {
+        "policyArn": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisioningTemplateResponseTypeDef = TypedDict(
+    "CreateProvisioningTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "defaultVersionId": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateProvisioningTemplateVersionResponseTypeDef = TypedDict(
+    "CreateProvisioningTemplateVersionResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "versionId": int,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRoleAliasResponseTypeDef = TypedDict(
+    "CreateRoleAliasResponseTypeDef",
+    {
+        "roleAlias": str,
+        "roleAliasArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduledAuditResponseTypeDef = TypedDict(
+    "CreateScheduledAuditResponseTypeDef",
+    {
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSecurityProfileResponseTypeDef = TypedDict(
+    "CreateSecurityProfileResponseTypeDef",
+    {
+        "securityProfileName": str,
+        "securityProfileArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamResponseTypeDef = TypedDict(
+    "CreateStreamResponseTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "description": str,
+        "streamVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingGroupResponseTypeDef = TypedDict(
+    "CreateThingGroupResponseTypeDef",
+    {
+        "thingGroupName": str,
+        "thingGroupArn": str,
+        "thingGroupId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingResponseTypeDef = TypedDict(
+    "CreateThingResponseTypeDef",
+    {
+        "thingName": str,
+        "thingArn": str,
+        "thingId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThingTypeResponseTypeDef = TypedDict(
+    "CreateThingTypeResponseTypeDef",
+    {
+        "thingTypeName": str,
+        "thingTypeArn": str,
+        "thingTypeId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCustomMetricResponseTypeDef = TypedDict(
+    "DescribeCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "metricType": CustomMetricTypeType,
+        "displayName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDimensionResponseTypeDef = TypedDict(
+    "DescribeDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "type": Literal["TOPIC_FILTER"],
+        "stringValues": List[str],
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEndpointResponseTypeDef = TypedDict(
+    "DescribeEndpointResponseTypeDef",
+    {
+        "endpointAddress": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeFleetMetricResponseTypeDef = TypedDict(
+    "DescribeFleetMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "queryString": str,
+        "aggregationType": AggregationTypeOutputTypeDef,
+        "period": int,
+        "aggregationField": str,
+        "description": str,
+        "queryVersion": str,
+        "indexName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "unit": FleetMetricUnitType,
+        "version": int,
+        "metricArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeIndexResponseTypeDef = TypedDict(
+    "DescribeIndexResponseTypeDef",
+    {
+        "indexName": str,
+        "indexStatus": IndexStatusType,
+        "schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeProvisioningTemplateVersionResponseTypeDef = TypedDict(
+    "DescribeProvisioningTemplateVersionResponseTypeDef",
+    {
+        "versionId": int,
+        "creationDate": datetime,
+        "templateBody": str,
+        "isDefaultVersion": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeScheduledAuditResponseTypeDef = TypedDict(
+    "DescribeScheduledAuditResponseTypeDef",
+    {
+        "frequency": AuditFrequencyType,
+        "dayOfMonth": str,
+        "dayOfWeek": DayOfWeekType,
+        "targetCheckNames": List[str],
+        "scheduledAuditName": str,
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThingRegistrationTaskResponseTypeDef = TypedDict(
+    "DescribeThingRegistrationTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "templateBody": str,
+        "inputFileBucket": str,
+        "inputFileKey": str,
+        "roleArn": str,
+        "status": StatusType,
+        "message": str,
+        "successCount": int,
+        "failureCount": int,
+        "percentageProgress": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeThingResponseTypeDef = TypedDict(
+    "DescribeThingResponseTypeDef",
+    {
+        "defaultClientId": str,
+        "thingName": str,
+        "thingId": str,
+        "thingArn": str,
+        "thingTypeName": str,
+        "attributes": Dict[str, str],
+        "version": int,
+        "billingGroupName": str,
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
+GetCardinalityResponseTypeDef = TypedDict(
+    "GetCardinalityResponseTypeDef",
+    {
+        "cardinality": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetJobDocumentResponseTypeDef = TypedDict(
+    "GetJobDocumentResponseTypeDef",
+    {
+        "document": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetLoggingOptionsResponseTypeDef = TypedDict(
+    "GetLoggingOptionsResponseTypeDef",
+    {
+        "roleArn": str,
+        "logLevel": LogLevelType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageResponseTypeDef = TypedDict(
+    "GetPackageResponseTypeDef",
+    {
+        "packageName": str,
+        "packageArn": str,
+        "description": str,
+        "defaultVersionName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPackageVersionResponseTypeDef = TypedDict(
+    "GetPackageVersionResponseTypeDef",
+    {
+        "packageVersionArn": str,
+        "packageName": str,
+        "versionName": str,
+        "description": str,
+        "attributes": Dict[str, str],
+        "status": PackageVersionStatusType,
+        "errorReason": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyResponseTypeDef = TypedDict(
+    "GetPolicyResponseTypeDef",
+    {
+        "policyName": str,
+        "policyArn": str,
+        "policyDocument": str,
+        "defaultVersionId": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "generationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetPolicyVersionResponseTypeDef = TypedDict(
+    "GetPolicyVersionResponseTypeDef",
+    {
+        "policyArn": str,
+        "policyName": str,
+        "policyDocument": str,
+        "policyVersionId": str,
+        "isDefaultVersion": bool,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "generationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetRegistrationCodeResponseTypeDef = TypedDict(
+    "GetRegistrationCodeResponseTypeDef",
+    {
+        "registrationCode": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetV2LoggingOptionsResponseTypeDef = TypedDict(
+    "GetV2LoggingOptionsResponseTypeDef",
+    {
+        "roleArn": str,
+        "defaultLogLevel": LogLevelType,
+        "disableAllLogs": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAttachedPoliciesResponseTypeDef = TypedDict(
     "ListAttachedPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCustomMetricsResponseTypeDef = TypedDict(
+    "ListCustomMetricsResponseTypeDef",
+    {
+        "metricNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDimensionsResponseTypeDef = TypedDict(
+    "ListDimensionsResponseTypeDef",
+    {
+        "dimensionNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndicesResponseTypeDef = TypedDict(
+    "ListIndicesResponseTypeDef",
+    {
+        "indexNames": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPoliciesResponseTypeDef = TypedDict(
     "ListPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListPolicyPrincipalsResponseTypeDef = TypedDict(
+    "ListPolicyPrincipalsResponseTypeDef",
+    {
+        "principals": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPrincipalPoliciesResponseTypeDef = TypedDict(
     "ListPrincipalPoliciesResponseTypeDef",
     {
         "policies": List[PolicyTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAssetPropertyValueOutputTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueOutputTypeDef",
+ListPrincipalThingsResponseTypeDef = TypedDict(
+    "ListPrincipalThingsResponseTypeDef",
     {
-        "value": AssetPropertyVariantOutputTypeDef,
-        "timestamp": AssetPropertyTimestampOutputTypeDef,
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssetPropertyValueOutputTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueOutputTypeDef",
+
+ListRoleAliasesResponseTypeDef = TypedDict(
+    "ListRoleAliasesResponseTypeDef",
     {
-        "quality": str,
+        "roleAliases": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AssetPropertyValueOutputTypeDef(
-    _RequiredAssetPropertyValueOutputTypeDef, _OptionalAssetPropertyValueOutputTypeDef
-):
-    pass
+ListTargetsForPolicyResponseTypeDef = TypedDict(
+    "ListTargetsForPolicyResponseTypeDef",
+    {
+        "targets": List[str],
+        "nextMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-_RequiredAssetPropertyValueTypeDef = TypedDict(
-    "_RequiredAssetPropertyValueTypeDef",
+ListThingPrincipalsResponseTypeDef = TypedDict(
+    "ListThingPrincipalsResponseTypeDef",
     {
-        "value": AssetPropertyVariantTypeDef,
-        "timestamp": AssetPropertyTimestampTypeDef,
+        "principals": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalAssetPropertyValueTypeDef = TypedDict(
-    "_OptionalAssetPropertyValueTypeDef",
+
+ListThingRegistrationTaskReportsResponseTypeDef = TypedDict(
+    "ListThingRegistrationTaskReportsResponseTypeDef",
     {
-        "quality": str,
+        "resourceLinks": List[str],
+        "reportType": ReportTypeType,
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AssetPropertyValueTypeDef(
-    _RequiredAssetPropertyValueTypeDef, _OptionalAssetPropertyValueTypeDef
-):
-    pass
+ListThingRegistrationTasksResponseTypeDef = TypedDict(
+    "ListThingRegistrationTasksResponseTypeDef",
+    {
+        "taskIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingsInBillingGroupResponseTypeDef = TypedDict(
+    "ListThingsInBillingGroupResponseTypeDef",
+    {
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListThingsInThingGroupResponseTypeDef = TypedDict(
+    "ListThingsInThingGroupResponseTypeDef",
+    {
+        "things": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCACertificateResponseTypeDef = TypedDict(
+    "RegisterCACertificateResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateResponseTypeDef = TypedDict(
+    "RegisterCertificateResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterCertificateWithoutCAResponseTypeDef = TypedDict(
+    "RegisterCertificateWithoutCAResponseTypeDef",
+    {
+        "certificateArn": str,
+        "certificateId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RegisterThingResponseTypeDef = TypedDict(
+    "RegisterThingResponseTypeDef",
+    {
+        "certificatePem": str,
+        "resourceArns": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SetDefaultAuthorizerResponseTypeDef = TypedDict(
+    "SetDefaultAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartAuditMitigationActionsTaskResponseTypeDef = TypedDict(
+    "StartAuditMitigationActionsTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDetectMitigationActionsTaskResponseTypeDef = TypedDict(
+    "StartDetectMitigationActionsTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartOnDemandAuditTaskResponseTypeDef = TypedDict(
+    "StartOnDemandAuditTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartThingRegistrationTaskResponseTypeDef = TypedDict(
+    "StartThingRegistrationTaskResponseTypeDef",
+    {
+        "taskId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestInvokeAuthorizerResponseTypeDef = TypedDict(
+    "TestInvokeAuthorizerResponseTypeDef",
+    {
+        "isAuthenticated": bool,
+        "principalId": str,
+        "policyDocuments": List[str],
+        "refreshAfterInSeconds": int,
+        "disconnectAfterInSeconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TransferCertificateResponseTypeDef = TypedDict(
+    "TransferCertificateResponseTypeDef",
+    {
+        "transferredCertificateArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
+    {
+        "authorizerName": str,
+        "authorizerArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBillingGroupResponseTypeDef = TypedDict(
+    "UpdateBillingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCustomMetricResponseTypeDef = TypedDict(
+    "UpdateCustomMetricResponseTypeDef",
+    {
+        "metricName": str,
+        "metricArn": str,
+        "metricType": CustomMetricTypeType,
+        "displayName": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDimensionResponseTypeDef = TypedDict(
+    "UpdateDimensionResponseTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "type": Literal["TOPIC_FILTER"],
+        "stringValues": List[str],
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDomainConfigurationResponseTypeDef = TypedDict(
+    "UpdateDomainConfigurationResponseTypeDef",
+    {
+        "domainConfigurationName": str,
+        "domainConfigurationArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDynamicThingGroupResponseTypeDef = TypedDict(
+    "UpdateDynamicThingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMitigationActionResponseTypeDef = TypedDict(
+    "UpdateMitigationActionResponseTypeDef",
+    {
+        "actionArn": str,
+        "actionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRoleAliasResponseTypeDef = TypedDict(
+    "UpdateRoleAliasResponseTypeDef",
+    {
+        "roleAlias": str,
+        "roleAliasArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateScheduledAuditResponseTypeDef = TypedDict(
+    "UpdateScheduledAuditResponseTypeDef",
+    {
+        "scheduledAuditArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateStreamResponseTypeDef = TypedDict(
+    "UpdateStreamResponseTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "description": str,
+        "streamVersion": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateThingGroupResponseTypeDef = TypedDict(
+    "UpdateThingGroupResponseTypeDef",
+    {
+        "version": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ThingGroupPropertiesOutputTypeDef = TypedDict(
     "ThingGroupPropertiesOutputTypeDef",
     {
         "thingGroupDescription": str,
         "attributePayload": AttributePayloadOutputTypeDef,
     },
@@ -7586,24 +5941,24 @@
     pass
 
 ListAuditMitigationActionsExecutionsResponseTypeDef = TypedDict(
     "ListAuditMitigationActionsExecutionsResponseTypeDef",
     {
         "actionsExecutions": List[AuditMitigationActionExecutionMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditMitigationActionsTasksResponseTypeDef = TypedDict(
     "ListAuditMitigationActionsTasksResponseTypeDef",
     {
         "tasks": List[AuditMitigationActionsTaskMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartAuditMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "StartAuditMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
@@ -7614,18 +5969,18 @@
 )
 
 DescribeAccountAuditConfigurationResponseTypeDef = TypedDict(
     "DescribeAccountAuditConfigurationResponseTypeDef",
     {
         "roleArn": str,
         "auditNotificationTargetConfigurations": Dict[
-            Literal["SNS"], AuditNotificationTargetOutputTypeDef
+            Literal["SNS"], AuditNotificationTargetTypeDef
         ],
-        "auditCheckConfigurations": Dict[str, AuditCheckConfigurationOutputTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "auditCheckConfigurations": Dict[str, AuditCheckConfigurationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateAccountAuditConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAccountAuditConfigurationRequestRequestTypeDef",
     {
         "roleArn": str,
@@ -7638,15 +5993,15 @@
 )
 
 ListAuditTasksResponseTypeDef = TypedDict(
     "ListAuditTasksResponseTypeDef",
     {
         "tasks": List[AuditTaskMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredTestAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredTestAuthorizationRequestRequestTypeDef",
     {
         "authInfos": Sequence[AuthInfoTypeDef],
@@ -7669,51 +6024,42 @@
 ):
     pass
 
 DescribeAuthorizerResponseTypeDef = TypedDict(
     "DescribeAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDefaultAuthorizerResponseTypeDef = TypedDict(
     "DescribeDefaultAuthorizerResponseTypeDef",
     {
         "authorizerDescription": AuthorizerDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuthorizersResponseTypeDef = TypedDict(
     "ListAuthorizersResponseTypeDef",
     {
         "authorizers": List[AuthorizerSummaryTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AwsJobAbortConfigTypeDef = TypedDict(
     "AwsJobAbortConfigTypeDef",
     {
         "abortCriteriaList": Sequence[AwsJobAbortCriteriaTypeDef],
     },
 )
 
-AwsJobExponentialRolloutRateOutputTypeDef = TypedDict(
-    "AwsJobExponentialRolloutRateOutputTypeDef",
-    {
-        "baseRatePerMinute": int,
-        "incrementFactor": float,
-        "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaOutputTypeDef,
-    },
-)
-
 AwsJobExponentialRolloutRateTypeDef = TypedDict(
     "AwsJobExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
         "incrementFactor": float,
         "rateIncreaseCriteria": AwsJobRateIncreaseCriteriaTypeDef,
     },
@@ -7723,16 +6069,16 @@
     "BehaviorCriteriaOutputTypeDef",
     {
         "comparisonOperator": ComparisonOperatorType,
         "value": MetricValueOutputTypeDef,
         "durationSeconds": int,
         "consecutiveDatapointsToAlarm": int,
         "consecutiveDatapointsToClear": int,
-        "statisticalThreshold": StatisticalThresholdOutputTypeDef,
-        "mlDetectionConfig": MachineLearningDetectionConfigOutputTypeDef,
+        "statisticalThreshold": StatisticalThresholdTypeDef,
+        "mlDetectionConfig": MachineLearningDetectionConfigTypeDef,
     },
     total=False,
 )
 
 BehaviorCriteriaTypeDef = TypedDict(
     "BehaviorCriteriaTypeDef",
     {
@@ -7748,37 +6094,18 @@
 )
 
 GetBehaviorModelTrainingSummariesResponseTypeDef = TypedDict(
     "GetBehaviorModelTrainingSummariesResponseTypeDef",
     {
         "summaries": List[BehaviorModelTrainingSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredMetricToRetainOutputTypeDef = TypedDict(
-    "_RequiredMetricToRetainOutputTypeDef",
-    {
-        "metric": str,
-    },
-)
-_OptionalMetricToRetainOutputTypeDef = TypedDict(
-    "_OptionalMetricToRetainOutputTypeDef",
-    {
-        "metricDimension": MetricDimensionOutputTypeDef,
-    },
-    total=False,
-)
-
-class MetricToRetainOutputTypeDef(
-    _RequiredMetricToRetainOutputTypeDef, _OptionalMetricToRetainOutputTypeDef
-):
-    pass
-
 _RequiredMetricToRetainTypeDef = TypedDict(
     "_RequiredMetricToRetainTypeDef",
     {
         "metric": str,
     },
 )
 _OptionalMetricToRetainTypeDef = TypedDict(
@@ -7795,17 +6122,17 @@
 DescribeBillingGroupResponseTypeDef = TypedDict(
     "DescribeBillingGroupResponseTypeDef",
     {
         "billingGroupName": str,
         "billingGroupId": str,
         "billingGroupArn": str,
         "version": int,
-        "billingGroupProperties": BillingGroupPropertiesOutputTypeDef,
+        "billingGroupProperties": BillingGroupPropertiesTypeDef,
         "billingGroupMetadata": BillingGroupMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateBillingGroupRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBillingGroupRequestRequestTypeDef",
     {
         "billingGroupName": str,
@@ -7827,15 +6154,15 @@
     pass
 
 GetBucketsAggregationResponseTypeDef = TypedDict(
     "GetBucketsAggregationResponseTypeDef",
     {
         "totalCount": int,
         "buckets": List[BucketTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketsAggregationTypeTypeDef = TypedDict(
     "BucketsAggregationTypeTypeDef",
     {
         "termsAggregation": TermsAggregationTypeDef,
@@ -7863,15 +6190,15 @@
 )
 
 ListCACertificatesResponseTypeDef = TypedDict(
     "ListCACertificatesResponseTypeDef",
     {
         "certificates": List[CACertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CertificateDescriptionTypeDef = TypedDict(
     "CertificateDescriptionTypeDef",
     {
         "certificateArn": str,
@@ -7893,32 +6220,32 @@
 )
 
 ListCertificatesByCAResponseTypeDef = TypedDict(
     "ListCertificatesByCAResponseTypeDef",
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCertificatesResponseTypeDef = TypedDict(
     "ListCertificatesResponseTypeDef",
     {
         "certificates": List[CertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomCodeSigningOutputTypeDef = TypedDict(
     "CustomCodeSigningOutputTypeDef",
     {
         "signature": CodeSigningSignatureOutputTypeDef,
-        "certificateChain": CodeSigningCertificateChainOutputTypeDef,
+        "certificateChain": CodeSigningCertificateChainTypeDef,
         "hashAlgorithm": str,
         "signatureAlgorithm": str,
     },
     total=False,
 )
 
 CustomCodeSigningTypeDef = TypedDict(
@@ -7931,18 +6258,18 @@
     },
     total=False,
 )
 
 DescribeEventConfigurationsResponseTypeDef = TypedDict(
     "DescribeEventConfigurationsResponseTypeDef",
     {
-        "eventConfigurations": Dict[EventTypeType, ConfigurationOutputTypeDef],
+        "eventConfigurations": Dict[EventTypeType, ConfigurationTypeDef],
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventConfigurationsRequestRequestTypeDef = TypedDict(
     "UpdateEventConfigurationsRequestRequestTypeDef",
     {
         "eventConfigurations": Mapping[EventTypeType, ConfigurationTypeDef],
@@ -8129,14 +6456,23 @@
 
 class CreateScheduledAuditRequestRequestTypeDef(
     _RequiredCreateScheduledAuditRequestRequestTypeDef,
     _OptionalCreateScheduledAuditRequestRequestTypeDef,
 ):
     pass
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": List[TagTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Sequence[TagTypeDef],
     },
 )
@@ -8186,14 +6522,25 @@
 
 class UpdateDomainConfigurationRequestRequestTypeDef(
     _RequiredUpdateDomainConfigurationRequestRequestTypeDef,
     _OptionalUpdateDomainConfigurationRequestRequestTypeDef,
 ):
     pass
 
+SchedulingConfigOutputTypeDef = TypedDict(
+    "SchedulingConfigOutputTypeDef",
+    {
+        "startTime": str,
+        "endTime": str,
+        "endBehavior": JobEndBehaviorType,
+        "maintenanceWindows": List[MaintenanceWindowTypeDef],
+    },
+    total=False,
+)
+
 SchedulingConfigTypeDef = TypedDict(
     "SchedulingConfigTypeDef",
     {
         "startTime": str,
         "endTime": str,
         "endBehavior": JobEndBehaviorType,
         "maintenanceWindows": Sequence[MaintenanceWindowTypeDef],
@@ -8204,26 +6551,26 @@
 CreateKeysAndCertificateResponseTypeDef = TypedDict(
     "CreateKeysAndCertificateResponseTypeDef",
     {
         "certificateArn": str,
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProvisioningClaimResponseTypeDef = TypedDict(
     "CreateProvisioningClaimResponseTypeDef",
     {
         "certificateId": str,
         "certificatePem": str,
         "keyPair": KeyPairTypeDef,
         "expiration": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
@@ -8245,14 +6592,32 @@
 
 class CreateProvisioningTemplateRequestRequestTypeDef(
     _RequiredCreateProvisioningTemplateRequestRequestTypeDef,
     _OptionalCreateProvisioningTemplateRequestRequestTypeDef,
 ):
     pass
 
+DescribeProvisioningTemplateResponseTypeDef = TypedDict(
+    "DescribeProvisioningTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateName": str,
+        "description": str,
+        "creationDate": datetime,
+        "lastModifiedDate": datetime,
+        "defaultVersionId": int,
+        "templateBody": str,
+        "enabled": bool,
+        "provisioningRoleArn": str,
+        "preProvisioningHook": ProvisioningHookTypeDef,
+        "type": TemplateTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProvisioningTemplateRequestRequestTypeDef",
     {
         "templateName": str,
     },
 )
 _OptionalUpdateProvisioningTemplateRequestRequestTypeDef = TypedDict(
@@ -8299,148 +6664,151 @@
     {
         "taskStatus": AuditTaskStatusType,
         "taskType": AuditTaskTypeType,
         "taskStartTime": datetime,
         "taskStatistics": TaskStatisticsTypeDef,
         "scheduledAuditName": str,
         "auditDetails": Dict[str, AuditCheckDetailsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredRegisterCACertificateRequestRequestTypeDef",
+    {
+        "caCertificate": str,
+    },
+)
+_OptionalRegisterCACertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalRegisterCACertificateRequestRequestTypeDef",
+    {
+        "verificationCertificate": str,
+        "setAsActive": bool,
+        "allowAutoRegistration": bool,
+        "registrationConfig": RegistrationConfigTypeDef,
+        "tags": Sequence[TagTypeDef],
+        "certificateMode": CertificateModeType,
+    },
+    total=False,
+)
+
+class RegisterCACertificateRequestRequestTypeDef(
+    _RequiredRegisterCACertificateRequestRequestTypeDef,
+    _OptionalRegisterCACertificateRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateCACertificateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCACertificateRequestRequestTypeDef",
+    {
+        "certificateId": str,
+    },
+)
+_OptionalUpdateCACertificateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCACertificateRequestRequestTypeDef",
+    {
+        "newStatus": CACertificateStatusType,
+        "newAutoRegistrationStatus": AutoRegistrationStatusType,
+        "registrationConfig": RegistrationConfigTypeDef,
+        "removeAutoRegistration": bool,
     },
+    total=False,
 )
 
+class UpdateCACertificateRequestRequestTypeDef(
+    _RequiredUpdateCACertificateRequestRequestTypeDef,
+    _OptionalUpdateCACertificateRequestRequestTypeDef,
+):
+    pass
+
 DescribeDomainConfigurationResponseTypeDef = TypedDict(
     "DescribeDomainConfigurationResponseTypeDef",
     {
         "domainConfigurationName": str,
         "domainConfigurationArn": str,
         "domainName": str,
         "serverCertificates": List[ServerCertificateSummaryTypeDef],
-        "authorizerConfig": AuthorizerConfigOutputTypeDef,
+        "authorizerConfig": AuthorizerConfigTypeDef,
         "domainConfigurationStatus": DomainConfigurationStatusType,
         "serviceType": ServiceTypeType,
         "domainType": DomainTypeType,
         "lastStatusChangeDate": datetime,
-        "tlsConfig": TlsConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SchedulingConfigOutputTypeDef = TypedDict(
-    "SchedulingConfigOutputTypeDef",
-    {
-        "startTime": str,
-        "endTime": str,
-        "endBehavior": JobEndBehaviorType,
-        "maintenanceWindows": List[MaintenanceWindowOutputTypeDef],
+        "tlsConfig": TlsConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeManagedJobTemplateResponseTypeDef = TypedDict(
     "DescribeManagedJobTemplateResponseTypeDef",
     {
         "templateName": str,
         "templateArn": str,
         "description": str,
         "templateVersion": str,
         "environments": List[str],
         "documentParameters": List[DocumentParameterTypeDef],
         "document": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeProvisioningTemplateResponseTypeDef = TypedDict(
-    "DescribeProvisioningTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateName": str,
-        "description": str,
-        "creationDate": datetime,
-        "lastModifiedDate": datetime,
-        "defaultVersionId": int,
-        "templateBody": str,
-        "enabled": bool,
-        "provisioningRoleArn": str,
-        "preProvisioningHook": ProvisioningHookOutputTypeDef,
-        "type": TemplateTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRoleAliasResponseTypeDef = TypedDict(
     "DescribeRoleAliasResponseTypeDef",
     {
         "roleAliasDescription": RoleAliasDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeThingTypeResponseTypeDef = TypedDict(
     "DescribeThingTypeResponseTypeDef",
     {
         "thingTypeName": str,
         "thingTypeId": str,
         "thingTypeArn": str,
         "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingTypeDefinitionTypeDef = TypedDict(
     "ThingTypeDefinitionTypeDef",
     {
         "thingTypeName": str,
         "thingTypeArn": str,
         "thingTypeProperties": ThingTypePropertiesOutputTypeDef,
         "thingTypeMetadata": ThingTypeMetadataTypeDef,
     },
     total=False,
 )
 
-DestinationOutputTypeDef = TypedDict(
-    "DestinationOutputTypeDef",
-    {
-        "s3Destination": S3DestinationOutputTypeDef,
-    },
-    total=False,
-)
-
 DestinationTypeDef = TypedDict(
     "DestinationTypeDef",
     {
         "s3Destination": S3DestinationTypeDef,
     },
     total=False,
 )
 
 ListDetectMitigationActionsExecutionsResponseTypeDef = TypedDict(
     "ListDetectMitigationActionsExecutionsResponseTypeDef",
     {
         "actionsExecutions": List[DetectMitigationActionExecutionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainConfigurationsResponseTypeDef = TypedDict(
     "ListDomainConfigurationsResponseTypeDef",
     {
         "domainConfigurations": List[DomainConfigurationSummaryTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DynamoDBv2ActionOutputTypeDef = TypedDict(
-    "DynamoDBv2ActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "putItem": PutItemInputOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DynamoDBv2ActionTypeDef = TypedDict(
     "DynamoDBv2ActionTypeDef",
     {
         "roleArn": str,
@@ -8448,24 +6816,15 @@
     },
 )
 
 GetEffectivePoliciesResponseTypeDef = TypedDict(
     "GetEffectivePoliciesResponseTypeDef",
     {
         "effectivePolicies": List[EffectivePolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ExponentialRolloutRateOutputTypeDef = TypedDict(
-    "ExponentialRolloutRateOutputTypeDef",
-    {
-        "baseRatePerMinute": int,
-        "incrementFactor": float,
-        "rateIncreaseCriteria": RateIncreaseCriteriaOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExponentialRolloutRateTypeDef = TypedDict(
     "ExponentialRolloutRateTypeDef",
     {
         "baseRatePerMinute": int,
@@ -8479,16 +6838,16 @@
     {
         "thingGroupIndexingMode": ThingGroupIndexingModeType,
     },
 )
 _OptionalThingGroupIndexingConfigurationOutputTypeDef = TypedDict(
     "_OptionalThingGroupIndexingConfigurationOutputTypeDef",
     {
-        "managedFields": List[FieldOutputTypeDef],
-        "customFields": List[FieldOutputTypeDef],
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
     },
     total=False,
 )
 
 class ThingGroupIndexingConfigurationOutputTypeDef(
     _RequiredThingGroupIndexingConfigurationOutputTypeDef,
     _OptionalThingGroupIndexingConfigurationOutputTypeDef,
@@ -8511,32 +6870,14 @@
 )
 
 class ThingGroupIndexingConfigurationTypeDef(
     _RequiredThingGroupIndexingConfigurationTypeDef, _OptionalThingGroupIndexingConfigurationTypeDef
 ):
     pass
 
-StreamFileOutputTypeDef = TypedDict(
-    "StreamFileOutputTypeDef",
-    {
-        "fileId": int,
-        "s3Location": S3LocationOutputTypeDef,
-    },
-    total=False,
-)
-
-FileLocationOutputTypeDef = TypedDict(
-    "FileLocationOutputTypeDef",
-    {
-        "stream": StreamOutputTypeDef,
-        "s3Location": S3LocationOutputTypeDef,
-    },
-    total=False,
-)
-
 StreamFileTypeDef = TypedDict(
     "StreamFileTypeDef",
     {
         "fileId": int,
         "s3Location": S3LocationTypeDef,
     },
     total=False,
@@ -8552,87 +6893,931 @@
 )
 
 ListFleetMetricsResponseTypeDef = TypedDict(
     "ListFleetMetricsResponseTypeDef",
     {
         "fleetMetrics": List[FleetMetricNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef = (
+    TypedDict(
+        "GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef",
+        {
+            "securityProfileName": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListActiveViolationsRequestListActiveViolationsPaginateTypeDef = TypedDict(
+    "ListActiveViolationsRequestListActiveViolationsPaginateTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    {
+        "target": str,
+    },
+)
+_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef",
+    {
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef(
+    _RequiredListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    _OptionalListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+        "findingId": str,
+    },
+)
+_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "actionStatus": AuditMitigationActionsExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef(
+    _RequiredListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    _OptionalListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef",
+    {
+        "auditTaskId": str,
+        "findingId": str,
+        "taskStatus": AuditMitigationActionsTaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef(
+    _RequiredListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    _OptionalListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+):
+    pass
+
+_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
+    "_RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef = TypedDict(
+    "_OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef",
+    {
+        "taskType": AuditTaskTypeType,
+        "taskStatus": AuditTaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAuditTasksRequestListAuditTasksPaginateTypeDef(
+    _RequiredListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    _OptionalListAuditTasksRequestListAuditTasksPaginateTypeDef,
+):
+    pass
+
+ListAuthorizersRequestListAuthorizersPaginateTypeDef = TypedDict(
+    "ListAuthorizersRequestListAuthorizersPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "status": AuthorizerStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListBillingGroupsRequestListBillingGroupsPaginateTypeDef = TypedDict(
+    "ListBillingGroupsRequestListBillingGroupsPaginateTypeDef",
+    {
+        "namePrefixFilter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCACertificatesRequestListCACertificatesPaginateTypeDef = TypedDict(
+    "ListCACertificatesRequestListCACertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "templateName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
+    "_RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    {
+        "caCertificateId": str,
+    },
+)
+_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef = TypedDict(
+    "_OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef(
+    _RequiredListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    _OptionalListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+):
+    pass
+
+ListCertificatesRequestListCertificatesPaginateTypeDef = TypedDict(
+    "ListCertificatesRequestListCertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListCustomMetricsRequestListCustomMetricsPaginateTypeDef = TypedDict(
+    "ListCustomMetricsRequestListCustomMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
+ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef = TypedDict(
+    "ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef",
+    {
+        "taskId": str,
+        "violationId": str,
+        "thingName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef = TypedDict(
+    "_OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef(
+    _RequiredListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    _OptionalListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+):
+    pass
+
+ListDimensionsRequestListDimensionsPaginateTypeDef = TypedDict(
+    "ListDimensionsRequestListDimensionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef = TypedDict(
+    "ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef",
+    {
+        "serviceType": ServiceTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFleetMetricsRequestListFleetMetricsPaginateTypeDef = TypedDict(
+    "ListFleetMetricsRequestListFleetMetricsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListIndicesRequestListIndicesPaginateTypeDef = TypedDict(
+    "ListIndicesRequestListIndicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
+    "_RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    {
+        "jobId": str,
+    },
+)
+_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef = TypedDict(
+    "_OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef",
+    {
+        "status": JobExecutionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef(
+    _RequiredListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    _OptionalListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+):
+    pass
+
+_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
+    "_RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef = TypedDict(
+    "_OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef",
+    {
+        "status": JobExecutionStatusType,
+        "namespaceId": str,
+        "jobId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef(
+    _RequiredListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    _OptionalListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+):
+    pass
+
+ListJobTemplatesRequestListJobTemplatesPaginateTypeDef = TypedDict(
+    "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListJobsRequestListJobsPaginateTypeDef = TypedDict(
+    "ListJobsRequestListJobsPaginateTypeDef",
+    {
+        "status": JobStatusType,
+        "targetSelection": TargetSelectionType,
+        "thingGroupName": str,
+        "thingGroupId": str,
+        "namespaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef = TypedDict(
+    "ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef",
+    {
+        "templateName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
+    "_RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    {
+        "thingName": str,
+        "metricName": str,
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef = TypedDict(
+    "_OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef",
+    {
+        "dimensionName": str,
+        "dimensionValueOperator": DimensionValueOperatorType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMetricValuesRequestListMetricValuesPaginateTypeDef(
+    _RequiredListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    _OptionalListMetricValuesRequestListMetricValuesPaginateTypeDef,
+):
+    pass
+
+ListMitigationActionsRequestListMitigationActionsPaginateTypeDef = TypedDict(
+    "ListMitigationActionsRequestListMitigationActionsPaginateTypeDef",
+    {
+        "actionType": MitigationActionTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef = TypedDict(
+    "ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef",
+    {
+        "otaUpdateStatus": OTAUpdateStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef = TypedDict(
+    "ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "packageName": str,
+    },
+)
+_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef",
+    {
+        "status": PackageVersionStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPackageVersionsRequestListPackageVersionsPaginateTypeDef(
+    _RequiredListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    _OptionalListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+):
+    pass
+
+ListPackagesRequestListPackagesPaginateTypeDef = TypedDict(
+    "ListPackagesRequestListPackagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    {
+        "policyName": str,
+    },
+)
+_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef(
+    _RequiredListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    _OptionalListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+):
+    pass
+
+_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    {
+        "principal": str,
+    },
+)
+_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef(
+    _RequiredListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    _OptionalListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+):
+    pass
+
+_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
+    "_RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    {
+        "principal": str,
+    },
+)
+_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef = TypedDict(
+    "_OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef(
+    _RequiredListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    _OptionalListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+):
+    pass
+
+_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    {
+        "templateName": str,
+    },
+)
+_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef(
+    _RequiredListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    _OptionalListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+):
+    pass
+
+ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef = TypedDict(
+    "ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
+    "_RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    {
+        "findingId": str,
+    },
+)
+_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef = TypedDict(
+    "_OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef(
+    _RequiredListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    _OptionalListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+):
+    pass
+
+ListRoleAliasesRequestListRoleAliasesPaginateTypeDef = TypedDict(
+    "ListRoleAliasesRequestListRoleAliasesPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef = TypedDict(
+    "ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+        {
+            "securityProfileTargetArn": str,
+        },
+    )
+)
+_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef",
+        {
+            "recursive": bool,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef(
+    _RequiredListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    _OptionalListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+):
+    pass
+
+ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef = TypedDict(
+    "ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef",
+    {
+        "dimensionName": str,
+        "metricName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStreamsRequestListStreamsPaginateTypeDef = TypedDict(
+    "ListStreamsRequestListStreamsPaginateTypeDef",
+    {
+        "ascendingOrder": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    {
+        "policyName": str,
+    },
+)
+_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef(
+    _RequiredListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    _OptionalListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+):
+    pass
+
+_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
+    TypedDict(
+        "_RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+        {
+            "securityProfileName": str,
+        },
+    )
+)
+_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef = (
+    TypedDict(
+        "_OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef(
+    _RequiredListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    _OptionalListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+):
+    pass
+
+_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
+    "_RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef = TypedDict(
+    "_OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef(
+    _RequiredListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    _OptionalListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+):
+    pass
+
+ListThingGroupsRequestListThingGroupsPaginateTypeDef = TypedDict(
+    "ListThingGroupsRequestListThingGroupsPaginateTypeDef",
+    {
+        "parentGroup": str,
+        "namePrefixFilter": str,
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
+    "_RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    {
+        "thingName": str,
+    },
+)
+_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef = TypedDict(
+    "_OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef(
+    _RequiredListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    _OptionalListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+):
+    pass
+
+_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
+    "_RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    {
+        "taskId": str,
+        "reportType": ReportTypeType,
+    },
+)
+_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef = TypedDict(
+    "_OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef(
+    _RequiredListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    _OptionalListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+):
+    pass
+
+ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef = TypedDict(
+    "ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef",
+    {
+        "status": StatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListThingTypesRequestListThingTypesPaginateTypeDef = TypedDict(
+    "ListThingTypesRequestListThingTypesPaginateTypeDef",
+    {
+        "thingTypeName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
+    "_RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    {
+        "billingGroupName": str,
+    },
+)
+_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef = TypedDict(
+    "_OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef(
+    _RequiredListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    _OptionalListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+):
+    pass
+
+_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
+    "_RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    {
+        "thingGroupName": str,
+    },
+)
+_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef = TypedDict(
+    "_OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef",
+    {
+        "recursive": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef(
+    _RequiredListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    _OptionalListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+):
+    pass
+
+ListThingsRequestListThingsPaginateTypeDef = TypedDict(
+    "ListThingsRequestListThingsPaginateTypeDef",
+    {
+        "attributeName": str,
+        "attributeValue": str,
+        "thingTypeName": str,
+        "usePrefixAttributeValue": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef = TypedDict(
+    "ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTopicRulesRequestListTopicRulesPaginateTypeDef = TypedDict(
+    "ListTopicRulesRequestListTopicRulesPaginateTypeDef",
+    {
+        "topic": str,
+        "ruleDisabled": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef = TypedDict(
+    "ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef",
+    {
+        "targetType": LogTargetTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
+    "_RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef",
+    {
+        "startTime": Union[datetime, str],
+        "endTime": Union[datetime, str],
+    },
+)
+_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef = TypedDict(
+    "_OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef",
+    {
+        "thingName": str,
+        "securityProfileName": str,
+        "behaviorCriteriaType": BehaviorCriteriaTypeType,
+        "listSuppressedAlerts": bool,
+        "verificationState": VerificationStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListViolationEventsRequestListViolationEventsPaginateTypeDef(
+    _RequiredListViolationEventsRequestListViolationEventsPaginateTypeDef,
+    _OptionalListViolationEventsRequestListViolationEventsPaginateTypeDef,
+):
+    pass
+
 GetPackageConfigurationResponseTypeDef = TypedDict(
     "GetPackageConfigurationResponseTypeDef",
     {
-        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdatePackageConfigurationRequestRequestTypeDef",
+    {
+        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
+        "clientToken": str,
+    },
+    total=False,
+)
+
 GetPercentilesResponseTypeDef = TypedDict(
     "GetPercentilesResponseTypeDef",
     {
         "percentiles": List[PercentPairTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStatisticsResponseTypeDef = TypedDict(
     "GetStatisticsResponseTypeDef",
     {
         "statistics": StatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListBillingGroupsResponseTypeDef = TypedDict(
     "ListBillingGroupsResponseTypeDef",
     {
         "billingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingGroupsForThingResponseTypeDef = TypedDict(
     "ListThingGroupsForThingResponseTypeDef",
     {
         "thingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingGroupsResponseTypeDef = TypedDict(
     "ListThingGroupsResponseTypeDef",
     {
         "thingGroups": List[GroupNameAndArnTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ThingGroupMetadataTypeDef = TypedDict(
     "ThingGroupMetadataTypeDef",
     {
         "parentGroupName": str,
         "rootToParentThingGroups": List[GroupNameAndArnTypeDef],
         "creationDate": datetime,
     },
     total=False,
 )
 
-HttpAuthorizationOutputTypeDef = TypedDict(
-    "HttpAuthorizationOutputTypeDef",
-    {
-        "sigv4": SigV4AuthorizationOutputTypeDef,
-    },
-    total=False,
-)
-
 HttpAuthorizationTypeDef = TypedDict(
     "HttpAuthorizationTypeDef",
     {
         "sigv4": SigV4AuthorizationTypeDef,
     },
     total=False,
 )
@@ -8645,16 +7830,16 @@
 )
 _OptionalThingIndexingConfigurationOutputTypeDef = TypedDict(
     "_OptionalThingIndexingConfigurationOutputTypeDef",
     {
         "thingConnectivityIndexingMode": ThingConnectivityIndexingModeType,
         "deviceDefenderIndexingMode": DeviceDefenderIndexingModeType,
         "namedShadowIndexingMode": NamedShadowIndexingModeType,
-        "managedFields": List[FieldOutputTypeDef],
-        "customFields": List[FieldOutputTypeDef],
+        "managedFields": List[FieldTypeDef],
+        "customFields": List[FieldTypeDef],
         "filter": IndexingFilterOutputTypeDef,
     },
     total=False,
 )
 
 class ThingIndexingConfigurationOutputTypeDef(
     _RequiredThingIndexingConfigurationOutputTypeDef,
@@ -8721,15 +7906,15 @@
     },
     total=False,
 )
 
 JobExecutionsRetryConfigOutputTypeDef = TypedDict(
     "JobExecutionsRetryConfigOutputTypeDef",
     {
-        "criteriaList": List[RetryCriteriaOutputTypeDef],
+        "criteriaList": List[RetryCriteriaTypeDef],
     },
 )
 
 JobExecutionsRetryConfigTypeDef = TypedDict(
     "JobExecutionsRetryConfigTypeDef",
     {
         "criteriaList": Sequence[RetryCriteriaTypeDef],
@@ -8737,149 +7922,140 @@
 )
 
 ListJobsResponseTypeDef = TypedDict(
     "ListJobsResponseTypeDef",
     {
         "jobs": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobTemplatesResponseTypeDef = TypedDict(
     "ListJobTemplatesResponseTypeDef",
     {
         "jobTemplates": List[JobTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListManagedJobTemplatesResponseTypeDef = TypedDict(
     "ListManagedJobTemplatesResponseTypeDef",
     {
         "managedJobTemplates": List[ManagedJobTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMitigationActionsResponseTypeDef = TypedDict(
     "ListMitigationActionsResponseTypeDef",
     {
         "actionIdentifiers": List[MitigationActionIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOTAUpdatesResponseTypeDef = TypedDict(
     "ListOTAUpdatesResponseTypeDef",
     {
         "otaUpdates": List[OTAUpdateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOutgoingCertificatesResponseTypeDef = TypedDict(
     "ListOutgoingCertificatesResponseTypeDef",
     {
         "outgoingCertificates": List[OutgoingCertificateTypeDef],
         "nextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackageVersionsResponseTypeDef = TypedDict(
     "ListPackageVersionsResponseTypeDef",
     {
         "packageVersionSummaries": List[PackageVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPackagesResponseTypeDef = TypedDict(
     "ListPackagesResponseTypeDef",
     {
         "packageSummaries": List[PackageSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPolicyVersionsResponseTypeDef = TypedDict(
     "ListPolicyVersionsResponseTypeDef",
     {
         "policyVersions": List[PolicyVersionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningTemplateVersionsResponseTypeDef = TypedDict(
     "ListProvisioningTemplateVersionsResponseTypeDef",
     {
         "versions": List[ProvisioningTemplateVersionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListProvisioningTemplatesResponseTypeDef = TypedDict(
     "ListProvisioningTemplatesResponseTypeDef",
     {
         "templates": List[ProvisioningTemplateSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListScheduledAuditsResponseTypeDef = TypedDict(
     "ListScheduledAuditsResponseTypeDef",
     {
         "scheduledAudits": List[ScheduledAuditMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityProfilesResponseTypeDef = TypedDict(
     "ListSecurityProfilesResponseTypeDef",
     {
         "securityProfileIdentifiers": List[SecurityProfileIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsResponseTypeDef = TypedDict(
     "ListStreamsResponseTypeDef",
     {
         "streams": List[StreamSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": List[TagOutputTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsForSecurityProfileResponseTypeDef = TypedDict(
     "ListTargetsForSecurityProfileResponseTypeDef",
     {
         "securityProfileTargets": List[SecurityProfileTargetTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SecurityProfileTargetMappingTypeDef = TypedDict(
     "SecurityProfileTargetMappingTypeDef",
     {
         "securityProfileIdentifier": SecurityProfileIdentifierTypeDef,
@@ -8889,50 +8065,27 @@
 )
 
 ListThingsResponseTypeDef = TypedDict(
     "ListThingsResponseTypeDef",
     {
         "things": List[ThingAttributeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTopicRulesResponseTypeDef = TypedDict(
     "ListTopicRulesResponseTypeDef",
     {
         "rules": List[TopicRuleListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredLocationActionOutputTypeDef = TypedDict(
-    "_RequiredLocationActionOutputTypeDef",
-    {
-        "roleArn": str,
-        "trackerName": str,
-        "deviceId": str,
-        "latitude": str,
-        "longitude": str,
-    },
-)
-_OptionalLocationActionOutputTypeDef = TypedDict(
-    "_OptionalLocationActionOutputTypeDef",
-    {
-        "timestamp": LocationTimestampOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class LocationActionOutputTypeDef(
-    _RequiredLocationActionOutputTypeDef, _OptionalLocationActionOutputTypeDef
-):
-    pass
-
 _RequiredLocationActionTypeDef = TypedDict(
     "_RequiredLocationActionTypeDef",
     {
         "roleArn": str,
         "trackerName": str,
         "deviceId": str,
         "latitude": str,
@@ -8949,15 +8102,15 @@
 
 class LocationActionTypeDef(_RequiredLocationActionTypeDef, _OptionalLocationActionTypeDef):
     pass
 
 LogTargetConfigurationTypeDef = TypedDict(
     "LogTargetConfigurationTypeDef",
     {
-        "logTarget": LogTargetOutputTypeDef,
+        "logTarget": LogTargetTypeDef,
         "logLevel": LogLevelType,
     },
     total=False,
 )
 
 SetV2LoggingLevelRequestRequestTypeDef = TypedDict(
     "SetV2LoggingLevelRequestRequestTypeDef",
@@ -8973,20 +8126,20 @@
         "loggingOptionsPayload": LoggingOptionsPayloadTypeDef,
     },
 )
 
 MitigationActionParamsOutputTypeDef = TypedDict(
     "MitigationActionParamsOutputTypeDef",
     {
-        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsOutputTypeDef,
-        "updateCACertificateParams": UpdateCACertificateParamsOutputTypeDef,
+        "updateDeviceCertificateParams": UpdateDeviceCertificateParamsTypeDef,
+        "updateCACertificateParams": UpdateCACertificateParamsTypeDef,
         "addThingsToThingGroupParams": AddThingsToThingGroupParamsOutputTypeDef,
-        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsOutputTypeDef,
-        "enableIoTLoggingParams": EnableIoTLoggingParamsOutputTypeDef,
-        "publishFindingToSnsParams": PublishFindingToSnsParamsOutputTypeDef,
+        "replaceDefaultPolicyVersionParams": ReplaceDefaultPolicyVersionParamsTypeDef,
+        "enableIoTLoggingParams": EnableIoTLoggingParamsTypeDef,
+        "publishFindingToSnsParams": PublishFindingToSnsParamsTypeDef,
     },
     total=False,
 )
 
 MitigationActionParamsTypeDef = TypedDict(
     "MitigationActionParamsTypeDef",
     {
@@ -9004,15 +8157,15 @@
     "MqttHeadersOutputTypeDef",
     {
         "payloadFormatIndicator": str,
         "contentType": str,
         "responseTopic": str,
         "correlationData": str,
         "messageExpiry": str,
-        "userProperties": List[UserPropertyOutputTypeDef],
+        "userProperties": List[UserPropertyTypeDef],
     },
     total=False,
 )
 
 MqttHeadersTypeDef = TypedDict(
     "MqttHeadersTypeDef",
     {
@@ -9022,31 +8175,14 @@
         "correlationData": str,
         "messageExpiry": str,
         "userProperties": Sequence[UserPropertyTypeDef],
     },
     total=False,
 )
 
-ResourceIdentifierOutputTypeDef = TypedDict(
-    "ResourceIdentifierOutputTypeDef",
-    {
-        "deviceCertificateId": str,
-        "caCertificateId": str,
-        "cognitoIdentityPoolId": str,
-        "clientId": str,
-        "policyVersionIdentifier": PolicyVersionIdentifierOutputTypeDef,
-        "account": str,
-        "iamRoleArn": str,
-        "roleAliasArn": str,
-        "issuerCertificateIdentifier": IssuerCertificateIdentifierOutputTypeDef,
-        "deviceCertificateArn": str,
-    },
-    total=False,
-)
-
 ResourceIdentifierTypeDef = TypedDict(
     "ResourceIdentifierTypeDef",
     {
         "deviceCertificateId": str,
         "caCertificateId": str,
         "cognitoIdentityPoolId": str,
         "clientId": str,
@@ -9056,62 +8192,14 @@
         "roleAliasArn": str,
         "issuerCertificateIdentifier": IssuerCertificateIdentifierTypeDef,
         "deviceCertificateArn": str,
     },
     total=False,
 )
 
-_RequiredRegisterCACertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredRegisterCACertificateRequestRequestTypeDef",
-    {
-        "caCertificate": str,
-    },
-)
-_OptionalRegisterCACertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalRegisterCACertificateRequestRequestTypeDef",
-    {
-        "verificationCertificate": str,
-        "setAsActive": bool,
-        "allowAutoRegistration": bool,
-        "registrationConfig": RegistrationConfigTypeDef,
-        "tags": Sequence[TagTypeDef],
-        "certificateMode": CertificateModeType,
-    },
-    total=False,
-)
-
-class RegisterCACertificateRequestRequestTypeDef(
-    _RequiredRegisterCACertificateRequestRequestTypeDef,
-    _OptionalRegisterCACertificateRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateCACertificateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCACertificateRequestRequestTypeDef",
-    {
-        "certificateId": str,
-    },
-)
-_OptionalUpdateCACertificateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCACertificateRequestRequestTypeDef",
-    {
-        "newStatus": CACertificateStatusType,
-        "newAutoRegistrationStatus": AutoRegistrationStatusType,
-        "registrationConfig": RegistrationConfigTypeDef,
-        "removeAutoRegistration": bool,
-    },
-    total=False,
-)
-
-class UpdateCACertificateRequestRequestTypeDef(
-    _RequiredUpdateCACertificateRequestRequestTypeDef,
-    _OptionalUpdateCACertificateRequestRequestTypeDef,
-):
-    pass
-
 _RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef = TypedDict(
     "_RequiredStartDetectMitigationActionsTaskRequestRequestTypeDef",
     {
         "taskId": str,
         "target": DetectMitigationActionsTaskTargetTypeDef,
         "actions": Sequence[str],
         "clientRequestToken": str,
@@ -9174,21 +8262,21 @@
 
 _RequiredTimestreamActionOutputTypeDef = TypedDict(
     "_RequiredTimestreamActionOutputTypeDef",
     {
         "roleArn": str,
         "databaseName": str,
         "tableName": str,
-        "dimensions": List[TimestreamDimensionOutputTypeDef],
+        "dimensions": List[TimestreamDimensionTypeDef],
     },
 )
 _OptionalTimestreamActionOutputTypeDef = TypedDict(
     "_OptionalTimestreamActionOutputTypeDef",
     {
-        "timestamp": TimestreamTimestampOutputTypeDef,
+        "timestamp": TimestreamTimestampTypeDef,
     },
     total=False,
 )
 
 class TimestreamActionOutputTypeDef(
     _RequiredTimestreamActionOutputTypeDef, _OptionalTimestreamActionOutputTypeDef
 ):
@@ -9247,38 +8335,29 @@
         "statusReason": str,
         "httpUrlProperties": HttpUrlDestinationPropertiesTypeDef,
         "vpcProperties": VpcDestinationPropertiesTypeDef,
     },
     total=False,
 )
 
-UpdatePackageConfigurationRequestRequestTypeDef = TypedDict(
-    "UpdatePackageConfigurationRequestRequestTypeDef",
-    {
-        "versionUpdateByJobsConfig": VersionUpdateByJobsConfigTypeDef,
-        "clientToken": str,
-    },
-    total=False,
-)
-
 ValidateSecurityProfileBehaviorsResponseTypeDef = TypedDict(
     "ValidateSecurityProfileBehaviorsResponseTypeDef",
     {
         "valid": bool,
         "validationErrors": List[ValidationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricValuesResponseTypeDef = TypedDict(
     "ListMetricValuesResponseTypeDef",
     {
         "metricDatumList": List[MetricDatumTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeniedTypeDef = TypedDict(
     "DeniedTypeDef",
     {
         "implicitDeny": ImplicitDenyTypeDef,
@@ -9286,15 +8365,15 @@
     },
     total=False,
 )
 
 _RequiredPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
     "_RequiredPutAssetPropertyValueEntryOutputTypeDef",
     {
-        "propertyValues": List[AssetPropertyValueOutputTypeDef],
+        "propertyValues": List[AssetPropertyValueTypeDef],
     },
 )
 _OptionalPutAssetPropertyValueEntryOutputTypeDef = TypedDict(
     "_OptionalPutAssetPropertyValueEntryOutputTypeDef",
     {
         "entryId": str,
         "assetId": str,
@@ -9417,23 +8496,14 @@
 )
 
 class UpdateThingGroupRequestRequestTypeDef(
     _RequiredUpdateThingGroupRequestRequestTypeDef, _OptionalUpdateThingGroupRequestRequestTypeDef
 ):
     pass
 
-AwsJobExecutionsRolloutConfigOutputTypeDef = TypedDict(
-    "AwsJobExecutionsRolloutConfigOutputTypeDef",
-    {
-        "maximumPerMinute": int,
-        "exponentialRate": AwsJobExponentialRolloutRateOutputTypeDef,
-    },
-    total=False,
-)
-
 AwsJobExecutionsRolloutConfigTypeDef = TypedDict(
     "AwsJobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": AwsJobExponentialRolloutRateTypeDef,
     },
     total=False,
@@ -9445,15 +8515,15 @@
         "name": str,
     },
 )
 _OptionalBehaviorOutputTypeDef = TypedDict(
     "_OptionalBehaviorOutputTypeDef",
     {
         "metric": str,
-        "metricDimension": MetricDimensionOutputTypeDef,
+        "metricDimension": MetricDimensionTypeDef,
         "criteria": BehaviorCriteriaOutputTypeDef,
         "suppressAlerts": bool,
     },
     total=False,
 )
 
 class BehaviorOutputTypeDef(_RequiredBehaviorOutputTypeDef, _OptionalBehaviorOutputTypeDef):
@@ -9502,89 +8572,55 @@
 ):
     pass
 
 DescribeCACertificateResponseTypeDef = TypedDict(
     "DescribeCACertificateResponseTypeDef",
     {
         "certificateDescription": CACertificateDescriptionTypeDef,
-        "registrationConfig": RegistrationConfigOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "registrationConfig": RegistrationConfigTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCertificateResponseTypeDef = TypedDict(
     "DescribeCertificateResponseTypeDef",
     {
         "certificateDescription": CertificateDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListThingTypesResponseTypeDef = TypedDict(
     "ListThingTypesResponseTypeDef",
     {
         "thingTypes": List[ThingTypeDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSigningJobParameterOutputTypeDef = TypedDict(
-    "StartSigningJobParameterOutputTypeDef",
-    {
-        "signingProfileParameter": SigningProfileParameterOutputTypeDef,
-        "signingProfileName": str,
-        "destination": DestinationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 StartSigningJobParameterTypeDef = TypedDict(
     "StartSigningJobParameterTypeDef",
     {
         "signingProfileParameter": SigningProfileParameterTypeDef,
         "signingProfileName": str,
         "destination": DestinationTypeDef,
     },
     total=False,
 )
 
-JobExecutionsRolloutConfigOutputTypeDef = TypedDict(
-    "JobExecutionsRolloutConfigOutputTypeDef",
-    {
-        "maximumPerMinute": int,
-        "exponentialRate": ExponentialRolloutRateOutputTypeDef,
-    },
-    total=False,
-)
-
 JobExecutionsRolloutConfigTypeDef = TypedDict(
     "JobExecutionsRolloutConfigTypeDef",
     {
         "maximumPerMinute": int,
         "exponentialRate": ExponentialRolloutRateTypeDef,
     },
     total=False,
 )
 
-StreamInfoTypeDef = TypedDict(
-    "StreamInfoTypeDef",
-    {
-        "streamId": str,
-        "streamArn": str,
-        "streamVersion": int,
-        "description": str,
-        "files": List[StreamFileOutputTypeDef],
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "roleArn": str,
-    },
-    total=False,
-)
-
 _RequiredCreateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStreamRequestRequestTypeDef",
     {
         "streamId": str,
         "files": Sequence[StreamFileTypeDef],
         "roleArn": str,
     },
@@ -9599,14 +8635,29 @@
 )
 
 class CreateStreamRequestRequestTypeDef(
     _RequiredCreateStreamRequestRequestTypeDef, _OptionalCreateStreamRequestRequestTypeDef
 ):
     pass
 
+StreamInfoTypeDef = TypedDict(
+    "StreamInfoTypeDef",
+    {
+        "streamId": str,
+        "streamArn": str,
+        "streamVersion": int,
+        "description": str,
+        "files": List[StreamFileTypeDef],
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "roleArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateStreamRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStreamRequestRequestTypeDef",
     {
         "streamId": str,
     },
 )
 _OptionalUpdateStreamRequestRequestTypeDef = TypedDict(
@@ -9633,30 +8684,30 @@
         "version": int,
         "thingGroupProperties": ThingGroupPropertiesOutputTypeDef,
         "thingGroupMetadata": ThingGroupMetadataTypeDef,
         "indexName": str,
         "queryString": str,
         "queryVersion": str,
         "status": DynamicGroupStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHttpActionOutputTypeDef = TypedDict(
     "_RequiredHttpActionOutputTypeDef",
     {
         "url": str,
     },
 )
 _OptionalHttpActionOutputTypeDef = TypedDict(
     "_OptionalHttpActionOutputTypeDef",
     {
         "confirmationUrl": str,
-        "headers": List[HttpActionHeaderOutputTypeDef],
-        "auth": HttpAuthorizationOutputTypeDef,
+        "headers": List[HttpActionHeaderTypeDef],
+        "auth": HttpAuthorizationTypeDef,
     },
     total=False,
 )
 
 class HttpActionOutputTypeDef(_RequiredHttpActionOutputTypeDef, _OptionalHttpActionOutputTypeDef):
     pass
 
@@ -9680,15 +8731,15 @@
     pass
 
 GetIndexingConfigurationResponseTypeDef = TypedDict(
     "GetIndexingConfigurationResponseTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationOutputTypeDef,
         "thingGroupIndexingConfiguration": ThingGroupIndexingConfigurationOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIndexingConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateIndexingConfigurationRequestRequestTypeDef",
     {
         "thingIndexingConfiguration": ThingIndexingConfigurationTypeDef,
@@ -9697,66 +8748,66 @@
     total=False,
 )
 
 DescribeJobExecutionResponseTypeDef = TypedDict(
     "DescribeJobExecutionResponseTypeDef",
     {
         "execution": JobExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobExecutionsForJobResponseTypeDef = TypedDict(
     "ListJobExecutionsForJobResponseTypeDef",
     {
         "executionSummaries": List[JobExecutionSummaryForJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobExecutionsForThingResponseTypeDef = TypedDict(
     "ListJobExecutionsForThingResponseTypeDef",
     {
         "executionSummaries": List[JobExecutionSummaryForThingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecurityProfilesForTargetResponseTypeDef = TypedDict(
     "ListSecurityProfilesForTargetResponseTypeDef",
     {
         "securityProfileTargetMappings": List[SecurityProfileTargetMappingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListV2LoggingLevelsResponseTypeDef = TypedDict(
     "ListV2LoggingLevelsResponseTypeDef",
     {
         "logTargetConfigurations": List[LogTargetConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMitigationActionResponseTypeDef = TypedDict(
     "DescribeMitigationActionResponseTypeDef",
     {
         "actionName": str,
         "actionType": MitigationActionTypeType,
         "actionArn": str,
         "actionId": str,
         "roleArn": str,
         "actionParams": MitigationActionParamsOutputTypeDef,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MitigationActionTypeDef = TypedDict(
     "MitigationActionTypeDef",
     {
         "name": str,
@@ -9850,15 +8901,15 @@
 class RepublishActionTypeDef(_RequiredRepublishActionTypeDef, _OptionalRepublishActionTypeDef):
     pass
 
 _RequiredAuditSuppressionTypeDef = TypedDict(
     "_RequiredAuditSuppressionTypeDef",
     {
         "checkName": str,
-        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
+        "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 _OptionalAuditSuppressionTypeDef = TypedDict(
     "_OptionalAuditSuppressionTypeDef",
     {
         "expirationDate": datetime,
         "suppressIndefinitely": bool,
@@ -9866,46 +8917,14 @@
     },
     total=False,
 )
 
 class AuditSuppressionTypeDef(_RequiredAuditSuppressionTypeDef, _OptionalAuditSuppressionTypeDef):
     pass
 
-DescribeAuditSuppressionResponseTypeDef = TypedDict(
-    "DescribeAuditSuppressionResponseTypeDef",
-    {
-        "checkName": str,
-        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
-        "expirationDate": datetime,
-        "suppressIndefinitely": bool,
-        "description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-NonCompliantResourceTypeDef = TypedDict(
-    "NonCompliantResourceTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
-        "additionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
-RelatedResourceTypeDef = TypedDict(
-    "RelatedResourceTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceIdentifier": ResourceIdentifierOutputTypeDef,
-        "additionalInfo": Dict[str, str],
-    },
-    total=False,
-)
-
 _RequiredCreateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "clientRequestToken": str,
     },
@@ -9938,24 +8957,36 @@
     "DescribeAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
 
+DescribeAuditSuppressionResponseTypeDef = TypedDict(
+    "DescribeAuditSuppressionResponseTypeDef",
+    {
+        "checkName": str,
+        "resourceIdentifier": ResourceIdentifierTypeDef,
+        "expirationDate": datetime,
+        "suppressIndefinitely": bool,
+        "description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListAuditFindingsRequestListAuditFindingsPaginateTypeDef = TypedDict(
     "ListAuditFindingsRequestListAuditFindingsPaginateTypeDef",
     {
         "taskId": str,
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "startTime": Union[datetime, str],
         "endTime": Union[datetime, str],
         "listSuppressedFindings": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditFindingsRequestRequestTypeDef = TypedDict(
     "ListAuditFindingsRequestRequestTypeDef",
     {
@@ -9973,15 +9004,15 @@
 
 ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef = TypedDict(
     "ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
         "ascendingOrder": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListAuditSuppressionsRequestRequestTypeDef = TypedDict(
     "ListAuditSuppressionsRequestRequestTypeDef",
     {
@@ -9990,14 +9021,34 @@
         "ascendingOrder": bool,
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+NonCompliantResourceTypeDef = TypedDict(
+    "NonCompliantResourceTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceIdentifier": ResourceIdentifierTypeDef,
+        "additionalInfo": Dict[str, str],
+    },
+    total=False,
+)
+
+RelatedResourceTypeDef = TypedDict(
+    "RelatedResourceTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+        "resourceIdentifier": ResourceIdentifierTypeDef,
+        "additionalInfo": Dict[str, str],
+    },
+    total=False,
+)
+
 _RequiredUpdateAuditSuppressionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuditSuppressionRequestRequestTypeDef",
     {
         "checkName": str,
         "resourceIdentifier": ResourceIdentifierTypeDef,
     },
 )
@@ -10019,15 +9070,15 @@
 
 SearchIndexResponseTypeDef = TypedDict(
     "SearchIndexResponseTypeDef",
     {
         "nextToken": str,
         "things": List[ThingDocumentTypeDef],
         "thingGroups": List[ThingGroupDocumentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTopicRuleDestinationRequestRequestTypeDef = TypedDict(
     "CreateTopicRuleDestinationRequestRequestTypeDef",
     {
         "destinationConfiguration": TopicRuleDestinationConfigurationTypeDef,
@@ -10035,31 +9086,31 @@
 )
 
 ListTopicRuleDestinationsResponseTypeDef = TypedDict(
     "ListTopicRuleDestinationsResponseTypeDef",
     {
         "destinationSummaries": List[TopicRuleDestinationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTopicRuleDestinationResponseTypeDef = TypedDict(
     "CreateTopicRuleDestinationResponseTypeDef",
     {
         "topicRuleDestination": TopicRuleDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTopicRuleDestinationResponseTypeDef = TypedDict(
     "GetTopicRuleDestinationResponseTypeDef",
     {
         "topicRuleDestination": TopicRuleDestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuthResultTypeDef = TypedDict(
     "AuthResultTypeDef",
     {
         "authInfo": AuthInfoOutputTypeDef,
@@ -10107,38 +9158,38 @@
 DescribeSecurityProfileResponseTypeDef = TypedDict(
     "DescribeSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
         "behaviors": List[BehaviorOutputTypeDef],
-        "alertTargets": Dict[Literal["SNS"], AlertTargetOutputTypeDef],
+        "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
-        "additionalMetricsToRetainV2": List[MetricToRetainOutputTypeDef],
+        "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSecurityProfileResponseTypeDef = TypedDict(
     "UpdateSecurityProfileResponseTypeDef",
     {
         "securityProfileName": str,
         "securityProfileArn": str,
         "securityProfileDescription": str,
         "behaviors": List[BehaviorOutputTypeDef],
-        "alertTargets": Dict[Literal["SNS"], AlertTargetOutputTypeDef],
+        "alertTargets": Dict[Literal["SNS"], AlertTargetTypeDef],
         "additionalMetricsToRetain": List[str],
-        "additionalMetricsToRetainV2": List[MetricToRetainOutputTypeDef],
+        "additionalMetricsToRetainV2": List[MetricToRetainTypeDef],
         "version": int,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ViolationEventTypeDef = TypedDict(
     "ViolationEventTypeDef",
     {
         "violationId": str,
@@ -10215,15 +9266,15 @@
     },
 )
 
 CodeSigningOutputTypeDef = TypedDict(
     "CodeSigningOutputTypeDef",
     {
         "awsSignerJobId": str,
-        "startSigningJobParameter": StartSigningJobParameterOutputTypeDef,
+        "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningOutputTypeDef,
     },
     total=False,
 )
 
 CodeSigningTypeDef = TypedDict(
     "CodeSigningTypeDef",
@@ -10231,66 +9282,14 @@
         "awsSignerJobId": str,
         "startSigningJobParameter": StartSigningJobParameterTypeDef,
         "customCodeSigning": CustomCodeSigningTypeDef,
     },
     total=False,
 )
 
-DescribeJobTemplateResponseTypeDef = TypedDict(
-    "DescribeJobTemplateResponseTypeDef",
-    {
-        "jobTemplateArn": str,
-        "jobTemplateId": str,
-        "description": str,
-        "documentSource": str,
-        "document": str,
-        "createdAt": datetime,
-        "presignedUrlConfig": PresignedUrlConfigOutputTypeDef,
-        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigOutputTypeDef,
-        "abortConfig": AbortConfigOutputTypeDef,
-        "timeoutConfig": TimeoutConfigOutputTypeDef,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
-        "maintenanceWindows": List[MaintenanceWindowOutputTypeDef],
-        "destinationPackageVersions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-JobTypeDef = TypedDict(
-    "JobTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "targetSelection": TargetSelectionType,
-        "status": JobStatusType,
-        "forceCanceled": bool,
-        "reasonCode": str,
-        "comment": str,
-        "targets": List[str],
-        "description": str,
-        "presignedUrlConfig": PresignedUrlConfigOutputTypeDef,
-        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigOutputTypeDef,
-        "abortConfig": AbortConfigOutputTypeDef,
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "completedAt": datetime,
-        "jobProcessDetails": JobProcessDetailsTypeDef,
-        "timeoutConfig": TimeoutConfigOutputTypeDef,
-        "namespaceId": str,
-        "jobTemplateArn": str,
-        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
-        "documentParameters": Dict[str, str],
-        "isConcurrent": bool,
-        "schedulingConfig": SchedulingConfigOutputTypeDef,
-        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
-        "destinationPackageVersions": List[str],
-    },
-    total=False,
-)
-
 _RequiredCreateJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateJobRequestRequestTypeDef",
     {
         "jobId": str,
         "targets": Sequence[str],
     },
 )
@@ -10347,14 +9346,66 @@
 )
 
 class CreateJobTemplateRequestRequestTypeDef(
     _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
+DescribeJobTemplateResponseTypeDef = TypedDict(
+    "DescribeJobTemplateResponseTypeDef",
+    {
+        "jobTemplateArn": str,
+        "jobTemplateId": str,
+        "description": str,
+        "documentSource": str,
+        "document": str,
+        "createdAt": datetime,
+        "presignedUrlConfig": PresignedUrlConfigTypeDef,
+        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
+        "timeoutConfig": TimeoutConfigTypeDef,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "maintenanceWindows": List[MaintenanceWindowTypeDef],
+        "destinationPackageVersions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+JobTypeDef = TypedDict(
+    "JobTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "targetSelection": TargetSelectionType,
+        "status": JobStatusType,
+        "forceCanceled": bool,
+        "reasonCode": str,
+        "comment": str,
+        "targets": List[str],
+        "description": str,
+        "presignedUrlConfig": PresignedUrlConfigTypeDef,
+        "jobExecutionsRolloutConfig": JobExecutionsRolloutConfigTypeDef,
+        "abortConfig": AbortConfigOutputTypeDef,
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "completedAt": datetime,
+        "jobProcessDetails": JobProcessDetailsTypeDef,
+        "timeoutConfig": TimeoutConfigTypeDef,
+        "namespaceId": str,
+        "jobTemplateArn": str,
+        "jobExecutionsRetryConfig": JobExecutionsRetryConfigOutputTypeDef,
+        "documentParameters": Dict[str, str],
+        "isConcurrent": bool,
+        "schedulingConfig": SchedulingConfigOutputTypeDef,
+        "scheduledJobRollouts": List[ScheduledJobRolloutTypeDef],
+        "destinationPackageVersions": List[str],
+    },
+    total=False,
+)
+
 _RequiredUpdateJobRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 _OptionalUpdateJobRequestRequestTypeDef = TypedDict(
@@ -10376,29 +9427,29 @@
 ):
     pass
 
 DescribeStreamResponseTypeDef = TypedDict(
     "DescribeStreamResponseTypeDef",
     {
         "streamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAuditMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeAuditMitigationActionsTaskResponseTypeDef",
     {
         "taskStatus": AuditMitigationActionsTaskStatusType,
         "startTime": datetime,
         "endTime": datetime,
         "taskStatistics": Dict[str, TaskStatisticsForAuditCheckTypeDef],
         "target": AuditMitigationActionsTaskTargetOutputTypeDef,
         "auditCheckToActionsMapping": Dict[str, List[str]],
         "actionsDefinition": List[MitigationActionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectMitigationActionsTaskSummaryTypeDef = TypedDict(
     "DetectMitigationActionsTaskSummaryTypeDef",
     {
         "taskId": str,
@@ -10416,15 +9467,15 @@
 )
 
 ListAuditSuppressionsResponseTypeDef = TypedDict(
     "ListAuditSuppressionsResponseTypeDef",
     {
         "suppressions": List[AuditSuppressionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AuditFindingTypeDef = TypedDict(
     "AuditFindingTypeDef",
     {
         "findingId": str,
@@ -10443,52 +9494,52 @@
 )
 
 ListRelatedResourcesForAuditFindingResponseTypeDef = TypedDict(
     "ListRelatedResourcesForAuditFindingResponseTypeDef",
     {
         "relatedResources": List[RelatedResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TestAuthorizationResponseTypeDef = TypedDict(
     "TestAuthorizationResponseTypeDef",
     {
         "authResults": List[AuthResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ActionOutputTypeDef = TypedDict(
     "ActionOutputTypeDef",
     {
-        "dynamoDB": DynamoDBActionOutputTypeDef,
-        "dynamoDBv2": DynamoDBv2ActionOutputTypeDef,
-        "lambda": LambdaActionOutputTypeDef,
-        "sns": SnsActionOutputTypeDef,
-        "sqs": SqsActionOutputTypeDef,
-        "kinesis": KinesisActionOutputTypeDef,
+        "dynamoDB": DynamoDBActionTypeDef,
+        "dynamoDBv2": DynamoDBv2ActionTypeDef,
+        "lambda": LambdaActionTypeDef,
+        "sns": SnsActionTypeDef,
+        "sqs": SqsActionTypeDef,
+        "kinesis": KinesisActionTypeDef,
         "republish": RepublishActionOutputTypeDef,
-        "s3": S3ActionOutputTypeDef,
-        "firehose": FirehoseActionOutputTypeDef,
-        "cloudwatchMetric": CloudwatchMetricActionOutputTypeDef,
-        "cloudwatchAlarm": CloudwatchAlarmActionOutputTypeDef,
-        "cloudwatchLogs": CloudwatchLogsActionOutputTypeDef,
-        "elasticsearch": ElasticsearchActionOutputTypeDef,
-        "salesforce": SalesforceActionOutputTypeDef,
-        "iotAnalytics": IotAnalyticsActionOutputTypeDef,
-        "iotEvents": IotEventsActionOutputTypeDef,
+        "s3": S3ActionTypeDef,
+        "firehose": FirehoseActionTypeDef,
+        "cloudwatchMetric": CloudwatchMetricActionTypeDef,
+        "cloudwatchAlarm": CloudwatchAlarmActionTypeDef,
+        "cloudwatchLogs": CloudwatchLogsActionTypeDef,
+        "elasticsearch": ElasticsearchActionTypeDef,
+        "salesforce": SalesforceActionTypeDef,
+        "iotAnalytics": IotAnalyticsActionTypeDef,
+        "iotEvents": IotEventsActionTypeDef,
         "iotSiteWise": IotSiteWiseActionOutputTypeDef,
-        "stepFunctions": StepFunctionsActionOutputTypeDef,
+        "stepFunctions": StepFunctionsActionTypeDef,
         "timestream": TimestreamActionOutputTypeDef,
         "http": HttpActionOutputTypeDef,
         "kafka": KafkaActionOutputTypeDef,
-        "openSearch": OpenSearchActionOutputTypeDef,
-        "location": LocationActionOutputTypeDef,
+        "openSearch": OpenSearchActionTypeDef,
+        "location": LocationActionTypeDef,
     },
     total=False,
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
@@ -10520,34 +9571,34 @@
 )
 
 ListActiveViolationsResponseTypeDef = TypedDict(
     "ListActiveViolationsResponseTypeDef",
     {
         "activeViolations": List[ActiveViolationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListViolationEventsResponseTypeDef = TypedDict(
     "ListViolationEventsResponseTypeDef",
     {
         "violationEvents": List[ViolationEventTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OTAUpdateFileOutputTypeDef = TypedDict(
     "OTAUpdateFileOutputTypeDef",
     {
         "fileName": str,
         "fileType": int,
         "fileVersion": str,
-        "fileLocation": FileLocationOutputTypeDef,
+        "fileLocation": FileLocationTypeDef,
         "codeSigning": CodeSigningOutputTypeDef,
         "attributes": Dict[str, str],
     },
     total=False,
 )
 
 OTAUpdateFileTypeDef = TypedDict(
@@ -10564,49 +9615,49 @@
 )
 
 DescribeJobResponseTypeDef = TypedDict(
     "DescribeJobResponseTypeDef",
     {
         "documentSource": str,
         "job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDetectMitigationActionsTaskResponseTypeDef = TypedDict(
     "DescribeDetectMitigationActionsTaskResponseTypeDef",
     {
         "taskSummary": DetectMitigationActionsTaskSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDetectMitigationActionsTasksResponseTypeDef = TypedDict(
     "ListDetectMitigationActionsTasksResponseTypeDef",
     {
         "tasks": List[DetectMitigationActionsTaskSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAuditFindingResponseTypeDef = TypedDict(
     "DescribeAuditFindingResponseTypeDef",
     {
         "finding": AuditFindingTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAuditFindingsResponseTypeDef = TypedDict(
     "ListAuditFindingsResponseTypeDef",
     {
         "findings": List[AuditFindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TopicRuleTypeDef = TypedDict(
     "TopicRuleTypeDef",
     {
         "ruleName": str,
@@ -10648,16 +9699,16 @@
         "otaUpdateId": str,
         "otaUpdateArn": str,
         "creationDate": datetime,
         "lastModifiedDate": datetime,
         "description": str,
         "targets": List[str],
         "protocols": List[ProtocolType],
-        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigOutputTypeDef,
-        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigOutputTypeDef,
+        "awsJobExecutionsRolloutConfig": AwsJobExecutionsRolloutConfigTypeDef,
+        "awsJobPresignedUrlConfig": AwsJobPresignedUrlConfigTypeDef,
         "targetSelection": TargetSelectionType,
         "otaUpdateFiles": List[OTAUpdateFileOutputTypeDef],
         "otaUpdateStatus": OTAUpdateStatusType,
         "awsIotJobId": str,
         "awsIotJobArn": str,
         "errorInfo": ErrorInfoTypeDef,
         "additionalParameters": Dict[str, str],
@@ -10696,15 +9747,15 @@
     pass
 
 GetTopicRuleResponseTypeDef = TypedDict(
     "GetTopicRuleResponseTypeDef",
     {
         "ruleArn": str,
         "rule": TopicRuleTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateTopicRuleRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTopicRuleRequestRequestTypeDef",
     {
         "ruleName": str,
@@ -10732,10 +9783,10 @@
     },
 )
 
 GetOTAUpdateResponseTypeDef = TypedDict(
     "GetOTAUpdateResponseTypeDef",
     {
         "otaUpdateInfo": OTAUpdateInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/PKG-INFO` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-iot
-Version: 1.28.12
-Summary: Type annotations for boto3.IoT 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-iot.svg?color=blue)](https://pypi.org/project/mypy-boto3-iot)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-iot)](https://pepy.tech/project/mypy-boto3-iot)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.IoT 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
+[boto3.IoT 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot.html#IoT)
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
 [mypy-boto3-iot docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_iot/).
 
 See how it helps to find and fix potential bugs:
 
@@ -645,167 +645,110 @@
 ### Typed dictionaries
 
 `mypy_boto3_iot.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_iot.type_defs import (
-    AbortCriteriaOutputTypeDef,
     AbortCriteriaTypeDef,
     AcceptCertificateTransferRequestRequestTypeDef,
-    CloudwatchAlarmActionOutputTypeDef,
-    CloudwatchLogsActionOutputTypeDef,
-    CloudwatchMetricActionOutputTypeDef,
-    DynamoDBActionOutputTypeDef,
-    ElasticsearchActionOutputTypeDef,
-    FirehoseActionOutputTypeDef,
-    IotAnalyticsActionOutputTypeDef,
-    IotEventsActionOutputTypeDef,
-    KafkaActionOutputTypeDef,
-    KinesisActionOutputTypeDef,
-    LambdaActionOutputTypeDef,
-    OpenSearchActionOutputTypeDef,
-    S3ActionOutputTypeDef,
-    SalesforceActionOutputTypeDef,
-    SnsActionOutputTypeDef,
-    SqsActionOutputTypeDef,
-    StepFunctionsActionOutputTypeDef,
     CloudwatchAlarmActionTypeDef,
     CloudwatchLogsActionTypeDef,
     CloudwatchMetricActionTypeDef,
     DynamoDBActionTypeDef,
     ElasticsearchActionTypeDef,
     FirehoseActionTypeDef,
     IotAnalyticsActionTypeDef,
     IotEventsActionTypeDef,
-    KafkaActionTypeDef,
+    KafkaActionOutputTypeDef,
     KinesisActionTypeDef,
     LambdaActionTypeDef,
     OpenSearchActionTypeDef,
     S3ActionTypeDef,
     SalesforceActionTypeDef,
     SnsActionTypeDef,
     SqsActionTypeDef,
     StepFunctionsActionTypeDef,
+    KafkaActionTypeDef,
     MetricValueOutputTypeDef,
     ViolationEventAdditionalInfoTypeDef,
     AddThingToBillingGroupRequestRequestTypeDef,
     AddThingToThingGroupRequestRequestTypeDef,
     AddThingsToThingGroupParamsOutputTypeDef,
     AddThingsToThingGroupParamsTypeDef,
     AggregationTypeOutputTypeDef,
     AggregationTypeTypeDef,
-    AlertTargetOutputTypeDef,
     AlertTargetTypeDef,
     PolicyTypeDef,
-    AssetPropertyTimestampOutputTypeDef,
     AssetPropertyTimestampTypeDef,
-    AssetPropertyVariantOutputTypeDef,
     AssetPropertyVariantTypeDef,
     AssociateTargetsWithJobRequestRequestTypeDef,
-    AssociateTargetsWithJobResponseTypeDef,
+    ResponseMetadataTypeDef,
     AttachPolicyRequestRequestTypeDef,
     AttachPrincipalPolicyRequestRequestTypeDef,
     AttachSecurityProfileRequestRequestTypeDef,
     AttachThingPrincipalRequestRequestTypeDef,
     AttributePayloadOutputTypeDef,
     AttributePayloadTypeDef,
-    AuditCheckConfigurationOutputTypeDef,
     AuditCheckConfigurationTypeDef,
     AuditCheckDetailsTypeDef,
     AuditMitigationActionExecutionMetadataTypeDef,
     AuditMitigationActionsTaskMetadataTypeDef,
     AuditMitigationActionsTaskTargetOutputTypeDef,
     AuditMitigationActionsTaskTargetTypeDef,
-    AuditNotificationTargetOutputTypeDef,
     AuditNotificationTargetTypeDef,
     AuditTaskMetadataTypeDef,
     AuthInfoOutputTypeDef,
     AuthInfoTypeDef,
-    AuthorizerConfigOutputTypeDef,
     AuthorizerConfigTypeDef,
     AuthorizerDescriptionTypeDef,
     AuthorizerSummaryTypeDef,
     AwsJobAbortCriteriaTypeDef,
-    AwsJobRateIncreaseCriteriaOutputTypeDef,
     AwsJobRateIncreaseCriteriaTypeDef,
-    AwsJobPresignedUrlConfigOutputTypeDef,
     AwsJobPresignedUrlConfigTypeDef,
     AwsJobTimeoutConfigTypeDef,
-    MachineLearningDetectionConfigOutputTypeDef,
-    StatisticalThresholdOutputTypeDef,
     MachineLearningDetectionConfigTypeDef,
-    MetricValueTypeDef,
     StatisticalThresholdTypeDef,
+    MetricValueTypeDef,
     BehaviorModelTrainingSummaryTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     BillingGroupMetadataTypeDef,
-    BillingGroupPropertiesOutputTypeDef,
     BillingGroupPropertiesTypeDef,
     BucketTypeDef,
     TermsAggregationTypeDef,
     CertificateValidityTypeDef,
     CACertificateTypeDef,
     CancelAuditMitigationActionsTaskRequestRequestTypeDef,
     CancelAuditTaskRequestRequestTypeDef,
     CancelCertificateTransferRequestRequestTypeDef,
     CancelDetectMitigationActionsTaskRequestRequestTypeDef,
     CancelJobExecutionRequestRequestTypeDef,
     CancelJobRequestRequestTypeDef,
-    CancelJobResponseTypeDef,
     TransferDataTypeDef,
     CertificateTypeDef,
-    CodeSigningCertificateChainOutputTypeDef,
     CodeSigningCertificateChainTypeDef,
     CodeSigningSignatureOutputTypeDef,
     CodeSigningSignatureTypeDef,
-    ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     ConfirmTopicRuleDestinationRequestRequestTypeDef,
     TagTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    CreateBillingGroupResponseTypeDef,
     CreateCertificateFromCsrRequestRequestTypeDef,
-    CreateCertificateFromCsrResponseTypeDef,
-    CreateCustomMetricResponseTypeDef,
-    CreateDimensionResponseTypeDef,
     TlsConfigTypeDef,
-    CreateDomainConfigurationResponseTypeDef,
-    CreateDynamicThingGroupResponseTypeDef,
-    CreateFleetMetricResponseTypeDef,
     PresignedUrlConfigTypeDef,
     TimeoutConfigTypeDef,
-    CreateJobResponseTypeDef,
     MaintenanceWindowTypeDef,
-    CreateJobTemplateResponseTypeDef,
     CreateKeysAndCertificateRequestRequestTypeDef,
     KeyPairTypeDef,
-    CreateMitigationActionResponseTypeDef,
-    CreateOTAUpdateResponseTypeDef,
     CreatePackageRequestRequestTypeDef,
-    CreatePackageResponseTypeDef,
     CreatePackageVersionRequestRequestTypeDef,
-    CreatePackageVersionResponseTypeDef,
-    CreatePolicyResponseTypeDef,
     CreatePolicyVersionRequestRequestTypeDef,
-    CreatePolicyVersionResponseTypeDef,
     CreateProvisioningClaimRequestRequestTypeDef,
     ProvisioningHookTypeDef,
-    CreateProvisioningTemplateResponseTypeDef,
     CreateProvisioningTemplateVersionRequestRequestTypeDef,
-    CreateProvisioningTemplateVersionResponseTypeDef,
-    CreateRoleAliasResponseTypeDef,
-    CreateScheduledAuditResponseTypeDef,
-    CreateSecurityProfileResponseTypeDef,
-    CreateStreamResponseTypeDef,
-    CreateThingGroupResponseTypeDef,
-    CreateThingResponseTypeDef,
     ThingTypePropertiesTypeDef,
-    CreateThingTypeResponseTypeDef,
     DeleteAccountAuditConfigurationRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteBillingGroupRequestRequestTypeDef,
     DeleteCACertificateRequestRequestTypeDef,
     DeleteCertificateRequestRequestTypeDef,
     DeleteCustomMetricRequestRequestTypeDef,
     DeleteDimensionRequestRequestTypeDef,
@@ -838,371 +781,309 @@
     DescribeAuditMitigationActionsTaskRequestRequestTypeDef,
     TaskStatisticsForAuditCheckTypeDef,
     DescribeAuditTaskRequestRequestTypeDef,
     TaskStatisticsTypeDef,
     DescribeAuthorizerRequestRequestTypeDef,
     DescribeBillingGroupRequestRequestTypeDef,
     DescribeCACertificateRequestRequestTypeDef,
-    RegistrationConfigOutputTypeDef,
+    RegistrationConfigTypeDef,
     DescribeCertificateRequestRequestTypeDef,
     DescribeCustomMetricRequestRequestTypeDef,
-    DescribeCustomMetricResponseTypeDef,
     DescribeDetectMitigationActionsTaskRequestRequestTypeDef,
     DescribeDimensionRequestRequestTypeDef,
-    DescribeDimensionResponseTypeDef,
     DescribeDomainConfigurationRequestRequestTypeDef,
     ServerCertificateSummaryTypeDef,
-    TlsConfigOutputTypeDef,
     DescribeEndpointRequestRequestTypeDef,
-    DescribeEndpointResponseTypeDef,
     DescribeFleetMetricRequestRequestTypeDef,
     DescribeIndexRequestRequestTypeDef,
-    DescribeIndexResponseTypeDef,
     DescribeJobExecutionRequestRequestTypeDef,
     DescribeJobRequestRequestTypeDef,
     DescribeJobTemplateRequestRequestTypeDef,
-    MaintenanceWindowOutputTypeDef,
-    PresignedUrlConfigOutputTypeDef,
-    TimeoutConfigOutputTypeDef,
     DescribeManagedJobTemplateRequestRequestTypeDef,
     DocumentParameterTypeDef,
     DescribeMitigationActionRequestRequestTypeDef,
     DescribeProvisioningTemplateRequestRequestTypeDef,
-    ProvisioningHookOutputTypeDef,
     DescribeProvisioningTemplateVersionRequestRequestTypeDef,
-    DescribeProvisioningTemplateVersionResponseTypeDef,
     DescribeRoleAliasRequestRequestTypeDef,
     RoleAliasDescriptionTypeDef,
     DescribeScheduledAuditRequestRequestTypeDef,
-    DescribeScheduledAuditResponseTypeDef,
     DescribeSecurityProfileRequestRequestTypeDef,
     DescribeStreamRequestRequestTypeDef,
     DescribeThingGroupRequestRequestTypeDef,
     DescribeThingRegistrationTaskRequestRequestTypeDef,
-    DescribeThingRegistrationTaskResponseTypeDef,
     DescribeThingRequestRequestTypeDef,
-    DescribeThingResponseTypeDef,
     DescribeThingTypeRequestRequestTypeDef,
     ThingTypeMetadataTypeDef,
     ThingTypePropertiesOutputTypeDef,
-    S3DestinationOutputTypeDef,
     S3DestinationTypeDef,
     DetachPolicyRequestRequestTypeDef,
     DetachPrincipalPolicyRequestRequestTypeDef,
     DetachSecurityProfileRequestRequestTypeDef,
     DetachThingPrincipalRequestRequestTypeDef,
     DetectMitigationActionExecutionTypeDef,
     DetectMitigationActionsTaskStatisticsTypeDef,
     DetectMitigationActionsTaskTargetOutputTypeDef,
     ViolationEventOccurrenceRangeOutputTypeDef,
     DetectMitigationActionsTaskTargetTypeDef,
     DisableTopicRuleRequestRequestTypeDef,
     DomainConfigurationSummaryTypeDef,
-    PutItemInputOutputTypeDef,
     PutItemInputTypeDef,
     EffectivePolicyTypeDef,
-    EmptyResponseMetadataTypeDef,
-    EnableIoTLoggingParamsOutputTypeDef,
     EnableIoTLoggingParamsTypeDef,
     EnableTopicRuleRequestRequestTypeDef,
     ErrorInfoTypeDef,
-    RateIncreaseCriteriaOutputTypeDef,
     RateIncreaseCriteriaTypeDef,
-    FieldOutputTypeDef,
     FieldTypeDef,
-    S3LocationOutputTypeDef,
-    StreamOutputTypeDef,
     S3LocationTypeDef,
     StreamTypeDef,
     FleetMetricNameAndArnTypeDef,
-    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetBehaviorModelTrainingSummariesRequestRequestTypeDef,
     GetCardinalityRequestRequestTypeDef,
-    GetCardinalityResponseTypeDef,
     GetEffectivePoliciesRequestRequestTypeDef,
     GetJobDocumentRequestRequestTypeDef,
-    GetJobDocumentResponseTypeDef,
-    GetLoggingOptionsResponseTypeDef,
     GetOTAUpdateRequestRequestTypeDef,
-    VersionUpdateByJobsConfigOutputTypeDef,
+    VersionUpdateByJobsConfigTypeDef,
     GetPackageRequestRequestTypeDef,
-    GetPackageResponseTypeDef,
     GetPackageVersionRequestRequestTypeDef,
-    GetPackageVersionResponseTypeDef,
     GetPercentilesRequestRequestTypeDef,
     PercentPairTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetPolicyResponseTypeDef,
     GetPolicyVersionRequestRequestTypeDef,
-    GetPolicyVersionResponseTypeDef,
-    GetRegistrationCodeResponseTypeDef,
     GetStatisticsRequestRequestTypeDef,
     StatisticsTypeDef,
     GetTopicRuleDestinationRequestRequestTypeDef,
     GetTopicRuleRequestRequestTypeDef,
-    GetV2LoggingOptionsResponseTypeDef,
     GroupNameAndArnTypeDef,
-    HttpActionHeaderOutputTypeDef,
     HttpActionHeaderTypeDef,
-    SigV4AuthorizationOutputTypeDef,
     SigV4AuthorizationTypeDef,
     HttpContextTypeDef,
     HttpUrlDestinationConfigurationTypeDef,
     HttpUrlDestinationPropertiesTypeDef,
     HttpUrlDestinationSummaryTypeDef,
     IndexingFilterOutputTypeDef,
     IndexingFilterTypeDef,
-    IssuerCertificateIdentifierOutputTypeDef,
     IssuerCertificateIdentifierTypeDef,
     JobExecutionStatusDetailsTypeDef,
     JobExecutionSummaryTypeDef,
-    RetryCriteriaOutputTypeDef,
     RetryCriteriaTypeDef,
     JobProcessDetailsTypeDef,
     JobSummaryTypeDef,
     JobTemplateSummaryTypeDef,
     ScheduledJobRolloutTypeDef,
-    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
     ListActiveViolationsRequestRequestTypeDef,
-    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
     ListAttachedPoliciesRequestRequestTypeDef,
-    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
     ListAuditMitigationActionsExecutionsRequestRequestTypeDef,
-    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
     ListAuditMitigationActionsTasksRequestRequestTypeDef,
-    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
     ListAuditTasksRequestRequestTypeDef,
-    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
     ListAuthorizersRequestRequestTypeDef,
-    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
     ListBillingGroupsRequestRequestTypeDef,
-    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
     ListCACertificatesRequestRequestTypeDef,
-    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
     ListCertificatesByCARequestRequestTypeDef,
-    ListCertificatesRequestListCertificatesPaginateTypeDef,
     ListCertificatesRequestRequestTypeDef,
-    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
     ListCustomMetricsRequestRequestTypeDef,
-    ListCustomMetricsResponseTypeDef,
-    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
     ListDetectMitigationActionsExecutionsRequestRequestTypeDef,
-    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
     ListDetectMitigationActionsTasksRequestRequestTypeDef,
-    ListDimensionsRequestListDimensionsPaginateTypeDef,
     ListDimensionsRequestRequestTypeDef,
-    ListDimensionsResponseTypeDef,
-    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
     ListDomainConfigurationsRequestRequestTypeDef,
-    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
     ListFleetMetricsRequestRequestTypeDef,
-    ListIndicesRequestListIndicesPaginateTypeDef,
     ListIndicesRequestRequestTypeDef,
-    ListIndicesResponseTypeDef,
-    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
     ListJobExecutionsForJobRequestRequestTypeDef,
-    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
     ListJobExecutionsForThingRequestRequestTypeDef,
-    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
     ListJobTemplatesRequestRequestTypeDef,
-    ListJobsRequestListJobsPaginateTypeDef,
     ListJobsRequestRequestTypeDef,
-    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
     ListManagedJobTemplatesRequestRequestTypeDef,
     ManagedJobTemplateSummaryTypeDef,
-    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
     ListMetricValuesRequestRequestTypeDef,
-    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
     ListMitigationActionsRequestRequestTypeDef,
     MitigationActionIdentifierTypeDef,
-    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
     ListOTAUpdatesRequestRequestTypeDef,
     OTAUpdateSummaryTypeDef,
-    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
     ListOutgoingCertificatesRequestRequestTypeDef,
     OutgoingCertificateTypeDef,
-    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
     ListPackageVersionsRequestRequestTypeDef,
     PackageVersionSummaryTypeDef,
-    ListPackagesRequestListPackagesPaginateTypeDef,
     ListPackagesRequestRequestTypeDef,
     PackageSummaryTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
-    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
     ListPolicyPrincipalsRequestRequestTypeDef,
-    ListPolicyPrincipalsResponseTypeDef,
     ListPolicyVersionsRequestRequestTypeDef,
     PolicyVersionTypeDef,
-    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
     ListPrincipalPoliciesRequestRequestTypeDef,
-    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
     ListPrincipalThingsRequestRequestTypeDef,
-    ListPrincipalThingsResponseTypeDef,
-    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
     ListProvisioningTemplateVersionsRequestRequestTypeDef,
     ProvisioningTemplateVersionSummaryTypeDef,
-    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
     ListProvisioningTemplatesRequestRequestTypeDef,
     ProvisioningTemplateSummaryTypeDef,
-    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
     ListRelatedResourcesForAuditFindingRequestRequestTypeDef,
-    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
     ListRoleAliasesRequestRequestTypeDef,
-    ListRoleAliasesResponseTypeDef,
-    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
     ListScheduledAuditsRequestRequestTypeDef,
     ScheduledAuditMetadataTypeDef,
-    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
     ListSecurityProfilesForTargetRequestRequestTypeDef,
-    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
     ListSecurityProfilesRequestRequestTypeDef,
     SecurityProfileIdentifierTypeDef,
-    ListStreamsRequestListStreamsPaginateTypeDef,
     ListStreamsRequestRequestTypeDef,
     StreamSummaryTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    TagOutputTypeDef,
-    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
     ListTargetsForPolicyRequestRequestTypeDef,
-    ListTargetsForPolicyResponseTypeDef,
-    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
     ListTargetsForSecurityProfileRequestRequestTypeDef,
     SecurityProfileTargetTypeDef,
-    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
     ListThingGroupsForThingRequestRequestTypeDef,
-    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
     ListThingGroupsRequestRequestTypeDef,
-    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
     ListThingPrincipalsRequestRequestTypeDef,
-    ListThingPrincipalsResponseTypeDef,
-    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
     ListThingRegistrationTaskReportsRequestRequestTypeDef,
-    ListThingRegistrationTaskReportsResponseTypeDef,
-    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
     ListThingRegistrationTasksRequestRequestTypeDef,
-    ListThingRegistrationTasksResponseTypeDef,
-    ListThingTypesRequestListThingTypesPaginateTypeDef,
     ListThingTypesRequestRequestTypeDef,
-    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
     ListThingsInBillingGroupRequestRequestTypeDef,
-    ListThingsInBillingGroupResponseTypeDef,
-    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
     ListThingsInThingGroupRequestRequestTypeDef,
-    ListThingsInThingGroupResponseTypeDef,
-    ListThingsRequestListThingsPaginateTypeDef,
     ListThingsRequestRequestTypeDef,
     ThingAttributeTypeDef,
-    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
     ListTopicRuleDestinationsRequestRequestTypeDef,
-    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
     ListTopicRulesRequestRequestTypeDef,
     TopicRuleListItemTypeDef,
-    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
     ListV2LoggingLevelsRequestRequestTypeDef,
-    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     ListViolationEventsRequestRequestTypeDef,
-    LocationTimestampOutputTypeDef,
     LocationTimestampTypeDef,
-    LogTargetOutputTypeDef,
     LogTargetTypeDef,
     LoggingOptionsPayloadTypeDef,
-    PublishFindingToSnsParamsOutputTypeDef,
-    ReplaceDefaultPolicyVersionParamsOutputTypeDef,
-    UpdateCACertificateParamsOutputTypeDef,
-    UpdateDeviceCertificateParamsOutputTypeDef,
     PublishFindingToSnsParamsTypeDef,
     ReplaceDefaultPolicyVersionParamsTypeDef,
     UpdateCACertificateParamsTypeDef,
     UpdateDeviceCertificateParamsTypeDef,
     MqttContextTypeDef,
-    UserPropertyOutputTypeDef,
     UserPropertyTypeDef,
-    PaginatorConfigTypeDef,
-    PolicyVersionIdentifierOutputTypeDef,
     PolicyVersionIdentifierTypeDef,
     PutVerificationStateOnViolationRequestRequestTypeDef,
-    RegistrationConfigTypeDef,
-    RegisterCACertificateResponseTypeDef,
     RegisterCertificateRequestRequestTypeDef,
-    RegisterCertificateResponseTypeDef,
     RegisterCertificateWithoutCARequestRequestTypeDef,
-    RegisterCertificateWithoutCAResponseTypeDef,
     RegisterThingRequestRequestTypeDef,
-    RegisterThingResponseTypeDef,
     RejectCertificateTransferRequestRequestTypeDef,
     RemoveThingFromBillingGroupRequestRequestTypeDef,
     RemoveThingFromThingGroupRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     SearchIndexRequestRequestTypeDef,
     ThingGroupDocumentTypeDef,
     SetDefaultAuthorizerRequestRequestTypeDef,
-    SetDefaultAuthorizerResponseTypeDef,
     SetDefaultPolicyVersionRequestRequestTypeDef,
     SetV2LoggingOptionsRequestRequestTypeDef,
-    SigningProfileParameterOutputTypeDef,
     SigningProfileParameterTypeDef,
-    StartAuditMitigationActionsTaskResponseTypeDef,
     ViolationEventOccurrenceRangeTypeDef,
-    StartDetectMitigationActionsTaskResponseTypeDef,
     StartOnDemandAuditTaskRequestRequestTypeDef,
-    StartOnDemandAuditTaskResponseTypeDef,
     StartThingRegistrationTaskRequestRequestTypeDef,
-    StartThingRegistrationTaskResponseTypeDef,
     StopThingRegistrationTaskRequestRequestTypeDef,
     TlsContextTypeDef,
-    TestInvokeAuthorizerResponseTypeDef,
     ThingConnectivityTypeDef,
-    TimestreamDimensionOutputTypeDef,
-    TimestreamTimestampOutputTypeDef,
     TimestreamDimensionTypeDef,
     TimestreamTimestampTypeDef,
     VpcDestinationConfigurationTypeDef,
     VpcDestinationSummaryTypeDef,
     VpcDestinationPropertiesTypeDef,
     TransferCertificateRequestRequestTypeDef,
-    TransferCertificateResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    UpdateBillingGroupResponseTypeDef,
     UpdateCertificateRequestRequestTypeDef,
     UpdateCustomMetricRequestRequestTypeDef,
-    UpdateCustomMetricResponseTypeDef,
     UpdateDimensionRequestRequestTypeDef,
-    UpdateDimensionResponseTypeDef,
-    UpdateDomainConfigurationResponseTypeDef,
-    UpdateDynamicThingGroupResponseTypeDef,
-    UpdateMitigationActionResponseTypeDef,
-    VersionUpdateByJobsConfigTypeDef,
     UpdatePackageRequestRequestTypeDef,
     UpdatePackageVersionRequestRequestTypeDef,
     UpdateRoleAliasRequestRequestTypeDef,
-    UpdateRoleAliasResponseTypeDef,
     UpdateScheduledAuditRequestRequestTypeDef,
-    UpdateScheduledAuditResponseTypeDef,
-    UpdateStreamResponseTypeDef,
-    UpdateThingGroupResponseTypeDef,
     UpdateThingGroupsForThingRequestRequestTypeDef,
     UpdateTopicRuleDestinationRequestRequestTypeDef,
     ValidationErrorTypeDef,
     AbortConfigOutputTypeDef,
     AbortConfigTypeDef,
     MetricDatumTypeDef,
-    DescribeFleetMetricResponseTypeDef,
     UpdateFleetMetricRequestRequestTypeDef,
     AllowedTypeDef,
     ExplicitDenyTypeDef,
     ImplicitDenyTypeDef,
+    AssetPropertyValueTypeDef,
+    AssociateTargetsWithJobResponseTypeDef,
+    CancelJobResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateBillingGroupResponseTypeDef,
+    CreateCertificateFromCsrResponseTypeDef,
+    CreateCustomMetricResponseTypeDef,
+    CreateDimensionResponseTypeDef,
+    CreateDomainConfigurationResponseTypeDef,
+    CreateDynamicThingGroupResponseTypeDef,
+    CreateFleetMetricResponseTypeDef,
+    CreateJobResponseTypeDef,
+    CreateJobTemplateResponseTypeDef,
+    CreateMitigationActionResponseTypeDef,
+    CreateOTAUpdateResponseTypeDef,
+    CreatePackageResponseTypeDef,
+    CreatePackageVersionResponseTypeDef,
+    CreatePolicyResponseTypeDef,
+    CreatePolicyVersionResponseTypeDef,
+    CreateProvisioningTemplateResponseTypeDef,
+    CreateProvisioningTemplateVersionResponseTypeDef,
+    CreateRoleAliasResponseTypeDef,
+    CreateScheduledAuditResponseTypeDef,
+    CreateSecurityProfileResponseTypeDef,
+    CreateStreamResponseTypeDef,
+    CreateThingGroupResponseTypeDef,
+    CreateThingResponseTypeDef,
+    CreateThingTypeResponseTypeDef,
+    DescribeCustomMetricResponseTypeDef,
+    DescribeDimensionResponseTypeDef,
+    DescribeEndpointResponseTypeDef,
+    DescribeFleetMetricResponseTypeDef,
+    DescribeIndexResponseTypeDef,
+    DescribeProvisioningTemplateVersionResponseTypeDef,
+    DescribeScheduledAuditResponseTypeDef,
+    DescribeThingRegistrationTaskResponseTypeDef,
+    DescribeThingResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCardinalityResponseTypeDef,
+    GetJobDocumentResponseTypeDef,
+    GetLoggingOptionsResponseTypeDef,
+    GetPackageResponseTypeDef,
+    GetPackageVersionResponseTypeDef,
+    GetPolicyResponseTypeDef,
+    GetPolicyVersionResponseTypeDef,
+    GetRegistrationCodeResponseTypeDef,
+    GetV2LoggingOptionsResponseTypeDef,
     ListAttachedPoliciesResponseTypeDef,
+    ListCustomMetricsResponseTypeDef,
+    ListDimensionsResponseTypeDef,
+    ListIndicesResponseTypeDef,
     ListPoliciesResponseTypeDef,
+    ListPolicyPrincipalsResponseTypeDef,
     ListPrincipalPoliciesResponseTypeDef,
-    AssetPropertyValueOutputTypeDef,
-    AssetPropertyValueTypeDef,
+    ListPrincipalThingsResponseTypeDef,
+    ListRoleAliasesResponseTypeDef,
+    ListTargetsForPolicyResponseTypeDef,
+    ListThingPrincipalsResponseTypeDef,
+    ListThingRegistrationTaskReportsResponseTypeDef,
+    ListThingRegistrationTasksResponseTypeDef,
+    ListThingsInBillingGroupResponseTypeDef,
+    ListThingsInThingGroupResponseTypeDef,
+    RegisterCACertificateResponseTypeDef,
+    RegisterCertificateResponseTypeDef,
+    RegisterCertificateWithoutCAResponseTypeDef,
+    RegisterThingResponseTypeDef,
+    SetDefaultAuthorizerResponseTypeDef,
+    StartAuditMitigationActionsTaskResponseTypeDef,
+    StartDetectMitigationActionsTaskResponseTypeDef,
+    StartOnDemandAuditTaskResponseTypeDef,
+    StartThingRegistrationTaskResponseTypeDef,
+    TestInvokeAuthorizerResponseTypeDef,
+    TransferCertificateResponseTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateBillingGroupResponseTypeDef,
+    UpdateCustomMetricResponseTypeDef,
+    UpdateDimensionResponseTypeDef,
+    UpdateDomainConfigurationResponseTypeDef,
+    UpdateDynamicThingGroupResponseTypeDef,
+    UpdateMitigationActionResponseTypeDef,
+    UpdateRoleAliasResponseTypeDef,
+    UpdateScheduledAuditResponseTypeDef,
+    UpdateStreamResponseTypeDef,
+    UpdateThingGroupResponseTypeDef,
     ThingGroupPropertiesOutputTypeDef,
     CreateThingRequestRequestTypeDef,
     ThingGroupPropertiesTypeDef,
     UpdateThingRequestRequestTypeDef,
     ListAuditMitigationActionsExecutionsResponseTypeDef,
     ListAuditMitigationActionsTasksResponseTypeDef,
     StartAuditMitigationActionsTaskRequestRequestTypeDef,
@@ -1210,20 +1091,18 @@
     UpdateAccountAuditConfigurationRequestRequestTypeDef,
     ListAuditTasksResponseTypeDef,
     TestAuthorizationRequestRequestTypeDef,
     DescribeAuthorizerResponseTypeDef,
     DescribeDefaultAuthorizerResponseTypeDef,
     ListAuthorizersResponseTypeDef,
     AwsJobAbortConfigTypeDef,
-    AwsJobExponentialRolloutRateOutputTypeDef,
     AwsJobExponentialRolloutRateTypeDef,
     BehaviorCriteriaOutputTypeDef,
     BehaviorCriteriaTypeDef,
     GetBehaviorModelTrainingSummariesResponseTypeDef,
-    MetricToRetainOutputTypeDef,
     MetricToRetainTypeDef,
     DescribeBillingGroupResponseTypeDef,
     UpdateBillingGroupRequestRequestTypeDef,
     GetBucketsAggregationResponseTypeDef,
     BucketsAggregationTypeTypeDef,
     CACertificateDescriptionTypeDef,
     ListCACertificatesResponseTypeDef,
@@ -1238,55 +1117,110 @@
     CreateBillingGroupRequestRequestTypeDef,
     CreateCustomMetricRequestRequestTypeDef,
     CreateDimensionRequestRequestTypeDef,
     CreateFleetMetricRequestRequestTypeDef,
     CreatePolicyRequestRequestTypeDef,
     CreateRoleAliasRequestRequestTypeDef,
     CreateScheduledAuditRequestRequestTypeDef,
+    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDomainConfigurationRequestRequestTypeDef,
     UpdateDomainConfigurationRequestRequestTypeDef,
+    SchedulingConfigOutputTypeDef,
     SchedulingConfigTypeDef,
     CreateKeysAndCertificateResponseTypeDef,
     CreateProvisioningClaimResponseTypeDef,
     CreateProvisioningTemplateRequestRequestTypeDef,
+    DescribeProvisioningTemplateResponseTypeDef,
     UpdateProvisioningTemplateRequestRequestTypeDef,
     CreateThingTypeRequestRequestTypeDef,
     DescribeAuditTaskResponseTypeDef,
+    RegisterCACertificateRequestRequestTypeDef,
+    UpdateCACertificateRequestRequestTypeDef,
     DescribeDomainConfigurationResponseTypeDef,
-    SchedulingConfigOutputTypeDef,
     DescribeManagedJobTemplateResponseTypeDef,
-    DescribeProvisioningTemplateResponseTypeDef,
     DescribeRoleAliasResponseTypeDef,
     DescribeThingTypeResponseTypeDef,
     ThingTypeDefinitionTypeDef,
-    DestinationOutputTypeDef,
     DestinationTypeDef,
     ListDetectMitigationActionsExecutionsResponseTypeDef,
     ListDomainConfigurationsResponseTypeDef,
-    DynamoDBv2ActionOutputTypeDef,
     DynamoDBv2ActionTypeDef,
     GetEffectivePoliciesResponseTypeDef,
-    ExponentialRolloutRateOutputTypeDef,
     ExponentialRolloutRateTypeDef,
     ThingGroupIndexingConfigurationOutputTypeDef,
     ThingGroupIndexingConfigurationTypeDef,
-    StreamFileOutputTypeDef,
-    FileLocationOutputTypeDef,
     StreamFileTypeDef,
     FileLocationTypeDef,
     ListFleetMetricsResponseTypeDef,
+    GetBehaviorModelTrainingSummariesRequestGetBehaviorModelTrainingSummariesPaginateTypeDef,
+    ListActiveViolationsRequestListActiveViolationsPaginateTypeDef,
+    ListAttachedPoliciesRequestListAttachedPoliciesPaginateTypeDef,
+    ListAuditMitigationActionsExecutionsRequestListAuditMitigationActionsExecutionsPaginateTypeDef,
+    ListAuditMitigationActionsTasksRequestListAuditMitigationActionsTasksPaginateTypeDef,
+    ListAuditTasksRequestListAuditTasksPaginateTypeDef,
+    ListAuthorizersRequestListAuthorizersPaginateTypeDef,
+    ListBillingGroupsRequestListBillingGroupsPaginateTypeDef,
+    ListCACertificatesRequestListCACertificatesPaginateTypeDef,
+    ListCertificatesByCARequestListCertificatesByCAPaginateTypeDef,
+    ListCertificatesRequestListCertificatesPaginateTypeDef,
+    ListCustomMetricsRequestListCustomMetricsPaginateTypeDef,
+    ListDetectMitigationActionsExecutionsRequestListDetectMitigationActionsExecutionsPaginateTypeDef,
+    ListDetectMitigationActionsTasksRequestListDetectMitigationActionsTasksPaginateTypeDef,
+    ListDimensionsRequestListDimensionsPaginateTypeDef,
+    ListDomainConfigurationsRequestListDomainConfigurationsPaginateTypeDef,
+    ListFleetMetricsRequestListFleetMetricsPaginateTypeDef,
+    ListIndicesRequestListIndicesPaginateTypeDef,
+    ListJobExecutionsForJobRequestListJobExecutionsForJobPaginateTypeDef,
+    ListJobExecutionsForThingRequestListJobExecutionsForThingPaginateTypeDef,
+    ListJobTemplatesRequestListJobTemplatesPaginateTypeDef,
+    ListJobsRequestListJobsPaginateTypeDef,
+    ListManagedJobTemplatesRequestListManagedJobTemplatesPaginateTypeDef,
+    ListMetricValuesRequestListMetricValuesPaginateTypeDef,
+    ListMitigationActionsRequestListMitigationActionsPaginateTypeDef,
+    ListOTAUpdatesRequestListOTAUpdatesPaginateTypeDef,
+    ListOutgoingCertificatesRequestListOutgoingCertificatesPaginateTypeDef,
+    ListPackageVersionsRequestListPackageVersionsPaginateTypeDef,
+    ListPackagesRequestListPackagesPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListPolicyPrincipalsRequestListPolicyPrincipalsPaginateTypeDef,
+    ListPrincipalPoliciesRequestListPrincipalPoliciesPaginateTypeDef,
+    ListPrincipalThingsRequestListPrincipalThingsPaginateTypeDef,
+    ListProvisioningTemplateVersionsRequestListProvisioningTemplateVersionsPaginateTypeDef,
+    ListProvisioningTemplatesRequestListProvisioningTemplatesPaginateTypeDef,
+    ListRelatedResourcesForAuditFindingRequestListRelatedResourcesForAuditFindingPaginateTypeDef,
+    ListRoleAliasesRequestListRoleAliasesPaginateTypeDef,
+    ListScheduledAuditsRequestListScheduledAuditsPaginateTypeDef,
+    ListSecurityProfilesForTargetRequestListSecurityProfilesForTargetPaginateTypeDef,
+    ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef,
+    ListStreamsRequestListStreamsPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    ListTargetsForPolicyRequestListTargetsForPolicyPaginateTypeDef,
+    ListTargetsForSecurityProfileRequestListTargetsForSecurityProfilePaginateTypeDef,
+    ListThingGroupsForThingRequestListThingGroupsForThingPaginateTypeDef,
+    ListThingGroupsRequestListThingGroupsPaginateTypeDef,
+    ListThingPrincipalsRequestListThingPrincipalsPaginateTypeDef,
+    ListThingRegistrationTaskReportsRequestListThingRegistrationTaskReportsPaginateTypeDef,
+    ListThingRegistrationTasksRequestListThingRegistrationTasksPaginateTypeDef,
+    ListThingTypesRequestListThingTypesPaginateTypeDef,
+    ListThingsInBillingGroupRequestListThingsInBillingGroupPaginateTypeDef,
+    ListThingsInThingGroupRequestListThingsInThingGroupPaginateTypeDef,
+    ListThingsRequestListThingsPaginateTypeDef,
+    ListTopicRuleDestinationsRequestListTopicRuleDestinationsPaginateTypeDef,
+    ListTopicRulesRequestListTopicRulesPaginateTypeDef,
+    ListV2LoggingLevelsRequestListV2LoggingLevelsPaginateTypeDef,
+    ListViolationEventsRequestListViolationEventsPaginateTypeDef,
     GetPackageConfigurationResponseTypeDef,
+    UpdatePackageConfigurationRequestRequestTypeDef,
     GetPercentilesResponseTypeDef,
     GetStatisticsResponseTypeDef,
     ListBillingGroupsResponseTypeDef,
     ListThingGroupsForThingResponseTypeDef,
     ListThingGroupsResponseTypeDef,
     ThingGroupMetadataTypeDef,
-    HttpAuthorizationOutputTypeDef,
     HttpAuthorizationTypeDef,
     ThingIndexingConfigurationOutputTypeDef,
     ThingIndexingConfigurationTypeDef,
     JobExecutionTypeDef,
     JobExecutionSummaryForJobTypeDef,
     JobExecutionSummaryForThingTypeDef,
     JobExecutionsRetryConfigOutputTypeDef,
@@ -1301,64 +1235,55 @@
     ListPackagesResponseTypeDef,
     ListPolicyVersionsResponseTypeDef,
     ListProvisioningTemplateVersionsResponseTypeDef,
     ListProvisioningTemplatesResponseTypeDef,
     ListScheduledAuditsResponseTypeDef,
     ListSecurityProfilesResponseTypeDef,
     ListStreamsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTargetsForSecurityProfileResponseTypeDef,
     SecurityProfileTargetMappingTypeDef,
     ListThingsResponseTypeDef,
     ListTopicRulesResponseTypeDef,
-    LocationActionOutputTypeDef,
     LocationActionTypeDef,
     LogTargetConfigurationTypeDef,
     SetV2LoggingLevelRequestRequestTypeDef,
     SetLoggingOptionsRequestRequestTypeDef,
     MitigationActionParamsOutputTypeDef,
     MitigationActionParamsTypeDef,
     MqttHeadersOutputTypeDef,
     MqttHeadersTypeDef,
-    ResourceIdentifierOutputTypeDef,
     ResourceIdentifierTypeDef,
-    RegisterCACertificateRequestRequestTypeDef,
-    UpdateCACertificateRequestRequestTypeDef,
     StartDetectMitigationActionsTaskRequestRequestTypeDef,
     TestInvokeAuthorizerRequestRequestTypeDef,
     ThingDocumentTypeDef,
     TimestreamActionOutputTypeDef,
     TimestreamActionTypeDef,
     TopicRuleDestinationConfigurationTypeDef,
     TopicRuleDestinationSummaryTypeDef,
     TopicRuleDestinationTypeDef,
-    UpdatePackageConfigurationRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsResponseTypeDef,
     ListMetricValuesResponseTypeDef,
     DeniedTypeDef,
     PutAssetPropertyValueEntryOutputTypeDef,
     PutAssetPropertyValueEntryTypeDef,
     CreateDynamicThingGroupRequestRequestTypeDef,
     CreateThingGroupRequestRequestTypeDef,
     UpdateDynamicThingGroupRequestRequestTypeDef,
     UpdateThingGroupRequestRequestTypeDef,
-    AwsJobExecutionsRolloutConfigOutputTypeDef,
     AwsJobExecutionsRolloutConfigTypeDef,
     BehaviorOutputTypeDef,
     BehaviorTypeDef,
     GetBucketsAggregationRequestRequestTypeDef,
     DescribeCACertificateResponseTypeDef,
     DescribeCertificateResponseTypeDef,
     ListThingTypesResponseTypeDef,
-    StartSigningJobParameterOutputTypeDef,
     StartSigningJobParameterTypeDef,
-    JobExecutionsRolloutConfigOutputTypeDef,
     JobExecutionsRolloutConfigTypeDef,
-    StreamInfoTypeDef,
     CreateStreamRequestRequestTypeDef,
+    StreamInfoTypeDef,
     UpdateStreamRequestRequestTypeDef,
     DescribeThingGroupResponseTypeDef,
     HttpActionOutputTypeDef,
     HttpActionTypeDef,
     GetIndexingConfigurationResponseTypeDef,
     UpdateIndexingConfigurationRequestRequestTypeDef,
     DescribeJobExecutionResponseTypeDef,
@@ -1369,24 +1294,24 @@
     DescribeMitigationActionResponseTypeDef,
     MitigationActionTypeDef,
     CreateMitigationActionRequestRequestTypeDef,
     UpdateMitigationActionRequestRequestTypeDef,
     RepublishActionOutputTypeDef,
     RepublishActionTypeDef,
     AuditSuppressionTypeDef,
-    DescribeAuditSuppressionResponseTypeDef,
-    NonCompliantResourceTypeDef,
-    RelatedResourceTypeDef,
     CreateAuditSuppressionRequestRequestTypeDef,
     DeleteAuditSuppressionRequestRequestTypeDef,
     DescribeAuditSuppressionRequestRequestTypeDef,
+    DescribeAuditSuppressionResponseTypeDef,
     ListAuditFindingsRequestListAuditFindingsPaginateTypeDef,
     ListAuditFindingsRequestRequestTypeDef,
     ListAuditSuppressionsRequestListAuditSuppressionsPaginateTypeDef,
     ListAuditSuppressionsRequestRequestTypeDef,
+    NonCompliantResourceTypeDef,
+    RelatedResourceTypeDef,
     UpdateAuditSuppressionRequestRequestTypeDef,
     SearchIndexResponseTypeDef,
     CreateTopicRuleDestinationRequestRequestTypeDef,
     ListTopicRuleDestinationsResponseTypeDef,
     CreateTopicRuleDestinationResponseTypeDef,
     GetTopicRuleDestinationResponseTypeDef,
     AuthResultTypeDef,
@@ -1397,18 +1322,18 @@
     UpdateSecurityProfileResponseTypeDef,
     ViolationEventTypeDef,
     CreateSecurityProfileRequestRequestTypeDef,
     UpdateSecurityProfileRequestRequestTypeDef,
     ValidateSecurityProfileBehaviorsRequestRequestTypeDef,
     CodeSigningOutputTypeDef,
     CodeSigningTypeDef,
-    DescribeJobTemplateResponseTypeDef,
-    JobTypeDef,
     CreateJobRequestRequestTypeDef,
     CreateJobTemplateRequestRequestTypeDef,
+    DescribeJobTemplateResponseTypeDef,
+    JobTypeDef,
     UpdateJobRequestRequestTypeDef,
     DescribeStreamResponseTypeDef,
     DescribeAuditMitigationActionsTaskResponseTypeDef,
     DetectMitigationActionsTaskSummaryTypeDef,
     ListAuditSuppressionsResponseTypeDef,
     AuditFindingTypeDef,
     ListRelatedResourcesForAuditFindingResponseTypeDef,
@@ -1431,15 +1356,15 @@
     GetTopicRuleResponseTypeDef,
     CreateTopicRuleRequestRequestTypeDef,
     ReplaceTopicRuleRequestRequestTypeDef,
     GetOTAUpdateResponseTypeDef,
 )
 
 
-def get_structure() -> AbortCriteriaOutputTypeDef:
+def get_structure() -> AbortCriteriaTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-iot-1.28.12/mypy_boto3_iot.egg-info/SOURCES.txt` & `mypy-boto3-iot-1.28.15/mypy_boto3_iot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-iot-1.28.12/setup.py` & `mypy-boto3-iot-1.28.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-iot",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_iot"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.IoT 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.IoT 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

