# Comparing `tmp/mypy-boto3-emr-1.28.12.tar.gz` & `tmp/mypy-boto3-emr-1.28.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-emr-1.28.12.tar", last modified: Thu Jul 27 05:34:40 2023, max compression
+gzip compressed data, was "mypy-boto3-emr-1.28.15.tar", last modified: Fri Jul 28 20:42:46 2023, max compression
```

## Comparing `mypy-boto3-emr-1.28.12.tar` & `mypy-boto3-emr-1.28.15.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.264515 mypy-boto3-emr-1.28.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-27 05:34:40.256515 mypy-boto3-emr-1.28.12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23699 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.256515 mypy-boto3-emr-1.28.12/mypy_boto3_emr/
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43838 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43764 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12282 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12270 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93670 2023-07-27 05:22:00.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93532 2023-07-27 05:21:59.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 05:34:40.256515 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-27 05:34:40.000000 mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 05:34:40.264515 mypy-boto3-emr-1.28.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-27 05:21:57.000000 mypy-boto3-emr-1.28.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.897084 mypy-boto3-emr-1.28.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-07-28 20:42:46.897084 mypy-boto3-emr-1.28.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22840 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.885084 mypy-boto3-emr-1.28.15/mypy_boto3_emr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43838 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43764 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15820 2023-07-28 20:25:26.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15818 2023-07-28 20:25:26.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12250 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    84915 2023-07-28 20:25:28.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84797 2023-07-28 20:25:27.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 20:42:46.897084 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-28 20:42:46.000000 mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 20:42:46.897084 mypy-boto3-emr-1.28.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-28 20:25:25.000000 mypy-boto3-emr-1.28.15/setup.py
```

### Comparing `mypy-boto3-emr-1.28.12/LICENSE` & `mypy-boto3-emr-1.28.15/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/PKG-INFO` & `mypy-boto3-emr-1.28.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.28.12
-Summary: Type annotations for boto3.EMR 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -425,224 +425,203 @@
 ### Typed dictionaries
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
-    AddInstanceFleetOutputTypeDef,
-    AddInstanceGroupsOutputTypeDef,
-    AddJobFlowStepsOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplicationOutputTypeDef,
     ApplicationTypeDef,
-    ScalingConstraintsOutputTypeDef,
-    AutoScalingPolicyStateChangeReasonTypeDef,
     ScalingConstraintsTypeDef,
-    AutoTerminationPolicyOutputTypeDef,
+    AutoScalingPolicyStateChangeReasonTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
-    PortRangeOutputTypeDef,
     PortRangeTypeDef,
     ScriptBootstrapActionConfigOutputTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
     ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
-    KerberosAttributesOutputTypeDef,
-    PlacementGroupConfigOutputTypeDef,
-    TagOutputTypeDef,
+    KerberosAttributesTypeDef,
+    PlacementGroupConfigTypeDef,
     CommandTypeDef,
-    ComputeLimitsOutputTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
-    CreateSecurityConfigurationOutputTypeDef,
-    CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
     DescribeJobFlowsInputRequestTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
-    DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
-    VolumeSpecificationOutputTypeDef,
     EbsVolumeTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExecutionEngineConfigOutputTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
-    KeyValueOutputTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
-    SpotProvisioningSpecificationOutputTypeDef,
     SpotProvisioningSpecificationTypeDef,
-    OnDemandResizingSpecificationOutputTypeDef,
-    SpotResizingSpecificationOutputTypeDef,
     OnDemandResizingSpecificationTypeDef,
     SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyOutputTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
     PlacementTypeOutputTypeDef,
-    KerberosAttributesTypeDef,
-    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
-    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
-    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
-    ListInstancesInputListInstancesPaginateTypeDef,
     ListInstancesInputRequestTypeDef,
-    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
     ListNotebookExecutionsInputRequestTypeDef,
     ReleaseLabelFilterTypeDef,
-    ListReleaseLabelsOutputTypeDef,
-    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
-    ListStepsInputListStepsPaginateTypeDef,
     ListStepsInputRequestTypeDef,
-    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
-    ListStudiosInputListStudiosPaginateTypeDef,
     ListStudiosInputRequestTypeDef,
     StudioSummaryTypeDef,
     ListSupportedInstanceTypesInputRequestTypeDef,
     SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
-    ModifyClusterOutputTypeDef,
     NotebookS3LocationForOutputTypeDef,
     OutputNotebookS3LocationForOutputTypeDef,
     NotebookS3LocationFromInputTypeDef,
-    OnDemandCapacityReservationOptionsOutputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
-    PaginatorConfigTypeDef,
-    PlacementGroupConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
-    RunJobFlowOutputTypeDef,
-    SimpleScalingPolicyConfigurationOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
-    StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
+    AddInstanceFleetOutputTypeDef,
+    AddInstanceGroupsOutputTypeDef,
+    AddJobFlowStepsOutputTypeDef,
+    CreateSecurityConfigurationOutputTypeDef,
+    CreateStudioOutputTypeDef,
+    DescribeSecurityConfigurationOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListReleaseLabelsOutputTypeDef,
+    ModifyClusterOutputTypeDef,
+    RunJobFlowOutputTypeDef,
+    StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
+    StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
     BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
     CloudWatchAlarmDefinitionOutputTypeDef,
     CloudWatchAlarmDefinitionTypeDef,
     ClusterStatusTypeDef,
-    StudioTypeDef,
     ListBootstrapActionsOutputTypeDef,
-    ManagedScalingPolicyOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
-    InstanceFleetResizingSpecificationsOutputTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyOutputTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
+    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
+    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+    ListInstancesInputListInstancesPaginateTypeDef,
+    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
+    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
+    ListStepsInputListStepsPaginateTypeDef,
+    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
+    ListStudiosInputListStudiosPaginateTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
     ListSupportedInstanceTypesOutputTypeDef,
     NotebookExecutionSummaryTypeDef,
     NotebookExecutionTypeDef,
-    OnDemandProvisioningSpecificationOutputTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
-    ScalingActionOutputTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
+    DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
     ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
-    DescribeStudioOutputTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
     StepConfigOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
-    InstanceFleetProvisioningSpecificationsOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
@@ -669,15 +648,15 @@
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddInstanceFleetOutputTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-1.28.12/README.md` & `mypy-boto3-emr-1.28.15/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -393,224 +393,203 @@
 ### Typed dictionaries
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
-    AddInstanceFleetOutputTypeDef,
-    AddInstanceGroupsOutputTypeDef,
-    AddJobFlowStepsOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplicationOutputTypeDef,
     ApplicationTypeDef,
-    ScalingConstraintsOutputTypeDef,
-    AutoScalingPolicyStateChangeReasonTypeDef,
     ScalingConstraintsTypeDef,
-    AutoTerminationPolicyOutputTypeDef,
+    AutoScalingPolicyStateChangeReasonTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
-    PortRangeOutputTypeDef,
     PortRangeTypeDef,
     ScriptBootstrapActionConfigOutputTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
     ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
-    KerberosAttributesOutputTypeDef,
-    PlacementGroupConfigOutputTypeDef,
-    TagOutputTypeDef,
+    KerberosAttributesTypeDef,
+    PlacementGroupConfigTypeDef,
     CommandTypeDef,
-    ComputeLimitsOutputTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
-    CreateSecurityConfigurationOutputTypeDef,
-    CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
     DescribeJobFlowsInputRequestTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
-    DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
-    VolumeSpecificationOutputTypeDef,
     EbsVolumeTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExecutionEngineConfigOutputTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
-    KeyValueOutputTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
-    SpotProvisioningSpecificationOutputTypeDef,
     SpotProvisioningSpecificationTypeDef,
-    OnDemandResizingSpecificationOutputTypeDef,
-    SpotResizingSpecificationOutputTypeDef,
     OnDemandResizingSpecificationTypeDef,
     SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyOutputTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
     PlacementTypeOutputTypeDef,
-    KerberosAttributesTypeDef,
-    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
-    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
-    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
-    ListInstancesInputListInstancesPaginateTypeDef,
     ListInstancesInputRequestTypeDef,
-    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
     ListNotebookExecutionsInputRequestTypeDef,
     ReleaseLabelFilterTypeDef,
-    ListReleaseLabelsOutputTypeDef,
-    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
-    ListStepsInputListStepsPaginateTypeDef,
     ListStepsInputRequestTypeDef,
-    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
-    ListStudiosInputListStudiosPaginateTypeDef,
     ListStudiosInputRequestTypeDef,
     StudioSummaryTypeDef,
     ListSupportedInstanceTypesInputRequestTypeDef,
     SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
-    ModifyClusterOutputTypeDef,
     NotebookS3LocationForOutputTypeDef,
     OutputNotebookS3LocationForOutputTypeDef,
     NotebookS3LocationFromInputTypeDef,
-    OnDemandCapacityReservationOptionsOutputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
-    PaginatorConfigTypeDef,
-    PlacementGroupConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
-    RunJobFlowOutputTypeDef,
-    SimpleScalingPolicyConfigurationOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
-    StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
+    AddInstanceFleetOutputTypeDef,
+    AddInstanceGroupsOutputTypeDef,
+    AddJobFlowStepsOutputTypeDef,
+    CreateSecurityConfigurationOutputTypeDef,
+    CreateStudioOutputTypeDef,
+    DescribeSecurityConfigurationOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListReleaseLabelsOutputTypeDef,
+    ModifyClusterOutputTypeDef,
+    RunJobFlowOutputTypeDef,
+    StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
+    StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
     BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
     CloudWatchAlarmDefinitionOutputTypeDef,
     CloudWatchAlarmDefinitionTypeDef,
     ClusterStatusTypeDef,
-    StudioTypeDef,
     ListBootstrapActionsOutputTypeDef,
-    ManagedScalingPolicyOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
-    InstanceFleetResizingSpecificationsOutputTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyOutputTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
+    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
+    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+    ListInstancesInputListInstancesPaginateTypeDef,
+    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
+    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
+    ListStepsInputListStepsPaginateTypeDef,
+    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
+    ListStudiosInputListStudiosPaginateTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
     ListSupportedInstanceTypesOutputTypeDef,
     NotebookExecutionSummaryTypeDef,
     NotebookExecutionTypeDef,
-    OnDemandProvisioningSpecificationOutputTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
-    ScalingActionOutputTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
+    DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
     ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
-    DescribeStudioOutputTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
     StepConfigOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
-    InstanceFleetProvisioningSpecificationsOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
@@ -637,15 +616,15 @@
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddInstanceFleetOutputTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/__init__.py` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/__init__.pyi` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/__main__.py` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EMR 1.28.12\nVersion:         1.28.12\nBuilder version:"
-        " 7.15.2\nDocs:           "
+        "Type annotations for boto3.EMR 1.28.15\nVersion:         1.28.15\nBuilder version:"
+        " 7.16.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR\nOther"
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

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/client.py` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/client.pyi` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/literals.py` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/literals.pyi` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/paginator.py` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 class ListBootstrapActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listbootstrapactionspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBootstrapActionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listbootstrapactionspaginator)
         """
 
 
@@ -112,45 +112,45 @@
 
     def paginate(
         self,
         *,
         CreatedAfter: Union[datetime, str] = ...,
         CreatedBefore: Union[datetime, str] = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listclusterspaginator)
         """
 
 
 class ListInstanceFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancefleetspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstanceFleetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancefleetspaginator)
         """
 
 
 class ListInstanceGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancegroupspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstanceGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancegroupspaginator)
         """
 
 
@@ -165,15 +165,15 @@
         *,
         ClusterId: str,
         InstanceGroupId: str = ...,
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancespaginator)
         """
 
 
@@ -187,30 +187,30 @@
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: Union[datetime, str] = ...,
         To: Union[datetime, str] = ...,
         ExecutionEngineId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNotebookExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listnotebookexecutionspaginator)
         """
 
 
 class ListSecurityConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listsecurityconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listsecurityconfigurationspaginator)
         """
 
 
@@ -222,15 +222,15 @@
 
     def paginate(
         self,
         *,
         ClusterId: str,
         StepStates: Sequence[StepStateType] = ...,
         StepIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStepsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststepspaginator)
         """
 
 
@@ -241,28 +241,28 @@
     """
 
     def paginate(
         self,
         *,
         StudioId: str = ...,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStudioSessionMappingsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudioSessionMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiosessionmappingspaginator)
         """
 
 
 class ListStudiosPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiospaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStudiosOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiospaginator)
         """
```

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/paginator.pyi` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 class ListBootstrapActionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listbootstrapactionspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListBootstrapActionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListBootstrapActions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listbootstrapactionspaginator)
         """
 
 class ListClustersPaginator(Paginator):
@@ -108,43 +108,43 @@
 
     def paginate(
         self,
         *,
         CreatedAfter: Union[datetime, str] = ...,
         CreatedBefore: Union[datetime, str] = ...,
         ClusterStates: Sequence[ClusterStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListClustersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listclusterspaginator)
         """
 
 class ListInstanceFleetsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancefleetspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstanceFleetsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceFleets.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancefleetspaginator)
         """
 
 class ListInstanceGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancegroupspaginator)
     """
 
     def paginate(
-        self, *, ClusterId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ClusterId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstanceGroupsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstanceGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancegroupspaginator)
         """
 
 class ListInstancesPaginator(Paginator):
@@ -158,15 +158,15 @@
         *,
         ClusterId: str,
         InstanceGroupId: str = ...,
         InstanceGroupTypes: Sequence[InstanceGroupTypeType] = ...,
         InstanceFleetId: str = ...,
         InstanceFleetType: InstanceFleetTypeType = ...,
         InstanceStates: Sequence[InstanceStateType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListInstancesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListInstances.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listinstancespaginator)
         """
 
 class ListNotebookExecutionsPaginator(Paginator):
@@ -179,29 +179,29 @@
         self,
         *,
         EditorId: str = ...,
         Status: NotebookExecutionStatusType = ...,
         From: Union[datetime, str] = ...,
         To: Union[datetime, str] = ...,
         ExecutionEngineId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListNotebookExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListNotebookExecutions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listnotebookexecutionspaginator)
         """
 
 class ListSecurityConfigurationsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listsecurityconfigurationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListSecurityConfigurationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSecurityConfigurations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#listsecurityconfigurationspaginator)
         """
 
 class ListStepsPaginator(Paginator):
@@ -212,15 +212,15 @@
 
     def paginate(
         self,
         *,
         ClusterId: str,
         StepStates: Sequence[StepStateType] = ...,
         StepIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStepsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListSteps.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststepspaginator)
         """
 
 class ListStudioSessionMappingsPaginator(Paginator):
