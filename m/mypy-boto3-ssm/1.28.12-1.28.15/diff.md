# Comparing `tmp/mypy-boto3-ssm-1.28.12.tar.gz` & `tmp/mypy-boto3-ssm-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ssm-1.28.12.tar", last modified: Thu Jul 27 11:49:42 2023, max compression
+gzip compressed data, was "mypy-boto3-ssm-1.28.15.tar", last modified: Fri Jul 28 20:43:49 2023, max compression
```

## Comparing `mypy-boto3-ssm-1.28.12.tar` & `mypy-boto3-ssm-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.701330 mypy-boto3-ssm-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    47440 2023-07-27 11:49:42.701330 mypy-boto3-ssm-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    45969 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.693330 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/
--rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   131264 2023-07-27 11:47:18.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   131071 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-27 11:47:21.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-07-27 11:47:21.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    59186 2023-07-27 11:47:20.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    59137 2023-07-27 11:47:20.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   217858 2023-07-27 11:47:28.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   217610 2023-07-27 11:47:23.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 11:47:17.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-27 11:47:20.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-27 11:47:20.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 11:49:42.701330 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47440 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 11:49:42.000000 mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 11:49:42.701330 mypy-boto3-ssm-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 11:47:16.000000 mypy-boto3-ssm-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.085937 mypy-boto3-ssm-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46800 2023-07-28 20:43:49.081937 mypy-boto3-ssm-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    45329 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.073937 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/
+-rw-r--r--   0 runner    (1001) docker     (123)    12702 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12701 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131264 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131071 2023-07-28 20:39:51.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28172 2023-07-28 20:39:56.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28170 2023-07-28 20:39:56.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    59186 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59137 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   213242 2023-07-28 20:40:02.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213000 2023-07-28 20:39:59.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-07-28 20:39:52.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:43:49.081937 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46800 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:43:48.000000 mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:43:49.085937 mypy-boto3-ssm-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:39:50.000000 mypy-boto3-ssm-1.28.15/setup.py
```

### Comparing `mypy-boto3-ssm-1.28.12/LICENSE` & `mypy-boto3-ssm-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/PKG-INFO` & `mypy-boto3-ssm-1.28.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.28.12
-Summary: Type annotations for boto3.SSM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -643,17 +643,15 @@
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
-    AlarmOutputTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
     AssociationStatusOutputTypeDef,
     TargetOutputTypeDef,
@@ -667,15 +665,14 @@
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CloudWatchOutputConfigOutputTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigOutputTypeDef,
     ComplianceExecutionSummaryOutputTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
@@ -734,19 +731,17 @@
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
-    DocumentRequiresOutputTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
-    DocumentReviewCommentSourceOutputTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -759,33 +754,31 @@
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
     MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
-    LoggingInfoOutputTypeDef,
+    LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
-    MetadataValueOutputTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
     PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
-    S3OutputLocationOutputTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
@@ -794,40 +787,33 @@
     ListDocumentVersionsRequestRequestTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    LoggingInfoTypeDef,
     MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersOutputTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
     NotificationConfigTypeDef,
-    MaintenanceWindowStepFunctionsParametersOutputTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
-    OpsItemDataValueOutputTypeDef,
     OpsItemIdentityTypeDef,
-    OpsItemNotificationOutputTypeDef,
-    RelatedOpsItemOutputTypeDef,
     ParameterInlinePolicyTypeDef,
     PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
-    ResourceDataSyncOrganizationalUnitOutputTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
-    ResourceDataSyncDestinationDataSharingOutputTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
     ResumeSessionRequestRequestTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
     StartSessionRequestRequestTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
@@ -908,17 +894,22 @@
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
     DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
+    DocumentIdentifierTypeDef,
+    GetDocumentResultTypeDef,
+    OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
+    OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
+    GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
     DescribeActivationsRequestRequestTypeDef,
     DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
@@ -985,40 +976,36 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribePatchBaselinesResultTypeDef,
     PatchGroupPatchBaselineMappingTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
-    DocumentIdentifierTypeDef,
-    GetDocumentResultTypeDef,
     DocumentDescriptionTypeDef,
     ListDocumentsRequestListDocumentsPaginateTypeDef,
     ListDocumentsRequestRequestTypeDef,
     DocumentReviewerResponseSourceTypeDef,
     DocumentReviewsTypeDef,
     ListDocumentVersionsResultTypeDef,
     EffectivePatchTypeDef,
     GetCommandInvocationRequestCommandExecutedWaitTypeDef,
     InventoryGroupTypeDef,
     ListInventoryEntriesRequestRequestTypeDef,
     GetInventoryRequestGetInventoryPaginateTypeDef,
     GetInventoryRequestRequestTypeDef,
-    GetOpsMetadataResultTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
-    InstanceAssociationOutputLocationOutputTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
     InventoryItemSchemaTypeDef,
     PutInventoryRequestRequestTypeDef,
     InventoryResultEntityTypeDef,
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
@@ -1026,25 +1013,22 @@
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
     OpsEntityTypeDef,
-    OpsItemSummaryTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
-    OpsItemTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
     PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
     ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
-    ResourceDataSyncS3DestinationOutputTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
@@ -1056,16 +1040,18 @@
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
     ListCommandInvocationsResultTypeDef,
     MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
-    DescribePatchGroupsResultTypeDef,
     ListDocumentsResultTypeDef,
+    DescribeOpsItemsResponseTypeDef,
+    GetOpsItemResponseTypeDef,
+    DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
     DocumentMetadataResponseInfoTypeDef,
     UpdateDocumentMetadataRequestRequestTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     InventoryAggregatorTypeDef,
@@ -1073,18 +1059,16 @@
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
     MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
-    DescribeOpsItemsResponseTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
-    GetOpsItemResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
     PatchRuleOutputTypeDef,
     PatchRuleTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
     ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
```

### Comparing `mypy-boto3-ssm-1.28.12/README.md` & `mypy-boto3-ssm-1.28.15/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -611,17 +611,15 @@
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
-    AlarmOutputTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
     AssociationStatusOutputTypeDef,
     TargetOutputTypeDef,
@@ -635,15 +633,14 @@
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CloudWatchOutputConfigOutputTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigOutputTypeDef,
     ComplianceExecutionSummaryOutputTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
@@ -702,19 +699,17 @@
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
-    DocumentRequiresOutputTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
-    DocumentReviewCommentSourceOutputTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -727,33 +722,31 @@
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
     MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
-    LoggingInfoOutputTypeDef,
+    LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
-    MetadataValueOutputTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
     PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
-    S3OutputLocationOutputTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
@@ -762,40 +755,33 @@
     ListDocumentVersionsRequestRequestTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    LoggingInfoTypeDef,
     MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersOutputTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
     NotificationConfigTypeDef,
-    MaintenanceWindowStepFunctionsParametersOutputTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
-    OpsItemDataValueOutputTypeDef,
     OpsItemIdentityTypeDef,
-    OpsItemNotificationOutputTypeDef,
-    RelatedOpsItemOutputTypeDef,
     ParameterInlinePolicyTypeDef,
     PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
-    ResourceDataSyncOrganizationalUnitOutputTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
-    ResourceDataSyncDestinationDataSharingOutputTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
     ResumeSessionRequestRequestTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
     StartSessionRequestRequestTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
@@ -876,17 +862,22 @@
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
     DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
+    DocumentIdentifierTypeDef,
+    GetDocumentResultTypeDef,
+    OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
+    OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
+    GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
     DescribeActivationsRequestRequestTypeDef,
     DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
@@ -953,40 +944,36 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribePatchBaselinesResultTypeDef,
     PatchGroupPatchBaselineMappingTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
-    DocumentIdentifierTypeDef,
-    GetDocumentResultTypeDef,
     DocumentDescriptionTypeDef,
     ListDocumentsRequestListDocumentsPaginateTypeDef,
     ListDocumentsRequestRequestTypeDef,
     DocumentReviewerResponseSourceTypeDef,
     DocumentReviewsTypeDef,
     ListDocumentVersionsResultTypeDef,
     EffectivePatchTypeDef,
     GetCommandInvocationRequestCommandExecutedWaitTypeDef,
     InventoryGroupTypeDef,
     ListInventoryEntriesRequestRequestTypeDef,
     GetInventoryRequestGetInventoryPaginateTypeDef,
     GetInventoryRequestRequestTypeDef,
-    GetOpsMetadataResultTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
-    InstanceAssociationOutputLocationOutputTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
     InventoryItemSchemaTypeDef,
     PutInventoryRequestRequestTypeDef,
     InventoryResultEntityTypeDef,
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
@@ -994,25 +981,22 @@
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
     OpsEntityTypeDef,
-    OpsItemSummaryTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
-    OpsItemTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
     PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
     ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
-    ResourceDataSyncS3DestinationOutputTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
@@ -1024,16 +1008,18 @@
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
     ListCommandInvocationsResultTypeDef,
     MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
-    DescribePatchGroupsResultTypeDef,
     ListDocumentsResultTypeDef,
+    DescribeOpsItemsResponseTypeDef,
+    GetOpsItemResponseTypeDef,
+    DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
     DocumentMetadataResponseInfoTypeDef,
     UpdateDocumentMetadataRequestRequestTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     InventoryAggregatorTypeDef,
@@ -1041,18 +1027,16 @@
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
     MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
-    DescribeOpsItemsResponseTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
-    GetOpsItemResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
     PatchRuleOutputTypeDef,
     PatchRuleTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
     ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