@@ -230,27 +230,27 @@
     """
 
     def paginate(
         self,
         *,
         StudioId: str = ...,
         IdentityType: IdentityTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStudioSessionMappingsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudioSessionMappings.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiosessionmappingspaginator)
         """
 
 class ListStudiosPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiospaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListStudiosOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR.Paginator.ListStudios.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/paginators/#liststudiospaginator)
         """
```

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/type_defs.py` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for emr service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_emr.type_defs import AddInstanceFleetOutputTypeDef
+    from mypy_boto3_emr.type_defs import ResponseMetadataTypeDef
 
-    data: AddInstanceFleetOutputTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -61,224 +61,203 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AddInstanceFleetOutputTypeDef",
-    "AddInstanceGroupsOutputTypeDef",
-    "AddJobFlowStepsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplicationOutputTypeDef",
     "ApplicationTypeDef",
-    "ScalingConstraintsOutputTypeDef",
-    "AutoScalingPolicyStateChangeReasonTypeDef",
     "ScalingConstraintsTypeDef",
-    "AutoTerminationPolicyOutputTypeDef",
+    "AutoScalingPolicyStateChangeReasonTypeDef",
     "AutoTerminationPolicyTypeDef",
     "BlockPublicAccessConfigurationMetadataTypeDef",
-    "PortRangeOutputTypeDef",
     "PortRangeTypeDef",
     "ScriptBootstrapActionConfigOutputTypeDef",
     "ScriptBootstrapActionConfigTypeDef",
     "CancelStepsInfoTypeDef",
     "CancelStepsInputRequestTypeDef",
-    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "ClusterStateChangeReasonTypeDef",
     "ClusterTimelineTypeDef",
     "ErrorDetailTypeDef",
     "Ec2InstanceAttributesTypeDef",
-    "KerberosAttributesOutputTypeDef",
-    "PlacementGroupConfigOutputTypeDef",
-    "TagOutputTypeDef",
+    "KerberosAttributesTypeDef",
+    "PlacementGroupConfigTypeDef",
     "CommandTypeDef",
-    "ComputeLimitsOutputTypeDef",
     "ComputeLimitsTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
-    "CreateSecurityConfigurationOutputTypeDef",
-    "CreateStudioOutputTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
     "DeleteStudioInputRequestTypeDef",
     "DeleteStudioSessionMappingInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterInputRequestTypeDef",
     "DescribeJobFlowsInputRequestTypeDef",
     "DescribeNotebookExecutionInputRequestTypeDef",
     "DescribeReleaseLabelInputRequestTypeDef",
     "OSReleaseTypeDef",
     "SimplifiedApplicationTypeDef",
     "DescribeSecurityConfigurationInputRequestTypeDef",
-    "DescribeSecurityConfigurationOutputTypeDef",
     "DescribeStepInputRequestTypeDef",
     "DescribeStudioInputRequestTypeDef",
     "VolumeSpecificationTypeDef",
-    "VolumeSpecificationOutputTypeDef",
     "EbsVolumeTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExecutionEngineConfigOutputTypeDef",
     "ExecutionEngineConfigTypeDef",
     "FailureDetailsTypeDef",
     "GetAutoTerminationPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsInputRequestTypeDef",
     "GetManagedScalingPolicyInputRequestTypeDef",
     "GetStudioSessionMappingInputRequestTypeDef",
     "SessionMappingDetailTypeDef",
-    "KeyValueOutputTypeDef",
     "KeyValueTypeDef",
     "HadoopStepConfigTypeDef",
-    "SpotProvisioningSpecificationOutputTypeDef",
     "SpotProvisioningSpecificationTypeDef",
-    "OnDemandResizingSpecificationOutputTypeDef",
-    "SpotResizingSpecificationOutputTypeDef",
     "OnDemandResizingSpecificationTypeDef",
     "SpotResizingSpecificationTypeDef",
     "InstanceFleetStateChangeReasonTypeDef",
     "InstanceFleetTimelineTypeDef",
     "InstanceGroupDetailTypeDef",
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
     "InstanceResizePolicyOutputTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
     "PlacementTypeOutputTypeDef",
-    "KerberosAttributesTypeDef",
-    "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
-    "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
-    "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
     "ListInstanceGroupsInputRequestTypeDef",
-    "ListInstancesInputListInstancesPaginateTypeDef",
     "ListInstancesInputRequestTypeDef",
-    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     "ListNotebookExecutionsInputRequestTypeDef",
     "ReleaseLabelFilterTypeDef",
-    "ListReleaseLabelsOutputTypeDef",
-    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
     "ListSecurityConfigurationsInputRequestTypeDef",
     "SecurityConfigurationSummaryTypeDef",
-    "ListStepsInputListStepsPaginateTypeDef",
     "ListStepsInputRequestTypeDef",
-    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
     "ListStudioSessionMappingsInputRequestTypeDef",
     "SessionMappingSummaryTypeDef",
-    "ListStudiosInputListStudiosPaginateTypeDef",
     "ListStudiosInputRequestTypeDef",
     "StudioSummaryTypeDef",
     "ListSupportedInstanceTypesInputRequestTypeDef",
     "SupportedInstanceTypeTypeDef",
     "ModifyClusterInputRequestTypeDef",
-    "ModifyClusterOutputTypeDef",
     "NotebookS3LocationForOutputTypeDef",
     "OutputNotebookS3LocationForOutputTypeDef",
     "NotebookS3LocationFromInputTypeDef",
-    "OnDemandCapacityReservationOptionsOutputTypeDef",
     "OnDemandCapacityReservationOptionsTypeDef",
     "OutputNotebookS3LocationFromInputTypeDef",
-    "PaginatorConfigTypeDef",
-    "PlacementGroupConfigTypeDef",
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     "RemoveAutoTerminationPolicyInputRequestTypeDef",
     "RemoveManagedScalingPolicyInputRequestTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SupportedProductConfigTypeDef",
-    "RunJobFlowOutputTypeDef",
-    "SimpleScalingPolicyConfigurationOutputTypeDef",
     "SimpleScalingPolicyConfigurationTypeDef",
     "SetTerminationProtectionInputRequestTypeDef",
     "SetVisibleToAllUsersInputRequestTypeDef",
-    "StartNotebookExecutionOutputTypeDef",
     "StepExecutionStatusDetailTypeDef",
     "StepStateChangeReasonTypeDef",
     "StepTimelineTypeDef",
     "StopNotebookExecutionInputRequestTypeDef",
     "TerminateJobFlowsInputRequestTypeDef",
     "UpdateStudioInputRequestTypeDef",
     "UpdateStudioSessionMappingInputRequestTypeDef",
+    "AddInstanceFleetOutputTypeDef",
+    "AddInstanceGroupsOutputTypeDef",
+    "AddJobFlowStepsOutputTypeDef",
+    "CreateSecurityConfigurationOutputTypeDef",
+    "CreateStudioOutputTypeDef",
+    "DescribeSecurityConfigurationOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListReleaseLabelsOutputTypeDef",
+    "ModifyClusterOutputTypeDef",
+    "RunJobFlowOutputTypeDef",
+    "StartNotebookExecutionOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
+    "StudioTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
     "BlockPublicAccessConfigurationOutputTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
     "BootstrapActionConfigOutputTypeDef",
     "BootstrapActionConfigTypeDef",
     "CancelStepsOutputTypeDef",
     "CloudWatchAlarmDefinitionOutputTypeDef",
     "CloudWatchAlarmDefinitionTypeDef",
     "ClusterStatusTypeDef",
-    "StudioTypeDef",
     "ListBootstrapActionsOutputTypeDef",
-    "ManagedScalingPolicyOutputTypeDef",
     "ManagedScalingPolicyTypeDef",
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
     "DescribeStepInputStepCompleteWaitTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
     "HadoopJarStepConfigOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
-    "InstanceFleetResizingSpecificationsOutputTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
     "ShrinkPolicyOutputTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
+    "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
+    "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    "ListInstancesInputListInstancesPaginateTypeDef",
+    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
+    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
+    "ListStepsInputListStepsPaginateTypeDef",
+    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
+    "ListStudiosInputListStudiosPaginateTypeDef",
     "ListReleaseLabelsInputRequestTypeDef",
     "ListSecurityConfigurationsOutputTypeDef",
     "ListStudioSessionMappingsOutputTypeDef",
     "ListStudiosOutputTypeDef",
     "ListSupportedInstanceTypesOutputTypeDef",
     "NotebookExecutionSummaryTypeDef",
     "NotebookExecutionTypeDef",
-    "OnDemandProvisioningSpecificationOutputTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
-    "ScalingActionOutputTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
+    "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
     "ScalingTriggerOutputTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
-    "DescribeStudioOutputTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
     "StepConfigOutputTypeDef",
     "StepConfigTypeDef",
     "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
     "ListNotebookExecutionsOutputTypeDef",
     "DescribeNotebookExecutionOutputTypeDef",
-    "InstanceFleetProvisioningSpecificationsOutputTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
     "ScalingRuleOutputTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
@@ -304,39 +283,22 @@
     "DescribeJobFlowsOutputTypeDef",
     "ListInstanceGroupsOutputTypeDef",
     "AddInstanceGroupsInputRequestTypeDef",
     "JobFlowInstancesConfigTypeDef",
     "RunJobFlowInputRequestTypeDef",
 )
 
-AddInstanceFleetOutputTypeDef = TypedDict(
-    "AddInstanceFleetOutputTypeDef",
-    {
-        "ClusterId": str,
-        "InstanceFleetId": str,
-        "ClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddInstanceGroupsOutputTypeDef = TypedDict(
-    "AddInstanceGroupsOutputTypeDef",
-    {
-        "JobFlowId": str,
-        "InstanceGroupIds": List[str],
-        "ClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddJobFlowStepsOutputTypeDef = TypedDict(
-    "AddJobFlowStepsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "StepIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -363,16 +325,16 @@
         "Version": str,
         "Args": Sequence[str],
         "AdditionalInfo": Mapping[str, str],
     },
     total=False,
 )
 
-ScalingConstraintsOutputTypeDef = TypedDict(
-    "ScalingConstraintsOutputTypeDef",
+ScalingConstraintsTypeDef = TypedDict(
+    "ScalingConstraintsTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
 )
 
 AutoScalingPolicyStateChangeReasonTypeDef = TypedDict(
@@ -380,30 +342,14 @@
     {
         "Code": AutoScalingPolicyStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
 )
 
-ScalingConstraintsTypeDef = TypedDict(
-    "ScalingConstraintsTypeDef",
-    {
-        "MinCapacity": int,
-        "MaxCapacity": int,
-    },
-)
-
-AutoTerminationPolicyOutputTypeDef = TypedDict(
-    "AutoTerminationPolicyOutputTypeDef",
-    {
-        "IdleTimeout": int,
-    },
-    total=False,
-)
-
 AutoTerminationPolicyTypeDef = TypedDict(
     "AutoTerminationPolicyTypeDef",
     {
         "IdleTimeout": int,
     },
     total=False,
 )
@@ -412,33 +358,14 @@
     "BlockPublicAccessConfigurationMetadataTypeDef",
     {
         "CreationDateTime": datetime,
         "CreatedByArn": str,
     },
 )
 
-_RequiredPortRangeOutputTypeDef = TypedDict(
-    "_RequiredPortRangeOutputTypeDef",
-    {
-        "MinRange": int,
-    },
-)
-_OptionalPortRangeOutputTypeDef = TypedDict(
-    "_OptionalPortRangeOutputTypeDef",
-    {
-        "MaxRange": int,
-    },
-    total=False,
-)
-
-
-class PortRangeOutputTypeDef(_RequiredPortRangeOutputTypeDef, _OptionalPortRangeOutputTypeDef):
-    pass
-
-
 _RequiredPortRangeTypeDef = TypedDict(
     "_RequiredPortRangeTypeDef",
     {
         "MinRange": int,
     },
 )
 _OptionalPortRangeTypeDef = TypedDict(
@@ -525,23 +452,14 @@
 
 class CancelStepsInputRequestTypeDef(
     _RequiredCancelStepsInputRequestTypeDef, _OptionalCancelStepsInputRequestTypeDef
 ):
     pass
 
 
-MetricDimensionOutputTypeDef = TypedDict(
-    "MetricDimensionOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -590,102 +508,69 @@
         "ServiceAccessSecurityGroup": str,
         "AdditionalMasterSecurityGroups": List[str],
         "AdditionalSlaveSecurityGroups": List[str],
     },
     total=False,
 )
 
-_RequiredKerberosAttributesOutputTypeDef = TypedDict(
-    "_RequiredKerberosAttributesOutputTypeDef",
+_RequiredKerberosAttributesTypeDef = TypedDict(
+    "_RequiredKerberosAttributesTypeDef",
     {
         "Realm": str,
         "KdcAdminPassword": str,
     },
 )
-_OptionalKerberosAttributesOutputTypeDef = TypedDict(
-    "_OptionalKerberosAttributesOutputTypeDef",
+_OptionalKerberosAttributesTypeDef = TypedDict(
+    "_OptionalKerberosAttributesTypeDef",
     {
         "CrossRealmTrustPrincipalPassword": str,
         "ADDomainJoinUser": str,
         "ADDomainJoinPassword": str,
     },
     total=False,
 )
 
 
-class KerberosAttributesOutputTypeDef(
-    _RequiredKerberosAttributesOutputTypeDef, _OptionalKerberosAttributesOutputTypeDef
+class KerberosAttributesTypeDef(
+    _RequiredKerberosAttributesTypeDef, _OptionalKerberosAttributesTypeDef
 ):
     pass
 
 
-_RequiredPlacementGroupConfigOutputTypeDef = TypedDict(
-    "_RequiredPlacementGroupConfigOutputTypeDef",
+_RequiredPlacementGroupConfigTypeDef = TypedDict(
+    "_RequiredPlacementGroupConfigTypeDef",
     {
         "InstanceRole": InstanceRoleTypeType,
     },
 )
-_OptionalPlacementGroupConfigOutputTypeDef = TypedDict(
-    "_OptionalPlacementGroupConfigOutputTypeDef",
+_OptionalPlacementGroupConfigTypeDef = TypedDict(
+    "_OptionalPlacementGroupConfigTypeDef",
     {
         "PlacementStrategy": PlacementGroupStrategyType,
     },
     total=False,
 )
 
 
-class PlacementGroupConfigOutputTypeDef(
-    _RequiredPlacementGroupConfigOutputTypeDef, _OptionalPlacementGroupConfigOutputTypeDef
+class PlacementGroupConfigTypeDef(
+    _RequiredPlacementGroupConfigTypeDef, _OptionalPlacementGroupConfigTypeDef
 ):
     pass
 
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
     {
         "Name": str,
         "ScriptPath": str,
         "Args": List[str],
     },
     total=False,
 )
 
-_RequiredComputeLimitsOutputTypeDef = TypedDict(
-    "_RequiredComputeLimitsOutputTypeDef",
-    {
-        "UnitType": ComputeLimitsUnitTypeType,
-        "MinimumCapacityUnits": int,
-        "MaximumCapacityUnits": int,
-    },
-)
-_OptionalComputeLimitsOutputTypeDef = TypedDict(
-    "_OptionalComputeLimitsOutputTypeDef",
-    {
-        "MaximumOnDemandCapacityUnits": int,
-        "MaximumCoreCapacityUnits": int,
-    },
-    total=False,
-)
-
-
-class ComputeLimitsOutputTypeDef(
-    _RequiredComputeLimitsOutputTypeDef, _OptionalComputeLimitsOutputTypeDef
-):
-    pass
-
-
 _RequiredComputeLimitsTypeDef = TypedDict(
     "_RequiredComputeLimitsTypeDef",
     {
         "UnitType": ComputeLimitsUnitTypeType,
         "MinimumCapacityUnits": int,
         "MaximumCapacityUnits": int,
     },
@@ -728,32 +613,14 @@
     "CreateSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
         "SecurityConfiguration": str,
     },
 )
 
-CreateSecurityConfigurationOutputTypeDef = TypedDict(
-    "CreateSecurityConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "CreationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStudioOutputTypeDef = TypedDict(
-    "CreateStudioOutputTypeDef",
-    {
-        "StudioId": str,
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateStudioSessionMappingInputRequestTypeDef = TypedDict(
     "_RequiredCreateStudioSessionMappingInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
     },
@@ -886,24 +753,14 @@
 DescribeSecurityConfigurationInputRequestTypeDef = TypedDict(
     "DescribeSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeSecurityConfigurationOutputTypeDef = TypedDict(
-    "DescribeSecurityConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "SecurityConfiguration": str,
-        "CreationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeStepInputRequestTypeDef = TypedDict(
     "DescribeStepInputRequestTypeDef",
     {
         "ClusterId": str,
         "StepId": str,
     },
 )
@@ -934,76 +791,23 @@
 
 class VolumeSpecificationTypeDef(
     _RequiredVolumeSpecificationTypeDef, _OptionalVolumeSpecificationTypeDef
 ):
     pass
 
 
-_RequiredVolumeSpecificationOutputTypeDef = TypedDict(
-    "_RequiredVolumeSpecificationOutputTypeDef",
-    {
-        "VolumeType": str,
-        "SizeInGB": int,
-    },
-)
-_OptionalVolumeSpecificationOutputTypeDef = TypedDict(
-    "_OptionalVolumeSpecificationOutputTypeDef",
-    {
-        "Iops": int,
-        "Throughput": int,
-    },
-    total=False,
-)
-
-
-class VolumeSpecificationOutputTypeDef(
-    _RequiredVolumeSpecificationOutputTypeDef, _OptionalVolumeSpecificationOutputTypeDef
-):
-    pass
-
-
 EbsVolumeTypeDef = TypedDict(
     "EbsVolumeTypeDef",
     {
         "Device": str,
         "VolumeId": str,
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
-_RequiredExecutionEngineConfigOutputTypeDef = TypedDict(
-    "_RequiredExecutionEngineConfigOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalExecutionEngineConfigOutputTypeDef = TypedDict(
-    "_OptionalExecutionEngineConfigOutputTypeDef",
-    {
-        "Type": Literal["EMR"],
-        "MasterInstanceSecurityGroupId": str,
-        "ExecutionRoleArn": str,
-    },
-    total=False,
-)
-
-
-class ExecutionEngineConfigOutputTypeDef(
-    _RequiredExecutionEngineConfigOutputTypeDef, _OptionalExecutionEngineConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredExecutionEngineConfigTypeDef = TypedDict(
     "_RequiredExecutionEngineConfigTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalExecutionEngineConfigTypeDef = TypedDict(
@@ -1089,23 +893,14 @@
         "SessionPolicyArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-KeyValueOutputTypeDef = TypedDict(
-    "KeyValueOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 KeyValueTypeDef = TypedDict(
     "KeyValueTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -1118,38 +913,14 @@
         "Properties": Dict[str, str],
         "MainClass": str,
         "Args": List[str],
     },
     total=False,
 )
 
-_RequiredSpotProvisioningSpecificationOutputTypeDef = TypedDict(
-    "_RequiredSpotProvisioningSpecificationOutputTypeDef",
-    {
-        "TimeoutDurationMinutes": int,
-        "TimeoutAction": SpotProvisioningTimeoutActionType,
-    },
-)
-_OptionalSpotProvisioningSpecificationOutputTypeDef = TypedDict(
-    "_OptionalSpotProvisioningSpecificationOutputTypeDef",
-    {
-        "BlockDurationMinutes": int,
-        "AllocationStrategy": SpotProvisioningAllocationStrategyType,
-    },
-    total=False,
-)
-
-
-class SpotProvisioningSpecificationOutputTypeDef(
-    _RequiredSpotProvisioningSpecificationOutputTypeDef,
-    _OptionalSpotProvisioningSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredSpotProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredSpotProvisioningSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
         "TimeoutAction": SpotProvisioningTimeoutActionType,
     },
 )
@@ -1165,28 +936,14 @@
 
 class SpotProvisioningSpecificationTypeDef(
     _RequiredSpotProvisioningSpecificationTypeDef, _OptionalSpotProvisioningSpecificationTypeDef
 ):
     pass
 
 
-OnDemandResizingSpecificationOutputTypeDef = TypedDict(
-    "OnDemandResizingSpecificationOutputTypeDef",
-    {
-        "TimeoutDurationMinutes": int,
-    },
-)
-
-SpotResizingSpecificationOutputTypeDef = TypedDict(
-    "SpotResizingSpecificationOutputTypeDef",
-    {
-        "TimeoutDurationMinutes": int,
-    },
-)
-
 OnDemandResizingSpecificationTypeDef = TypedDict(
     "OnDemandResizingSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
     },
 )
 
@@ -1347,60 +1104,24 @@
     {
         "AvailabilityZone": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-_RequiredKerberosAttributesTypeDef = TypedDict(
-    "_RequiredKerberosAttributesTypeDef",
-    {
-        "Realm": str,
-        "KdcAdminPassword": str,
-    },
-)
-_OptionalKerberosAttributesTypeDef = TypedDict(
-    "_OptionalKerberosAttributesTypeDef",
-    {
-        "CrossRealmTrustPrincipalPassword": str,
-        "ADDomainJoinUser": str,
-        "ADDomainJoinPassword": str,
-    },
-    total=False,
-)
-
-
-class KerberosAttributesTypeDef(
-    _RequiredKerberosAttributesTypeDef, _OptionalKerberosAttributesTypeDef
-):
-    pass
-
-
-_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
-    "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
-    "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
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
 
-
-class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
-    _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-    _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListBootstrapActionsInputRequestTypeDef = TypedDict(
     "_RequiredListBootstrapActionsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListBootstrapActionsInputRequestTypeDef = TypedDict(
@@ -1415,58 +1136,25 @@
 class ListBootstrapActionsInputRequestTypeDef(
     _RequiredListBootstrapActionsInputRequestTypeDef,
     _OptionalListBootstrapActionsInputRequestTypeDef,
 ):
     pass
 
 
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
-    {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "ClusterStates": Sequence[ClusterStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ClusterStates": Sequence[ClusterStateType],
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
-    _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-    _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceFleetsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceFleetsInputRequestTypeDef = TypedDict(
@@ -1480,36 +1168,14 @@
 
 class ListInstanceFleetsInputRequestTypeDef(
     _RequiredListInstanceFleetsInputRequestTypeDef, _OptionalListInstanceFleetsInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
-    _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-    _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInstanceGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceGroupsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceGroupsInputRequestTypeDef = TypedDict(
@@ -1523,41 +1189,14 @@
 
 class ListInstanceGroupsInputRequestTypeDef(
     _RequiredListInstanceGroupsInputRequestTypeDef, _OptionalListInstanceGroupsInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesInputListInstancesPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesInputListInstancesPaginateTypeDef",
-    {
-        "InstanceGroupId": str,
-        "InstanceGroupTypes": Sequence[InstanceGroupTypeType],
-        "InstanceFleetId": str,
-        "InstanceFleetType": InstanceFleetTypeType,
-        "InstanceStates": Sequence[InstanceStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInstancesInputListInstancesPaginateTypeDef(
-    _RequiredListInstancesInputListInstancesPaginateTypeDef,
-    _OptionalListInstancesInputListInstancesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListInstancesInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstancesInputRequestTypeDef = TypedDict(
@@ -1576,27 +1215,14 @@
 
 class ListInstancesInputRequestTypeDef(
     _RequiredListInstancesInputRequestTypeDef, _OptionalListInstancesInputRequestTypeDef
 ):
     pass
 
 
-ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
-    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
-    {
-        "EditorId": str,
-        "Status": NotebookExecutionStatusType,
-        "From": Union[datetime, str],
-        "To": Union[datetime, str],
-        "ExecutionEngineId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNotebookExecutionsInputRequestTypeDef = TypedDict(
     "ListNotebookExecutionsInputRequestTypeDef",
     {
         "EditorId": str,
         "Status": NotebookExecutionStatusType,
         "From": Union[datetime, str],
         "To": Union[datetime, str],
@@ -1611,31 +1237,14 @@
     {
         "Prefix": str,
         "Application": str,
     },
     total=False,
 )
 
-ListReleaseLabelsOutputTypeDef = TypedDict(
-    "ListReleaseLabelsOutputTypeDef",
-    {
-        "ReleaseLabels": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
-    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityConfigurationsInputRequestTypeDef = TypedDict(
     "ListSecurityConfigurationsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
@@ -1645,37 +1254,14 @@
     {
         "Name": str,
         "CreationDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListStepsInputListStepsPaginateTypeDef = TypedDict(
-    "_RequiredListStepsInputListStepsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListStepsInputListStepsPaginateTypeDef = TypedDict(
-    "_OptionalListStepsInputListStepsPaginateTypeDef",
-    {
-        "StepStates": Sequence[StepStateType],
-        "StepIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListStepsInputListStepsPaginateTypeDef(
-    _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListStepsInputRequestTypeDef = TypedDict(
     "_RequiredListStepsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListStepsInputRequestTypeDef = TypedDict(
@@ -1691,24 +1277,14 @@
 
 class ListStepsInputRequestTypeDef(
     _RequiredListStepsInputRequestTypeDef, _OptionalListStepsInputRequestTypeDef
 ):
     pass
 
 
-ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
-    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
-    {
-        "StudioId": str,
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStudioSessionMappingsInputRequestTypeDef = TypedDict(
     "ListStudioSessionMappingsInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "Marker": str,
     },
@@ -1724,22 +1300,14 @@
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-ListStudiosInputListStudiosPaginateTypeDef = TypedDict(
-    "ListStudiosInputListStudiosPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStudiosInputRequestTypeDef = TypedDict(
     "ListStudiosInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
@@ -1815,22 +1383,14 @@
 
 class ModifyClusterInputRequestTypeDef(
     _RequiredModifyClusterInputRequestTypeDef, _OptionalModifyClusterInputRequestTypeDef
 ):
     pass
 
 
-ModifyClusterOutputTypeDef = TypedDict(
-    "ModifyClusterOutputTypeDef",
-    {
-        "StepConcurrencyLevel": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NotebookS3LocationForOutputTypeDef = TypedDict(
     "NotebookS3LocationForOutputTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
@@ -1850,24 +1410,14 @@
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
 )
 
-OnDemandCapacityReservationOptionsOutputTypeDef = TypedDict(
-    "OnDemandCapacityReservationOptionsOutputTypeDef",
-    {
-        "UsageStrategy": Literal["use-capacity-reservations-first"],
-        "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
-        "CapacityReservationResourceGroupArn": str,
-    },
-    total=False,
-)
-
 OnDemandCapacityReservationOptionsTypeDef = TypedDict(
     "OnDemandCapacityReservationOptionsTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
         "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
         "CapacityReservationResourceGroupArn": str,
     },
@@ -1879,45 +1429,14 @@
     {
         "Bucket": str,
         "Key": str,
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
-_RequiredPlacementGroupConfigTypeDef = TypedDict(
-    "_RequiredPlacementGroupConfigTypeDef",
-    {
-        "InstanceRole": InstanceRoleTypeType,
-    },
-)
-_OptionalPlacementGroupConfigTypeDef = TypedDict(
-    "_OptionalPlacementGroupConfigTypeDef",
-    {
-        "PlacementStrategy": PlacementGroupStrategyType,
-    },
-    total=False,
-)
-
-
-class PlacementGroupConfigTypeDef(
-    _RequiredPlacementGroupConfigTypeDef, _OptionalPlacementGroupConfigTypeDef
-):
-    pass
-
-
 RemoveAutoScalingPolicyInputRequestTypeDef = TypedDict(
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
     },
 )
@@ -1940,66 +1459,23 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
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
 SupportedProductConfigTypeDef = TypedDict(
     "SupportedProductConfigTypeDef",
     {
         "Name": str,
         "Args": Sequence[str],
     },
     total=False,
 )
 
-RunJobFlowOutputTypeDef = TypedDict(
-    "RunJobFlowOutputTypeDef",
-    {
-        "JobFlowId": str,
-        "ClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredSimpleScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSimpleScalingPolicyConfigurationOutputTypeDef",
-    {
-        "ScalingAdjustment": int,
-    },
-)
-_OptionalSimpleScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSimpleScalingPolicyConfigurationOutputTypeDef",
-    {
-        "AdjustmentType": AdjustmentTypeType,
-        "CoolDown": int,
-    },
-    total=False,
-)
-
-
-class SimpleScalingPolicyConfigurationOutputTypeDef(
-    _RequiredSimpleScalingPolicyConfigurationOutputTypeDef,
-    _OptionalSimpleScalingPolicyConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredSimpleScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredSimpleScalingPolicyConfigurationTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalSimpleScalingPolicyConfigurationTypeDef = TypedDict(
@@ -2031,22 +1507,14 @@
     "SetVisibleToAllUsersInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "VisibleToAllUsers": bool,
     },
 )
 
-StartNotebookExecutionOutputTypeDef = TypedDict(
-    "StartNotebookExecutionOutputTypeDef",
-    {
-        "NotebookExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStepExecutionStatusDetailTypeDef = TypedDict(
     "_RequiredStepExecutionStatusDetailTypeDef",
     {
         "State": StepExecutionStateType,
         "CreationDateTime": datetime,
     },
 )
@@ -2145,14 +1613,111 @@
 class UpdateStudioSessionMappingInputRequestTypeDef(
     _RequiredUpdateStudioSessionMappingInputRequestTypeDef,
     _OptionalUpdateStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
 
+AddInstanceFleetOutputTypeDef = TypedDict(
+    "AddInstanceFleetOutputTypeDef",
+    {
+        "ClusterId": str,
+        "InstanceFleetId": str,
+        "ClusterArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddInstanceGroupsOutputTypeDef = TypedDict(
+    "AddInstanceGroupsOutputTypeDef",
+    {
+        "JobFlowId": str,
+        "InstanceGroupIds": List[str],
+        "ClusterArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddJobFlowStepsOutputTypeDef = TypedDict(
+    "AddJobFlowStepsOutputTypeDef",
+    {
+        "StepIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSecurityConfigurationOutputTypeDef = TypedDict(
+    "CreateSecurityConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "CreationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStudioOutputTypeDef = TypedDict(
+    "CreateStudioOutputTypeDef",
+    {
+        "StudioId": str,
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSecurityConfigurationOutputTypeDef = TypedDict(
+    "DescribeSecurityConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "SecurityConfiguration": str,
+        "CreationDateTime": datetime,
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
+ListReleaseLabelsOutputTypeDef = TypedDict(
+    "ListReleaseLabelsOutputTypeDef",
+    {
+        "ReleaseLabels": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyClusterOutputTypeDef = TypedDict(
+    "ModifyClusterOutputTypeDef",
+    {
+        "StepConcurrencyLevel": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RunJobFlowOutputTypeDef = TypedDict(
+    "RunJobFlowOutputTypeDef",
+    {
+        "JobFlowId": str,
+        "ClusterArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartNotebookExecutionOutputTypeDef = TypedDict(
+    "StartNotebookExecutionOutputTypeDef",
+    {
+        "NotebookExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2185,28 +1750,52 @@
 
 class CreateStudioInputRequestTypeDef(
     _RequiredCreateStudioInputRequestTypeDef, _OptionalCreateStudioInputRequestTypeDef
 ):
     pass
 
 
+StudioTypeDef = TypedDict(
+    "StudioTypeDef",
+    {
+        "StudioId": str,
+        "StudioArn": str,
+        "Name": str,
+        "Description": str,
+        "AuthMode": AuthModeType,
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "ServiceRole": str,
+        "UserRole": str,
+        "WorkspaceSecurityGroupId": str,
+        "EngineSecurityGroupId": str,
+        "Url": str,
+        "CreationTime": datetime,
+        "DefaultS3Location": str,
+        "IdpAuthUrl": str,
+        "IdpRelayStateParameterName": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 AutoScalingPolicyStatusTypeDef = TypedDict(
     "AutoScalingPolicyStatusTypeDef",
     {
         "State": AutoScalingPolicyStateType,
         "StateChangeReason": AutoScalingPolicyStateChangeReasonTypeDef,
     },
     total=False,
 )
 
 GetAutoTerminationPolicyOutputTypeDef = TypedDict(
     "GetAutoTerminationPolicyOutputTypeDef",
     {
-        "AutoTerminationPolicy": AutoTerminationPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAutoTerminationPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutAutoTerminationPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
@@ -2233,15 +1822,15 @@
     {
         "BlockPublicSecurityGroupRules": bool,
     },
 )
 _OptionalBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "_OptionalBlockPublicAccessConfigurationOutputTypeDef",
     {
-        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeOutputTypeDef],
+        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeTypeDef],
     },
     total=False,
 )
 
 
 class BlockPublicAccessConfigurationOutputTypeDef(
     _RequiredBlockPublicAccessConfigurationOutputTypeDef,
@@ -2287,15 +1876,15 @@
     },
 )
 
 CancelStepsOutputTypeDef = TypedDict(
     "CancelStepsOutputTypeDef",
     {
         "CancelStepsInfoList": List[CancelStepsInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmDefinitionOutputTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
@@ -2307,15 +1896,15 @@
 _OptionalCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
     "_OptionalCloudWatchAlarmDefinitionOutputTypeDef",
     {
         "EvaluationPeriods": int,
         "Namespace": str,
         "Statistic": StatisticType,
         "Unit": UnitType,
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 
 class CloudWatchAlarmDefinitionOutputTypeDef(
     _RequiredCloudWatchAlarmDefinitionOutputTypeDef, _OptionalCloudWatchAlarmDefinitionOutputTypeDef
@@ -2358,55 +1947,23 @@
         "StateChangeReason": ClusterStateChangeReasonTypeDef,
         "Timeline": ClusterTimelineTypeDef,
         "ErrorDetails": List[ErrorDetailTypeDef],
     },
     total=False,
 )
 
-StudioTypeDef = TypedDict(
-    "StudioTypeDef",
-    {
-        "StudioId": str,
-        "StudioArn": str,
-        "Name": str,
-        "Description": str,
-        "AuthMode": AuthModeType,
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "ServiceRole": str,
-        "UserRole": str,
-        "WorkspaceSecurityGroupId": str,
-        "EngineSecurityGroupId": str,
-        "Url": str,
-        "CreationTime": datetime,
-        "DefaultS3Location": str,
-        "IdpAuthUrl": str,
-        "IdpRelayStateParameterName": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 ListBootstrapActionsOutputTypeDef = TypedDict(
     "ListBootstrapActionsOutputTypeDef",
     {
         "BootstrapActions": List[CommandTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ManagedScalingPolicyOutputTypeDef = TypedDict(
-    "ManagedScalingPolicyOutputTypeDef",
-    {
-        "ComputeLimits": ComputeLimitsOutputTypeDef,
-    },
-    total=False,
-)
-
 ManagedScalingPolicyTypeDef = TypedDict(
     "ManagedScalingPolicyTypeDef",
     {
         "ComputeLimits": ComputeLimitsTypeDef,
     },
     total=False,
 )
@@ -2489,15 +2046,15 @@
 DescribeReleaseLabelOutputTypeDef = TypedDict(
     "DescribeReleaseLabelOutputTypeDef",
     {
         "ReleaseLabel": str,
         "Applications": List[SimplifiedApplicationTypeDef],
         "NextToken": str,
         "AvailableOSReleases": List[OSReleaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEbsBlockDeviceConfigTypeDef = TypedDict(
     "_RequiredEbsBlockDeviceConfigTypeDef",
     {
         "VolumeSpecification": VolumeSpecificationTypeDef,
@@ -2517,38 +2074,38 @@
 ):
     pass
 
 
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
-        "VolumeSpecification": VolumeSpecificationOutputTypeDef,
+        "VolumeSpecification": VolumeSpecificationTypeDef,
         "Device": str,
     },
     total=False,
 )
 
 GetStudioSessionMappingOutputTypeDef = TypedDict(
     "GetStudioSessionMappingOutputTypeDef",
     {
         "SessionMapping": SessionMappingDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHadoopJarStepConfigOutputTypeDef = TypedDict(
     "_RequiredHadoopJarStepConfigOutputTypeDef",
     {
         "Jar": str,
     },
 )
 _OptionalHadoopJarStepConfigOutputTypeDef = TypedDict(
     "_OptionalHadoopJarStepConfigOutputTypeDef",
     {
-        "Properties": List[KeyValueOutputTypeDef],
+        "Properties": List[KeyValueTypeDef],
         "MainClass": str,
         "Args": List[str],
     },
     total=False,
 )
 
 
@@ -2577,23 +2134,14 @@
 
 class HadoopJarStepConfigTypeDef(
     _RequiredHadoopJarStepConfigTypeDef, _OptionalHadoopJarStepConfigTypeDef
 ):
     pass
 
 
-InstanceFleetResizingSpecificationsOutputTypeDef = TypedDict(
-    "InstanceFleetResizingSpecificationsOutputTypeDef",
-    {
-        "SpotResizeSpecification": SpotResizingSpecificationOutputTypeDef,
-        "OnDemandResizeSpecification": OnDemandResizingSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
 InstanceFleetResizingSpecificationsTypeDef = TypedDict(
     "InstanceFleetResizingSpecificationsTypeDef",
     {
         "SpotResizeSpecification": SpotResizingSpecificationTypeDef,
         "OnDemandResizeSpecification": OnDemandResizingSpecificationTypeDef,
     },
     total=False,
@@ -2675,14 +2223,180 @@
 
 class JobFlowInstancesDetailTypeDef(
     _RequiredJobFlowInstancesDetailTypeDef, _OptionalJobFlowInstancesDetailTypeDef
 ):
     pass
 
 
+_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
+    "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
+    "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
+    _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+):
+    pass
+
+
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "CreatedAfter": Union[datetime, str],
+        "CreatedBefore": Union[datetime, str],
+        "ClusterStates": Sequence[ClusterStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
+    _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+    _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
+    _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+    _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesInputListInstancesPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesInputListInstancesPaginateTypeDef",
+    {
+        "InstanceGroupId": str,
+        "InstanceGroupTypes": Sequence[InstanceGroupTypeType],
+        "InstanceFleetId": str,
+        "InstanceFleetType": InstanceFleetTypeType,
+        "InstanceStates": Sequence[InstanceStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInstancesInputListInstancesPaginateTypeDef(
+    _RequiredListInstancesInputListInstancesPaginateTypeDef,
+    _OptionalListInstancesInputListInstancesPaginateTypeDef,
+):
+    pass
+
+
+ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
+    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
+    {
+        "EditorId": str,
+        "Status": NotebookExecutionStatusType,
+        "From": Union[datetime, str],
+        "To": Union[datetime, str],
+        "ExecutionEngineId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
+    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListStepsInputListStepsPaginateTypeDef = TypedDict(
+    "_RequiredListStepsInputListStepsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListStepsInputListStepsPaginateTypeDef = TypedDict(
+    "_OptionalListStepsInputListStepsPaginateTypeDef",
+    {
+        "StepStates": Sequence[StepStateType],
+        "StepIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListStepsInputListStepsPaginateTypeDef(
+    _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
+):
+    pass
+
+
+ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
+    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
+    {
+        "StudioId": str,
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStudiosInputListStudiosPaginateTypeDef = TypedDict(
+    "ListStudiosInputListStudiosPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListReleaseLabelsInputRequestTypeDef = TypedDict(
     "ListReleaseLabelsInputRequestTypeDef",
     {
         "Filters": ReleaseLabelFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2690,42 +2404,42 @@
 )
 
 ListSecurityConfigurationsOutputTypeDef = TypedDict(
     "ListSecurityConfigurationsOutputTypeDef",
     {
         "SecurityConfigurations": List[SecurityConfigurationSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudioSessionMappingsOutputTypeDef = TypedDict(
     "ListStudioSessionMappingsOutputTypeDef",
     {
         "SessionMappings": List[SessionMappingSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudiosOutputTypeDef = TypedDict(
     "ListStudiosOutputTypeDef",
     {
         "Studios": List[StudioSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSupportedInstanceTypesOutputTypeDef = TypedDict(
     "ListSupportedInstanceTypesOutputTypeDef",
     {
         "SupportedInstanceTypes": List[SupportedInstanceTypeTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotebookExecutionSummaryTypeDef = TypedDict(
     "NotebookExecutionSummaryTypeDef",
     {
         "NotebookExecutionId": str,
@@ -2741,55 +2455,33 @@
 )
 
 NotebookExecutionTypeDef = TypedDict(
     "NotebookExecutionTypeDef",
     {
         "NotebookExecutionId": str,
         "EditorId": str,
-        "ExecutionEngine": ExecutionEngineConfigOutputTypeDef,
+        "ExecutionEngine": ExecutionEngineConfigTypeDef,
         "NotebookExecutionName": str,
         "NotebookParams": str,
         "Status": NotebookExecutionStatusType,
         "StartTime": datetime,
         "EndTime": datetime,
         "Arn": str,
         "OutputNotebookURI": str,
         "LastStateChangeReason": str,
         "NotebookInstanceSecurityGroupId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "NotebookS3Location": NotebookS3LocationForOutputTypeDef,
         "OutputNotebookS3Location": OutputNotebookS3LocationForOutputTypeDef,
         "OutputNotebookFormat": Literal["HTML"],
         "EnvironmentVariables": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredOnDemandProvisioningSpecificationOutputTypeDef = TypedDict(
-    "_RequiredOnDemandProvisioningSpecificationOutputTypeDef",
-    {
-        "AllocationStrategy": Literal["lowest-price"],
-    },
-)
-_OptionalOnDemandProvisioningSpecificationOutputTypeDef = TypedDict(
-    "_OptionalOnDemandProvisioningSpecificationOutputTypeDef",
-    {
-        "CapacityReservationOptions": OnDemandCapacityReservationOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class OnDemandProvisioningSpecificationOutputTypeDef(
-    _RequiredOnDemandProvisioningSpecificationOutputTypeDef,
-    _OptionalOnDemandProvisioningSpecificationOutputTypeDef,
-):
-    pass
-
-
 _RequiredOnDemandProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredOnDemandProvisioningSpecificationTypeDef",
     {
         "AllocationStrategy": Literal["lowest-price"],
     },
 )
 _OptionalOnDemandProvisioningSpecificationTypeDef = TypedDict(
@@ -2836,35 +2528,14 @@
 class StartNotebookExecutionInputRequestTypeDef(
     _RequiredStartNotebookExecutionInputRequestTypeDef,
     _OptionalStartNotebookExecutionInputRequestTypeDef,
 ):
     pass
 
 
-_RequiredScalingActionOutputTypeDef = TypedDict(
-    "_RequiredScalingActionOutputTypeDef",
-    {
-        "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationOutputTypeDef,
-    },
-)
-_OptionalScalingActionOutputTypeDef = TypedDict(
-    "_OptionalScalingActionOutputTypeDef",
-    {
-        "Market": MarketTypeType,
-    },
-    total=False,
-)
-
-
-class ScalingActionOutputTypeDef(
-    _RequiredScalingActionOutputTypeDef, _OptionalScalingActionOutputTypeDef
-):
-    pass
-
-
 _RequiredScalingActionTypeDef = TypedDict(
     "_RequiredScalingActionTypeDef",
     {
         "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationTypeDef,
     },
 )
 _OptionalScalingActionTypeDef = TypedDict(
@@ -2887,20 +2558,28 @@
         "StateChangeReason": StepStateChangeReasonTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
         "Timeline": StepTimelineTypeDef,
     },
     total=False,
 )
 
+DescribeStudioOutputTypeDef = TypedDict(
+    "DescribeStudioOutputTypeDef",
+    {
+        "Studio": StudioTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationOutputTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
@@ -2955,48 +2634,40 @@
         "RequestedAmiVersion": str,
         "RunningAmiVersion": str,
         "ReleaseLabel": str,
         "AutoTerminate": bool,
         "TerminationProtected": bool,
         "VisibleToAllUsers": bool,
         "Applications": List[ApplicationOutputTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ServiceRole": str,
         "NormalizedInstanceHours": int,
         "MasterPublicDnsName": str,
         "Configurations": List["ConfigurationOutputTypeDef"],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
         "CustomAmiId": str,
         "EbsRootVolumeSize": int,
         "RepoUpgradeOnBoot": RepoUpgradeOnBootType,
-        "KerberosAttributes": KerberosAttributesOutputTypeDef,
+        "KerberosAttributes": KerberosAttributesTypeDef,
         "ClusterArn": str,
         "OutpostArn": str,
         "StepConcurrencyLevel": int,
-        "PlacementGroups": List[PlacementGroupConfigOutputTypeDef],
+        "PlacementGroups": List[PlacementGroupConfigTypeDef],
         "OSReleaseLabel": str,
     },
     total=False,
 )
 
-DescribeStudioOutputTypeDef = TypedDict(
-    "DescribeStudioOutputTypeDef",
-    {
-        "Studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetManagedScalingPolicyOutputTypeDef = TypedDict(
     "GetManagedScalingPolicyOutputTypeDef",
     {
-        "ManagedScalingPolicy": ManagedScalingPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ManagedScalingPolicy": ManagedScalingPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutManagedScalingPolicyInputRequestTypeDef = TypedDict(
     "PutManagedScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
@@ -3005,15 +2676,15 @@
 )
 
 GetClusterSessionCredentialsOutputTypeDef = TypedDict(
     "GetClusterSessionCredentialsOutputTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "ExpiresAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EbsConfigurationTypeDef = TypedDict(
     "EbsConfigurationTypeDef",
     {
         "EbsBlockDeviceConfigs": Sequence[EbsBlockDeviceConfigTypeDef],
@@ -3145,35 +2816,26 @@
 )
 
 ListNotebookExecutionsOutputTypeDef = TypedDict(
     "ListNotebookExecutionsOutputTypeDef",
     {
         "NotebookExecutions": List[NotebookExecutionSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotebookExecutionOutputTypeDef = TypedDict(
     "DescribeNotebookExecutionOutputTypeDef",
     {
         "NotebookExecution": NotebookExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstanceFleetProvisioningSpecificationsOutputTypeDef = TypedDict(
-    "InstanceFleetProvisioningSpecificationsOutputTypeDef",
-    {
-        "SpotSpecification": SpotProvisioningSpecificationOutputTypeDef,
-        "OnDemandSpecification": OnDemandProvisioningSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
 InstanceFleetProvisioningSpecificationsTypeDef = TypedDict(
     "InstanceFleetProvisioningSpecificationsTypeDef",
     {
         "SpotSpecification": SpotProvisioningSpecificationTypeDef,
         "OnDemandSpecification": OnDemandProvisioningSpecificationTypeDef,
     },
     total=False,
@@ -3204,15 +2866,15 @@
     total=False,
 )
 
 _RequiredScalingRuleOutputTypeDef = TypedDict(
     "_RequiredScalingRuleOutputTypeDef",
     {
         "Name": str,
-        "Action": ScalingActionOutputTypeDef,
+        "Action": ScalingActionTypeDef,
         "Trigger": ScalingTriggerOutputTypeDef,
     },
 )
 _OptionalScalingRuleOutputTypeDef = TypedDict(
     "_OptionalScalingRuleOutputTypeDef",
     {
         "Description": str,
@@ -3249,23 +2911,23 @@
 
 
 ListClustersOutputTypeDef = TypedDict(
     "ListClustersOutputTypeDef",
     {
         "Clusters": List[ClusterSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClusterOutputTypeDef = TypedDict(
     "DescribeClusterOutputTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInstanceTypeConfigTypeDef = TypedDict(
     "_RequiredInstanceTypeConfigTypeDef",
     {
         "InstanceType": str,
@@ -3339,15 +3001,15 @@
 )
 
 ListInstancesOutputTypeDef = TypedDict(
     "ListInstancesOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceFleetTypeDef = TypedDict(
     "InstanceFleetTypeDef",
     {
         "Id": str,
@@ -3355,42 +3017,42 @@
         "Status": InstanceFleetStatusTypeDef,
         "InstanceFleetType": InstanceFleetTypeType,
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "ProvisionedOnDemandCapacity": int,
         "ProvisionedSpotCapacity": int,
         "InstanceTypeSpecifications": List[InstanceTypeSpecificationTypeDef],
-        "LaunchSpecifications": InstanceFleetProvisioningSpecificationsOutputTypeDef,
-        "ResizeSpecifications": InstanceFleetResizingSpecificationsOutputTypeDef,
+        "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
 ListStepsOutputTypeDef = TypedDict(
     "ListStepsOutputTypeDef",
     {
         "Steps": List[StepSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStepOutputTypeDef = TypedDict(
     "DescribeStepOutputTypeDef",
     {
         "Step": StepTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "Status": AutoScalingPolicyStatusTypeDef,
-        "Constraints": ScalingConstraintsOutputTypeDef,
+        "Constraints": ScalingConstraintsTypeDef,
         "Rules": List[ScalingRuleOutputTypeDef],
     },
     total=False,
 )
 
 AutoScalingPolicyTypeDef = TypedDict(
     "AutoScalingPolicyTypeDef",
@@ -3459,15 +3121,15 @@
 
 
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceGroupTypeDef = TypedDict(
     "InstanceGroupTypeDef",
     {
         "Id": str,
@@ -3495,15 +3157,15 @@
 PutAutoScalingPolicyOutputTypeDef = TypedDict(
     "PutAutoScalingPolicyOutputTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
         "AutoScalingPolicy": AutoScalingPolicyDescriptionTypeDef,
         "ClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInstanceGroupConfigTypeDef = TypedDict(
     "_RequiredInstanceGroupConfigTypeDef",
     {
         "InstanceRole": InstanceRoleTypeType,
@@ -3549,24 +3211,24 @@
     },
 )
 
 DescribeJobFlowsOutputTypeDef = TypedDict(
     "DescribeJobFlowsOutputTypeDef",
     {
         "JobFlows": List[JobFlowDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceGroupsOutputTypeDef = TypedDict(
     "ListInstanceGroupsOutputTypeDef",
     {
         "InstanceGroups": List[InstanceGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddInstanceGroupsInputRequestTypeDef = TypedDict(
     "AddInstanceGroupsInputRequestTypeDef",
     {
         "InstanceGroups": Sequence[InstanceGroupConfigTypeDef],
```

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/type_defs.pyi` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for emr service type definitions.
 
 [Open documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/type_defs/)
 
 Usage::
 
     ```python
-    from mypy_boto3_emr.type_defs import AddInstanceFleetOutputTypeDef
+    from mypy_boto3_emr.type_defs import ResponseMetadataTypeDef
 
-    data: AddInstanceFleetOutputTypeDef = {...}
+    data: ResponseMetadataTypeDef = {...}
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -60,224 +60,203 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AddInstanceFleetOutputTypeDef",
-    "AddInstanceGroupsOutputTypeDef",
-    "AddJobFlowStepsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "ApplicationOutputTypeDef",
     "ApplicationTypeDef",
-    "ScalingConstraintsOutputTypeDef",
-    "AutoScalingPolicyStateChangeReasonTypeDef",
     "ScalingConstraintsTypeDef",
-    "AutoTerminationPolicyOutputTypeDef",
+    "AutoScalingPolicyStateChangeReasonTypeDef",
     "AutoTerminationPolicyTypeDef",
     "BlockPublicAccessConfigurationMetadataTypeDef",
-    "PortRangeOutputTypeDef",
     "PortRangeTypeDef",
     "ScriptBootstrapActionConfigOutputTypeDef",
     "ScriptBootstrapActionConfigTypeDef",
     "CancelStepsInfoTypeDef",
     "CancelStepsInputRequestTypeDef",
-    "MetricDimensionOutputTypeDef",
     "MetricDimensionTypeDef",
     "ClusterStateChangeReasonTypeDef",
     "ClusterTimelineTypeDef",
     "ErrorDetailTypeDef",
     "Ec2InstanceAttributesTypeDef",
-    "KerberosAttributesOutputTypeDef",
-    "PlacementGroupConfigOutputTypeDef",
-    "TagOutputTypeDef",
+    "KerberosAttributesTypeDef",
+    "PlacementGroupConfigTypeDef",
     "CommandTypeDef",
-    "ComputeLimitsOutputTypeDef",
     "ComputeLimitsTypeDef",
     "ConfigurationOutputTypeDef",
     "ConfigurationTypeDef",
     "CreateSecurityConfigurationInputRequestTypeDef",
-    "CreateSecurityConfigurationOutputTypeDef",
-    "CreateStudioOutputTypeDef",
     "CreateStudioSessionMappingInputRequestTypeDef",
     "UsernamePasswordTypeDef",
     "DeleteSecurityConfigurationInputRequestTypeDef",
     "DeleteStudioInputRequestTypeDef",
     "DeleteStudioSessionMappingInputRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeClusterInputRequestTypeDef",
     "DescribeJobFlowsInputRequestTypeDef",
     "DescribeNotebookExecutionInputRequestTypeDef",
     "DescribeReleaseLabelInputRequestTypeDef",
     "OSReleaseTypeDef",
     "SimplifiedApplicationTypeDef",
     "DescribeSecurityConfigurationInputRequestTypeDef",
-    "DescribeSecurityConfigurationOutputTypeDef",
     "DescribeStepInputRequestTypeDef",
     "DescribeStudioInputRequestTypeDef",
     "VolumeSpecificationTypeDef",
-    "VolumeSpecificationOutputTypeDef",
     "EbsVolumeTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ExecutionEngineConfigOutputTypeDef",
     "ExecutionEngineConfigTypeDef",
     "FailureDetailsTypeDef",
     "GetAutoTerminationPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsInputRequestTypeDef",
     "GetManagedScalingPolicyInputRequestTypeDef",
     "GetStudioSessionMappingInputRequestTypeDef",
     "SessionMappingDetailTypeDef",
-    "KeyValueOutputTypeDef",
     "KeyValueTypeDef",
     "HadoopStepConfigTypeDef",
-    "SpotProvisioningSpecificationOutputTypeDef",
     "SpotProvisioningSpecificationTypeDef",
-    "OnDemandResizingSpecificationOutputTypeDef",
-    "SpotResizingSpecificationOutputTypeDef",
     "OnDemandResizingSpecificationTypeDef",
     "SpotResizingSpecificationTypeDef",
     "InstanceFleetStateChangeReasonTypeDef",
     "InstanceFleetTimelineTypeDef",
     "InstanceGroupDetailTypeDef",
     "InstanceGroupStateChangeReasonTypeDef",
     "InstanceGroupTimelineTypeDef",
     "InstanceResizePolicyOutputTypeDef",
     "InstanceResizePolicyTypeDef",
     "InstanceStateChangeReasonTypeDef",
     "InstanceTimelineTypeDef",
     "JobFlowExecutionStatusDetailTypeDef",
     "PlacementTypeTypeDef",
     "PlacementTypeOutputTypeDef",
-    "KerberosAttributesTypeDef",
-    "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListBootstrapActionsInputRequestTypeDef",
-    "ListClustersInputListClustersPaginateTypeDef",
     "ListClustersInputRequestTypeDef",
-    "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
     "ListInstanceFleetsInputRequestTypeDef",
-    "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
     "ListInstanceGroupsInputRequestTypeDef",
-    "ListInstancesInputListInstancesPaginateTypeDef",
     "ListInstancesInputRequestTypeDef",
-    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
     "ListNotebookExecutionsInputRequestTypeDef",
     "ReleaseLabelFilterTypeDef",
-    "ListReleaseLabelsOutputTypeDef",
-    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
     "ListSecurityConfigurationsInputRequestTypeDef",
     "SecurityConfigurationSummaryTypeDef",
-    "ListStepsInputListStepsPaginateTypeDef",
     "ListStepsInputRequestTypeDef",
-    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
     "ListStudioSessionMappingsInputRequestTypeDef",
     "SessionMappingSummaryTypeDef",
-    "ListStudiosInputListStudiosPaginateTypeDef",
     "ListStudiosInputRequestTypeDef",
     "StudioSummaryTypeDef",
     "ListSupportedInstanceTypesInputRequestTypeDef",
     "SupportedInstanceTypeTypeDef",
     "ModifyClusterInputRequestTypeDef",
-    "ModifyClusterOutputTypeDef",
     "NotebookS3LocationForOutputTypeDef",
     "OutputNotebookS3LocationForOutputTypeDef",
     "NotebookS3LocationFromInputTypeDef",
-    "OnDemandCapacityReservationOptionsOutputTypeDef",
     "OnDemandCapacityReservationOptionsTypeDef",
     "OutputNotebookS3LocationFromInputTypeDef",
-    "PaginatorConfigTypeDef",
-    "PlacementGroupConfigTypeDef",
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     "RemoveAutoTerminationPolicyInputRequestTypeDef",
     "RemoveManagedScalingPolicyInputRequestTypeDef",
     "RemoveTagsInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "SupportedProductConfigTypeDef",
-    "RunJobFlowOutputTypeDef",
-    "SimpleScalingPolicyConfigurationOutputTypeDef",
     "SimpleScalingPolicyConfigurationTypeDef",
     "SetTerminationProtectionInputRequestTypeDef",
     "SetVisibleToAllUsersInputRequestTypeDef",
-    "StartNotebookExecutionOutputTypeDef",
     "StepExecutionStatusDetailTypeDef",
     "StepStateChangeReasonTypeDef",
     "StepTimelineTypeDef",
     "StopNotebookExecutionInputRequestTypeDef",
     "TerminateJobFlowsInputRequestTypeDef",
     "UpdateStudioInputRequestTypeDef",
     "UpdateStudioSessionMappingInputRequestTypeDef",
+    "AddInstanceFleetOutputTypeDef",
+    "AddInstanceGroupsOutputTypeDef",
+    "AddJobFlowStepsOutputTypeDef",
+    "CreateSecurityConfigurationOutputTypeDef",
+    "CreateStudioOutputTypeDef",
+    "DescribeSecurityConfigurationOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListReleaseLabelsOutputTypeDef",
+    "ModifyClusterOutputTypeDef",
+    "RunJobFlowOutputTypeDef",
+    "StartNotebookExecutionOutputTypeDef",
     "AddTagsInputRequestTypeDef",
     "CreateStudioInputRequestTypeDef",
+    "StudioTypeDef",
     "AutoScalingPolicyStatusTypeDef",
     "GetAutoTerminationPolicyOutputTypeDef",
     "PutAutoTerminationPolicyInputRequestTypeDef",
     "BlockPublicAccessConfigurationOutputTypeDef",
     "BlockPublicAccessConfigurationTypeDef",
     "BootstrapActionConfigOutputTypeDef",
     "BootstrapActionConfigTypeDef",
     "CancelStepsOutputTypeDef",
     "CloudWatchAlarmDefinitionOutputTypeDef",
     "CloudWatchAlarmDefinitionTypeDef",
     "ClusterStatusTypeDef",
-    "StudioTypeDef",
     "ListBootstrapActionsOutputTypeDef",
-    "ManagedScalingPolicyOutputTypeDef",
     "ManagedScalingPolicyTypeDef",
     "CredentialsTypeDef",
     "DescribeClusterInputClusterRunningWaitTypeDef",
     "DescribeClusterInputClusterTerminatedWaitTypeDef",
     "DescribeStepInputStepCompleteWaitTypeDef",
     "DescribeReleaseLabelOutputTypeDef",
     "EbsBlockDeviceConfigTypeDef",
     "EbsBlockDeviceTypeDef",
     "GetStudioSessionMappingOutputTypeDef",
     "HadoopJarStepConfigOutputTypeDef",
     "HadoopJarStepConfigTypeDef",
-    "InstanceFleetResizingSpecificationsOutputTypeDef",
     "InstanceFleetResizingSpecificationsTypeDef",
     "InstanceFleetStatusTypeDef",
     "InstanceGroupStatusTypeDef",
     "ShrinkPolicyOutputTypeDef",
     "ShrinkPolicyTypeDef",
     "InstanceStatusTypeDef",
     "JobFlowInstancesDetailTypeDef",
+    "ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    "ListClustersInputListClustersPaginateTypeDef",
+    "ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    "ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    "ListInstancesInputListInstancesPaginateTypeDef",
+    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
+    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
+    "ListStepsInputListStepsPaginateTypeDef",
+    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
+    "ListStudiosInputListStudiosPaginateTypeDef",
     "ListReleaseLabelsInputRequestTypeDef",
     "ListSecurityConfigurationsOutputTypeDef",
     "ListStudioSessionMappingsOutputTypeDef",
     "ListStudiosOutputTypeDef",
     "ListSupportedInstanceTypesOutputTypeDef",
     "NotebookExecutionSummaryTypeDef",
     "NotebookExecutionTypeDef",
-    "OnDemandProvisioningSpecificationOutputTypeDef",
     "OnDemandProvisioningSpecificationTypeDef",
     "StartNotebookExecutionInputRequestTypeDef",
-    "ScalingActionOutputTypeDef",
     "ScalingActionTypeDef",
     "StepStatusTypeDef",
+    "DescribeStudioOutputTypeDef",
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     "BootstrapActionDetailTypeDef",
     "ScalingTriggerOutputTypeDef",
     "ScalingTriggerTypeDef",
     "ClusterSummaryTypeDef",
     "ClusterTypeDef",
-    "DescribeStudioOutputTypeDef",
     "GetManagedScalingPolicyOutputTypeDef",
     "PutManagedScalingPolicyInputRequestTypeDef",
     "GetClusterSessionCredentialsOutputTypeDef",
     "EbsConfigurationTypeDef",
     "InstanceTypeSpecificationTypeDef",
     "StepConfigOutputTypeDef",
     "StepConfigTypeDef",
     "InstanceFleetModifyConfigTypeDef",
     "InstanceGroupModifyConfigTypeDef",
     "InstanceTypeDef",
     "ListNotebookExecutionsOutputTypeDef",
     "DescribeNotebookExecutionOutputTypeDef",
-    "InstanceFleetProvisioningSpecificationsOutputTypeDef",
     "InstanceFleetProvisioningSpecificationsTypeDef",
     "StepSummaryTypeDef",
     "StepTypeDef",
     "ScalingRuleOutputTypeDef",
     "ScalingRuleTypeDef",
     "ListClustersOutputTypeDef",
     "DescribeClusterOutputTypeDef",
@@ -303,39 +282,22 @@
     "DescribeJobFlowsOutputTypeDef",
     "ListInstanceGroupsOutputTypeDef",
     "AddInstanceGroupsInputRequestTypeDef",
     "JobFlowInstancesConfigTypeDef",
     "RunJobFlowInputRequestTypeDef",
 )
 
-AddInstanceFleetOutputTypeDef = TypedDict(
-    "AddInstanceFleetOutputTypeDef",
-    {
-        "ClusterId": str,
-        "InstanceFleetId": str,
-        "ClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddInstanceGroupsOutputTypeDef = TypedDict(
-    "AddInstanceGroupsOutputTypeDef",
-    {
-        "JobFlowId": str,
-        "InstanceGroupIds": List[str],
-        "ClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AddJobFlowStepsOutputTypeDef = TypedDict(
-    "AddJobFlowStepsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "StepIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -362,16 +324,16 @@
         "Version": str,
         "Args": Sequence[str],
         "AdditionalInfo": Mapping[str, str],
     },
     total=False,
 )
 
-ScalingConstraintsOutputTypeDef = TypedDict(
-    "ScalingConstraintsOutputTypeDef",
+ScalingConstraintsTypeDef = TypedDict(
+    "ScalingConstraintsTypeDef",
     {
         "MinCapacity": int,
         "MaxCapacity": int,
     },
 )
 
 AutoScalingPolicyStateChangeReasonTypeDef = TypedDict(
@@ -379,30 +341,14 @@
     {
         "Code": AutoScalingPolicyStateChangeReasonCodeType,
         "Message": str,
     },
     total=False,
 )
 
-ScalingConstraintsTypeDef = TypedDict(
-    "ScalingConstraintsTypeDef",
-    {
-        "MinCapacity": int,
-        "MaxCapacity": int,
-    },
-)
-
-AutoTerminationPolicyOutputTypeDef = TypedDict(
-    "AutoTerminationPolicyOutputTypeDef",
-    {
-        "IdleTimeout": int,
-    },
-    total=False,
-)
-
 AutoTerminationPolicyTypeDef = TypedDict(
     "AutoTerminationPolicyTypeDef",
     {
         "IdleTimeout": int,
     },
     total=False,
 )
@@ -411,31 +357,14 @@
     "BlockPublicAccessConfigurationMetadataTypeDef",
     {
         "CreationDateTime": datetime,
         "CreatedByArn": str,
     },
 )
 
-_RequiredPortRangeOutputTypeDef = TypedDict(
-    "_RequiredPortRangeOutputTypeDef",
-    {
-        "MinRange": int,
-    },
-)
-_OptionalPortRangeOutputTypeDef = TypedDict(
-    "_OptionalPortRangeOutputTypeDef",
-    {
-        "MaxRange": int,
-    },
-    total=False,
-)
-
-class PortRangeOutputTypeDef(_RequiredPortRangeOutputTypeDef, _OptionalPortRangeOutputTypeDef):
-    pass
-
 _RequiredPortRangeTypeDef = TypedDict(
     "_RequiredPortRangeTypeDef",
     {
         "MinRange": int,
     },
 )
 _OptionalPortRangeTypeDef = TypedDict(
@@ -514,23 +443,14 @@
 )
 
 class CancelStepsInputRequestTypeDef(
     _RequiredCancelStepsInputRequestTypeDef, _OptionalCancelStepsInputRequestTypeDef
 ):
     pass
 
-MetricDimensionOutputTypeDef = TypedDict(
-    "MetricDimensionOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 MetricDimensionTypeDef = TypedDict(
     "MetricDimensionTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -579,96 +499,65 @@
         "ServiceAccessSecurityGroup": str,
         "AdditionalMasterSecurityGroups": List[str],
         "AdditionalSlaveSecurityGroups": List[str],
     },
     total=False,
 )
 
-_RequiredKerberosAttributesOutputTypeDef = TypedDict(
-    "_RequiredKerberosAttributesOutputTypeDef",
+_RequiredKerberosAttributesTypeDef = TypedDict(
+    "_RequiredKerberosAttributesTypeDef",
     {
         "Realm": str,
         "KdcAdminPassword": str,
     },
 )
-_OptionalKerberosAttributesOutputTypeDef = TypedDict(
-    "_OptionalKerberosAttributesOutputTypeDef",
+_OptionalKerberosAttributesTypeDef = TypedDict(
+    "_OptionalKerberosAttributesTypeDef",
     {
         "CrossRealmTrustPrincipalPassword": str,
         "ADDomainJoinUser": str,
         "ADDomainJoinPassword": str,
     },
     total=False,
 )
 
-class KerberosAttributesOutputTypeDef(
-    _RequiredKerberosAttributesOutputTypeDef, _OptionalKerberosAttributesOutputTypeDef
+class KerberosAttributesTypeDef(
+    _RequiredKerberosAttributesTypeDef, _OptionalKerberosAttributesTypeDef
 ):
     pass
 
-_RequiredPlacementGroupConfigOutputTypeDef = TypedDict(
-    "_RequiredPlacementGroupConfigOutputTypeDef",
+_RequiredPlacementGroupConfigTypeDef = TypedDict(
+    "_RequiredPlacementGroupConfigTypeDef",
     {
         "InstanceRole": InstanceRoleTypeType,
     },
 )
-_OptionalPlacementGroupConfigOutputTypeDef = TypedDict(
-    "_OptionalPlacementGroupConfigOutputTypeDef",
+_OptionalPlacementGroupConfigTypeDef = TypedDict(
+    "_OptionalPlacementGroupConfigTypeDef",
     {
         "PlacementStrategy": PlacementGroupStrategyType,
     },
     total=False,
 )
 
-class PlacementGroupConfigOutputTypeDef(
-    _RequiredPlacementGroupConfigOutputTypeDef, _OptionalPlacementGroupConfigOutputTypeDef
+class PlacementGroupConfigTypeDef(
+    _RequiredPlacementGroupConfigTypeDef, _OptionalPlacementGroupConfigTypeDef
 ):
     pass
 
-TagOutputTypeDef = TypedDict(
-    "TagOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 CommandTypeDef = TypedDict(
     "CommandTypeDef",
     {
         "Name": str,
         "ScriptPath": str,
         "Args": List[str],
     },
     total=False,
 )
 
-_RequiredComputeLimitsOutputTypeDef = TypedDict(
-    "_RequiredComputeLimitsOutputTypeDef",
-    {
-        "UnitType": ComputeLimitsUnitTypeType,
-        "MinimumCapacityUnits": int,
-        "MaximumCapacityUnits": int,
-    },
-)
-_OptionalComputeLimitsOutputTypeDef = TypedDict(
-    "_OptionalComputeLimitsOutputTypeDef",
-    {
-        "MaximumOnDemandCapacityUnits": int,
-        "MaximumCoreCapacityUnits": int,
-    },
-    total=False,
-)
-
-class ComputeLimitsOutputTypeDef(
-    _RequiredComputeLimitsOutputTypeDef, _OptionalComputeLimitsOutputTypeDef
-):
-    pass
-
 _RequiredComputeLimitsTypeDef = TypedDict(
     "_RequiredComputeLimitsTypeDef",
     {
         "UnitType": ComputeLimitsUnitTypeType,
         "MinimumCapacityUnits": int,
         "MaximumCapacityUnits": int,
     },
@@ -709,32 +598,14 @@
     "CreateSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
         "SecurityConfiguration": str,
     },
 )
 
-CreateSecurityConfigurationOutputTypeDef = TypedDict(
-    "CreateSecurityConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "CreationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateStudioOutputTypeDef = TypedDict(
-    "CreateStudioOutputTypeDef",
-    {
-        "StudioId": str,
-        "Url": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateStudioSessionMappingInputRequestTypeDef = TypedDict(
     "_RequiredCreateStudioSessionMappingInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
     },
@@ -863,24 +734,14 @@
 DescribeSecurityConfigurationInputRequestTypeDef = TypedDict(
     "DescribeSecurityConfigurationInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeSecurityConfigurationOutputTypeDef = TypedDict(
-    "DescribeSecurityConfigurationOutputTypeDef",
-    {
-        "Name": str,
-        "SecurityConfiguration": str,
-        "CreationDateTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeStepInputRequestTypeDef = TypedDict(
     "DescribeStepInputRequestTypeDef",
     {
         "ClusterId": str,
         "StepId": str,
     },
 )
@@ -909,72 +770,23 @@
 )
 
 class VolumeSpecificationTypeDef(
     _RequiredVolumeSpecificationTypeDef, _OptionalVolumeSpecificationTypeDef
 ):
     pass
 
-_RequiredVolumeSpecificationOutputTypeDef = TypedDict(
-    "_RequiredVolumeSpecificationOutputTypeDef",
-    {
-        "VolumeType": str,
-        "SizeInGB": int,
-    },
-)
-_OptionalVolumeSpecificationOutputTypeDef = TypedDict(
-    "_OptionalVolumeSpecificationOutputTypeDef",
-    {
-        "Iops": int,
-        "Throughput": int,
-    },
-    total=False,
-)
-
-class VolumeSpecificationOutputTypeDef(
-    _RequiredVolumeSpecificationOutputTypeDef, _OptionalVolumeSpecificationOutputTypeDef
-):
-    pass
-
 EbsVolumeTypeDef = TypedDict(
     "EbsVolumeTypeDef",
     {
         "Device": str,
         "VolumeId": str,
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
-_RequiredExecutionEngineConfigOutputTypeDef = TypedDict(
-    "_RequiredExecutionEngineConfigOutputTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalExecutionEngineConfigOutputTypeDef = TypedDict(
-    "_OptionalExecutionEngineConfigOutputTypeDef",
-    {
-        "Type": Literal["EMR"],
-        "MasterInstanceSecurityGroupId": str,
-        "ExecutionRoleArn": str,
-    },
-    total=False,
-)
-
-class ExecutionEngineConfigOutputTypeDef(
-    _RequiredExecutionEngineConfigOutputTypeDef, _OptionalExecutionEngineConfigOutputTypeDef
-):
-    pass
-
 _RequiredExecutionEngineConfigTypeDef = TypedDict(
     "_RequiredExecutionEngineConfigTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalExecutionEngineConfigTypeDef = TypedDict(
@@ -1056,23 +868,14 @@
         "SessionPolicyArn": str,
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-KeyValueOutputTypeDef = TypedDict(
-    "KeyValueOutputTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 KeyValueTypeDef = TypedDict(
     "KeyValueTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -1085,36 +888,14 @@
         "Properties": Dict[str, str],
         "MainClass": str,
         "Args": List[str],
     },
     total=False,
 )
 
-_RequiredSpotProvisioningSpecificationOutputTypeDef = TypedDict(
-    "_RequiredSpotProvisioningSpecificationOutputTypeDef",
-    {
-        "TimeoutDurationMinutes": int,
-        "TimeoutAction": SpotProvisioningTimeoutActionType,
-    },
-)
-_OptionalSpotProvisioningSpecificationOutputTypeDef = TypedDict(
-    "_OptionalSpotProvisioningSpecificationOutputTypeDef",
-    {
-        "BlockDurationMinutes": int,
-        "AllocationStrategy": SpotProvisioningAllocationStrategyType,
-    },
-    total=False,
-)
-
-class SpotProvisioningSpecificationOutputTypeDef(
-    _RequiredSpotProvisioningSpecificationOutputTypeDef,
-    _OptionalSpotProvisioningSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredSpotProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredSpotProvisioningSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
         "TimeoutAction": SpotProvisioningTimeoutActionType,
     },
 )
@@ -1128,28 +909,14 @@
 )
 
 class SpotProvisioningSpecificationTypeDef(
     _RequiredSpotProvisioningSpecificationTypeDef, _OptionalSpotProvisioningSpecificationTypeDef
 ):
     pass
 
-OnDemandResizingSpecificationOutputTypeDef = TypedDict(
-    "OnDemandResizingSpecificationOutputTypeDef",
-    {
-        "TimeoutDurationMinutes": int,
-    },
-)
-
-SpotResizingSpecificationOutputTypeDef = TypedDict(
-    "SpotResizingSpecificationOutputTypeDef",
-    {
-        "TimeoutDurationMinutes": int,
-    },
-)
-
 OnDemandResizingSpecificationTypeDef = TypedDict(
     "OnDemandResizingSpecificationTypeDef",
     {
         "TimeoutDurationMinutes": int,
     },
 )
 
@@ -1306,56 +1073,24 @@
     {
         "AvailabilityZone": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-_RequiredKerberosAttributesTypeDef = TypedDict(
-    "_RequiredKerberosAttributesTypeDef",
-    {
-        "Realm": str,
-        "KdcAdminPassword": str,
-    },
-)
-_OptionalKerberosAttributesTypeDef = TypedDict(
-    "_OptionalKerberosAttributesTypeDef",
-    {
-        "CrossRealmTrustPrincipalPassword": str,
-        "ADDomainJoinUser": str,
-        "ADDomainJoinPassword": str,
-    },
-    total=False,
-)
-
-class KerberosAttributesTypeDef(
-    _RequiredKerberosAttributesTypeDef, _OptionalKerberosAttributesTypeDef
-):
-    pass
-
-_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
-    "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
-    "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
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
 
-class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
-    _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-    _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListBootstrapActionsInputRequestTypeDef = TypedDict(
     "_RequiredListBootstrapActionsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListBootstrapActionsInputRequestTypeDef = TypedDict(
@@ -1368,56 +1103,25 @@
 
 class ListBootstrapActionsInputRequestTypeDef(
     _RequiredListBootstrapActionsInputRequestTypeDef,
     _OptionalListBootstrapActionsInputRequestTypeDef,
 ):
     pass
 
-ListClustersInputListClustersPaginateTypeDef = TypedDict(
-    "ListClustersInputListClustersPaginateTypeDef",
-    {
-        "CreatedAfter": Union[datetime, str],
-        "CreatedBefore": Union[datetime, str],
-        "ClusterStates": Sequence[ClusterStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClustersInputRequestTypeDef = TypedDict(
     "ListClustersInputRequestTypeDef",
     {
         "CreatedAfter": Union[datetime, str],
         "CreatedBefore": Union[datetime, str],
         "ClusterStates": Sequence[ClusterStateType],
         "Marker": str,
     },
     total=False,
 )
 
-_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
-    _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-    _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListInstanceFleetsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceFleetsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceFleetsInputRequestTypeDef = TypedDict(
@@ -1429,34 +1133,14 @@
 )
 
 class ListInstanceFleetsInputRequestTypeDef(
     _RequiredListInstanceFleetsInputRequestTypeDef, _OptionalListInstanceFleetsInputRequestTypeDef
 ):
     pass
 
-_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
-    _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-    _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListInstanceGroupsInputRequestTypeDef = TypedDict(
     "_RequiredListInstanceGroupsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstanceGroupsInputRequestTypeDef = TypedDict(
@@ -1468,39 +1152,14 @@
 )
 
 class ListInstanceGroupsInputRequestTypeDef(
     _RequiredListInstanceGroupsInputRequestTypeDef, _OptionalListInstanceGroupsInputRequestTypeDef
 ):
     pass
 
-_RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
-    "_RequiredListInstancesInputListInstancesPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
-    "_OptionalListInstancesInputListInstancesPaginateTypeDef",
-    {
-        "InstanceGroupId": str,
-        "InstanceGroupTypes": Sequence[InstanceGroupTypeType],
-        "InstanceFleetId": str,
-        "InstanceFleetType": InstanceFleetTypeType,
-        "InstanceStates": Sequence[InstanceStateType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInstancesInputListInstancesPaginateTypeDef(
-    _RequiredListInstancesInputListInstancesPaginateTypeDef,
-    _OptionalListInstancesInputListInstancesPaginateTypeDef,
-):
-    pass
-
 _RequiredListInstancesInputRequestTypeDef = TypedDict(
     "_RequiredListInstancesInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListInstancesInputRequestTypeDef = TypedDict(
@@ -1517,27 +1176,14 @@
 )
 
 class ListInstancesInputRequestTypeDef(
     _RequiredListInstancesInputRequestTypeDef, _OptionalListInstancesInputRequestTypeDef
 ):
     pass
 
-ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
-    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
-    {
-        "EditorId": str,
-        "Status": NotebookExecutionStatusType,
-        "From": Union[datetime, str],
-        "To": Union[datetime, str],
-        "ExecutionEngineId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNotebookExecutionsInputRequestTypeDef = TypedDict(
     "ListNotebookExecutionsInputRequestTypeDef",
     {
         "EditorId": str,
         "Status": NotebookExecutionStatusType,
         "From": Union[datetime, str],
         "To": Union[datetime, str],
@@ -1552,31 +1198,14 @@
     {
         "Prefix": str,
         "Application": str,
     },
     total=False,
 )
 
-ListReleaseLabelsOutputTypeDef = TypedDict(
-    "ListReleaseLabelsOutputTypeDef",
-    {
-        "ReleaseLabels": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
-    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecurityConfigurationsInputRequestTypeDef = TypedDict(
     "ListSecurityConfigurationsInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
@@ -1586,35 +1215,14 @@
     {
         "Name": str,
         "CreationDateTime": datetime,
     },
     total=False,
 )
 
-_RequiredListStepsInputListStepsPaginateTypeDef = TypedDict(
-    "_RequiredListStepsInputListStepsPaginateTypeDef",
-    {
-        "ClusterId": str,
-    },
-)
-_OptionalListStepsInputListStepsPaginateTypeDef = TypedDict(
-    "_OptionalListStepsInputListStepsPaginateTypeDef",
-    {
-        "StepStates": Sequence[StepStateType],
-        "StepIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListStepsInputListStepsPaginateTypeDef(
-    _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
-):
-    pass
-
 _RequiredListStepsInputRequestTypeDef = TypedDict(
     "_RequiredListStepsInputRequestTypeDef",
     {
         "ClusterId": str,
     },
 )
 _OptionalListStepsInputRequestTypeDef = TypedDict(
@@ -1628,24 +1236,14 @@
 )
 
 class ListStepsInputRequestTypeDef(
     _RequiredListStepsInputRequestTypeDef, _OptionalListStepsInputRequestTypeDef
 ):
     pass
 
-ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
-    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
-    {
-        "StudioId": str,
-        "IdentityType": IdentityTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStudioSessionMappingsInputRequestTypeDef = TypedDict(
     "ListStudioSessionMappingsInputRequestTypeDef",
     {
         "StudioId": str,
         "IdentityType": IdentityTypeType,
         "Marker": str,
     },
@@ -1661,22 +1259,14 @@
         "IdentityType": IdentityTypeType,
         "SessionPolicyArn": str,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-ListStudiosInputListStudiosPaginateTypeDef = TypedDict(
-    "ListStudiosInputListStudiosPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStudiosInputRequestTypeDef = TypedDict(
     "ListStudiosInputRequestTypeDef",
     {
         "Marker": str,
     },
     total=False,
 )
@@ -1748,22 +1338,14 @@
 )
 
 class ModifyClusterInputRequestTypeDef(
     _RequiredModifyClusterInputRequestTypeDef, _OptionalModifyClusterInputRequestTypeDef
 ):
     pass
 
-ModifyClusterOutputTypeDef = TypedDict(
-    "ModifyClusterOutputTypeDef",
-    {
-        "StepConcurrencyLevel": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NotebookS3LocationForOutputTypeDef = TypedDict(
     "NotebookS3LocationForOutputTypeDef",
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
@@ -1783,24 +1365,14 @@
     {
         "Bucket": str,
         "Key": str,
     },
     total=False,
 )
 
-OnDemandCapacityReservationOptionsOutputTypeDef = TypedDict(
-    "OnDemandCapacityReservationOptionsOutputTypeDef",
-    {
-        "UsageStrategy": Literal["use-capacity-reservations-first"],
-        "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
-        "CapacityReservationResourceGroupArn": str,
-    },
-    total=False,
-)
-
 OnDemandCapacityReservationOptionsTypeDef = TypedDict(
     "OnDemandCapacityReservationOptionsTypeDef",
     {
         "UsageStrategy": Literal["use-capacity-reservations-first"],
         "CapacityReservationPreference": OnDemandCapacityReservationPreferenceType,
         "CapacityReservationResourceGroupArn": str,
     },
@@ -1812,43 +1384,14 @@
     {
         "Bucket": str,
         "Key": str,
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
-_RequiredPlacementGroupConfigTypeDef = TypedDict(
-    "_RequiredPlacementGroupConfigTypeDef",
-    {
-        "InstanceRole": InstanceRoleTypeType,
-    },
-)
-_OptionalPlacementGroupConfigTypeDef = TypedDict(
-    "_OptionalPlacementGroupConfigTypeDef",
-    {
-        "PlacementStrategy": PlacementGroupStrategyType,
-    },
-    total=False,
-)
-
-class PlacementGroupConfigTypeDef(
-    _RequiredPlacementGroupConfigTypeDef, _OptionalPlacementGroupConfigTypeDef
-):
-    pass
-
 RemoveAutoScalingPolicyInputRequestTypeDef = TypedDict(
     "RemoveAutoScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
     },
 )
@@ -1871,64 +1414,23 @@
     "RemoveTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
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
 SupportedProductConfigTypeDef = TypedDict(
     "SupportedProductConfigTypeDef",
     {
         "Name": str,
         "Args": Sequence[str],
     },
     total=False,
 )
 
-RunJobFlowOutputTypeDef = TypedDict(
-    "RunJobFlowOutputTypeDef",
-    {
-        "JobFlowId": str,
-        "ClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredSimpleScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSimpleScalingPolicyConfigurationOutputTypeDef",
-    {
-        "ScalingAdjustment": int,
-    },
-)
-_OptionalSimpleScalingPolicyConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSimpleScalingPolicyConfigurationOutputTypeDef",
-    {
-        "AdjustmentType": AdjustmentTypeType,
-        "CoolDown": int,
-    },
-    total=False,
-)
-
-class SimpleScalingPolicyConfigurationOutputTypeDef(
-    _RequiredSimpleScalingPolicyConfigurationOutputTypeDef,
-    _OptionalSimpleScalingPolicyConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredSimpleScalingPolicyConfigurationTypeDef = TypedDict(
     "_RequiredSimpleScalingPolicyConfigurationTypeDef",
     {
         "ScalingAdjustment": int,
     },
 )
 _OptionalSimpleScalingPolicyConfigurationTypeDef = TypedDict(
@@ -1958,22 +1460,14 @@
     "SetVisibleToAllUsersInputRequestTypeDef",
     {
         "JobFlowIds": Sequence[str],
         "VisibleToAllUsers": bool,
     },
 )
 
-StartNotebookExecutionOutputTypeDef = TypedDict(
-    "StartNotebookExecutionOutputTypeDef",
-    {
-        "NotebookExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredStepExecutionStatusDetailTypeDef = TypedDict(
     "_RequiredStepExecutionStatusDetailTypeDef",
     {
         "State": StepExecutionStateType,
         "CreationDateTime": datetime,
     },
 )
@@ -2066,14 +1560,111 @@
 
 class UpdateStudioSessionMappingInputRequestTypeDef(
     _RequiredUpdateStudioSessionMappingInputRequestTypeDef,
     _OptionalUpdateStudioSessionMappingInputRequestTypeDef,
 ):
     pass
 
+AddInstanceFleetOutputTypeDef = TypedDict(
+    "AddInstanceFleetOutputTypeDef",
+    {
+        "ClusterId": str,
+        "InstanceFleetId": str,
+        "ClusterArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddInstanceGroupsOutputTypeDef = TypedDict(
+    "AddInstanceGroupsOutputTypeDef",
+    {
+        "JobFlowId": str,
+        "InstanceGroupIds": List[str],
+        "ClusterArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AddJobFlowStepsOutputTypeDef = TypedDict(
+    "AddJobFlowStepsOutputTypeDef",
+    {
+        "StepIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSecurityConfigurationOutputTypeDef = TypedDict(
+    "CreateSecurityConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "CreationDateTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStudioOutputTypeDef = TypedDict(
+    "CreateStudioOutputTypeDef",
+    {
+        "StudioId": str,
+        "Url": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSecurityConfigurationOutputTypeDef = TypedDict(
+    "DescribeSecurityConfigurationOutputTypeDef",
+    {
+        "Name": str,
+        "SecurityConfiguration": str,
+        "CreationDateTime": datetime,
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
+ListReleaseLabelsOutputTypeDef = TypedDict(
+    "ListReleaseLabelsOutputTypeDef",
+    {
+        "ReleaseLabels": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyClusterOutputTypeDef = TypedDict(
+    "ModifyClusterOutputTypeDef",
+    {
+        "StepConcurrencyLevel": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RunJobFlowOutputTypeDef = TypedDict(
+    "RunJobFlowOutputTypeDef",
+    {
+        "JobFlowId": str,
+        "ClusterArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartNotebookExecutionOutputTypeDef = TypedDict(
+    "StartNotebookExecutionOutputTypeDef",
+    {
+        "NotebookExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AddTagsInputRequestTypeDef = TypedDict(
     "AddTagsInputRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -2104,28 +1695,52 @@
 )
 
 class CreateStudioInputRequestTypeDef(
     _RequiredCreateStudioInputRequestTypeDef, _OptionalCreateStudioInputRequestTypeDef
 ):
     pass
 
+StudioTypeDef = TypedDict(
+    "StudioTypeDef",
+    {
+        "StudioId": str,
+        "StudioArn": str,
+        "Name": str,
+        "Description": str,
+        "AuthMode": AuthModeType,
+        "VpcId": str,
+        "SubnetIds": List[str],
+        "ServiceRole": str,
+        "UserRole": str,
+        "WorkspaceSecurityGroupId": str,
+        "EngineSecurityGroupId": str,
+        "Url": str,
+        "CreationTime": datetime,
+        "DefaultS3Location": str,
+        "IdpAuthUrl": str,
+        "IdpRelayStateParameterName": str,
+        "Tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 AutoScalingPolicyStatusTypeDef = TypedDict(
     "AutoScalingPolicyStatusTypeDef",
     {
         "State": AutoScalingPolicyStateType,
         "StateChangeReason": AutoScalingPolicyStateChangeReasonTypeDef,
     },
     total=False,
 )
 
 GetAutoTerminationPolicyOutputTypeDef = TypedDict(
     "GetAutoTerminationPolicyOutputTypeDef",
     {
-        "AutoTerminationPolicy": AutoTerminationPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AutoTerminationPolicy": AutoTerminationPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAutoTerminationPolicyInputRequestTypeDef = TypedDict(
     "_RequiredPutAutoTerminationPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
@@ -2150,15 +1765,15 @@
     {
         "BlockPublicSecurityGroupRules": bool,
     },
 )
 _OptionalBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "_OptionalBlockPublicAccessConfigurationOutputTypeDef",
     {
-        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeOutputTypeDef],
+        "PermittedPublicSecurityGroupRuleRanges": List[PortRangeTypeDef],
     },
     total=False,
 )
 
 class BlockPublicAccessConfigurationOutputTypeDef(
     _RequiredBlockPublicAccessConfigurationOutputTypeDef,
     _OptionalBlockPublicAccessConfigurationOutputTypeDef,
@@ -2200,15 +1815,15 @@
     },
 )
 
 CancelStepsOutputTypeDef = TypedDict(
     "CancelStepsOutputTypeDef",
     {
         "CancelStepsInfoList": List[CancelStepsInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmDefinitionOutputTypeDef",
     {
         "ComparisonOperator": ComparisonOperatorType,
@@ -2220,15 +1835,15 @@
 _OptionalCloudWatchAlarmDefinitionOutputTypeDef = TypedDict(
     "_OptionalCloudWatchAlarmDefinitionOutputTypeDef",
     {
         "EvaluationPeriods": int,
         "Namespace": str,
         "Statistic": StatisticType,
         "Unit": UnitType,
-        "Dimensions": List[MetricDimensionOutputTypeDef],
+        "Dimensions": List[MetricDimensionTypeDef],
     },
     total=False,
 )
 
 class CloudWatchAlarmDefinitionOutputTypeDef(
     _RequiredCloudWatchAlarmDefinitionOutputTypeDef, _OptionalCloudWatchAlarmDefinitionOutputTypeDef
 ):
@@ -2267,53 +1882,21 @@
         "StateChangeReason": ClusterStateChangeReasonTypeDef,
         "Timeline": ClusterTimelineTypeDef,
         "ErrorDetails": List[ErrorDetailTypeDef],
     },
     total=False,
 )
 
-StudioTypeDef = TypedDict(
-    "StudioTypeDef",
-    {
-        "StudioId": str,
-        "StudioArn": str,
-        "Name": str,
-        "Description": str,
-        "AuthMode": AuthModeType,
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "ServiceRole": str,
-        "UserRole": str,
-        "WorkspaceSecurityGroupId": str,
-        "EngineSecurityGroupId": str,
-        "Url": str,
-        "CreationTime": datetime,
-        "DefaultS3Location": str,
-        "IdpAuthUrl": str,
-        "IdpRelayStateParameterName": str,
-        "Tags": List[TagOutputTypeDef],
-    },
-    total=False,
-)
-
 ListBootstrapActionsOutputTypeDef = TypedDict(
     "ListBootstrapActionsOutputTypeDef",
     {
         "BootstrapActions": List[CommandTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ManagedScalingPolicyOutputTypeDef = TypedDict(
-    "ManagedScalingPolicyOutputTypeDef",
-    {
-        "ComputeLimits": ComputeLimitsOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 ManagedScalingPolicyTypeDef = TypedDict(
     "ManagedScalingPolicyTypeDef",
     {
         "ComputeLimits": ComputeLimitsTypeDef,
     },
@@ -2392,15 +1975,15 @@
 DescribeReleaseLabelOutputTypeDef = TypedDict(
     "DescribeReleaseLabelOutputTypeDef",
     {
         "ReleaseLabel": str,
         "Applications": List[SimplifiedApplicationTypeDef],
         "NextToken": str,
         "AvailableOSReleases": List[OSReleaseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredEbsBlockDeviceConfigTypeDef = TypedDict(
     "_RequiredEbsBlockDeviceConfigTypeDef",
     {
         "VolumeSpecification": VolumeSpecificationTypeDef,
@@ -2418,38 +2001,38 @@
     _RequiredEbsBlockDeviceConfigTypeDef, _OptionalEbsBlockDeviceConfigTypeDef
 ):
     pass
 
 EbsBlockDeviceTypeDef = TypedDict(
     "EbsBlockDeviceTypeDef",
     {
-        "VolumeSpecification": VolumeSpecificationOutputTypeDef,
+        "VolumeSpecification": VolumeSpecificationTypeDef,
         "Device": str,
     },
     total=False,
 )
 
 GetStudioSessionMappingOutputTypeDef = TypedDict(
     "GetStudioSessionMappingOutputTypeDef",
     {
         "SessionMapping": SessionMappingDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHadoopJarStepConfigOutputTypeDef = TypedDict(
     "_RequiredHadoopJarStepConfigOutputTypeDef",
     {
         "Jar": str,
     },
 )
 _OptionalHadoopJarStepConfigOutputTypeDef = TypedDict(
     "_OptionalHadoopJarStepConfigOutputTypeDef",
     {
-        "Properties": List[KeyValueOutputTypeDef],
+        "Properties": List[KeyValueTypeDef],
         "MainClass": str,
         "Args": List[str],
     },
     total=False,
 )
 
 class HadoopJarStepConfigOutputTypeDef(
@@ -2474,23 +2057,14 @@
 )
 
 class HadoopJarStepConfigTypeDef(
     _RequiredHadoopJarStepConfigTypeDef, _OptionalHadoopJarStepConfigTypeDef
 ):
     pass
 
-InstanceFleetResizingSpecificationsOutputTypeDef = TypedDict(
-    "InstanceFleetResizingSpecificationsOutputTypeDef",
-    {
-        "SpotResizeSpecification": SpotResizingSpecificationOutputTypeDef,
-        "OnDemandResizeSpecification": OnDemandResizingSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
 InstanceFleetResizingSpecificationsTypeDef = TypedDict(
     "InstanceFleetResizingSpecificationsTypeDef",
     {
         "SpotResizeSpecification": SpotResizingSpecificationTypeDef,
         "OnDemandResizeSpecification": OnDemandResizingSpecificationTypeDef,
     },
     total=False,
@@ -2570,14 +2144,170 @@
 )
 
 class JobFlowInstancesDetailTypeDef(
     _RequiredJobFlowInstancesDetailTypeDef, _OptionalJobFlowInstancesDetailTypeDef
 ):
     pass
 
+_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
+    "_RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef = TypedDict(
+    "_OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef(
+    _RequiredListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    _OptionalListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+):
+    pass
+
+ListClustersInputListClustersPaginateTypeDef = TypedDict(
+    "ListClustersInputListClustersPaginateTypeDef",
+    {
+        "CreatedAfter": Union[datetime, str],
+        "CreatedBefore": Union[datetime, str],
+        "ClusterStates": Sequence[ClusterStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef(
+    _RequiredListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+    _OptionalListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef(
+    _RequiredListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+    _OptionalListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListInstancesInputListInstancesPaginateTypeDef = TypedDict(
+    "_RequiredListInstancesInputListInstancesPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListInstancesInputListInstancesPaginateTypeDef = TypedDict(
+    "_OptionalListInstancesInputListInstancesPaginateTypeDef",
+    {
+        "InstanceGroupId": str,
+        "InstanceGroupTypes": Sequence[InstanceGroupTypeType],
+        "InstanceFleetId": str,
+        "InstanceFleetType": InstanceFleetTypeType,
+        "InstanceStates": Sequence[InstanceStateType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInstancesInputListInstancesPaginateTypeDef(
+    _RequiredListInstancesInputListInstancesPaginateTypeDef,
+    _OptionalListInstancesInputListInstancesPaginateTypeDef,
+):
+    pass
+
+ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef = TypedDict(
+    "ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef",
+    {
+        "EditorId": str,
+        "Status": NotebookExecutionStatusType,
+        "From": Union[datetime, str],
+        "To": Union[datetime, str],
+        "ExecutionEngineId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef = TypedDict(
+    "ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListStepsInputListStepsPaginateTypeDef = TypedDict(
+    "_RequiredListStepsInputListStepsPaginateTypeDef",
+    {
+        "ClusterId": str,
+    },
+)
+_OptionalListStepsInputListStepsPaginateTypeDef = TypedDict(
+    "_OptionalListStepsInputListStepsPaginateTypeDef",
+    {
+        "StepStates": Sequence[StepStateType],
+        "StepIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListStepsInputListStepsPaginateTypeDef(
+    _RequiredListStepsInputListStepsPaginateTypeDef, _OptionalListStepsInputListStepsPaginateTypeDef
+):
+    pass
+
+ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef = TypedDict(
+    "ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef",
+    {
+        "StudioId": str,
+        "IdentityType": IdentityTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListStudiosInputListStudiosPaginateTypeDef = TypedDict(
+    "ListStudiosInputListStudiosPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListReleaseLabelsInputRequestTypeDef = TypedDict(
     "ListReleaseLabelsInputRequestTypeDef",
     {
         "Filters": ReleaseLabelFilterTypeDef,
         "NextToken": str,
         "MaxResults": int,
     },
@@ -2585,42 +2315,42 @@
 )
 
 ListSecurityConfigurationsOutputTypeDef = TypedDict(
     "ListSecurityConfigurationsOutputTypeDef",
     {
         "SecurityConfigurations": List[SecurityConfigurationSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudioSessionMappingsOutputTypeDef = TypedDict(
     "ListStudioSessionMappingsOutputTypeDef",
     {
         "SessionMappings": List[SessionMappingSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStudiosOutputTypeDef = TypedDict(
     "ListStudiosOutputTypeDef",
     {
         "Studios": List[StudioSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSupportedInstanceTypesOutputTypeDef = TypedDict(
     "ListSupportedInstanceTypesOutputTypeDef",
     {
         "SupportedInstanceTypes": List[SupportedInstanceTypeTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NotebookExecutionSummaryTypeDef = TypedDict(
     "NotebookExecutionSummaryTypeDef",
     {
         "NotebookExecutionId": str,
@@ -2636,53 +2366,33 @@
 )
 
 NotebookExecutionTypeDef = TypedDict(
     "NotebookExecutionTypeDef",
     {
         "NotebookExecutionId": str,
         "EditorId": str,
-        "ExecutionEngine": ExecutionEngineConfigOutputTypeDef,
+        "ExecutionEngine": ExecutionEngineConfigTypeDef,
         "NotebookExecutionName": str,
         "NotebookParams": str,
         "Status": NotebookExecutionStatusType,
         "StartTime": datetime,
         "EndTime": datetime,
         "Arn": str,
         "OutputNotebookURI": str,
         "LastStateChangeReason": str,
         "NotebookInstanceSecurityGroupId": str,
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "NotebookS3Location": NotebookS3LocationForOutputTypeDef,
         "OutputNotebookS3Location": OutputNotebookS3LocationForOutputTypeDef,
         "OutputNotebookFormat": Literal["HTML"],
         "EnvironmentVariables": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredOnDemandProvisioningSpecificationOutputTypeDef = TypedDict(
-    "_RequiredOnDemandProvisioningSpecificationOutputTypeDef",
-    {
-        "AllocationStrategy": Literal["lowest-price"],
-    },
-)
-_OptionalOnDemandProvisioningSpecificationOutputTypeDef = TypedDict(
-    "_OptionalOnDemandProvisioningSpecificationOutputTypeDef",
-    {
-        "CapacityReservationOptions": OnDemandCapacityReservationOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class OnDemandProvisioningSpecificationOutputTypeDef(
-    _RequiredOnDemandProvisioningSpecificationOutputTypeDef,
-    _OptionalOnDemandProvisioningSpecificationOutputTypeDef,
-):
-    pass
-
 _RequiredOnDemandProvisioningSpecificationTypeDef = TypedDict(
     "_RequiredOnDemandProvisioningSpecificationTypeDef",
     {
         "AllocationStrategy": Literal["lowest-price"],
     },
 )
 _OptionalOnDemandProvisioningSpecificationTypeDef = TypedDict(
@@ -2725,33 +2435,14 @@
 
 class StartNotebookExecutionInputRequestTypeDef(
     _RequiredStartNotebookExecutionInputRequestTypeDef,
     _OptionalStartNotebookExecutionInputRequestTypeDef,
 ):
     pass
 
-_RequiredScalingActionOutputTypeDef = TypedDict(
-    "_RequiredScalingActionOutputTypeDef",
-    {
-        "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationOutputTypeDef,
-    },
-)
-_OptionalScalingActionOutputTypeDef = TypedDict(
-    "_OptionalScalingActionOutputTypeDef",
-    {
-        "Market": MarketTypeType,
-    },
-    total=False,
-)
-
-class ScalingActionOutputTypeDef(
-    _RequiredScalingActionOutputTypeDef, _OptionalScalingActionOutputTypeDef
-):
-    pass
-
 _RequiredScalingActionTypeDef = TypedDict(
     "_RequiredScalingActionTypeDef",
     {
         "SimpleScalingPolicyConfiguration": SimpleScalingPolicyConfigurationTypeDef,
     },
 )
 _OptionalScalingActionTypeDef = TypedDict(
@@ -2772,20 +2463,28 @@
         "StateChangeReason": StepStateChangeReasonTypeDef,
         "FailureDetails": FailureDetailsTypeDef,
         "Timeline": StepTimelineTypeDef,
     },
     total=False,
 )
 
+DescribeStudioOutputTypeDef = TypedDict(
+    "DescribeStudioOutputTypeDef",
+    {
+        "Studio": StudioTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetBlockPublicAccessConfigurationOutputTypeDef = TypedDict(
     "GetBlockPublicAccessConfigurationOutputTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationOutputTypeDef,
         "BlockPublicAccessConfigurationMetadata": BlockPublicAccessConfigurationMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBlockPublicAccessConfigurationInputRequestTypeDef = TypedDict(
     "PutBlockPublicAccessConfigurationInputRequestTypeDef",
     {
         "BlockPublicAccessConfiguration": BlockPublicAccessConfigurationTypeDef,
@@ -2840,48 +2539,40 @@
         "RequestedAmiVersion": str,
         "RunningAmiVersion": str,
         "ReleaseLabel": str,
         "AutoTerminate": bool,
         "TerminationProtected": bool,
         "VisibleToAllUsers": bool,
         "Applications": List[ApplicationOutputTypeDef],
-        "Tags": List[TagOutputTypeDef],
+        "Tags": List[TagTypeDef],
         "ServiceRole": str,
         "NormalizedInstanceHours": int,
         "MasterPublicDnsName": str,
         "Configurations": List["ConfigurationOutputTypeDef"],
         "SecurityConfiguration": str,
         "AutoScalingRole": str,
         "ScaleDownBehavior": ScaleDownBehaviorType,
         "CustomAmiId": str,
         "EbsRootVolumeSize": int,
         "RepoUpgradeOnBoot": RepoUpgradeOnBootType,
-        "KerberosAttributes": KerberosAttributesOutputTypeDef,
+        "KerberosAttributes": KerberosAttributesTypeDef,
         "ClusterArn": str,
         "OutpostArn": str,
         "StepConcurrencyLevel": int,
-        "PlacementGroups": List[PlacementGroupConfigOutputTypeDef],
+        "PlacementGroups": List[PlacementGroupConfigTypeDef],
         "OSReleaseLabel": str,
     },
     total=False,
 )
 
-DescribeStudioOutputTypeDef = TypedDict(
-    "DescribeStudioOutputTypeDef",
-    {
-        "Studio": StudioTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetManagedScalingPolicyOutputTypeDef = TypedDict(
     "GetManagedScalingPolicyOutputTypeDef",
     {
-        "ManagedScalingPolicy": ManagedScalingPolicyOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ManagedScalingPolicy": ManagedScalingPolicyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutManagedScalingPolicyInputRequestTypeDef = TypedDict(
     "PutManagedScalingPolicyInputRequestTypeDef",
     {
         "ClusterId": str,
@@ -2890,15 +2581,15 @@
 )
 
 GetClusterSessionCredentialsOutputTypeDef = TypedDict(
     "GetClusterSessionCredentialsOutputTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "ExpiresAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EbsConfigurationTypeDef = TypedDict(
     "EbsConfigurationTypeDef",
     {
         "EbsBlockDeviceConfigs": Sequence[EbsBlockDeviceConfigTypeDef],
@@ -3022,35 +2713,26 @@
 )
 
 ListNotebookExecutionsOutputTypeDef = TypedDict(
     "ListNotebookExecutionsOutputTypeDef",
     {
         "NotebookExecutions": List[NotebookExecutionSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeNotebookExecutionOutputTypeDef = TypedDict(
     "DescribeNotebookExecutionOutputTypeDef",
     {
         "NotebookExecution": NotebookExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstanceFleetProvisioningSpecificationsOutputTypeDef = TypedDict(
-    "InstanceFleetProvisioningSpecificationsOutputTypeDef",
-    {
-        "SpotSpecification": SpotProvisioningSpecificationOutputTypeDef,
-        "OnDemandSpecification": OnDemandProvisioningSpecificationOutputTypeDef,
-    },
-    total=False,
-)
-
 InstanceFleetProvisioningSpecificationsTypeDef = TypedDict(
     "InstanceFleetProvisioningSpecificationsTypeDef",
     {
         "SpotSpecification": SpotProvisioningSpecificationTypeDef,
         "OnDemandSpecification": OnDemandProvisioningSpecificationTypeDef,
     },
     total=False,
@@ -3081,15 +2763,15 @@
     total=False,
 )
 
 _RequiredScalingRuleOutputTypeDef = TypedDict(
     "_RequiredScalingRuleOutputTypeDef",
     {
         "Name": str,
-        "Action": ScalingActionOutputTypeDef,
+        "Action": ScalingActionTypeDef,
         "Trigger": ScalingTriggerOutputTypeDef,
     },
 )
 _OptionalScalingRuleOutputTypeDef = TypedDict(
     "_OptionalScalingRuleOutputTypeDef",
     {
         "Description": str,
@@ -3122,23 +2804,23 @@
     pass
 
 ListClustersOutputTypeDef = TypedDict(
     "ListClustersOutputTypeDef",
     {
         "Clusters": List[ClusterSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClusterOutputTypeDef = TypedDict(
     "DescribeClusterOutputTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInstanceTypeConfigTypeDef = TypedDict(
     "_RequiredInstanceTypeConfigTypeDef",
     {
         "InstanceType": str,
@@ -3208,15 +2890,15 @@
 )
 
 ListInstancesOutputTypeDef = TypedDict(
     "ListInstancesOutputTypeDef",
     {
         "Instances": List[InstanceTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceFleetTypeDef = TypedDict(
     "InstanceFleetTypeDef",
     {
         "Id": str,
@@ -3224,42 +2906,42 @@
         "Status": InstanceFleetStatusTypeDef,
         "InstanceFleetType": InstanceFleetTypeType,
         "TargetOnDemandCapacity": int,
         "TargetSpotCapacity": int,
         "ProvisionedOnDemandCapacity": int,
         "ProvisionedSpotCapacity": int,
         "InstanceTypeSpecifications": List[InstanceTypeSpecificationTypeDef],
-        "LaunchSpecifications": InstanceFleetProvisioningSpecificationsOutputTypeDef,
-        "ResizeSpecifications": InstanceFleetResizingSpecificationsOutputTypeDef,
+        "LaunchSpecifications": InstanceFleetProvisioningSpecificationsTypeDef,
+        "ResizeSpecifications": InstanceFleetResizingSpecificationsTypeDef,
     },
     total=False,
 )
 
 ListStepsOutputTypeDef = TypedDict(
     "ListStepsOutputTypeDef",
     {
         "Steps": List[StepSummaryTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeStepOutputTypeDef = TypedDict(
     "DescribeStepOutputTypeDef",
     {
         "Step": StepTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingPolicyDescriptionTypeDef = TypedDict(
     "AutoScalingPolicyDescriptionTypeDef",
     {
         "Status": AutoScalingPolicyStatusTypeDef,
-        "Constraints": ScalingConstraintsOutputTypeDef,
+        "Constraints": ScalingConstraintsTypeDef,
         "Rules": List[ScalingRuleOutputTypeDef],
     },
     total=False,
 )
 
 AutoScalingPolicyTypeDef = TypedDict(
     "AutoScalingPolicyTypeDef",
@@ -3324,15 +3006,15 @@
     pass
 
 ListInstanceFleetsOutputTypeDef = TypedDict(
     "ListInstanceFleetsOutputTypeDef",
     {
         "InstanceFleets": List[InstanceFleetTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InstanceGroupTypeDef = TypedDict(
     "InstanceGroupTypeDef",
     {
         "Id": str,
@@ -3360,15 +3042,15 @@
 PutAutoScalingPolicyOutputTypeDef = TypedDict(
     "PutAutoScalingPolicyOutputTypeDef",
     {
         "ClusterId": str,
         "InstanceGroupId": str,
         "AutoScalingPolicy": AutoScalingPolicyDescriptionTypeDef,
         "ClusterArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredInstanceGroupConfigTypeDef = TypedDict(
     "_RequiredInstanceGroupConfigTypeDef",
     {
         "InstanceRole": InstanceRoleTypeType,
@@ -3412,24 +3094,24 @@
     },
 )
 
 DescribeJobFlowsOutputTypeDef = TypedDict(
     "DescribeJobFlowsOutputTypeDef",
     {
         "JobFlows": List[JobFlowDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInstanceGroupsOutputTypeDef = TypedDict(
     "ListInstanceGroupsOutputTypeDef",
     {
         "InstanceGroups": List[InstanceGroupTypeDef],
         "Marker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AddInstanceGroupsInputRequestTypeDef = TypedDict(
     "AddInstanceGroupsInputRequestTypeDef",
     {
         "InstanceGroups": Sequence[InstanceGroupConfigTypeDef],
```

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/waiter.py` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr/waiter.pyi` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/PKG-INFO` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-emr
-Version: 1.28.12
-Summary: Type annotations for boto3.EMR 1.28.12 service generated with mypy-boto3-builder 7.15.2
+Version: 1.28.15
+Summary: Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,24 +38,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-emr.svg?color=blue)](https://pypi.org/project/mypy-boto3-emr)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-emr)](https://pepy.tech/project/mypy-boto3-emr)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.EMR 1.28.12](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
+[boto3.EMR 1.28.15](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/emr.html#EMR)
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
 [mypy-boto3-emr docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_emr/).
 
 See how it helps to find and fix potential bugs:
 
@@ -425,224 +425,203 @@
 ### Typed dictionaries
 
 `mypy_boto3_emr.type_defs` module contains structures and shapes assembled to
 typed dictionaries for additional type checking.
 
 ```python
 from mypy_boto3_emr.type_defs import (
-    AddInstanceFleetOutputTypeDef,
-    AddInstanceGroupsOutputTypeDef,
-    AddJobFlowStepsOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     ApplicationOutputTypeDef,
     ApplicationTypeDef,
-    ScalingConstraintsOutputTypeDef,
-    AutoScalingPolicyStateChangeReasonTypeDef,
     ScalingConstraintsTypeDef,
-    AutoTerminationPolicyOutputTypeDef,
+    AutoScalingPolicyStateChangeReasonTypeDef,
     AutoTerminationPolicyTypeDef,
     BlockPublicAccessConfigurationMetadataTypeDef,
-    PortRangeOutputTypeDef,
     PortRangeTypeDef,
     ScriptBootstrapActionConfigOutputTypeDef,
     ScriptBootstrapActionConfigTypeDef,
     CancelStepsInfoTypeDef,
     CancelStepsInputRequestTypeDef,
-    MetricDimensionOutputTypeDef,
     MetricDimensionTypeDef,
     ClusterStateChangeReasonTypeDef,
     ClusterTimelineTypeDef,
     ErrorDetailTypeDef,
     Ec2InstanceAttributesTypeDef,
-    KerberosAttributesOutputTypeDef,
-    PlacementGroupConfigOutputTypeDef,
-    TagOutputTypeDef,
+    KerberosAttributesTypeDef,
+    PlacementGroupConfigTypeDef,
     CommandTypeDef,
-    ComputeLimitsOutputTypeDef,
     ComputeLimitsTypeDef,
     ConfigurationOutputTypeDef,
     ConfigurationTypeDef,
     CreateSecurityConfigurationInputRequestTypeDef,
-    CreateSecurityConfigurationOutputTypeDef,
-    CreateStudioOutputTypeDef,
     CreateStudioSessionMappingInputRequestTypeDef,
     UsernamePasswordTypeDef,
     DeleteSecurityConfigurationInputRequestTypeDef,
     DeleteStudioInputRequestTypeDef,
     DeleteStudioSessionMappingInputRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeClusterInputRequestTypeDef,
     DescribeJobFlowsInputRequestTypeDef,
     DescribeNotebookExecutionInputRequestTypeDef,
     DescribeReleaseLabelInputRequestTypeDef,
     OSReleaseTypeDef,
     SimplifiedApplicationTypeDef,
     DescribeSecurityConfigurationInputRequestTypeDef,
-    DescribeSecurityConfigurationOutputTypeDef,
     DescribeStepInputRequestTypeDef,
     DescribeStudioInputRequestTypeDef,
     VolumeSpecificationTypeDef,
-    VolumeSpecificationOutputTypeDef,
     EbsVolumeTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ExecutionEngineConfigOutputTypeDef,
     ExecutionEngineConfigTypeDef,
     FailureDetailsTypeDef,
     GetAutoTerminationPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsInputRequestTypeDef,
     GetManagedScalingPolicyInputRequestTypeDef,
     GetStudioSessionMappingInputRequestTypeDef,
     SessionMappingDetailTypeDef,
-    KeyValueOutputTypeDef,
     KeyValueTypeDef,
     HadoopStepConfigTypeDef,
-    SpotProvisioningSpecificationOutputTypeDef,
     SpotProvisioningSpecificationTypeDef,
-    OnDemandResizingSpecificationOutputTypeDef,
-    SpotResizingSpecificationOutputTypeDef,
     OnDemandResizingSpecificationTypeDef,
     SpotResizingSpecificationTypeDef,
     InstanceFleetStateChangeReasonTypeDef,
     InstanceFleetTimelineTypeDef,
     InstanceGroupDetailTypeDef,
     InstanceGroupStateChangeReasonTypeDef,
     InstanceGroupTimelineTypeDef,
     InstanceResizePolicyOutputTypeDef,
     InstanceResizePolicyTypeDef,
     InstanceStateChangeReasonTypeDef,
     InstanceTimelineTypeDef,
     JobFlowExecutionStatusDetailTypeDef,
     PlacementTypeTypeDef,
     PlacementTypeOutputTypeDef,
-    KerberosAttributesTypeDef,
-    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListBootstrapActionsInputRequestTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
     ListClustersInputRequestTypeDef,
-    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
     ListInstanceFleetsInputRequestTypeDef,
-    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
     ListInstanceGroupsInputRequestTypeDef,
-    ListInstancesInputListInstancesPaginateTypeDef,
     ListInstancesInputRequestTypeDef,
-    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
     ListNotebookExecutionsInputRequestTypeDef,
     ReleaseLabelFilterTypeDef,
-    ListReleaseLabelsOutputTypeDef,
-    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
     ListSecurityConfigurationsInputRequestTypeDef,
     SecurityConfigurationSummaryTypeDef,
-    ListStepsInputListStepsPaginateTypeDef,
     ListStepsInputRequestTypeDef,
-    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
     ListStudioSessionMappingsInputRequestTypeDef,
     SessionMappingSummaryTypeDef,
-    ListStudiosInputListStudiosPaginateTypeDef,
     ListStudiosInputRequestTypeDef,
     StudioSummaryTypeDef,
     ListSupportedInstanceTypesInputRequestTypeDef,
     SupportedInstanceTypeTypeDef,
     ModifyClusterInputRequestTypeDef,
-    ModifyClusterOutputTypeDef,
     NotebookS3LocationForOutputTypeDef,
     OutputNotebookS3LocationForOutputTypeDef,
     NotebookS3LocationFromInputTypeDef,
-    OnDemandCapacityReservationOptionsOutputTypeDef,
     OnDemandCapacityReservationOptionsTypeDef,
     OutputNotebookS3LocationFromInputTypeDef,
-    PaginatorConfigTypeDef,
-    PlacementGroupConfigTypeDef,
     RemoveAutoScalingPolicyInputRequestTypeDef,
     RemoveAutoTerminationPolicyInputRequestTypeDef,
     RemoveManagedScalingPolicyInputRequestTypeDef,
     RemoveTagsInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     SupportedProductConfigTypeDef,
-    RunJobFlowOutputTypeDef,
-    SimpleScalingPolicyConfigurationOutputTypeDef,
     SimpleScalingPolicyConfigurationTypeDef,
     SetTerminationProtectionInputRequestTypeDef,
     SetVisibleToAllUsersInputRequestTypeDef,
-    StartNotebookExecutionOutputTypeDef,
     StepExecutionStatusDetailTypeDef,
     StepStateChangeReasonTypeDef,
     StepTimelineTypeDef,
     StopNotebookExecutionInputRequestTypeDef,
     TerminateJobFlowsInputRequestTypeDef,
     UpdateStudioInputRequestTypeDef,
     UpdateStudioSessionMappingInputRequestTypeDef,
+    AddInstanceFleetOutputTypeDef,
+    AddInstanceGroupsOutputTypeDef,
+    AddJobFlowStepsOutputTypeDef,
+    CreateSecurityConfigurationOutputTypeDef,
+    CreateStudioOutputTypeDef,
+    DescribeSecurityConfigurationOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListReleaseLabelsOutputTypeDef,
+    ModifyClusterOutputTypeDef,
+    RunJobFlowOutputTypeDef,
+    StartNotebookExecutionOutputTypeDef,
     AddTagsInputRequestTypeDef,
     CreateStudioInputRequestTypeDef,
+    StudioTypeDef,
     AutoScalingPolicyStatusTypeDef,
     GetAutoTerminationPolicyOutputTypeDef,
     PutAutoTerminationPolicyInputRequestTypeDef,
     BlockPublicAccessConfigurationOutputTypeDef,
     BlockPublicAccessConfigurationTypeDef,
     BootstrapActionConfigOutputTypeDef,
     BootstrapActionConfigTypeDef,
     CancelStepsOutputTypeDef,
     CloudWatchAlarmDefinitionOutputTypeDef,
     CloudWatchAlarmDefinitionTypeDef,
     ClusterStatusTypeDef,
-    StudioTypeDef,
     ListBootstrapActionsOutputTypeDef,
-    ManagedScalingPolicyOutputTypeDef,
     ManagedScalingPolicyTypeDef,
     CredentialsTypeDef,
     DescribeClusterInputClusterRunningWaitTypeDef,
     DescribeClusterInputClusterTerminatedWaitTypeDef,
     DescribeStepInputStepCompleteWaitTypeDef,
     DescribeReleaseLabelOutputTypeDef,
     EbsBlockDeviceConfigTypeDef,
     EbsBlockDeviceTypeDef,
     GetStudioSessionMappingOutputTypeDef,
     HadoopJarStepConfigOutputTypeDef,
     HadoopJarStepConfigTypeDef,
-    InstanceFleetResizingSpecificationsOutputTypeDef,
     InstanceFleetResizingSpecificationsTypeDef,
     InstanceFleetStatusTypeDef,
     InstanceGroupStatusTypeDef,
     ShrinkPolicyOutputTypeDef,
     ShrinkPolicyTypeDef,
     InstanceStatusTypeDef,
     JobFlowInstancesDetailTypeDef,
+    ListBootstrapActionsInputListBootstrapActionsPaginateTypeDef,
+    ListClustersInputListClustersPaginateTypeDef,
+    ListInstanceFleetsInputListInstanceFleetsPaginateTypeDef,
+    ListInstanceGroupsInputListInstanceGroupsPaginateTypeDef,
+    ListInstancesInputListInstancesPaginateTypeDef,
+    ListNotebookExecutionsInputListNotebookExecutionsPaginateTypeDef,
+    ListSecurityConfigurationsInputListSecurityConfigurationsPaginateTypeDef,
+    ListStepsInputListStepsPaginateTypeDef,
+    ListStudioSessionMappingsInputListStudioSessionMappingsPaginateTypeDef,
+    ListStudiosInputListStudiosPaginateTypeDef,
     ListReleaseLabelsInputRequestTypeDef,
     ListSecurityConfigurationsOutputTypeDef,
     ListStudioSessionMappingsOutputTypeDef,
     ListStudiosOutputTypeDef,
     ListSupportedInstanceTypesOutputTypeDef,
     NotebookExecutionSummaryTypeDef,
     NotebookExecutionTypeDef,
-    OnDemandProvisioningSpecificationOutputTypeDef,
     OnDemandProvisioningSpecificationTypeDef,
     StartNotebookExecutionInputRequestTypeDef,
-    ScalingActionOutputTypeDef,
     ScalingActionTypeDef,
     StepStatusTypeDef,
+    DescribeStudioOutputTypeDef,
     GetBlockPublicAccessConfigurationOutputTypeDef,
     PutBlockPublicAccessConfigurationInputRequestTypeDef,
     BootstrapActionDetailTypeDef,
     ScalingTriggerOutputTypeDef,
     ScalingTriggerTypeDef,
     ClusterSummaryTypeDef,
     ClusterTypeDef,
-    DescribeStudioOutputTypeDef,
     GetManagedScalingPolicyOutputTypeDef,
     PutManagedScalingPolicyInputRequestTypeDef,
     GetClusterSessionCredentialsOutputTypeDef,
     EbsConfigurationTypeDef,
     InstanceTypeSpecificationTypeDef,
     StepConfigOutputTypeDef,
     StepConfigTypeDef,
     InstanceFleetModifyConfigTypeDef,
     InstanceGroupModifyConfigTypeDef,
     InstanceTypeDef,
     ListNotebookExecutionsOutputTypeDef,
     DescribeNotebookExecutionOutputTypeDef,
-    InstanceFleetProvisioningSpecificationsOutputTypeDef,
     InstanceFleetProvisioningSpecificationsTypeDef,
     StepSummaryTypeDef,
     StepTypeDef,
     ScalingRuleOutputTypeDef,
     ScalingRuleTypeDef,
     ListClustersOutputTypeDef,
     DescribeClusterOutputTypeDef,
@@ -669,15 +648,15 @@
     ListInstanceGroupsOutputTypeDef,
     AddInstanceGroupsInputRequestTypeDef,
     JobFlowInstancesConfigTypeDef,
     RunJobFlowInputRequestTypeDef,
 )
 
 
-def get_structure() -> AddInstanceFleetOutputTypeDef:
+def get_structure() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `mypy-boto3-emr-1.28.12/mypy_boto3_emr.egg-info/SOURCES.txt` & `mypy-boto3-emr-1.28.15/mypy_boto3_emr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-emr-1.28.12/setup.py` & `mypy-boto3-emr-1.28.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-emr",
-    version="1.28.12",
+    version="1.28.15",
     packages=["mypy_boto3_emr"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EMR 1.28.12 service generated with mypy-boto3-builder 7.15.2"
+        "Type annotations for boto3.EMR 1.28.15 service generated with mypy-boto3-builder 7.16.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