```

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__init__.py` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__init__.pyi` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/__main__.py` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.SSM 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.SSM 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM\nOther"
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

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/client.py` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/client.pyi` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/literals.py` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/literals.pyi` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/paginator.py` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/paginator.pyi` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/type_defs.py` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,17 +104,15 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountSharingInfoTypeDef",
-    "TagOutputTypeDef",
     "TagTypeDef",
-    "AlarmOutputTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
     "AssociationStatusOutputTypeDef",
     "TargetOutputTypeDef",
@@ -128,15 +126,14 @@
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
-    "CloudWatchOutputConfigOutputTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
     "NotificationConfigOutputTypeDef",
     "ComplianceExecutionSummaryOutputTypeDef",
     "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
@@ -195,19 +192,17 @@
     "PatchBaselineIdentityTypeDef",
     "DescribePatchGroupStateRequestRequestTypeDef",
     "DescribePatchPropertiesRequestRequestTypeDef",
     "SessionFilterTypeDef",
     "DisassociateOpsItemRelatedItemRequestRequestTypeDef",
     "DocumentDefaultVersionDescriptionTypeDef",
     "DocumentParameterTypeDef",
-    "DocumentRequiresOutputTypeDef",
     "ReviewInformationTypeDef",
     "DocumentFilterTypeDef",
     "DocumentKeyValuesFilterTypeDef",
-    "DocumentReviewCommentSourceOutputTypeDef",
     "DocumentReviewCommentSourceTypeDef",
     "DocumentVersionInfoTypeDef",
     "PatchStatusTypeDef",
     "FailureDetailsTypeDef",
     "GetAutomationExecutionRequestRequestTypeDef",
     "GetCalendarStateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -220,33 +215,31 @@
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
-    "LoggingInfoOutputTypeDef",
+    "LoggingInfoTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
-    "MetadataValueOutputTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
     "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
-    "S3OutputLocationOutputTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
     "InventoryDeletionSummaryItemTypeDef",
     "InventoryItemAttributeTypeDef",
     "InventoryItemTypeDef",
     "InventoryResultItemTypeDef",
     "LabelParameterVersionRequestRequestTypeDef",
@@ -255,40 +248,33 @@
     "ListDocumentVersionsRequestRequestTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "LoggingInfoTypeDef",
     "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
     "MaintenanceWindowLambdaParametersOutputTypeDef",
     "MaintenanceWindowLambdaParametersTypeDef",
     "NotificationConfigTypeDef",
-    "MaintenanceWindowStepFunctionsParametersOutputTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
-    "OpsItemDataValueOutputTypeDef",
     "OpsItemIdentityTypeDef",
-    "OpsItemNotificationOutputTypeDef",
-    "RelatedOpsItemOutputTypeDef",
     "ParameterInlinePolicyTypeDef",
     "PatchFilterOutputTypeDef",
     "PatchFilterTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
-    "ResourceDataSyncOrganizationalUnitOutputTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
-    "ResourceDataSyncDestinationDataSharingOutputTypeDef",
     "ResourceDataSyncDestinationDataSharingTypeDef",
     "ResumeSessionRequestRequestTypeDef",
     "SendAutomationSignalRequestRequestTypeDef",
     "SessionManagerOutputUrlTypeDef",
     "StartAssociationsOnceRequestRequestTypeDef",
     "StartSessionRequestRequestTypeDef",
     "StopAutomationExecutionRequestRequestTypeDef",
@@ -369,17 +355,22 @@
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
     "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "CreateDocumentRequestRequestTypeDef",
+    "DocumentIdentifierTypeDef",
+    "GetDocumentResultTypeDef",
+    "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
+    "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
     "CreateOpsMetadataRequestRequestTypeDef",
+    "GetOpsMetadataResultTypeDef",
     "UpdateOpsMetadataRequestRequestTypeDef",
     "DescribeActivationsRequestRequestTypeDef",
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
@@ -446,40 +437,36 @@
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "DescribePatchBaselinesResultTypeDef",
     "PatchGroupPatchBaselineMappingTypeDef",
     "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
     "UpdateDocumentDefaultVersionResultTypeDef",
-    "DocumentIdentifierTypeDef",
-    "GetDocumentResultTypeDef",
     "DocumentDescriptionTypeDef",
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     "ListDocumentsRequestRequestTypeDef",
     "DocumentReviewerResponseSourceTypeDef",
     "DocumentReviewsTypeDef",
     "ListDocumentVersionsResultTypeDef",
     "EffectivePatchTypeDef",
     "GetCommandInvocationRequestCommandExecutedWaitTypeDef",
     "InventoryGroupTypeDef",
     "ListInventoryEntriesRequestRequestTypeDef",
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     "GetInventoryRequestRequestTypeDef",
-    "GetOpsMetadataResultTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
-    "InstanceAssociationOutputLocationOutputTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
     "InventoryItemSchemaTypeDef",
     "PutInventoryRequestRequestTypeDef",
     "InventoryResultEntityTypeDef",
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
@@ -487,25 +474,22 @@
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
     "MaintenanceWindowRunCommandParametersTypeDef",
     "OpsEntityTypeDef",
-    "OpsItemSummaryTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
-    "OpsItemTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
     "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceTypeDef",
-    "ResourceDataSyncS3DestinationOutputTypeDef",
     "ResourceDataSyncS3DestinationTypeDef",
     "SessionTypeDef",
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
@@ -517,16 +501,18 @@
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
     "ListCommandInvocationsResultTypeDef",
     "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
-    "DescribePatchGroupsResultTypeDef",
     "ListDocumentsResultTypeDef",
+    "DescribeOpsItemsResponseTypeDef",
+    "GetOpsItemResponseTypeDef",
+    "DescribePatchGroupsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
     "DocumentMetadataResponseInfoTypeDef",
     "UpdateDocumentMetadataRequestRequestTypeDef",
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     "InventoryAggregatorTypeDef",
@@ -534,18 +520,16 @@
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
     "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
-    "DescribeOpsItemsResponseTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
-    "GetOpsItemResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
     "PatchRuleOutputTypeDef",
     "PatchRuleTypeDef",
     "ResourceDataSyncSourceWithStateTypeDef",
     "ResourceDataSyncSourceTypeDef",
     "DescribeSessionsResponseTypeDef",
@@ -606,37 +590,22 @@
     {
         "AccountId": str,
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AlarmOutputTypeDef = TypedDict(
-    "AlarmOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -860,23 +829,14 @@
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-CloudWatchOutputConfigOutputTypeDef = TypedDict(
-    "CloudWatchOutputConfigOutputTypeDef",
-    {
-        "CloudWatchLogGroupName": str,
-        "CloudWatchOutputEnabled": bool,
-    },
-    total=False,
-)
-
 CloudWatchOutputConfigTypeDef = TypedDict(
     "CloudWatchOutputConfigTypeDef",
     {
         "CloudWatchLogGroupName": str,
         "CloudWatchOutputEnabled": bool,
     },
     total=False,
@@ -1779,37 +1739,14 @@
         "Type": DocumentParameterTypeType,
         "Description": str,
         "DefaultValue": str,
     },
     total=False,
 )
 
-_RequiredDocumentRequiresOutputTypeDef = TypedDict(
-    "_RequiredDocumentRequiresOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDocumentRequiresOutputTypeDef = TypedDict(
-    "_OptionalDocumentRequiresOutputTypeDef",
-    {
-        "Version": str,
-        "RequireType": str,
-        "VersionName": str,
-    },
-    total=False,
-)
-
-
-class DocumentRequiresOutputTypeDef(
-    _RequiredDocumentRequiresOutputTypeDef, _OptionalDocumentRequiresOutputTypeDef
-):
-    pass
-
-
 ReviewInformationTypeDef = TypedDict(
     "ReviewInformationTypeDef",
     {
         "ReviewedTime": datetime,
         "Status": ReviewStatusType,
         "Reviewer": str,
     },
@@ -1829,23 +1766,14 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DocumentReviewCommentSourceOutputTypeDef = TypedDict(
-    "DocumentReviewCommentSourceOutputTypeDef",
-    {
-        "Type": Literal["Comment"],
-        "Content": str,
-    },
-    total=False,
-)
-
 DocumentReviewCommentSourceTypeDef = TypedDict(
     "DocumentReviewCommentSourceTypeDef",
     {
         "Type": Literal["Comment"],
         "Content": str,
     },
     total=False,
@@ -2068,33 +1996,31 @@
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-_RequiredLoggingInfoOutputTypeDef = TypedDict(
-    "_RequiredLoggingInfoOutputTypeDef",
+_RequiredLoggingInfoTypeDef = TypedDict(
+    "_RequiredLoggingInfoTypeDef",
     {
         "S3BucketName": str,
         "S3Region": str,
     },
 )
-_OptionalLoggingInfoOutputTypeDef = TypedDict(
-    "_OptionalLoggingInfoOutputTypeDef",
+_OptionalLoggingInfoTypeDef = TypedDict(
+    "_OptionalLoggingInfoTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
 
-class LoggingInfoOutputTypeDef(
-    _RequiredLoggingInfoOutputTypeDef, _OptionalLoggingInfoOutputTypeDef
-):
+class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
     pass
 
 
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
@@ -2133,22 +2059,14 @@
 
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
 
-MetadataValueOutputTypeDef = TypedDict(
-    "MetadataValueOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2350,24 +2268,14 @@
     {
         "DetailedStatus": str,
         "InstanceAssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
-S3OutputLocationOutputTypeDef = TypedDict(
-    "S3OutputLocationOutputTypeDef",
-    {
-        "OutputS3Region": str,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-    },
-    total=False,
-)
-
 S3OutputLocationTypeDef = TypedDict(
     "S3OutputLocationTypeDef",
     {
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
@@ -2593,34 +2501,14 @@
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
     },
 )
 
-_RequiredLoggingInfoTypeDef = TypedDict(
-    "_RequiredLoggingInfoTypeDef",
-    {
-        "S3BucketName": str,
-        "S3Region": str,
-    },
-)
-_OptionalLoggingInfoTypeDef = TypedDict(
-    "_OptionalLoggingInfoTypeDef",
-    {
-        "S3KeyPrefix": str,
-    },
-    total=False,
-)
-
-
-class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
-    pass
-
-
 MaintenanceWindowAutomationParametersOutputTypeDef = TypedDict(
     "MaintenanceWindowAutomationParametersOutputTypeDef",
     {
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
     },
     total=False,
@@ -2661,23 +2549,14 @@
         "NotificationArn": str,
         "NotificationEvents": Sequence[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
     total=False,
 )
 
-MaintenanceWindowStepFunctionsParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowStepFunctionsParametersOutputTypeDef",
-    {
-        "Input": str,
-        "Name": str,
-    },
-    total=False,
-)
-
 MaintenanceWindowStepFunctionsParametersTypeDef = TypedDict(
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     {
         "Input": str,
         "Name": str,
     },
     total=False,
@@ -2721,46 +2600,22 @@
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
 )
 
-OpsItemDataValueOutputTypeDef = TypedDict(
-    "OpsItemDataValueOutputTypeDef",
-    {
-        "Value": str,
-        "Type": OpsItemDataTypeType,
-    },
-    total=False,
-)
-
 OpsItemIdentityTypeDef = TypedDict(
     "OpsItemIdentityTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-OpsItemNotificationOutputTypeDef = TypedDict(
-    "OpsItemNotificationOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
-RelatedOpsItemOutputTypeDef = TypedDict(
-    "RelatedOpsItemOutputTypeDef",
-    {
-        "OpsItemId": str,
-    },
-)
-
 ParameterInlinePolicyTypeDef = TypedDict(
     "ParameterInlinePolicyTypeDef",
     {
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
@@ -2833,38 +2688,22 @@
 ResetServiceSettingRequestRequestTypeDef = TypedDict(
     "ResetServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
     },
 )
 
-ResourceDataSyncOrganizationalUnitOutputTypeDef = TypedDict(
-    "ResourceDataSyncOrganizationalUnitOutputTypeDef",
-    {
-        "OrganizationalUnitId": str,
-    },
-    total=False,
-)
-
 ResourceDataSyncOrganizationalUnitTypeDef = TypedDict(
     "ResourceDataSyncOrganizationalUnitTypeDef",
     {
         "OrganizationalUnitId": str,
     },
     total=False,
 )
 
-ResourceDataSyncDestinationDataSharingOutputTypeDef = TypedDict(
-    "ResourceDataSyncDestinationDataSharingOutputTypeDef",
-    {
-        "DestinationDataSharingType": str,
-    },
-    total=False,
-)
-
 ResourceDataSyncDestinationDataSharingTypeDef = TypedDict(
     "ResourceDataSyncDestinationDataSharingTypeDef",
     {
         "DestinationDataSharingType": str,
     },
     total=False,
 )
@@ -3041,15 +2880,15 @@
         "DefaultInstanceName": str,
         "IamRole": str,
         "RegistrationLimit": int,
         "RegistrationsCount": int,
         "ExpirationDate": datetime,
         "Expired": bool,
         "CreatedDate": datetime,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
@@ -3120,15 +2959,15 @@
 ):
     pass
 
 
 _RequiredAlarmConfigurationOutputTypeDef = TypedDict(
     "_RequiredAlarmConfigurationOutputTypeDef",
     {
-        "Alarms": List[AlarmOutputTypeDef],
+        "Alarms": List[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationOutputTypeDef = TypedDict(
     "_OptionalAlarmConfigurationOutputTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
@@ -3435,15 +3274,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "TagList": List[TagOutputTypeDef],
+        "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutInventoryResultTypeDef = TypedDict(
     "PutInventoryResultTypeDef",
     {
@@ -3765,15 +3604,15 @@
         "ExecutionEndDateTime": str,
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "StandardOutputContent": str,
         "StandardOutputUrl": str,
         "StandardErrorContent": str,
         "StandardErrorUrl": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCommandInvocationsRequestRequestTypeDef = TypedDict(
     "ListCommandInvocationsRequestRequestTypeDef",
     {
@@ -3813,24 +3652,24 @@
         "StatusDetails": str,
         "TraceOutput": str,
         "StandardOutputUrl": str,
         "StandardErrorUrl": str,
         "CommandPlugins": List[CommandPluginTypeDef],
         "ServiceRole": str,
         "NotificationConfig": NotificationConfigOutputTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
     },
     total=False,
 )
 
 MaintenanceWindowRunCommandParametersOutputTypeDef = TypedDict(
     "MaintenanceWindowRunCommandParametersOutputTypeDef",
     {
         "Comment": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "DocumentVersion": str,
         "NotificationConfig": NotificationConfigOutputTypeDef,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "Parameters": Dict[str, List[str]],
@@ -4062,14 +3901,80 @@
 
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
 
+DocumentIdentifierTypeDef = TypedDict(
+    "DocumentIdentifierTypeDef",
+    {
+        "Name": str,
+        "CreatedDate": datetime,
+        "DisplayName": str,
+        "Owner": str,
+        "VersionName": str,
+        "PlatformTypes": List[PlatformTypeType],
+        "DocumentVersion": str,
+        "DocumentType": DocumentTypeType,
+        "SchemaVersion": str,
+        "DocumentFormat": DocumentFormatType,
+        "TargetType": str,
+        "Tags": List[TagTypeDef],
+        "Requires": List[DocumentRequiresTypeDef],
+        "ReviewStatus": ReviewStatusType,
+        "Author": str,
+    },
+    total=False,
+)
+
+GetDocumentResultTypeDef = TypedDict(
+    "GetDocumentResultTypeDef",
+    {
+        "Name": str,
+        "CreatedDate": datetime,
+        "DisplayName": str,
+        "VersionName": str,
+        "DocumentVersion": str,
+        "Status": DocumentStatusType,
+        "StatusInformation": str,
+        "Content": str,
+        "DocumentType": DocumentTypeType,
+        "DocumentFormat": DocumentFormatType,
+        "Requires": List[DocumentRequiresTypeDef],
+        "AttachmentsContent": List[AttachmentContentTypeDef],
+        "ReviewStatus": ReviewStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OpsItemSummaryTypeDef = TypedDict(
+    "OpsItemSummaryTypeDef",
+    {
+        "CreatedBy": str,
+        "CreatedTime": datetime,
+        "LastModifiedBy": str,
+        "LastModifiedTime": datetime,
+        "Priority": int,
+        "Source": str,
+        "Status": OpsItemStatusType,
+        "OpsItemId": str,
+        "Title": str,
+        "OperationalData": Dict[str, OpsItemDataValueTypeDef],
+        "Category": str,
+        "Severity": str,
+        "OpsItemType": str,
+        "ActualStartTime": datetime,
+        "ActualEndTime": datetime,
+        "PlannedStartTime": datetime,
+        "PlannedEndTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsItemRequestRequestTypeDef",
     {
         "Description": str,
         "Source": str,
         "Title": str,
     },
@@ -4097,14 +4002,43 @@
 
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
 
+OpsItemTypeDef = TypedDict(
+    "OpsItemTypeDef",
+    {
+        "CreatedBy": str,
+        "OpsItemType": str,
+        "CreatedTime": datetime,
+        "Description": str,
+        "LastModifiedBy": str,
+        "LastModifiedTime": datetime,
+        "Notifications": List[OpsItemNotificationTypeDef],
+        "Priority": int,
+        "RelatedOpsItems": List[RelatedOpsItemTypeDef],
+        "Status": OpsItemStatusType,
+        "OpsItemId": str,
+        "Version": str,
+        "Title": str,
+        "Source": str,
+        "OperationalData": Dict[str, OpsItemDataValueTypeDef],
+        "Category": str,
+        "Severity": str,
+        "ActualStartTime": datetime,
+        "ActualEndTime": datetime,
+        "PlannedStartTime": datetime,
+        "PlannedEndTime": datetime,
+        "OpsItemArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalUpdateOpsItemRequestRequestTypeDef = TypedDict(
@@ -4154,14 +4088,24 @@
 
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
 
+GetOpsMetadataResultTypeDef = TypedDict(
+    "GetOpsMetadataResultTypeDef",
+    {
+        "ResourceId": str,
+        "Metadata": Dict[str, MetadataValueTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -5328,56 +5272,14 @@
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DocumentIdentifierTypeDef = TypedDict(
-    "DocumentIdentifierTypeDef",
-    {
-        "Name": str,
-        "CreatedDate": datetime,
-        "DisplayName": str,
-        "Owner": str,
-        "VersionName": str,
-        "PlatformTypes": List[PlatformTypeType],
-        "DocumentVersion": str,
-        "DocumentType": DocumentTypeType,
-        "SchemaVersion": str,
-        "DocumentFormat": DocumentFormatType,
-        "TargetType": str,
-        "Tags": List[TagOutputTypeDef],
-        "Requires": List[DocumentRequiresOutputTypeDef],
-        "ReviewStatus": ReviewStatusType,
-        "Author": str,
-    },
-    total=False,
-)
-
-GetDocumentResultTypeDef = TypedDict(
-    "GetDocumentResultTypeDef",
-    {
-        "Name": str,
-        "CreatedDate": datetime,
-        "DisplayName": str,
-        "VersionName": str,
-        "DocumentVersion": str,
-        "Status": DocumentStatusType,
-        "StatusInformation": str,
-        "Content": str,
-        "DocumentType": DocumentTypeType,
-        "DocumentFormat": DocumentFormatType,
-        "Requires": List[DocumentRequiresOutputTypeDef],
-        "AttachmentsContent": List[AttachmentContentTypeDef],
-        "ReviewStatus": ReviewStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DocumentDescriptionTypeDef = TypedDict(
     "DocumentDescriptionTypeDef",
     {
         "Sha1": str,
         "Hash": str,
         "HashType": DocumentHashTypeType,
         "Name": str,
@@ -5393,17 +5295,17 @@
         "PlatformTypes": List[PlatformTypeType],
         "DocumentType": DocumentTypeType,
         "SchemaVersion": str,
         "LatestVersion": str,
         "DefaultVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "AttachmentsInformation": List[AttachmentInformationTypeDef],
-        "Requires": List[DocumentRequiresOutputTypeDef],
+        "Requires": List[DocumentRequiresTypeDef],
         "Author": str,
         "ReviewInformation": List[ReviewInformationTypeDef],
         "ApprovedVersion": str,
         "PendingReviewVersion": str,
         "ReviewStatus": ReviewStatusType,
         "Category": List[str],
         "CategoryEnum": List[str],
@@ -5434,15 +5336,15 @@
 
 DocumentReviewerResponseSourceTypeDef = TypedDict(
     "DocumentReviewerResponseSourceTypeDef",
     {
         "CreateTime": datetime,
         "UpdatedTime": datetime,
         "ReviewStatus": ReviewStatusType,
-        "Comment": List[DocumentReviewCommentSourceOutputTypeDef],
+        "Comment": List[DocumentReviewCommentSourceTypeDef],
         "Reviewer": str,
     },
     total=False,
 )
 
 _RequiredDocumentReviewsTypeDef = TypedDict(
     "_RequiredDocumentReviewsTypeDef",
@@ -5557,24 +5459,14 @@
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-GetOpsMetadataResultTypeDef = TypedDict(
-    "GetOpsMetadataResultTypeDef",
-    {
-        "ResourceId": str,
-        "Metadata": Dict[str, MetadataValueOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 OpsAggregatorTypeDef = TypedDict(
     "OpsAggregatorTypeDef",
     {
         "AggregatorType": str,
         "TypeName": str,
         "AttributeName": str,
         "Values": Mapping[str, str],
@@ -5684,22 +5576,14 @@
         "AssociationOverview": InstanceAggregatedAssociationOverviewTypeDef,
         "SourceId": str,
         "SourceType": SourceTypeType,
     },
     total=False,
 )
 
-InstanceAssociationOutputLocationOutputTypeDef = TypedDict(
-    "InstanceAssociationOutputLocationOutputTypeDef",
-    {
-        "S3Location": S3OutputLocationOutputTypeDef,
-    },
-    total=False,
-)
-
 InstanceAssociationOutputLocationTypeDef = TypedDict(
     "InstanceAssociationOutputLocationTypeDef",
     {
         "S3Location": S3OutputLocationTypeDef,
     },
     total=False,
 )
@@ -5853,38 +5737,14 @@
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
 )
 
-OpsItemSummaryTypeDef = TypedDict(
-    "OpsItemSummaryTypeDef",
-    {
-        "CreatedBy": str,
-        "CreatedTime": datetime,
-        "LastModifiedBy": str,
-        "LastModifiedTime": datetime,
-        "Priority": int,
-        "Source": str,
-        "Status": OpsItemStatusType,
-        "OpsItemId": str,
-        "Title": str,
-        "OperationalData": Dict[str, OpsItemDataValueOutputTypeDef],
-        "Category": str,
-        "Severity": str,
-        "OpsItemType": str,
-        "ActualStartTime": datetime,
-        "ActualEndTime": datetime,
-        "PlannedStartTime": datetime,
-        "PlannedEndTime": datetime,
-    },
-    total=False,
-)
-
 OpsItemEventSummaryTypeDef = TypedDict(
     "OpsItemEventSummaryTypeDef",
     {
         "OpsItemId": str,
         "EventId": str,
         "Source": str,
         "DetailType": str,
@@ -5907,43 +5767,14 @@
         "CreatedTime": datetime,
         "LastModifiedBy": OpsItemIdentityTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-OpsItemTypeDef = TypedDict(
-    "OpsItemTypeDef",
-    {
-        "CreatedBy": str,
-        "OpsItemType": str,
-        "CreatedTime": datetime,
-        "Description": str,
-        "LastModifiedBy": str,
-        "LastModifiedTime": datetime,
-        "Notifications": List[OpsItemNotificationOutputTypeDef],
-        "Priority": int,
-        "RelatedOpsItems": List[RelatedOpsItemOutputTypeDef],
-        "Status": OpsItemStatusType,
-        "OpsItemId": str,
-        "Version": str,
-        "Title": str,
-        "Source": str,
-        "OperationalData": Dict[str, OpsItemDataValueOutputTypeDef],
-        "Category": str,
-        "Severity": str,
-        "ActualStartTime": datetime,
-        "ActualEndTime": datetime,
-        "PlannedStartTime": datetime,
-        "PlannedEndTime": datetime,
-        "OpsItemArn": str,
-    },
-    total=False,
-)
-
 ParameterHistoryTypeDef = TypedDict(
     "ParameterHistoryTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "KeyId": str,
         "LastModifiedDate": datetime,
@@ -5997,15 +5828,15 @@
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     {
-        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitOutputTypeDef],
+        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
 
 class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
@@ -6032,40 +5863,14 @@
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
 
-_RequiredResourceDataSyncS3DestinationOutputTypeDef = TypedDict(
-    "_RequiredResourceDataSyncS3DestinationOutputTypeDef",
-    {
-        "BucketName": str,
-        "SyncFormat": Literal["JsonSerDe"],
-        "Region": str,
-    },
-)
-_OptionalResourceDataSyncS3DestinationOutputTypeDef = TypedDict(
-    "_OptionalResourceDataSyncS3DestinationOutputTypeDef",
-    {
-        "Prefix": str,
-        "AWSKMSKeyARN": str,
-        "DestinationDataSharing": ResourceDataSyncDestinationDataSharingOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class ResourceDataSyncS3DestinationOutputTypeDef(
-    _RequiredResourceDataSyncS3DestinationOutputTypeDef,
-    _OptionalResourceDataSyncS3DestinationOutputTypeDef,
-):
-    pass
-
-
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -6152,15 +5957,15 @@
         "MaxErrors": str,
         "TargetCount": int,
         "CompletedCount": int,
         "ErrorCount": int,
         "DeliveryTimedOutCount": int,
         "ServiceRole": str,
         "NotificationConfig": NotificationConfigOutputTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "TimeoutSeconds": int,
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
@@ -6211,15 +6016,15 @@
         "WindowId": str,
         "WindowTaskId": str,
         "TaskArn": str,
         "Type": MaintenanceWindowTaskTypeType,
         "Targets": List[TargetOutputTypeDef],
         "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "Priority": int,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "ServiceRoleArn": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
@@ -6327,15 +6132,15 @@
 )
 
 MaintenanceWindowTaskInvocationParametersOutputTypeDef = TypedDict(
     "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     {
         "RunCommand": MaintenanceWindowRunCommandParametersOutputTypeDef,
         "Automation": MaintenanceWindowAutomationParametersOutputTypeDef,
-        "StepFunctions": MaintenanceWindowStepFunctionsParametersOutputTypeDef,
+        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
         "Lambda": MaintenanceWindowLambdaParametersOutputTypeDef,
     },
     total=False,
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
@@ -6367,27 +6172,44 @@
         "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
-DescribePatchGroupsResultTypeDef = TypedDict(
-    "DescribePatchGroupsResultTypeDef",
+ListDocumentsResultTypeDef = TypedDict(
+    "ListDocumentsResultTypeDef",
     {
-        "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
+        "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDocumentsResultTypeDef = TypedDict(
-    "ListDocumentsResultTypeDef",
+DescribeOpsItemsResponseTypeDef = TypedDict(
+    "DescribeOpsItemsResponseTypeDef",
     {
-        "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
+        "NextToken": str,
+        "OpsItemSummaries": List[OpsItemSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpsItemResponseTypeDef = TypedDict(
+    "GetOpsItemResponseTypeDef",
+    {
+        "OpsItem": OpsItemTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchGroupsResultTypeDef = TypedDict(
+    "DescribePatchGroupsResultTypeDef",
+    {
+        "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDocumentResultTypeDef = TypedDict(
     "CreateDocumentResultTypeDef",
@@ -6549,23 +6371,14 @@
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeOpsItemsResponseTypeDef = TypedDict(
-    "DescribeOpsItemsResponseTypeDef",
-    {
-        "NextToken": str,
-        "OpsItemSummaries": List[OpsItemSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListOpsItemEventsResponseTypeDef = TypedDict(
     "ListOpsItemEventsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemEventSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6576,22 +6389,14 @@
     {
         "NextToken": str,
         "Summaries": List[OpsItemRelatedItemSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOpsItemResponseTypeDef = TypedDict(
-    "GetOpsItemResponseTypeDef",
-    {
-        "OpsItem": OpsItemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetParameterHistoryResultTypeDef = TypedDict(
     "GetParameterHistoryResultTypeDef",
     {
         "Parameters": List[ParameterHistoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6752,15 +6557,15 @@
         "Overview": AssociationOverviewTypeDef,
         "DocumentVersion": str,
         "AutomationTargetParameterName": str,
         "Parameters": Dict[str, List[str]],
         "AssociationId": str,
         "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "LastExecutionDate": datetime,
         "LastSuccessfulExecutionDate": datetime,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
@@ -6782,15 +6587,15 @@
         "AssociationVersion": str,
         "CreatedDate": datetime,
         "Name": str,
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
         "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
@@ -6812,15 +6617,15 @@
     {
         "InstanceId": str,
         "Parameters": Dict[str, List[str]],
         "AutomationTargetParameterName": str,
         "DocumentVersion": str,
         "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
@@ -7082,15 +6887,15 @@
         "ServiceRoleArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
         "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7104,15 +6909,15 @@
         "TaskArn": str,
         "ServiceRoleArn": str,
         "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7253,15 +7058,15 @@
 
 ResourceDataSyncItemTypeDef = TypedDict(
     "ResourceDataSyncItemTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
-        "S3Destination": ResourceDataSyncS3DestinationOutputTypeDef,
+        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "LastSyncTime": datetime,
         "LastSuccessfulSyncTime": datetime,
         "SyncLastModifiedTime": datetime,
         "LastStatus": LastResourceDataSyncStatusType,
         "SyncCreatedTime": datetime,
         "LastSyncStatusMessage": str,
     },
```

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/type_defs.pyi` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -103,17 +103,15 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountSharingInfoTypeDef",
-    "TagOutputTypeDef",
     "TagTypeDef",
-    "AlarmOutputTypeDef",
     "AlarmTypeDef",
     "AlarmStateInformationTypeDef",
     "AssociateOpsItemRelatedItemRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AssociationOverviewTypeDef",
     "AssociationStatusOutputTypeDef",
     "TargetOutputTypeDef",
@@ -127,15 +125,14 @@
     "AttachmentsSourceTypeDef",
     "AutomationExecutionFilterTypeDef",
     "ResolvedTargetsTypeDef",
     "ProgressCountersTypeDef",
     "PatchSourceTypeDef",
     "CancelCommandRequestRequestTypeDef",
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
-    "CloudWatchOutputConfigOutputTypeDef",
     "CloudWatchOutputConfigTypeDef",
     "CommandFilterTypeDef",
     "CommandPluginTypeDef",
     "NotificationConfigOutputTypeDef",
     "ComplianceExecutionSummaryOutputTypeDef",
     "ComplianceExecutionSummaryTypeDef",
     "ComplianceItemEntryTypeDef",
@@ -194,19 +191,17 @@
     "PatchBaselineIdentityTypeDef",
     "DescribePatchGroupStateRequestRequestTypeDef",
     "DescribePatchPropertiesRequestRequestTypeDef",
     "SessionFilterTypeDef",
     "DisassociateOpsItemRelatedItemRequestRequestTypeDef",
     "DocumentDefaultVersionDescriptionTypeDef",
     "DocumentParameterTypeDef",
-    "DocumentRequiresOutputTypeDef",
     "ReviewInformationTypeDef",
     "DocumentFilterTypeDef",
     "DocumentKeyValuesFilterTypeDef",
-    "DocumentReviewCommentSourceOutputTypeDef",
     "DocumentReviewCommentSourceTypeDef",
     "DocumentVersionInfoTypeDef",
     "PatchStatusTypeDef",
     "FailureDetailsTypeDef",
     "GetAutomationExecutionRequestRequestTypeDef",
     "GetCalendarStateRequestRequestTypeDef",
     "WaiterConfigTypeDef",
@@ -219,33 +214,31 @@
     "GetInventorySchemaRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef",
     "GetMaintenanceWindowExecutionTaskRequestRequestTypeDef",
     "MaintenanceWindowTaskParameterValueExpressionOutputTypeDef",
     "GetMaintenanceWindowRequestRequestTypeDef",
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
-    "LoggingInfoOutputTypeDef",
+    "LoggingInfoTypeDef",
     "GetOpsItemRequestRequestTypeDef",
     "GetOpsMetadataRequestRequestTypeDef",
-    "MetadataValueOutputTypeDef",
     "OpsFilterTypeDef",
     "OpsResultAttributeTypeDef",
     "GetParameterHistoryRequestRequestTypeDef",
     "GetParameterRequestRequestTypeDef",
     "ParameterTypeDef",
     "GetParametersRequestRequestTypeDef",
     "GetPatchBaselineForPatchGroupRequestRequestTypeDef",
     "GetPatchBaselineRequestRequestTypeDef",
     "PatchSourceOutputTypeDef",
     "GetResourcePoliciesRequestRequestTypeDef",
     "GetResourcePoliciesResponseEntryTypeDef",
     "GetServiceSettingRequestRequestTypeDef",
     "ServiceSettingTypeDef",
     "InstanceAggregatedAssociationOverviewTypeDef",
-    "S3OutputLocationOutputTypeDef",
     "S3OutputLocationTypeDef",
     "S3OutputUrlTypeDef",
     "InventoryDeletionSummaryItemTypeDef",
     "InventoryItemAttributeTypeDef",
     "InventoryItemTypeDef",
     "InventoryResultItemTypeDef",
     "LabelParameterVersionRequestRequestTypeDef",
@@ -254,40 +247,33 @@
     "ListDocumentVersionsRequestRequestTypeDef",
     "OpsItemEventFilterTypeDef",
     "OpsItemRelatedItemsFilterTypeDef",
     "OpsMetadataFilterTypeDef",
     "OpsMetadataTypeDef",
     "ListResourceDataSyncRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "LoggingInfoTypeDef",
     "MaintenanceWindowAutomationParametersOutputTypeDef",
     "MaintenanceWindowAutomationParametersTypeDef",
     "MaintenanceWindowLambdaParametersOutputTypeDef",
     "MaintenanceWindowLambdaParametersTypeDef",
     "NotificationConfigTypeDef",
-    "MaintenanceWindowStepFunctionsParametersOutputTypeDef",
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     "MaintenanceWindowTaskParameterValueExpressionTypeDef",
     "ModifyDocumentPermissionRequestRequestTypeDef",
     "OpsEntityItemTypeDef",
-    "OpsItemDataValueOutputTypeDef",
     "OpsItemIdentityTypeDef",
-    "OpsItemNotificationOutputTypeDef",
-    "RelatedOpsItemOutputTypeDef",
     "ParameterInlinePolicyTypeDef",
     "PatchFilterOutputTypeDef",
     "PatchFilterTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RegisterDefaultPatchBaselineRequestRequestTypeDef",
     "RegisterPatchBaselineForPatchGroupRequestRequestTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
     "ResetServiceSettingRequestRequestTypeDef",
-    "ResourceDataSyncOrganizationalUnitOutputTypeDef",
     "ResourceDataSyncOrganizationalUnitTypeDef",
-    "ResourceDataSyncDestinationDataSharingOutputTypeDef",
     "ResourceDataSyncDestinationDataSharingTypeDef",
     "ResumeSessionRequestRequestTypeDef",
     "SendAutomationSignalRequestRequestTypeDef",
     "SessionManagerOutputUrlTypeDef",
     "StartAssociationsOnceRequestRequestTypeDef",
     "StartSessionRequestRequestTypeDef",
     "StopAutomationExecutionRequestRequestTypeDef",
@@ -368,17 +354,22 @@
     "CompliantSummaryTypeDef",
     "NonCompliantSummaryTypeDef",
     "CreateActivationRequestRequestTypeDef",
     "DescribeMaintenanceWindowsForTargetRequestRequestTypeDef",
     "RegisterTargetWithMaintenanceWindowRequestRequestTypeDef",
     "UpdateMaintenanceWindowTargetRequestRequestTypeDef",
     "CreateDocumentRequestRequestTypeDef",
+    "DocumentIdentifierTypeDef",
+    "GetDocumentResultTypeDef",
+    "OpsItemSummaryTypeDef",
     "CreateOpsItemRequestRequestTypeDef",
+    "OpsItemTypeDef",
     "UpdateOpsItemRequestRequestTypeDef",
     "CreateOpsMetadataRequestRequestTypeDef",
+    "GetOpsMetadataResultTypeDef",
     "UpdateOpsMetadataRequestRequestTypeDef",
     "DescribeActivationsRequestRequestTypeDef",
     "DescribeActivationsRequestDescribeActivationsPaginateTypeDef",
     "DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef",
     "DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef",
     "DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef",
     "DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef",
@@ -445,40 +436,36 @@
     "DescribeParametersRequestDescribeParametersPaginateTypeDef",
     "DescribeParametersRequestRequestTypeDef",
     "DescribePatchBaselinesResultTypeDef",
     "PatchGroupPatchBaselineMappingTypeDef",
     "DescribeSessionsRequestDescribeSessionsPaginateTypeDef",
     "DescribeSessionsRequestRequestTypeDef",
     "UpdateDocumentDefaultVersionResultTypeDef",
-    "DocumentIdentifierTypeDef",
-    "GetDocumentResultTypeDef",
     "DocumentDescriptionTypeDef",
     "ListDocumentsRequestListDocumentsPaginateTypeDef",
     "ListDocumentsRequestRequestTypeDef",
     "DocumentReviewerResponseSourceTypeDef",
     "DocumentReviewsTypeDef",
     "ListDocumentVersionsResultTypeDef",
     "EffectivePatchTypeDef",
     "GetCommandInvocationRequestCommandExecutedWaitTypeDef",
     "InventoryGroupTypeDef",
     "ListInventoryEntriesRequestRequestTypeDef",
     "GetInventoryRequestGetInventoryPaginateTypeDef",
     "GetInventoryRequestRequestTypeDef",
-    "GetOpsMetadataResultTypeDef",
     "OpsAggregatorTypeDef",
     "GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef",
     "GetOpsSummaryRequestRequestTypeDef",
     "GetParameterResultTypeDef",
     "GetParametersByPathResultTypeDef",
     "GetParametersResultTypeDef",
     "GetResourcePoliciesResponseTypeDef",
     "GetServiceSettingResultTypeDef",
     "ResetServiceSettingResultTypeDef",
     "InstanceInformationTypeDef",
-    "InstanceAssociationOutputLocationOutputTypeDef",
     "InstanceAssociationOutputLocationTypeDef",
     "InstanceAssociationOutputUrlTypeDef",
     "InventoryDeletionSummaryTypeDef",
     "InventoryItemSchemaTypeDef",
     "PutInventoryRequestRequestTypeDef",
     "InventoryResultEntityTypeDef",
     "ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef",
@@ -486,25 +473,22 @@
     "ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef",
     "ListOpsItemRelatedItemsRequestRequestTypeDef",
     "ListOpsMetadataRequestListOpsMetadataPaginateTypeDef",
     "ListOpsMetadataRequestRequestTypeDef",
     "ListOpsMetadataResultTypeDef",
     "MaintenanceWindowRunCommandParametersTypeDef",
     "OpsEntityTypeDef",
-    "OpsItemSummaryTypeDef",
     "OpsItemEventSummaryTypeDef",
     "OpsItemRelatedItemSummaryTypeDef",
-    "OpsItemTypeDef",
     "ParameterHistoryTypeDef",
     "ParameterMetadataTypeDef",
     "PatchFilterGroupOutputTypeDef",
     "PatchFilterGroupTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     "ResourceDataSyncAwsOrganizationsSourceTypeDef",
-    "ResourceDataSyncS3DestinationOutputTypeDef",
     "ResourceDataSyncS3DestinationTypeDef",
     "SessionTypeDef",
     "DescribeActivationsResultTypeDef",
     "AssociationExecutionTypeDef",
     "CommandTypeDef",
     "GetMaintenanceWindowExecutionTaskResultTypeDef",
     "MaintenanceWindowExecutionTaskIdentityTypeDef",
@@ -516,16 +500,18 @@
     "DescribeMaintenanceWindowTargetsResultTypeDef",
     "DescribeAssociationExecutionTargetsResultTypeDef",
     "ListCommandInvocationsResultTypeDef",
     "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     "ListComplianceItemsResultTypeDef",
     "ComplianceSummaryItemTypeDef",
     "ResourceComplianceSummaryItemTypeDef",
-    "DescribePatchGroupsResultTypeDef",
     "ListDocumentsResultTypeDef",
+    "DescribeOpsItemsResponseTypeDef",
+    "GetOpsItemResponseTypeDef",
+    "DescribePatchGroupsResultTypeDef",
     "CreateDocumentResultTypeDef",
     "DescribeDocumentResultTypeDef",
     "UpdateDocumentResultTypeDef",
     "DocumentMetadataResponseInfoTypeDef",
     "UpdateDocumentMetadataRequestRequestTypeDef",
     "DescribeEffectivePatchesForPatchBaselineResultTypeDef",
     "InventoryAggregatorTypeDef",
@@ -533,18 +519,16 @@
     "InstanceAssociationStatusInfoTypeDef",
     "DeleteInventoryResultTypeDef",
     "InventoryDeletionStatusItemTypeDef",
     "GetInventorySchemaResultTypeDef",
     "GetInventoryResultTypeDef",
     "MaintenanceWindowTaskInvocationParametersTypeDef",
     "GetOpsSummaryResultTypeDef",
-    "DescribeOpsItemsResponseTypeDef",
     "ListOpsItemEventsResponseTypeDef",
     "ListOpsItemRelatedItemsResponseTypeDef",
-    "GetOpsItemResponseTypeDef",
     "GetParameterHistoryResultTypeDef",
     "DescribeParametersResultTypeDef",
     "PatchRuleOutputTypeDef",
     "PatchRuleTypeDef",
     "ResourceDataSyncSourceWithStateTypeDef",
     "ResourceDataSyncSourceTypeDef",
     "DescribeSessionsResponseTypeDef",
@@ -605,37 +589,22 @@
     {
         "AccountId": str,
         "SharedDocumentVersion": str,
     },
     total=False,
 )
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AlarmOutputTypeDef = TypedDict(
-    "AlarmOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-
 AlarmTypeDef = TypedDict(
     "AlarmTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -853,23 +822,14 @@
 CancelMaintenanceWindowExecutionRequestRequestTypeDef = TypedDict(
     "CancelMaintenanceWindowExecutionRequestRequestTypeDef",
     {
         "WindowExecutionId": str,
     },
 )
 
-CloudWatchOutputConfigOutputTypeDef = TypedDict(
-    "CloudWatchOutputConfigOutputTypeDef",
-    {
-        "CloudWatchLogGroupName": str,
-        "CloudWatchOutputEnabled": bool,
-    },
-    total=False,
-)
-
 CloudWatchOutputConfigTypeDef = TypedDict(
     "CloudWatchOutputConfigTypeDef",
     {
         "CloudWatchLogGroupName": str,
         "CloudWatchOutputEnabled": bool,
     },
     total=False,
@@ -1736,35 +1696,14 @@
         "Type": DocumentParameterTypeType,
         "Description": str,
         "DefaultValue": str,
     },
     total=False,
 )
 
-_RequiredDocumentRequiresOutputTypeDef = TypedDict(
-    "_RequiredDocumentRequiresOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalDocumentRequiresOutputTypeDef = TypedDict(
-    "_OptionalDocumentRequiresOutputTypeDef",
-    {
-        "Version": str,
-        "RequireType": str,
-        "VersionName": str,
-    },
-    total=False,
-)
-
-class DocumentRequiresOutputTypeDef(
-    _RequiredDocumentRequiresOutputTypeDef, _OptionalDocumentRequiresOutputTypeDef
-):
-    pass
-
 ReviewInformationTypeDef = TypedDict(
     "ReviewInformationTypeDef",
     {
         "ReviewedTime": datetime,
         "Status": ReviewStatusType,
         "Reviewer": str,
     },
@@ -1784,23 +1723,14 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-DocumentReviewCommentSourceOutputTypeDef = TypedDict(
-    "DocumentReviewCommentSourceOutputTypeDef",
-    {
-        "Type": Literal["Comment"],
-        "Content": str,
-    },
-    total=False,
-)
-
 DocumentReviewCommentSourceTypeDef = TypedDict(
     "DocumentReviewCommentSourceTypeDef",
     {
         "Type": Literal["Comment"],
         "Content": str,
     },
     total=False,
@@ -2015,32 +1945,30 @@
     "GetMaintenanceWindowTaskRequestRequestTypeDef",
     {
         "WindowId": str,
         "WindowTaskId": str,
     },
 )
 
-_RequiredLoggingInfoOutputTypeDef = TypedDict(
-    "_RequiredLoggingInfoOutputTypeDef",
+_RequiredLoggingInfoTypeDef = TypedDict(
+    "_RequiredLoggingInfoTypeDef",
     {
         "S3BucketName": str,
         "S3Region": str,
     },
 )
-_OptionalLoggingInfoOutputTypeDef = TypedDict(
-    "_OptionalLoggingInfoOutputTypeDef",
+_OptionalLoggingInfoTypeDef = TypedDict(
+    "_OptionalLoggingInfoTypeDef",
     {
         "S3KeyPrefix": str,
     },
     total=False,
 )
 
-class LoggingInfoOutputTypeDef(
-    _RequiredLoggingInfoOutputTypeDef, _OptionalLoggingInfoOutputTypeDef
-):
+class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
     pass
 
 _RequiredGetOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredGetOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
@@ -2074,22 +2002,14 @@
 )
 
 class GetOpsMetadataRequestRequestTypeDef(
     _RequiredGetOpsMetadataRequestRequestTypeDef, _OptionalGetOpsMetadataRequestRequestTypeDef
 ):
     pass
 
-MetadataValueOutputTypeDef = TypedDict(
-    "MetadataValueOutputTypeDef",
-    {
-        "Value": str,
-    },
-    total=False,
-)
-
 _RequiredOpsFilterTypeDef = TypedDict(
     "_RequiredOpsFilterTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
     },
 )
@@ -2279,24 +2199,14 @@
     {
         "DetailedStatus": str,
         "InstanceAssociationStatusAggregatedCount": Dict[str, int],
     },
     total=False,
 )
 
-S3OutputLocationOutputTypeDef = TypedDict(
-    "S3OutputLocationOutputTypeDef",
-    {
-        "OutputS3Region": str,
-        "OutputS3BucketName": str,
-        "OutputS3KeyPrefix": str,
-    },
-    total=False,
-)
-
 S3OutputLocationTypeDef = TypedDict(
     "S3OutputLocationTypeDef",
     {
         "OutputS3Region": str,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
     },
@@ -2510,32 +2420,14 @@
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceType": ResourceTypeForTaggingType,
         "ResourceId": str,
     },
 )
 
-_RequiredLoggingInfoTypeDef = TypedDict(
-    "_RequiredLoggingInfoTypeDef",
-    {
-        "S3BucketName": str,
-        "S3Region": str,
-    },
-)
-_OptionalLoggingInfoTypeDef = TypedDict(
-    "_OptionalLoggingInfoTypeDef",
-    {
-        "S3KeyPrefix": str,
-    },
-    total=False,
-)
-
-class LoggingInfoTypeDef(_RequiredLoggingInfoTypeDef, _OptionalLoggingInfoTypeDef):
-    pass
-
 MaintenanceWindowAutomationParametersOutputTypeDef = TypedDict(
     "MaintenanceWindowAutomationParametersOutputTypeDef",
     {
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
     },
     total=False,
@@ -2576,23 +2468,14 @@
         "NotificationArn": str,
         "NotificationEvents": Sequence[NotificationEventType],
         "NotificationType": NotificationTypeType,
     },
     total=False,
 )
 
-MaintenanceWindowStepFunctionsParametersOutputTypeDef = TypedDict(
-    "MaintenanceWindowStepFunctionsParametersOutputTypeDef",
-    {
-        "Input": str,
-        "Name": str,
-    },
-    total=False,
-)
-
 MaintenanceWindowStepFunctionsParametersTypeDef = TypedDict(
     "MaintenanceWindowStepFunctionsParametersTypeDef",
     {
         "Input": str,
         "Name": str,
     },
     total=False,
@@ -2634,46 +2517,22 @@
     {
         "CaptureTime": str,
         "Content": List[Dict[str, str]],
     },
     total=False,
 )
 
-OpsItemDataValueOutputTypeDef = TypedDict(
-    "OpsItemDataValueOutputTypeDef",
-    {
-        "Value": str,
-        "Type": OpsItemDataTypeType,
-    },
-    total=False,
-)
-
 OpsItemIdentityTypeDef = TypedDict(
     "OpsItemIdentityTypeDef",
     {
         "Arn": str,
     },
     total=False,
 )
 
-OpsItemNotificationOutputTypeDef = TypedDict(
-    "OpsItemNotificationOutputTypeDef",
-    {
-        "Arn": str,
-    },
-    total=False,
-)
-
-RelatedOpsItemOutputTypeDef = TypedDict(
-    "RelatedOpsItemOutputTypeDef",
-    {
-        "OpsItemId": str,
-    },
-)
-
 ParameterInlinePolicyTypeDef = TypedDict(
     "ParameterInlinePolicyTypeDef",
     {
         "PolicyText": str,
         "PolicyType": str,
         "PolicyStatus": str,
     },
@@ -2744,38 +2603,22 @@
 ResetServiceSettingRequestRequestTypeDef = TypedDict(
     "ResetServiceSettingRequestRequestTypeDef",
     {
         "SettingId": str,
     },
 )
 
-ResourceDataSyncOrganizationalUnitOutputTypeDef = TypedDict(
-    "ResourceDataSyncOrganizationalUnitOutputTypeDef",
-    {
-        "OrganizationalUnitId": str,
-    },
-    total=False,
-)
-
 ResourceDataSyncOrganizationalUnitTypeDef = TypedDict(
     "ResourceDataSyncOrganizationalUnitTypeDef",
     {
         "OrganizationalUnitId": str,
     },
     total=False,
 )
 
-ResourceDataSyncDestinationDataSharingOutputTypeDef = TypedDict(
-    "ResourceDataSyncDestinationDataSharingOutputTypeDef",
-    {
-        "DestinationDataSharingType": str,
-    },
-    total=False,
-)
-
 ResourceDataSyncDestinationDataSharingTypeDef = TypedDict(
     "ResourceDataSyncDestinationDataSharingTypeDef",
     {
         "DestinationDataSharingType": str,
     },
     total=False,
 )
@@ -2944,15 +2787,15 @@
         "DefaultInstanceName": str,
         "IamRole": str,
         "RegistrationLimit": int,
         "RegistrationsCount": int,
         "ExpirationDate": datetime,
         "Expired": bool,
         "CreatedDate": datetime,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
@@ -3019,15 +2862,15 @@
     _RequiredPutParameterRequestRequestTypeDef, _OptionalPutParameterRequestRequestTypeDef
 ):
     pass
 
 _RequiredAlarmConfigurationOutputTypeDef = TypedDict(
     "_RequiredAlarmConfigurationOutputTypeDef",
     {
-        "Alarms": List[AlarmOutputTypeDef],
+        "Alarms": List[AlarmTypeDef],
     },
 )
 _OptionalAlarmConfigurationOutputTypeDef = TypedDict(
     "_OptionalAlarmConfigurationOutputTypeDef",
     {
         "IgnorePollAlarmFailure": bool,
     },
@@ -3330,15 +3173,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResultTypeDef = TypedDict(
     "ListTagsForResourceResultTypeDef",
     {
-        "TagList": List[TagOutputTypeDef],
+        "TagList": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutInventoryResultTypeDef = TypedDict(
     "PutInventoryResultTypeDef",
     {
@@ -3654,15 +3497,15 @@
         "ExecutionEndDateTime": str,
         "Status": CommandInvocationStatusType,
         "StatusDetails": str,
         "StandardOutputContent": str,
         "StandardOutputUrl": str,
         "StandardErrorContent": str,
         "StandardErrorUrl": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCommandInvocationsRequestRequestTypeDef = TypedDict(
     "ListCommandInvocationsRequestRequestTypeDef",
     {
@@ -3702,24 +3545,24 @@
         "StatusDetails": str,
         "TraceOutput": str,
         "StandardOutputUrl": str,
         "StandardErrorUrl": str,
         "CommandPlugins": List[CommandPluginTypeDef],
         "ServiceRole": str,
         "NotificationConfig": NotificationConfigOutputTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
     },
     total=False,
 )
 
 MaintenanceWindowRunCommandParametersOutputTypeDef = TypedDict(
     "MaintenanceWindowRunCommandParametersOutputTypeDef",
     {
         "Comment": str,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "DocumentHash": str,
         "DocumentHashType": DocumentHashTypeType,
         "DocumentVersion": str,
         "NotificationConfig": NotificationConfigOutputTypeDef,
         "OutputS3BucketName": str,
         "OutputS3KeyPrefix": str,
         "Parameters": Dict[str, List[str]],
@@ -3939,14 +3782,80 @@
 )
 
 class CreateDocumentRequestRequestTypeDef(
     _RequiredCreateDocumentRequestRequestTypeDef, _OptionalCreateDocumentRequestRequestTypeDef
 ):
     pass
 
+DocumentIdentifierTypeDef = TypedDict(
+    "DocumentIdentifierTypeDef",
+    {
+        "Name": str,
+        "CreatedDate": datetime,
+        "DisplayName": str,
+        "Owner": str,
+        "VersionName": str,
+        "PlatformTypes": List[PlatformTypeType],
+        "DocumentVersion": str,
+        "DocumentType": DocumentTypeType,
+        "SchemaVersion": str,
+        "DocumentFormat": DocumentFormatType,
+        "TargetType": str,
+        "Tags": List[TagTypeDef],
+        "Requires": List[DocumentRequiresTypeDef],
+        "ReviewStatus": ReviewStatusType,
+        "Author": str,
+    },
+    total=False,
+)
+
+GetDocumentResultTypeDef = TypedDict(
+    "GetDocumentResultTypeDef",
+    {
+        "Name": str,
+        "CreatedDate": datetime,
+        "DisplayName": str,
+        "VersionName": str,
+        "DocumentVersion": str,
+        "Status": DocumentStatusType,
+        "StatusInformation": str,
+        "Content": str,
+        "DocumentType": DocumentTypeType,
+        "DocumentFormat": DocumentFormatType,
+        "Requires": List[DocumentRequiresTypeDef],
+        "AttachmentsContent": List[AttachmentContentTypeDef],
+        "ReviewStatus": ReviewStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+OpsItemSummaryTypeDef = TypedDict(
+    "OpsItemSummaryTypeDef",
+    {
+        "CreatedBy": str,
+        "CreatedTime": datetime,
+        "LastModifiedBy": str,
+        "LastModifiedTime": datetime,
+        "Priority": int,
+        "Source": str,
+        "Status": OpsItemStatusType,
+        "OpsItemId": str,
+        "Title": str,
+        "OperationalData": Dict[str, OpsItemDataValueTypeDef],
+        "Category": str,
+        "Severity": str,
+        "OpsItemType": str,
+        "ActualStartTime": datetime,
+        "ActualEndTime": datetime,
+        "PlannedStartTime": datetime,
+        "PlannedEndTime": datetime,
+    },
+    total=False,
+)
+
 _RequiredCreateOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateOpsItemRequestRequestTypeDef",
     {
         "Description": str,
         "Source": str,
         "Title": str,
     },
@@ -3972,14 +3881,43 @@
 )
 
 class CreateOpsItemRequestRequestTypeDef(
     _RequiredCreateOpsItemRequestRequestTypeDef, _OptionalCreateOpsItemRequestRequestTypeDef
 ):
     pass
 
+OpsItemTypeDef = TypedDict(
+    "OpsItemTypeDef",
+    {
+        "CreatedBy": str,
+        "OpsItemType": str,
+        "CreatedTime": datetime,
+        "Description": str,
+        "LastModifiedBy": str,
+        "LastModifiedTime": datetime,
+        "Notifications": List[OpsItemNotificationTypeDef],
+        "Priority": int,
+        "RelatedOpsItems": List[RelatedOpsItemTypeDef],
+        "Status": OpsItemStatusType,
+        "OpsItemId": str,
+        "Version": str,
+        "Title": str,
+        "Source": str,
+        "OperationalData": Dict[str, OpsItemDataValueTypeDef],
+        "Category": str,
+        "Severity": str,
+        "ActualStartTime": datetime,
+        "ActualEndTime": datetime,
+        "PlannedStartTime": datetime,
+        "PlannedEndTime": datetime,
+        "OpsItemArn": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateOpsItemRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsItemRequestRequestTypeDef",
     {
         "OpsItemId": str,
     },
 )
 _OptionalUpdateOpsItemRequestRequestTypeDef = TypedDict(
@@ -4025,14 +3963,24 @@
 )
 
 class CreateOpsMetadataRequestRequestTypeDef(
     _RequiredCreateOpsMetadataRequestRequestTypeDef, _OptionalCreateOpsMetadataRequestRequestTypeDef
 ):
     pass
 
+GetOpsMetadataResultTypeDef = TypedDict(
+    "GetOpsMetadataResultTypeDef",
+    {
+        "ResourceId": str,
+        "Metadata": Dict[str, MetadataValueTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOpsMetadataRequestRequestTypeDef",
     {
         "OpsMetadataArn": str,
     },
 )
 _OptionalUpdateOpsMetadataRequestRequestTypeDef = TypedDict(
@@ -5133,56 +5081,14 @@
     "UpdateDocumentDefaultVersionResultTypeDef",
     {
         "Description": DocumentDefaultVersionDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DocumentIdentifierTypeDef = TypedDict(
-    "DocumentIdentifierTypeDef",
-    {
-        "Name": str,
-        "CreatedDate": datetime,
-        "DisplayName": str,
-        "Owner": str,
-        "VersionName": str,
-        "PlatformTypes": List[PlatformTypeType],
-        "DocumentVersion": str,
-        "DocumentType": DocumentTypeType,
-        "SchemaVersion": str,
-        "DocumentFormat": DocumentFormatType,
-        "TargetType": str,
-        "Tags": List[TagOutputTypeDef],
-        "Requires": List[DocumentRequiresOutputTypeDef],
-        "ReviewStatus": ReviewStatusType,
-        "Author": str,
-    },
-    total=False,
-)
-
-GetDocumentResultTypeDef = TypedDict(
-    "GetDocumentResultTypeDef",
-    {
-        "Name": str,
-        "CreatedDate": datetime,
-        "DisplayName": str,
-        "VersionName": str,
-        "DocumentVersion": str,
-        "Status": DocumentStatusType,
-        "StatusInformation": str,
-        "Content": str,
-        "DocumentType": DocumentTypeType,
-        "DocumentFormat": DocumentFormatType,
-        "Requires": List[DocumentRequiresOutputTypeDef],
-        "AttachmentsContent": List[AttachmentContentTypeDef],
-        "ReviewStatus": ReviewStatusType,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DocumentDescriptionTypeDef = TypedDict(
     "DocumentDescriptionTypeDef",
     {
         "Sha1": str,
         "Hash": str,
         "HashType": DocumentHashTypeType,
         "Name": str,
@@ -5198,17 +5104,17 @@
         "PlatformTypes": List[PlatformTypeType],
         "DocumentType": DocumentTypeType,
         "SchemaVersion": str,
         "LatestVersion": str,
         "DefaultVersion": str,
         "DocumentFormat": DocumentFormatType,
         "TargetType": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "AttachmentsInformation": List[AttachmentInformationTypeDef],
-        "Requires": List[DocumentRequiresOutputTypeDef],
+        "Requires": List[DocumentRequiresTypeDef],
         "Author": str,
         "ReviewInformation": List[ReviewInformationTypeDef],
         "ApprovedVersion": str,
         "PendingReviewVersion": str,
         "ReviewStatus": ReviewStatusType,
         "Category": List[str],
         "CategoryEnum": List[str],
@@ -5239,15 +5145,15 @@
 
 DocumentReviewerResponseSourceTypeDef = TypedDict(
     "DocumentReviewerResponseSourceTypeDef",
     {
         "CreateTime": datetime,
         "UpdatedTime": datetime,
         "ReviewStatus": ReviewStatusType,
-        "Comment": List[DocumentReviewCommentSourceOutputTypeDef],
+        "Comment": List[DocumentReviewCommentSourceTypeDef],
         "Reviewer": str,
     },
     total=False,
 )
 
 _RequiredDocumentReviewsTypeDef = TypedDict(
     "_RequiredDocumentReviewsTypeDef",
@@ -5356,24 +5262,14 @@
         "ResultAttributes": Sequence[ResultAttributeTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-GetOpsMetadataResultTypeDef = TypedDict(
-    "GetOpsMetadataResultTypeDef",
-    {
-        "ResourceId": str,
-        "Metadata": Dict[str, MetadataValueOutputTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 OpsAggregatorTypeDef = TypedDict(
     "OpsAggregatorTypeDef",
     {
         "AggregatorType": str,
         "TypeName": str,
         "AttributeName": str,
         "Values": Mapping[str, str],
@@ -5483,22 +5379,14 @@
         "AssociationOverview": InstanceAggregatedAssociationOverviewTypeDef,
         "SourceId": str,
         "SourceType": SourceTypeType,
     },
     total=False,
 )
 
-InstanceAssociationOutputLocationOutputTypeDef = TypedDict(
-    "InstanceAssociationOutputLocationOutputTypeDef",
-    {
-        "S3Location": S3OutputLocationOutputTypeDef,
-    },
-    total=False,
-)
-
 InstanceAssociationOutputLocationTypeDef = TypedDict(
     "InstanceAssociationOutputLocationTypeDef",
     {
         "S3Location": S3OutputLocationTypeDef,
     },
     total=False,
 )
@@ -5650,38 +5538,14 @@
     {
         "Id": str,
         "Data": Dict[str, OpsEntityItemTypeDef],
     },
     total=False,
 )
 
-OpsItemSummaryTypeDef = TypedDict(
-    "OpsItemSummaryTypeDef",
-    {
-        "CreatedBy": str,
-        "CreatedTime": datetime,
-        "LastModifiedBy": str,
-        "LastModifiedTime": datetime,
-        "Priority": int,
-        "Source": str,
-        "Status": OpsItemStatusType,
-        "OpsItemId": str,
-        "Title": str,
-        "OperationalData": Dict[str, OpsItemDataValueOutputTypeDef],
-        "Category": str,
-        "Severity": str,
-        "OpsItemType": str,
-        "ActualStartTime": datetime,
-        "ActualEndTime": datetime,
-        "PlannedStartTime": datetime,
-        "PlannedEndTime": datetime,
-    },
-    total=False,
-)
-
 OpsItemEventSummaryTypeDef = TypedDict(
     "OpsItemEventSummaryTypeDef",
     {
         "OpsItemId": str,
         "EventId": str,
         "Source": str,
         "DetailType": str,
@@ -5704,43 +5568,14 @@
         "CreatedTime": datetime,
         "LastModifiedBy": OpsItemIdentityTypeDef,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-OpsItemTypeDef = TypedDict(
-    "OpsItemTypeDef",
-    {
-        "CreatedBy": str,
-        "OpsItemType": str,
-        "CreatedTime": datetime,
-        "Description": str,
-        "LastModifiedBy": str,
-        "LastModifiedTime": datetime,
-        "Notifications": List[OpsItemNotificationOutputTypeDef],
-        "Priority": int,
-        "RelatedOpsItems": List[RelatedOpsItemOutputTypeDef],
-        "Status": OpsItemStatusType,
-        "OpsItemId": str,
-        "Version": str,
-        "Title": str,
-        "Source": str,
-        "OperationalData": Dict[str, OpsItemDataValueOutputTypeDef],
-        "Category": str,
-        "Severity": str,
-        "ActualStartTime": datetime,
-        "ActualEndTime": datetime,
-        "PlannedStartTime": datetime,
-        "PlannedEndTime": datetime,
-        "OpsItemArn": str,
-    },
-    total=False,
-)
-
 ParameterHistoryTypeDef = TypedDict(
     "ParameterHistoryTypeDef",
     {
         "Name": str,
         "Type": ParameterTypeType,
         "KeyId": str,
         "LastModifiedDate": datetime,
@@ -5794,15 +5629,15 @@
     {
         "OrganizationSourceType": str,
     },
 )
 _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef = TypedDict(
     "_OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef",
     {
-        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitOutputTypeDef],
+        "OrganizationalUnits": List[ResourceDataSyncOrganizationalUnitTypeDef],
     },
     total=False,
 )
 
 class ResourceDataSyncAwsOrganizationsSourceOutputTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
@@ -5825,38 +5660,14 @@
 
 class ResourceDataSyncAwsOrganizationsSourceTypeDef(
     _RequiredResourceDataSyncAwsOrganizationsSourceTypeDef,
     _OptionalResourceDataSyncAwsOrganizationsSourceTypeDef,
 ):
     pass
 
-_RequiredResourceDataSyncS3DestinationOutputTypeDef = TypedDict(
-    "_RequiredResourceDataSyncS3DestinationOutputTypeDef",
-    {
-        "BucketName": str,
-        "SyncFormat": Literal["JsonSerDe"],
-        "Region": str,
-    },
-)
-_OptionalResourceDataSyncS3DestinationOutputTypeDef = TypedDict(
-    "_OptionalResourceDataSyncS3DestinationOutputTypeDef",
-    {
-        "Prefix": str,
-        "AWSKMSKeyARN": str,
-        "DestinationDataSharing": ResourceDataSyncDestinationDataSharingOutputTypeDef,
-    },
-    total=False,
-)
-
-class ResourceDataSyncS3DestinationOutputTypeDef(
-    _RequiredResourceDataSyncS3DestinationOutputTypeDef,
-    _OptionalResourceDataSyncS3DestinationOutputTypeDef,
-):
-    pass
-
 _RequiredResourceDataSyncS3DestinationTypeDef = TypedDict(
     "_RequiredResourceDataSyncS3DestinationTypeDef",
     {
         "BucketName": str,
         "SyncFormat": Literal["JsonSerDe"],
         "Region": str,
     },
@@ -5941,15 +5752,15 @@
         "MaxErrors": str,
         "TargetCount": int,
         "CompletedCount": int,
         "ErrorCount": int,
         "DeliveryTimedOutCount": int,
         "ServiceRole": str,
         "NotificationConfig": NotificationConfigOutputTypeDef,
-        "CloudWatchOutputConfig": CloudWatchOutputConfigOutputTypeDef,
+        "CloudWatchOutputConfig": CloudWatchOutputConfigTypeDef,
         "TimeoutSeconds": int,
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "TriggeredAlarms": List[AlarmStateInformationTypeDef],
     },
     total=False,
 )
 
@@ -6000,15 +5811,15 @@
         "WindowId": str,
         "WindowTaskId": str,
         "TaskArn": str,
         "Type": MaintenanceWindowTaskTypeType,
         "Targets": List[TargetOutputTypeDef],
         "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "Priority": int,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "ServiceRoleArn": str,
         "MaxConcurrency": str,
         "MaxErrors": str,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
@@ -6114,15 +5925,15 @@
 )
 
 MaintenanceWindowTaskInvocationParametersOutputTypeDef = TypedDict(
     "MaintenanceWindowTaskInvocationParametersOutputTypeDef",
     {
         "RunCommand": MaintenanceWindowRunCommandParametersOutputTypeDef,
         "Automation": MaintenanceWindowAutomationParametersOutputTypeDef,
-        "StepFunctions": MaintenanceWindowStepFunctionsParametersOutputTypeDef,
+        "StepFunctions": MaintenanceWindowStepFunctionsParametersTypeDef,
         "Lambda": MaintenanceWindowLambdaParametersOutputTypeDef,
     },
     total=False,
 )
 
 ListComplianceItemsResultTypeDef = TypedDict(
     "ListComplianceItemsResultTypeDef",
@@ -6154,27 +5965,44 @@
         "ExecutionSummary": ComplianceExecutionSummaryOutputTypeDef,
         "CompliantSummary": CompliantSummaryTypeDef,
         "NonCompliantSummary": NonCompliantSummaryTypeDef,
     },
     total=False,
 )
 
-DescribePatchGroupsResultTypeDef = TypedDict(
-    "DescribePatchGroupsResultTypeDef",
+ListDocumentsResultTypeDef = TypedDict(
+    "ListDocumentsResultTypeDef",
     {
-        "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
+        "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListDocumentsResultTypeDef = TypedDict(
-    "ListDocumentsResultTypeDef",
+DescribeOpsItemsResponseTypeDef = TypedDict(
+    "DescribeOpsItemsResponseTypeDef",
     {
-        "DocumentIdentifiers": List[DocumentIdentifierTypeDef],
+        "NextToken": str,
+        "OpsItemSummaries": List[OpsItemSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOpsItemResponseTypeDef = TypedDict(
+    "GetOpsItemResponseTypeDef",
+    {
+        "OpsItem": OpsItemTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribePatchGroupsResultTypeDef = TypedDict(
+    "DescribePatchGroupsResultTypeDef",
+    {
+        "Mappings": List[PatchGroupPatchBaselineMappingTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDocumentResultTypeDef = TypedDict(
     "CreateDocumentResultTypeDef",
@@ -6334,23 +6162,14 @@
     {
         "Entities": List[OpsEntityTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeOpsItemsResponseTypeDef = TypedDict(
-    "DescribeOpsItemsResponseTypeDef",
-    {
-        "NextToken": str,
-        "OpsItemSummaries": List[OpsItemSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 ListOpsItemEventsResponseTypeDef = TypedDict(
     "ListOpsItemEventsResponseTypeDef",
     {
         "NextToken": str,
         "Summaries": List[OpsItemEventSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6361,22 +6180,14 @@
     {
         "NextToken": str,
         "Summaries": List[OpsItemRelatedItemSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetOpsItemResponseTypeDef = TypedDict(
-    "GetOpsItemResponseTypeDef",
-    {
-        "OpsItem": OpsItemTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetParameterHistoryResultTypeDef = TypedDict(
     "GetParameterHistoryResultTypeDef",
     {
         "Parameters": List[ParameterHistoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -6531,15 +6342,15 @@
         "Overview": AssociationOverviewTypeDef,
         "DocumentVersion": str,
         "AutomationTargetParameterName": str,
         "Parameters": Dict[str, List[str]],
         "AssociationId": str,
         "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "LastExecutionDate": datetime,
         "LastSuccessfulExecutionDate": datetime,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
@@ -6561,15 +6372,15 @@
         "AssociationVersion": str,
         "CreatedDate": datetime,
         "Name": str,
         "DocumentVersion": str,
         "Parameters": Dict[str, List[str]],
         "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
@@ -6591,15 +6402,15 @@
     {
         "InstanceId": str,
         "Parameters": Dict[str, List[str]],
         "AutomationTargetParameterName": str,
         "DocumentVersion": str,
         "Targets": List[TargetOutputTypeDef],
         "ScheduleExpression": str,
-        "OutputLocation": InstanceAssociationOutputLocationOutputTypeDef,
+        "OutputLocation": InstanceAssociationOutputLocationTypeDef,
         "AssociationName": str,
         "MaxErrors": str,
         "MaxConcurrency": str,
         "ComplianceSeverity": AssociationComplianceSeverityType,
         "SyncCompliance": AssociationSyncComplianceType,
         "ApplyOnlyAtCronInterval": bool,
         "CalendarNames": List[str],
@@ -6847,15 +6658,15 @@
         "ServiceRoleArn": str,
         "TaskType": MaintenanceWindowTaskTypeType,
         "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -6869,15 +6680,15 @@
         "TaskArn": str,
         "ServiceRoleArn": str,
         "TaskParameters": Dict[str, MaintenanceWindowTaskParameterValueExpressionOutputTypeDef],
         "TaskInvocationParameters": MaintenanceWindowTaskInvocationParametersOutputTypeDef,
         "Priority": int,
         "MaxConcurrency": str,
         "MaxErrors": str,
-        "LoggingInfo": LoggingInfoOutputTypeDef,
+        "LoggingInfo": LoggingInfoTypeDef,
         "Name": str,
         "Description": str,
         "CutoffBehavior": MaintenanceWindowTaskCutoffBehaviorType,
         "AlarmConfiguration": AlarmConfigurationOutputTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -7014,15 +6825,15 @@
 
 ResourceDataSyncItemTypeDef = TypedDict(
     "ResourceDataSyncItemTypeDef",
     {
         "SyncName": str,
         "SyncType": str,
         "SyncSource": ResourceDataSyncSourceWithStateTypeDef,
-        "S3Destination": ResourceDataSyncS3DestinationOutputTypeDef,
+        "S3Destination": ResourceDataSyncS3DestinationTypeDef,
         "LastSyncTime": datetime,
         "LastSuccessfulSyncTime": datetime,
         "SyncLastModifiedTime": datetime,
         "LastStatus": LastResourceDataSyncStatusType,
         "SyncCreatedTime": datetime,
         "LastSyncStatusMessage": str,
     },
```

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/waiter.py` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm/waiter.pyi` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/PKG-INFO` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ssm
-Version: 1.28.12
-Summary: Type annotations for boto3.SSM 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-ssm.svg?color=blue)](https://pypi.org/project/mypy-boto3-ssm)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-ssm)](https://pepy.tech/project/mypy-boto3-ssm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.SSM 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
+[boto3.SSM 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
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
 [mypy-boto3-ssm docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ssm/).
 
 See how it helps to find and fix potential bugs:
 
@@ -643,17 +643,15 @@
 
 `mypy_boto3_ssm.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_ssm.type_defs import (
     AccountSharingInfoTypeDef,
-    TagOutputTypeDef,
     TagTypeDef,
-    AlarmOutputTypeDef,
     AlarmTypeDef,
     AlarmStateInformationTypeDef,
     AssociateOpsItemRelatedItemRequestRequestTypeDef,
     ResponseMetadataTypeDef,
     AssociationOverviewTypeDef,
     AssociationStatusOutputTypeDef,
     TargetOutputTypeDef,
@@ -667,15 +665,14 @@
     AttachmentsSourceTypeDef,
     AutomationExecutionFilterTypeDef,
     ResolvedTargetsTypeDef,
     ProgressCountersTypeDef,
     PatchSourceTypeDef,
     CancelCommandRequestRequestTypeDef,
     CancelMaintenanceWindowExecutionRequestRequestTypeDef,
-    CloudWatchOutputConfigOutputTypeDef,
     CloudWatchOutputConfigTypeDef,
     CommandFilterTypeDef,
     CommandPluginTypeDef,
     NotificationConfigOutputTypeDef,
     ComplianceExecutionSummaryOutputTypeDef,
     ComplianceExecutionSummaryTypeDef,
     ComplianceItemEntryTypeDef,
@@ -734,19 +731,17 @@
     PatchBaselineIdentityTypeDef,
     DescribePatchGroupStateRequestRequestTypeDef,
     DescribePatchPropertiesRequestRequestTypeDef,
     SessionFilterTypeDef,
     DisassociateOpsItemRelatedItemRequestRequestTypeDef,
     DocumentDefaultVersionDescriptionTypeDef,
     DocumentParameterTypeDef,
-    DocumentRequiresOutputTypeDef,
     ReviewInformationTypeDef,
     DocumentFilterTypeDef,
     DocumentKeyValuesFilterTypeDef,
-    DocumentReviewCommentSourceOutputTypeDef,
     DocumentReviewCommentSourceTypeDef,
     DocumentVersionInfoTypeDef,
     PatchStatusTypeDef,
     FailureDetailsTypeDef,
     GetAutomationExecutionRequestRequestTypeDef,
     GetCalendarStateRequestRequestTypeDef,
     WaiterConfigTypeDef,
@@ -759,33 +754,31 @@
     GetInventorySchemaRequestRequestTypeDef,
     GetMaintenanceWindowExecutionRequestRequestTypeDef,
     GetMaintenanceWindowExecutionTaskInvocationRequestRequestTypeDef,
     GetMaintenanceWindowExecutionTaskRequestRequestTypeDef,
     MaintenanceWindowTaskParameterValueExpressionOutputTypeDef,
     GetMaintenanceWindowRequestRequestTypeDef,
     GetMaintenanceWindowTaskRequestRequestTypeDef,
-    LoggingInfoOutputTypeDef,
+    LoggingInfoTypeDef,
     GetOpsItemRequestRequestTypeDef,
     GetOpsMetadataRequestRequestTypeDef,
-    MetadataValueOutputTypeDef,
     OpsFilterTypeDef,
     OpsResultAttributeTypeDef,
     GetParameterHistoryRequestRequestTypeDef,
     GetParameterRequestRequestTypeDef,
     ParameterTypeDef,
     GetParametersRequestRequestTypeDef,
     GetPatchBaselineForPatchGroupRequestRequestTypeDef,
     GetPatchBaselineRequestRequestTypeDef,
     PatchSourceOutputTypeDef,
     GetResourcePoliciesRequestRequestTypeDef,
     GetResourcePoliciesResponseEntryTypeDef,
     GetServiceSettingRequestRequestTypeDef,
     ServiceSettingTypeDef,
     InstanceAggregatedAssociationOverviewTypeDef,
-    S3OutputLocationOutputTypeDef,
     S3OutputLocationTypeDef,
     S3OutputUrlTypeDef,
     InventoryDeletionSummaryItemTypeDef,
     InventoryItemAttributeTypeDef,
     InventoryItemTypeDef,
     InventoryResultItemTypeDef,
     LabelParameterVersionRequestRequestTypeDef,
@@ -794,40 +787,33 @@
     ListDocumentVersionsRequestRequestTypeDef,
     OpsItemEventFilterTypeDef,
     OpsItemRelatedItemsFilterTypeDef,
     OpsMetadataFilterTypeDef,
     OpsMetadataTypeDef,
     ListResourceDataSyncRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    LoggingInfoTypeDef,
     MaintenanceWindowAutomationParametersOutputTypeDef,
     MaintenanceWindowAutomationParametersTypeDef,
     MaintenanceWindowLambdaParametersOutputTypeDef,
     MaintenanceWindowLambdaParametersTypeDef,
     NotificationConfigTypeDef,
-    MaintenanceWindowStepFunctionsParametersOutputTypeDef,
     MaintenanceWindowStepFunctionsParametersTypeDef,
     MaintenanceWindowTaskParameterValueExpressionTypeDef,
     ModifyDocumentPermissionRequestRequestTypeDef,
     OpsEntityItemTypeDef,
-    OpsItemDataValueOutputTypeDef,
     OpsItemIdentityTypeDef,
-    OpsItemNotificationOutputTypeDef,
-    RelatedOpsItemOutputTypeDef,
     ParameterInlinePolicyTypeDef,
     PatchFilterOutputTypeDef,
     PatchFilterTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterDefaultPatchBaselineRequestRequestTypeDef,
     RegisterPatchBaselineForPatchGroupRequestRequestTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
     ResetServiceSettingRequestRequestTypeDef,
-    ResourceDataSyncOrganizationalUnitOutputTypeDef,
     ResourceDataSyncOrganizationalUnitTypeDef,
-    ResourceDataSyncDestinationDataSharingOutputTypeDef,
     ResourceDataSyncDestinationDataSharingTypeDef,
     ResumeSessionRequestRequestTypeDef,
     SendAutomationSignalRequestRequestTypeDef,
     SessionManagerOutputUrlTypeDef,
     StartAssociationsOnceRequestRequestTypeDef,
     StartSessionRequestRequestTypeDef,
     StopAutomationExecutionRequestRequestTypeDef,
@@ -908,17 +894,22 @@
     CompliantSummaryTypeDef,
     NonCompliantSummaryTypeDef,
     CreateActivationRequestRequestTypeDef,
     DescribeMaintenanceWindowsForTargetRequestRequestTypeDef,
     RegisterTargetWithMaintenanceWindowRequestRequestTypeDef,
     UpdateMaintenanceWindowTargetRequestRequestTypeDef,
     CreateDocumentRequestRequestTypeDef,
+    DocumentIdentifierTypeDef,
+    GetDocumentResultTypeDef,
+    OpsItemSummaryTypeDef,
     CreateOpsItemRequestRequestTypeDef,
+    OpsItemTypeDef,
     UpdateOpsItemRequestRequestTypeDef,
     CreateOpsMetadataRequestRequestTypeDef,
+    GetOpsMetadataResultTypeDef,
     UpdateOpsMetadataRequestRequestTypeDef,
     DescribeActivationsRequestRequestTypeDef,
     DescribeActivationsRequestDescribeActivationsPaginateTypeDef,
     DescribeAssociationExecutionTargetsRequestDescribeAssociationExecutionTargetsPaginateTypeDef,
     DescribeAssociationExecutionsRequestDescribeAssociationExecutionsPaginateTypeDef,
     DescribeAutomationExecutionsRequestDescribeAutomationExecutionsPaginateTypeDef,
     DescribeEffectiveInstanceAssociationsRequestDescribeEffectiveInstanceAssociationsPaginateTypeDef,
@@ -985,40 +976,36 @@
     DescribeParametersRequestDescribeParametersPaginateTypeDef,
     DescribeParametersRequestRequestTypeDef,
     DescribePatchBaselinesResultTypeDef,
     PatchGroupPatchBaselineMappingTypeDef,
     DescribeSessionsRequestDescribeSessionsPaginateTypeDef,
     DescribeSessionsRequestRequestTypeDef,
     UpdateDocumentDefaultVersionResultTypeDef,
-    DocumentIdentifierTypeDef,
-    GetDocumentResultTypeDef,
     DocumentDescriptionTypeDef,
     ListDocumentsRequestListDocumentsPaginateTypeDef,
     ListDocumentsRequestRequestTypeDef,
     DocumentReviewerResponseSourceTypeDef,
     DocumentReviewsTypeDef,
     ListDocumentVersionsResultTypeDef,
     EffectivePatchTypeDef,
     GetCommandInvocationRequestCommandExecutedWaitTypeDef,
     InventoryGroupTypeDef,
     ListInventoryEntriesRequestRequestTypeDef,
     GetInventoryRequestGetInventoryPaginateTypeDef,
     GetInventoryRequestRequestTypeDef,
-    GetOpsMetadataResultTypeDef,
     OpsAggregatorTypeDef,
     GetOpsSummaryRequestGetOpsSummaryPaginateTypeDef,
     GetOpsSummaryRequestRequestTypeDef,
     GetParameterResultTypeDef,
     GetParametersByPathResultTypeDef,
     GetParametersResultTypeDef,
     GetResourcePoliciesResponseTypeDef,
     GetServiceSettingResultTypeDef,
     ResetServiceSettingResultTypeDef,
     InstanceInformationTypeDef,
-    InstanceAssociationOutputLocationOutputTypeDef,
     InstanceAssociationOutputLocationTypeDef,
     InstanceAssociationOutputUrlTypeDef,
     InventoryDeletionSummaryTypeDef,
     InventoryItemSchemaTypeDef,
     PutInventoryRequestRequestTypeDef,
     InventoryResultEntityTypeDef,
     ListOpsItemEventsRequestListOpsItemEventsPaginateTypeDef,
@@ -1026,25 +1013,22 @@
     ListOpsItemRelatedItemsRequestListOpsItemRelatedItemsPaginateTypeDef,
     ListOpsItemRelatedItemsRequestRequestTypeDef,
     ListOpsMetadataRequestListOpsMetadataPaginateTypeDef,
     ListOpsMetadataRequestRequestTypeDef,
     ListOpsMetadataResultTypeDef,
     MaintenanceWindowRunCommandParametersTypeDef,
     OpsEntityTypeDef,
-    OpsItemSummaryTypeDef,
     OpsItemEventSummaryTypeDef,
     OpsItemRelatedItemSummaryTypeDef,
-    OpsItemTypeDef,
     ParameterHistoryTypeDef,
     ParameterMetadataTypeDef,
     PatchFilterGroupOutputTypeDef,
     PatchFilterGroupTypeDef,
     ResourceDataSyncAwsOrganizationsSourceOutputTypeDef,
     ResourceDataSyncAwsOrganizationsSourceTypeDef,
-    ResourceDataSyncS3DestinationOutputTypeDef,
     ResourceDataSyncS3DestinationTypeDef,
     SessionTypeDef,
     DescribeActivationsResultTypeDef,
     AssociationExecutionTypeDef,
     CommandTypeDef,
     GetMaintenanceWindowExecutionTaskResultTypeDef,
     MaintenanceWindowExecutionTaskIdentityTypeDef,
@@ -1056,16 +1040,18 @@
     DescribeMaintenanceWindowTargetsResultTypeDef,
     DescribeAssociationExecutionTargetsResultTypeDef,
     ListCommandInvocationsResultTypeDef,
     MaintenanceWindowTaskInvocationParametersOutputTypeDef,
     ListComplianceItemsResultTypeDef,
     ComplianceSummaryItemTypeDef,
     ResourceComplianceSummaryItemTypeDef,
-    DescribePatchGroupsResultTypeDef,
     ListDocumentsResultTypeDef,
+    DescribeOpsItemsResponseTypeDef,
+    GetOpsItemResponseTypeDef,
+    DescribePatchGroupsResultTypeDef,
     CreateDocumentResultTypeDef,
     DescribeDocumentResultTypeDef,
     UpdateDocumentResultTypeDef,
     DocumentMetadataResponseInfoTypeDef,
     UpdateDocumentMetadataRequestRequestTypeDef,
     DescribeEffectivePatchesForPatchBaselineResultTypeDef,
     InventoryAggregatorTypeDef,
@@ -1073,18 +1059,16 @@
     InstanceAssociationStatusInfoTypeDef,
     DeleteInventoryResultTypeDef,
     InventoryDeletionStatusItemTypeDef,
     GetInventorySchemaResultTypeDef,
     GetInventoryResultTypeDef,
     MaintenanceWindowTaskInvocationParametersTypeDef,
     GetOpsSummaryResultTypeDef,
-    DescribeOpsItemsResponseTypeDef,
     ListOpsItemEventsResponseTypeDef,
     ListOpsItemRelatedItemsResponseTypeDef,
-    GetOpsItemResponseTypeDef,
     GetParameterHistoryResultTypeDef,
     DescribeParametersResultTypeDef,
     PatchRuleOutputTypeDef,
     PatchRuleTypeDef,
     ResourceDataSyncSourceWithStateTypeDef,
     ResourceDataSyncSourceTypeDef,
     DescribeSessionsResponseTypeDef,
```

### Comparing `mypy-boto3-ssm-1.28.12/mypy_boto3_ssm.egg-info/SOURCES.txt` & `mypy-boto3-ssm-1.28.15/mypy_boto3_ssm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ssm-1.28.12/setup.py` & `mypy-boto3-ssm-1.28.15/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ssm",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_ssm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.SSM 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.SSM 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

